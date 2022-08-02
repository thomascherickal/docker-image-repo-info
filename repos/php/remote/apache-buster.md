## `php:apache-buster`

```console
$ docker pull php@sha256:80ce26d96794f731cec2eb8b90d6a9f5a09126dc7f731633dfbba13687570834
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `php:apache-buster` - linux; amd64

```console
$ docker pull php@sha256:fd1bb8e268d9b363408b93487e1a61cc9b16366ad22637396506e8101a502881
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.6 MB (145561181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a70941141068f84c404d2a26f1b18f722601b23355a0ef79b5e7e0eafa5fd84d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 Aug 2022 01:20:24 GMT
ADD file:81dbfe4f9df4d280f7580380c0c5c93ba71fedba17b3072d2b7b4bce127f88a9 in / 
# Tue, 02 Aug 2022 01:20:24 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 06:30:58 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 02 Aug 2022 06:30:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 02 Aug 2022 06:31:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 06:31:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 06:31:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 06:34:51 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 02 Aug 2022 06:34:51 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 02 Aug 2022 06:34:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 02 Aug 2022 06:35:00 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 02 Aug 2022 06:35:01 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 02 Aug 2022 06:35:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 06:35:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 06:35:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 07:01:54 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 02 Aug 2022 07:28:58 GMT
ENV PHP_VERSION=8.1.8
# Tue, 02 Aug 2022 07:28:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Tue, 02 Aug 2022 07:28:58 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Tue, 02 Aug 2022 07:29:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 02 Aug 2022 07:29:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 02 Aug 2022 07:32:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 02 Aug 2022 07:32:21 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 02 Aug 2022 07:32:21 GMT
RUN docker-php-ext-enable sodium
# Tue, 02 Aug 2022 07:32:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 02 Aug 2022 07:32:22 GMT
STOPSIGNAL SIGWINCH
# Tue, 02 Aug 2022 07:32:22 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 02 Aug 2022 07:32:22 GMT
WORKDIR /var/www/html
# Tue, 02 Aug 2022 07:32:22 GMT
EXPOSE 80
# Tue, 02 Aug 2022 07:32:22 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:751ef25978b2971e15496369695ba51ed5b1b9aaca7e37b18a173d754d1ca820`  
		Last Modified: Tue, 02 Aug 2022 01:25:00 GMT  
		Size: 27.1 MB (27140083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674ea47a6cdfcd67bf3a92d4f2815eb980f3d8e469e450cb4c3d4e3b324f3a61`  
		Last Modified: Tue, 02 Aug 2022 08:59:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2135d02788749107cd72ae8364f4c834a1a99ff75005f23e5c68de8f88b6b5e`  
		Last Modified: Tue, 02 Aug 2022 08:59:45 GMT  
		Size: 76.7 MB (76684023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:522e09de4db0e5cb3d1db8214cb8c6bf59814b3c0809d65b7b319552ff7a0362`  
		Last Modified: Tue, 02 Aug 2022 08:59:33 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a57d944ae891864cb8626dfa4ab7f12157b09197249dd9e6c1d4a0c4ae41e39`  
		Last Modified: Tue, 02 Aug 2022 09:00:06 GMT  
		Size: 18.7 MB (18681698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:855ddab4d1fdba79d5c4ebce577de5369e71a33d05667fb64797509662dd309c`  
		Last Modified: Tue, 02 Aug 2022 09:00:03 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75678c9da41324a360fb9f1648e8add4a3446ed810a1a513fd1f3e2ef5d6e9d`  
		Last Modified: Tue, 02 Aug 2022 09:00:04 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215b621931b827740a98c8ea3ef62fdcda8865bb3e7a0c510c64c05c80fb215a`  
		Last Modified: Tue, 02 Aug 2022 09:06:38 GMT  
		Size: 12.1 MB (12060678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1341e75adc9a900deed4fa54252dfd4c5c4b42a41315fa0738010ddfbe7639e7`  
		Last Modified: Tue, 02 Aug 2022 09:06:35 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92aa5fa40d59f1ec7c03fe65eb4b883b20d3d0ea67ed7c851c517f130c1ae1d`  
		Last Modified: Tue, 02 Aug 2022 09:06:37 GMT  
		Size: 11.0 MB (10989120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92822a27607fdc0df8a9d0ac671b5c1aa28e1e3c7af6fcee9ec69de32b431b64`  
		Last Modified: Tue, 02 Aug 2022 09:06:35 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336d246ed12562d67aa00a07438009e6491c351feb0eab36d7739f4ed1fed63d`  
		Last Modified: Tue, 02 Aug 2022 09:06:35 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09707a3fd23ee419f459117c20d2cd79d74e4670b3ce6009dcf228c9dbde1424`  
		Last Modified: Tue, 02 Aug 2022 09:06:36 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:apache-buster` - linux; arm variant v5

```console
$ docker pull php@sha256:6735891ebe1106057fc9e1af212932170d736df17d4eb218bea075f05fb69967
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.8 MB (123815781 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acc79bff956b795fabfad88f2058a1a92dea3c9fe0f03bf2d341d767dc564e5e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Jul 2022 00:51:40 GMT
ADD file:ae02bb368b4b8ce35a4d250031394d4c6d9e5be3b02168f34922bd87dd2bc726 in / 
# Tue, 12 Jul 2022 00:51:40 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 18:54:49 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Jul 2022 18:54:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Jul 2022 18:55:43 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 18:55:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Jul 2022 18:55:45 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Jul 2022 19:01:41 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Jul 2022 19:01:41 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Jul 2022 19:02:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Jul 2022 19:02:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Jul 2022 19:02:07 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 12 Jul 2022 19:02:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jul 2022 19:02:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jul 2022 19:02:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Jul 2022 19:47:39 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 12 Jul 2022 19:47:40 GMT
ENV PHP_VERSION=8.1.8
# Tue, 12 Jul 2022 19:47:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Tue, 12 Jul 2022 19:47:41 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Tue, 12 Jul 2022 19:48:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Jul 2022 19:48:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:53:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 12 Jul 2022 19:53:27 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:53:28 GMT
RUN docker-php-ext-enable sodium
# Tue, 12 Jul 2022 19:53:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 12 Jul 2022 19:53:29 GMT
STOPSIGNAL SIGWINCH
# Tue, 12 Jul 2022 19:53:30 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 12 Jul 2022 19:53:30 GMT
WORKDIR /var/www/html
# Tue, 12 Jul 2022 19:53:31 GMT
EXPOSE 80
# Tue, 12 Jul 2022 19:53:31 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:e0c9a5e64041e18deb764eddbdc6c3d20b76797d8c2e2eb4c60d4cba21dc486e`  
		Last Modified: Tue, 12 Jul 2022 01:04:31 GMT  
		Size: 24.9 MB (24889765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dda97e7ce4e24751b4bc833f5d486ba6c9100caa19588af9dd0247ee10e03a2c`  
		Last Modified: Tue, 12 Jul 2022 21:43:24 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd44d4534ecfe92973ddb2cb0841ee60605b77232c71d4cbebb4373b90b5e9fd`  
		Last Modified: Tue, 12 Jul 2022 21:44:05 GMT  
		Size: 58.8 MB (58827228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:211aba584a39baf6785185cd5f9e74fbc6b997cde6102cf559c96d50115e7e6f`  
		Last Modified: Tue, 12 Jul 2022 21:43:24 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c635b46f95555615558c75d0d9b572dc3c31d245dd10e5ef2b48176682a2b5`  
		Last Modified: Tue, 12 Jul 2022 21:44:37 GMT  
		Size: 18.0 MB (18023958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20a788fa26e97efc9007cfa56ec9ff67726843d1c3e5a11ced4fabb38932f45a`  
		Last Modified: Tue, 12 Jul 2022 21:44:27 GMT  
		Size: 476.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f081795e7e8fd7b76e74c42de9dd87f98ecfdca372287f7b5e7f5a54e48d7c`  
		Last Modified: Tue, 12 Jul 2022 21:44:27 GMT  
		Size: 516.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bd2706aed6a3c2a74a8ec302ac09e4d2488c83789a5c56a9d192fbf5ae4b69`  
		Last Modified: Tue, 12 Jul 2022 21:50:46 GMT  
		Size: 12.1 MB (12058823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c504acf5a79ab51db6da8e5ea538bb2c4273a9233e9e43e4a8e2ab4e73936d98`  
		Last Modified: Tue, 12 Jul 2022 21:50:41 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3f7067abe97fd97177f18b6df0fced3fa81691eae4c23c428f903e4a7953ad5`  
		Last Modified: Tue, 12 Jul 2022 21:50:48 GMT  
		Size: 10.0 MB (10010426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd2c0dda193d529fd2ce0dee6c7a99c7a921f6e0cba49ce3f7a7c1d5d1d60fa`  
		Last Modified: Tue, 12 Jul 2022 21:50:41 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b673ace52f99f853b83bdf6f28354c8ec92bb4baf1abb3b2c6fddea31a4c0c`  
		Last Modified: Tue, 12 Jul 2022 21:50:41 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971ea54fa597d4c2d2c0d54c55daf1a8ec1df617307ac458559cff4605663610`  
		Last Modified: Tue, 12 Jul 2022 21:50:41 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:apache-buster` - linux; arm variant v7

```console
$ docker pull php@sha256:d279f165878501c8bd9749acb81c7fa91aa54d72e68905e5314ee04b004c4305
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.3 MB (121327443 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3f5745ea9d067f1bdd20cfb8452ad346395e34370ead40cb3d7b9f683fccc3d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Jul 2022 01:01:01 GMT
ADD file:973159cf2de6d7890ce8caf5c207ff8c15c19c5b6ea8dff5ff223a1cf75e3f60 in / 
# Tue, 12 Jul 2022 01:01:02 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 11:18:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Jul 2022 11:19:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Jul 2022 11:19:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 11:19:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Jul 2022 11:19:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Jul 2022 11:25:07 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Jul 2022 11:25:07 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Jul 2022 11:25:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Jul 2022 11:25:31 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Jul 2022 11:25:32 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 12 Jul 2022 11:25:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jul 2022 11:25:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jul 2022 11:25:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Jul 2022 12:07:27 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 12 Jul 2022 12:07:27 GMT
ENV PHP_VERSION=8.1.8
# Tue, 12 Jul 2022 12:07:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Tue, 12 Jul 2022 12:07:28 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Tue, 12 Jul 2022 12:07:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Jul 2022 12:07:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 12 Jul 2022 12:12:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 12 Jul 2022 12:12:38 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 12 Jul 2022 12:12:39 GMT
RUN docker-php-ext-enable sodium
# Tue, 12 Jul 2022 12:12:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 12 Jul 2022 12:12:40 GMT
STOPSIGNAL SIGWINCH
# Tue, 12 Jul 2022 12:12:41 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 12 Jul 2022 12:12:41 GMT
WORKDIR /var/www/html
# Tue, 12 Jul 2022 12:12:42 GMT
EXPOSE 80
# Tue, 12 Jul 2022 12:12:42 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:8031e2dc59e1b5a08ece8056d69de81b33dd5912c374507a775965a83ce367a8`  
		Last Modified: Tue, 12 Jul 2022 01:14:01 GMT  
		Size: 22.7 MB (22748029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d51ad527283699db749d8be4f8ef2a86d697365708e6c762de9f1529a02607`  
		Last Modified: Tue, 12 Jul 2022 14:07:05 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdc6b56980864e305b2dc2d20081a0a8ae1c722a0042336b1e4ecfc2b394f0b`  
		Last Modified: Tue, 12 Jul 2022 14:07:42 GMT  
		Size: 59.5 MB (59539377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce2b27d4ef22818fb817435acdf089af2a0a6f385059ac83dec79492abca387`  
		Last Modified: Tue, 12 Jul 2022 14:07:05 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db9f7cb4b7dcb8c366d491d6ddc2341d5bffe0016eb0aab4563c932b155452d`  
		Last Modified: Tue, 12 Jul 2022 14:08:13 GMT  
		Size: 17.5 MB (17479592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6e21070beb721bb0448eca063762d199e0e7e0b0bcc5cea2e73cd7bea36530`  
		Last Modified: Tue, 12 Jul 2022 14:08:04 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78fbc7aa6a4a8e04ade9bbefa2d3976877b756c431b32a786ee89adf686e6fb4`  
		Last Modified: Tue, 12 Jul 2022 14:08:03 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4feb13466d9859451f51fc9968e11f6f95aac6b66de22627b79177a261d3ea3`  
		Last Modified: Tue, 12 Jul 2022 14:14:51 GMT  
		Size: 12.1 MB (12058839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76966485385fd98403a376d5723790cc1e4e7007b1758dd17edd25e50f5cd08f`  
		Last Modified: Tue, 12 Jul 2022 14:14:45 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a73f6b5a53712b484d43de91c117680af6379adc8e1f551b35b86d9a92eb2d6`  
		Last Modified: Tue, 12 Jul 2022 14:14:52 GMT  
		Size: 9.5 MB (9496022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271bf91452ae1a1d2da6058343cec059f80bf8ceb66fe865307ae5fc2109049d`  
		Last Modified: Tue, 12 Jul 2022 14:14:45 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0f2db7d97f9b4a71d6bec2489375876eeef49e3164b2389bbd85887ee0c5ac5`  
		Last Modified: Tue, 12 Jul 2022 14:14:45 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:433bb5874f8498e9eb856a6f730835f053a15f3a19060e07a64eba6d934cc6d1`  
		Last Modified: Tue, 12 Jul 2022 14:14:45 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:apache-buster` - linux; arm64 variant v8

```console
$ docker pull php@sha256:b2df43f22457fa3b32bcceb777b646971b6c083607c732f20253a6a12c3e47d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.6 MB (137561743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d41640d52d0f5573e67cd55b74920a14a99aa434b0120d1e85a168811e1c221b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Jul 2022 00:41:02 GMT
ADD file:d6b43ca12a2cc7f73a66ace962f04878f02eab9345172028d77c21d3dc94fe0c in / 
# Tue, 12 Jul 2022 00:41:03 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 07:22:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Jul 2022 07:22:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Jul 2022 07:23:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 07:23:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Jul 2022 07:23:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Jul 2022 07:27:13 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Jul 2022 07:27:14 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Jul 2022 07:27:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Jul 2022 07:27:24 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Jul 2022 07:27:25 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 12 Jul 2022 07:27:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jul 2022 07:27:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jul 2022 07:27:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Jul 2022 08:00:22 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 12 Jul 2022 08:00:23 GMT
ENV PHP_VERSION=8.1.8
# Tue, 12 Jul 2022 08:00:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Tue, 12 Jul 2022 08:00:25 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Tue, 12 Jul 2022 08:00:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Jul 2022 08:00:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 12 Jul 2022 08:04:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 12 Jul 2022 08:04:22 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 12 Jul 2022 08:04:23 GMT
RUN docker-php-ext-enable sodium
# Tue, 12 Jul 2022 08:04:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 12 Jul 2022 08:04:24 GMT
STOPSIGNAL SIGWINCH
# Tue, 12 Jul 2022 08:04:26 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 12 Jul 2022 08:04:26 GMT
WORKDIR /var/www/html
# Tue, 12 Jul 2022 08:04:27 GMT
EXPOSE 80
# Tue, 12 Jul 2022 08:04:28 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:8bd5501da4f4b37ad7488bd0eafa32d8927de3bf1e32747545810f2ca65429ed`  
		Last Modified: Tue, 12 Jul 2022 00:47:14 GMT  
		Size: 25.9 MB (25914236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07cd63c5e4269e0b39fb91a87e09f47db678c328c4084cb07b21b5b70960d19`  
		Last Modified: Tue, 12 Jul 2022 09:07:19 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee40b52d5c59449185b4bb51a85f5ca11dbf210034e70475b305b30f1bdf22b`  
		Last Modified: Tue, 12 Jul 2022 09:07:29 GMT  
		Size: 70.4 MB (70364196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cf2b4b2a081b200b482f1d7354d71528cb993d7122a64d0cafe6f35f16c4ea`  
		Last Modified: Tue, 12 Jul 2022 09:07:18 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92316c4ae80e6255aec86b059f1511f81c0f94d48fac82ca54b8912560cc56fc`  
		Last Modified: Tue, 12 Jul 2022 09:07:51 GMT  
		Size: 18.4 MB (18366773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4767659cefe76767f66827ed7467ecf0ff2bccbf2f27f2a7d099045e4a0ede`  
		Last Modified: Tue, 12 Jul 2022 09:07:48 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d727a119900af87f25edd513d992a72b56c4adeeb04818cb73522802292e16`  
		Last Modified: Tue, 12 Jul 2022 09:07:48 GMT  
		Size: 483.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5baf0948752a66c4e802dd7dc82b62716445cfa67d4e15b8f743831e832ed0`  
		Last Modified: Tue, 12 Jul 2022 09:12:15 GMT  
		Size: 11.8 MB (11846550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94a9a2571b3e07edb5c6c2f5fdc0265f53d9ba99523cc95b1bda39d12db10b2c`  
		Last Modified: Tue, 12 Jul 2022 09:12:12 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d849ea26b14fc8a6e8c83df967329a13cfc0556254975827f4ff8fa41abbe28c`  
		Last Modified: Tue, 12 Jul 2022 09:12:14 GMT  
		Size: 11.1 MB (11064535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eae4994e56e800a1f6c3b56d39591af06c3920add8d8bf9bb815f8d5582290f`  
		Last Modified: Tue, 12 Jul 2022 09:12:12 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d2d4312d3927d98d9e99bf50239b15bf560fb485138fb9ed8e6b4f68b50f23`  
		Last Modified: Tue, 12 Jul 2022 09:12:12 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81ecd57e7f253c007221d603202490b7b79fb34f4abfd3312f626db564eff5fc`  
		Last Modified: Tue, 12 Jul 2022 09:12:12 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:apache-buster` - linux; 386

```console
$ docker pull php@sha256:01893f869771dcb7fd00fbef2756d5fb5a6f9d66bf1a36604c70472ad9e48fb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.0 MB (150989776 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb5693bf694caf947abf438b26a8cf1050e6a6766b3b69f96a451959468e9af0`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:47 GMT
ADD file:e8057ee44359188db14ad06a6f8e9cab7a301b479e0f7e0e61810abb0ecf48dd in / 
# Tue, 02 Aug 2022 00:39:47 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 06:27:02 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 02 Aug 2022 06:27:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 02 Aug 2022 06:27:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 06:27:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 06:27:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 06:30:44 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 02 Aug 2022 06:30:45 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 02 Aug 2022 06:30:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 02 Aug 2022 06:30:57 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 02 Aug 2022 06:30:58 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 02 Aug 2022 06:30:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 06:31:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 06:31:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 06:56:04 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 02 Aug 2022 07:21:13 GMT
ENV PHP_VERSION=8.1.8
# Tue, 02 Aug 2022 07:21:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Tue, 02 Aug 2022 07:21:15 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Tue, 02 Aug 2022 07:21:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 02 Aug 2022 07:21:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 02 Aug 2022 07:24:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 02 Aug 2022 07:24:08 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 02 Aug 2022 07:24:08 GMT
RUN docker-php-ext-enable sodium
# Tue, 02 Aug 2022 07:24:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 02 Aug 2022 07:24:10 GMT
STOPSIGNAL SIGWINCH
# Tue, 02 Aug 2022 07:24:12 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 02 Aug 2022 07:24:12 GMT
WORKDIR /var/www/html
# Tue, 02 Aug 2022 07:24:13 GMT
EXPOSE 80
# Tue, 02 Aug 2022 07:24:14 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:0481fdd8148a195a336acc1d5b3d6b0f7fe46395e01c9b674e3ff6974b6ac5a7`  
		Last Modified: Tue, 02 Aug 2022 00:46:14 GMT  
		Size: 27.8 MB (27799555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0973877ec0e368d96bbb3d54caaf9080f69efac8ac1205ad1fca4b0f3e1baa95`  
		Last Modified: Tue, 02 Aug 2022 08:53:52 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17ae80725d2fa6408c520a61aeaba5003aac7db68a5366895410a85760dd8e48`  
		Last Modified: Tue, 02 Aug 2022 08:54:04 GMT  
		Size: 81.2 MB (81229032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74926b9b0d6874e3e293e95eb4a461b6b2b6b92dae2f8806823e84bf63401ff1`  
		Last Modified: Tue, 02 Aug 2022 08:53:57 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3cdf37a63b5bde187c7745bfb3773ec389a961c2b20304ebbfb0ad050d4ced`  
		Last Modified: Tue, 02 Aug 2022 08:54:28 GMT  
		Size: 18.9 MB (18900221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc2764b9478bc915b8afaac186e7e5a02366c350ae93ef06be2065db3b91d4a0`  
		Last Modified: Tue, 02 Aug 2022 08:54:25 GMT  
		Size: 429.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30bf93c7aabf61651dce14b064c80a90a7ca2b0fe6f476174e65d2054d938613`  
		Last Modified: Tue, 02 Aug 2022 08:54:25 GMT  
		Size: 486.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc0b822ae8c5204a733268e8a342c2b3c3c50e5b0f4c4049097ec18b4c95e766`  
		Last Modified: Tue, 02 Aug 2022 09:02:51 GMT  
		Size: 11.8 MB (11847061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b61792762c055f3c485967ba30e1c5e32a51cc2a179bd8323e295eebf91b04f`  
		Last Modified: Tue, 02 Aug 2022 09:02:47 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35d8c4d76c3e115a7ff9dc9628c1e62b93df3514f9fb5d1173adbaf5573ccc34`  
		Last Modified: Tue, 02 Aug 2022 09:02:49 GMT  
		Size: 11.2 MB (11208462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac60a67eb38f8c4097a75197f71409173aa57995fb656f69013f23349dd6ee6`  
		Last Modified: Tue, 02 Aug 2022 09:02:47 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9096786af1d715df6019d6ff777816393f98982d8f9a819f7e9c52001992d3ac`  
		Last Modified: Tue, 02 Aug 2022 09:02:47 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b97902500ed4ed8a5ac9205d689a1c4be85a64453f06fffbc71adcd6aa2f2b`  
		Last Modified: Tue, 02 Aug 2022 09:02:47 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:apache-buster` - linux; mips64le

```console
$ docker pull php@sha256:543da9fc38af7559a92d9ed32897125afffa77127d5f37b8705e2642c185c47d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.6 MB (127624308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac361c6f59fce59d29ef02b14e8139d4c1b8b20b2910a10eac7f96c716bcc7b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Jul 2022 04:42:11 GMT
ADD file:7cc67dd9da4d585d8bdaed90523c7a817bb92aac2bb1f83554f2b46a49e0e392 in / 
# Tue, 12 Jul 2022 04:42:16 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 18:00:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Jul 2022 18:00:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Jul 2022 18:02:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 18:02:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Jul 2022 18:02:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Jul 2022 18:17:20 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Jul 2022 18:17:23 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Jul 2022 18:18:26 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Jul 2022 18:18:32 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Jul 2022 18:18:39 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 12 Jul 2022 18:18:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jul 2022 18:18:45 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jul 2022 18:18:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Jul 2022 20:12:48 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 12 Jul 2022 20:12:52 GMT
ENV PHP_VERSION=8.1.8
# Tue, 12 Jul 2022 20:12:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Tue, 12 Jul 2022 20:12:59 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Tue, 12 Jul 2022 20:13:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Jul 2022 20:13:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 12 Jul 2022 20:27:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 12 Jul 2022 20:27:24 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 12 Jul 2022 20:27:31 GMT
RUN docker-php-ext-enable sodium
# Tue, 12 Jul 2022 20:27:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 12 Jul 2022 20:27:38 GMT
STOPSIGNAL SIGWINCH
# Tue, 12 Jul 2022 20:27:41 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 12 Jul 2022 20:27:45 GMT
WORKDIR /var/www/html
# Tue, 12 Jul 2022 20:27:49 GMT
EXPOSE 80
# Tue, 12 Jul 2022 20:27:52 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:33fe211fd200b2017da34e0864d2aff58d6963435c4b3b7d15083f6860c2fe1e`  
		Last Modified: Tue, 12 Jul 2022 04:53:03 GMT  
		Size: 25.8 MB (25814577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f66bc37a8a5a6ccb7789f7306b3e70d56e0906eebf85b931830430a044a1cdf`  
		Last Modified: Wed, 13 Jul 2022 00:17:28 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e689156b0e5680ea5c4bf308a89ca47e317fe5b89ae8ef93ca51501b2d44c1f7`  
		Last Modified: Wed, 13 Jul 2022 00:18:16 GMT  
		Size: 61.4 MB (61409281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1917000b7bf5b948c06b04a5cb02b207b93ab7c25deab6fc203b8a187bedd823`  
		Last Modified: Wed, 13 Jul 2022 00:17:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b85ef42cd66e62484341a7944dc4213a1aa8e1eee5e9b6044a6c2bb633f6cb6`  
		Last Modified: Wed, 13 Jul 2022 00:18:49 GMT  
		Size: 18.4 MB (18402053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e557c2ea25f789a5dbe91cf85411f4c431e598318d18a5acbcd316194ef61451`  
		Last Modified: Wed, 13 Jul 2022 00:18:36 GMT  
		Size: 437.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7a90dce28b5b38b478ad80a3dc1997baba1201c5aa219483be17af7836356c`  
		Last Modified: Wed, 13 Jul 2022 00:18:36 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5310fc83f468a2731ea2ecd90b67945d072140fcb8a046c2bfda7c6064609489`  
		Last Modified: Wed, 13 Jul 2022 00:24:12 GMT  
		Size: 11.8 MB (11845549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2420806dfe45597fc77ac335d39435246dd3ddf2f0c3e1431256f4eef4a284af`  
		Last Modified: Wed, 13 Jul 2022 00:24:06 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792056853cdf31e133b5fe7c75fd5d3c463ee090884ab730e5443fa9b82a3de0`  
		Last Modified: Wed, 13 Jul 2022 00:24:16 GMT  
		Size: 10.1 MB (10147374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0af5a87bba63f0dbcca36993069bcef728fefa0b8c4af7857fc3aed835623f7`  
		Last Modified: Wed, 13 Jul 2022 00:24:06 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bbed56c9d22c4a6f7e34ea5b1a1015269948188c7f4dbb7fc33fe1652cccd75`  
		Last Modified: Wed, 13 Jul 2022 00:24:07 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4e8ee7502e91a2a72681ed954d2762394e735be57c6f7fb36cd78a3a8e8fa5`  
		Last Modified: Wed, 13 Jul 2022 00:24:07 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:apache-buster` - linux; ppc64le

```console
$ docker pull php@sha256:7130d4ea94c62c117f69711fec4e8f2caa9b453a52d363d44a2b7edd219f84c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.1 MB (156121190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eaf5a4b8c4ca11cf0f27244275ae59c0aa9f9793b5dbf58f739ba5bbab4b763`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 12 Jul 2022 01:26:17 GMT
ADD file:a6b8aff01d22eb4bfa373d809109de5f0a6a7cf7327f2f711c368ba2ecfcb529 in / 
# Tue, 12 Jul 2022 01:26:25 GMT
CMD ["bash"]
# Tue, 12 Jul 2022 17:17:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 12 Jul 2022 17:17:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 12 Jul 2022 17:19:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 12 Jul 2022 17:19:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Jul 2022 17:19:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 12 Jul 2022 17:25:14 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 12 Jul 2022 17:25:17 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 12 Jul 2022 17:26:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 12 Jul 2022 17:26:20 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 12 Jul 2022 17:26:25 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 12 Jul 2022 17:26:28 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jul 2022 17:26:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Jul 2022 17:26:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Jul 2022 18:14:09 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 12 Jul 2022 18:14:14 GMT
ENV PHP_VERSION=8.1.8
# Tue, 12 Jul 2022 18:14:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Tue, 12 Jul 2022 18:14:21 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Tue, 12 Jul 2022 18:15:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 12 Jul 2022 18:15:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 12 Jul 2022 18:20:52 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 12 Jul 2022 18:20:55 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 12 Jul 2022 18:21:02 GMT
RUN docker-php-ext-enable sodium
# Tue, 12 Jul 2022 18:21:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 12 Jul 2022 18:21:07 GMT
STOPSIGNAL SIGWINCH
# Tue, 12 Jul 2022 18:21:08 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 12 Jul 2022 18:21:10 GMT
WORKDIR /var/www/html
# Tue, 12 Jul 2022 18:21:14 GMT
EXPOSE 80
# Tue, 12 Jul 2022 18:21:21 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:6397b3c9c600936bac0b5fca48461dde424703aa59318fe69c30e207bad2e0b7`  
		Last Modified: Tue, 12 Jul 2022 01:38:08 GMT  
		Size: 30.6 MB (30560087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5247c6c7f3405e665f0ee64b8c43a9a738d8b33a17a709278c490d790a7eeae`  
		Last Modified: Tue, 12 Jul 2022 20:10:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a42d2d05cc16c0571707b33f217fa8b90d2050d370dd4306ddc65192cc23d37`  
		Last Modified: Tue, 12 Jul 2022 20:10:49 GMT  
		Size: 82.3 MB (82293843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9df172e090f85365ea48c1d319e473ebd186a1297bdacb558a0612e0a5616b4b`  
		Last Modified: Tue, 12 Jul 2022 20:10:34 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4431df9016610777bc4477aad3ad16aebb673af44b53f1dea44124075ed159a1`  
		Last Modified: Tue, 12 Jul 2022 20:11:19 GMT  
		Size: 19.8 MB (19821961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e14b9ecf8db84c1d64097bdd1689dfa64e068690173e12e05aaa71a928bfae`  
		Last Modified: Tue, 12 Jul 2022 20:11:15 GMT  
		Size: 479.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef377b001b728b66e46a5398137da7f9df2a13b81343d057ab77e5badc917f1`  
		Last Modified: Tue, 12 Jul 2022 20:11:14 GMT  
		Size: 519.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b6cff1830df85c5d5dee6c3cdc2e6c7f975f2e227e484b4d9d1a1620494e70`  
		Last Modified: Tue, 12 Jul 2022 20:16:20 GMT  
		Size: 12.1 MB (12060443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9d6a8d8abe4d7a9ad38ba0f2a8df32d1f1e2cfe3e39d7a474307c8ec47f194`  
		Last Modified: Tue, 12 Jul 2022 20:16:16 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15525321c12ad95adf2191f73cfe2febadf4dfb5d3ecb09b719b8741b542b22c`  
		Last Modified: Tue, 12 Jul 2022 20:16:19 GMT  
		Size: 11.4 MB (11379267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34ec4808a79a295330f6e5365b2dcd439dc3b57b0021aac49b11230d1feac9db`  
		Last Modified: Tue, 12 Jul 2022 20:16:16 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f3b917ad914b1d348b78f1ac539ef6b4654e35ebf03406b1063c2a1082bdb9`  
		Last Modified: Tue, 12 Jul 2022 20:16:16 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f037249210986788ddf423715861ecbfa391a517835ae9b93965b956d8f49ee7`  
		Last Modified: Tue, 12 Jul 2022 20:16:16 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:apache-buster` - linux; s390x

```console
$ docker pull php@sha256:fc1a392dbb667c6bed771ecc64711fe0bd71fbb096e706863ae842a900f3dac8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **131.2 MB (131181974 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c28156b4d8090d4d6165fe5448b2b9700bd0a2f876efd43ab9c94b0f419f65fa`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:56 GMT
ADD file:e455828726a550da92d8fc424a6d7694b6be24a8ca52a6152e2ee89d4f7269d0 in / 
# Tue, 02 Aug 2022 00:42:58 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 05:59:56 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 02 Aug 2022 05:59:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 02 Aug 2022 06:00:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 02 Aug 2022 06:00:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 06:00:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 06:02:30 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 02 Aug 2022 06:02:30 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 02 Aug 2022 06:02:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 02 Aug 2022 06:02:40 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 02 Aug 2022 06:02:41 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 02 Aug 2022 06:02:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 06:02:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 06:02:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 06:21:41 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 02 Aug 2022 06:40:41 GMT
ENV PHP_VERSION=8.1.8
# Tue, 02 Aug 2022 06:40:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Tue, 02 Aug 2022 06:40:41 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Tue, 02 Aug 2022 06:40:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 02 Aug 2022 06:40:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 02 Aug 2022 06:42:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 02 Aug 2022 06:42:46 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 02 Aug 2022 06:42:47 GMT
RUN docker-php-ext-enable sodium
# Tue, 02 Aug 2022 06:42:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 02 Aug 2022 06:42:47 GMT
STOPSIGNAL SIGWINCH
# Tue, 02 Aug 2022 06:42:47 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 02 Aug 2022 06:42:47 GMT
WORKDIR /var/www/html
# Tue, 02 Aug 2022 06:42:47 GMT
EXPOSE 80
# Tue, 02 Aug 2022 06:42:47 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:42614a0fa81c110340e6a5a5db155f27bbb6fa8c1e2421b2c2c5f148ea18f35d`  
		Last Modified: Tue, 02 Aug 2022 00:48:34 GMT  
		Size: 25.8 MB (25758761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b883a6875d4e368b4bac4f0112f3089a46a1b787117a10d7b9c13b284461cc6e`  
		Last Modified: Tue, 02 Aug 2022 07:55:00 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d72faaa2585bc85fd3828a007751f375a7354083d59b6895fd7e9528758c941a`  
		Last Modified: Tue, 02 Aug 2022 07:55:08 GMT  
		Size: 64.7 MB (64727260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d16fc92b1be1519e28ae95cf7c480ddda56ba96844d45aa689a012c289d2cda`  
		Last Modified: Tue, 02 Aug 2022 07:54:59 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd805f68adb2f93985a3f306cedb1bf77ebfd66fe6984291db3d5a6a89d9cbf1`  
		Last Modified: Tue, 02 Aug 2022 07:55:22 GMT  
		Size: 18.5 MB (18524893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ce084dfaa29d07ab07a038f6e536f64facce2b7ef90a94be44fba73089d6a7`  
		Last Modified: Tue, 02 Aug 2022 07:55:20 GMT  
		Size: 482.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e1c5049ce8c76b5499cd5f3007af36e555303f6d28297faf67b7f8100d4b2b0`  
		Last Modified: Tue, 02 Aug 2022 07:55:19 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ae8e69573ac715796c13cfa6af7b67db71239a3be25e0ac140f890af2bc7d0`  
		Last Modified: Tue, 02 Aug 2022 08:00:06 GMT  
		Size: 12.1 MB (12059098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0ad8153201aedce54e54320bab1309d31b479b2f0df7070d28d11bbcf21248`  
		Last Modified: Tue, 02 Aug 2022 08:00:05 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5297b65387698621b13db61c4c1e21f4eb0a1ff234202be43b70729ab4f1ae5`  
		Last Modified: Tue, 02 Aug 2022 08:00:06 GMT  
		Size: 10.1 MB (10106384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e92d9902275c965a486e9f304ee40c720fb61b78e011052b81f6d3ba4a9d3ab2`  
		Last Modified: Tue, 02 Aug 2022 08:00:04 GMT  
		Size: 2.5 KB (2458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79081493b2edf2375840f00eed06223fc66243bad3fe3d0ef1083bb9acba9199`  
		Last Modified: Tue, 02 Aug 2022 08:00:04 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c313ca71f15847b34be4a882c2b00561087c13dc91da06e32ade2999a9a1b7`  
		Last Modified: Tue, 02 Aug 2022 08:00:04 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
