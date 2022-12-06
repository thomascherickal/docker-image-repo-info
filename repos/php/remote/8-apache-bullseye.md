## `php:8-apache-bullseye`

```console
$ docker pull php@sha256:86b3a13ce3fc22e75b650520170d48fa98de5145caa0a1fd86edf534fd73f65d
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

### `php:8-apache-bullseye` - linux; amd64

```console
$ docker pull php@sha256:9e6e873c3f9fa0a9ea35d82982dbdee9026ce411450dd41fbea765c66b443d0f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.5 MB (165492813 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b26e8ec6140e8d119f768de1f93ac4e35212bd450c7f91d74595a02b93affa29`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:04:54 GMT
ADD file:d08e242792caa7f842fcf39a09ad59c97a856660e2013d5aed3e4a29197e9aaa in / 
# Tue, 15 Nov 2022 04:04:54 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 04:12:59 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 04:12:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 04:13:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:13:21 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 04:13:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 04:16:52 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 15 Nov 2022 04:16:52 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 15 Nov 2022 04:17:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 15 Nov 2022 04:17:02 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 15 Nov 2022 04:17:03 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 15 Nov 2022 04:17:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 04:17:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 04:17:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 04:44:12 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Nov 2022 02:33:22 GMT
ENV PHP_VERSION=8.1.13
# Tue, 29 Nov 2022 02:33:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 29 Nov 2022 02:33:22 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 29 Nov 2022 02:33:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Nov 2022 02:33:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:36:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Nov 2022 02:36:35 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:36:36 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Nov 2022 02:36:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Nov 2022 02:36:36 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Nov 2022 02:36:36 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:36:36 GMT
WORKDIR /var/www/html
# Tue, 29 Nov 2022 02:36:36 GMT
EXPOSE 80
# Tue, 29 Nov 2022 02:36:36 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:a603fa5e3b4127f210503aaa6189abf6286ee5a73deeaab460f8f33ebc6b64e2`  
		Last Modified: Tue, 15 Nov 2022 04:08:47 GMT  
		Size: 31.4 MB (31412630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c428f1a494230852524a2a5957cc5199c36c8b403305e0e877d580bd0ec9e763`  
		Last Modified: Tue, 15 Nov 2022 06:23:17 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:156740b07ef8a632f9f7bea4e57e4ee5541ade376adf9169351a1265382e39de`  
		Last Modified: Tue, 15 Nov 2022 06:23:30 GMT  
		Size: 91.6 MB (91634870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5a4c8af82f00730b7427e47bda7f76cea2e2b9aea421750bc9025aface98d8`  
		Last Modified: Tue, 15 Nov 2022 06:23:16 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25f85b498fd5bfc6cce951513219fe480850daba71e6e997741e984d18483971`  
		Last Modified: Tue, 15 Nov 2022 06:23:58 GMT  
		Size: 19.2 MB (19245291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b233e420ac7bbca645bb82c213029762acf1742400c076360dc303213c309d5`  
		Last Modified: Tue, 15 Nov 2022 06:23:55 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe42347c4ecfc90333acd9cad13912387eea39d13827a25cfa78727fa5d200e9`  
		Last Modified: Tue, 15 Nov 2022 06:23:56 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546eb18c40c63cf7ab23f9812d8d96ab7b85a79a423fb953348787b234d4cbbd`  
		Last Modified: Tue, 29 Nov 2022 04:17:31 GMT  
		Size: 12.1 MB (12144909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f9832512fc31373964282941d541778192758efb24c10f41cdb40a75802f36f`  
		Last Modified: Tue, 29 Nov 2022 04:17:28 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41b8e6bd463d8572766b5f5dc7962b74d8bd02e308f21b37c7591200c0723f0`  
		Last Modified: Tue, 29 Nov 2022 04:17:31 GMT  
		Size: 11.0 MB (11049529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9efb162a08fd96a21c5cb4f6a722b986e22e55aaed6e40026be0d1724510e55`  
		Last Modified: Tue, 29 Nov 2022 04:17:29 GMT  
		Size: 2.5 KB (2461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1c69b269028f8e56e39c7b25db28881f0faa3b214dc82a74769b05070677d8`  
		Last Modified: Tue, 29 Nov 2022 04:17:29 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff1edc4d072cdff50c31f427cffd4670da69f935a98b841115433037e9abfd0`  
		Last Modified: Tue, 29 Nov 2022 04:17:29 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache-bullseye` - linux; arm variant v5

```console
$ docker pull php@sha256:b6f5c6ae5d4b87d2174f7a782f51ca45eb64bcefeabab62933a8a2269c2a306f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.4 MB (143371454 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4058c37f70f985dbb5f82b0d04d8d24d2076ddd706c834c6b8a36252d71ce024`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:49:18 GMT
ADD file:1949af7e583a1b54055a421129c32315fc101e53e2cda05da3171ed461bde0a6 in / 
# Tue, 15 Nov 2022 01:49:19 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 01:57:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 01:57:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 01:58:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 01:58:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 01:58:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 02:01:52 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 15 Nov 2022 02:01:52 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 15 Nov 2022 02:02:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 15 Nov 2022 02:02:06 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 15 Nov 2022 02:02:07 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 15 Nov 2022 02:02:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 02:02:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 02:02:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 02:17:59 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Nov 2022 02:11:13 GMT
ENV PHP_VERSION=8.1.13
# Tue, 29 Nov 2022 02:11:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 29 Nov 2022 02:11:13 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 29 Nov 2022 02:11:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Nov 2022 02:11:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:15:06 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Nov 2022 02:15:07 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:15:08 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Nov 2022 02:15:08 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Nov 2022 02:15:09 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Nov 2022 02:15:09 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:15:09 GMT
WORKDIR /var/www/html
# Tue, 29 Nov 2022 02:15:09 GMT
EXPOSE 80
# Tue, 29 Nov 2022 02:15:09 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:b56836d864a6d857be3d12242b65962f2a2cf0d77c48cfb85bbbdf9d56a7e93d`  
		Last Modified: Tue, 15 Nov 2022 01:54:26 GMT  
		Size: 28.9 MB (28914126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf8f13a67ff628e982fa37f19e46a30b6c95f885b9caf0fe288d9e44fc0fe23`  
		Last Modified: Tue, 15 Nov 2022 03:18:33 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0b67f60155678149aec805bafe02c6067447f321279766240c3ae4d1bf9745`  
		Last Modified: Tue, 15 Nov 2022 03:18:47 GMT  
		Size: 73.7 MB (73687967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ee4232fc94727d61967ec10566bb2eb1be8604bec5ccee5d4cbf30b97fac1a7`  
		Last Modified: Tue, 15 Nov 2022 03:18:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34b8b60e851c4b269f4b5712234fdb5bf26b82175012efee89f2a93b46332cc`  
		Last Modified: Tue, 15 Nov 2022 03:19:23 GMT  
		Size: 18.6 MB (18554768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6920c0af9b512e8602f43052e8093089a43c2340e4061dacfa39bcd3b17efce4`  
		Last Modified: Tue, 15 Nov 2022 03:19:20 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0590765527cfdc9d56faac74f8393f036bf4d551848b5657bcdd822c34fd4be`  
		Last Modified: Tue, 15 Nov 2022 03:19:20 GMT  
		Size: 486.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b50765088e5c4a07668a1324db6f4d95e750f957aa09e1470347dd1e4602fc2`  
		Last Modified: Tue, 29 Nov 2022 02:54:27 GMT  
		Size: 12.1 MB (12143384 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca35e769fa2d1451b63e6d4e80eb548b994eca145550d9201889e7b5fb1b0fc`  
		Last Modified: Tue, 29 Nov 2022 02:54:24 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd45287d6b94733857fdbe10c07bd2d1c3b4e0440f521946fc08d2f1c7f3269`  
		Last Modified: Tue, 29 Nov 2022 02:54:27 GMT  
		Size: 10.1 MB (10065748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c128d48332f3660486926557a7e32c97a097b0515975d2ccaf7b084a5ecebe`  
		Last Modified: Tue, 29 Nov 2022 02:54:24 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86eb311fe24e4228d5431f0011427260b5c402327c3c51a536d246bb67b2a6cd`  
		Last Modified: Tue, 29 Nov 2022 02:54:24 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c14a5132717e1e2218db7273da69749e16dc295e085eafc3daab92f8ddef79e`  
		Last Modified: Tue, 29 Nov 2022 02:54:24 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache-bullseye` - linux; arm variant v7

```console
$ docker pull php@sha256:03974871afe0865c65741e8fa0ab3a84776b9e35a90273ddf1a478c3364040cc
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.6 MB (135581856 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cccf91fe6bcfd8f7b20758aea3d456c2abe9a8d8e7c8d6314305cd8e3c902b1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:25 GMT
ADD file:1b5c939bd2a35667d7fc44c3009a56ed92a932f512a73df1617dec6ccbd6e6b1 in / 
# Tue, 15 Nov 2022 03:43:26 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 03:55:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 03:55:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 03:56:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 03:56:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 03:56:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 03:58:58 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 15 Nov 2022 03:58:58 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 15 Nov 2022 03:59:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 15 Nov 2022 03:59:10 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 15 Nov 2022 03:59:10 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 15 Nov 2022 03:59:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 03:59:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 03:59:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 04:23:37 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Nov 2022 03:33:42 GMT
ENV PHP_VERSION=8.1.13
# Tue, 29 Nov 2022 03:33:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 29 Nov 2022 03:33:42 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 29 Nov 2022 03:33:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Nov 2022 03:33:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Nov 2022 03:36:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Nov 2022 03:36:38 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Nov 2022 03:36:39 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Nov 2022 03:36:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Nov 2022 03:36:39 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Nov 2022 03:36:39 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Nov 2022 03:36:39 GMT
WORKDIR /var/www/html
# Tue, 29 Nov 2022 03:36:40 GMT
EXPOSE 80
# Tue, 29 Nov 2022 03:36:40 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:fd18d0201d0ce0c5e103902d894f5d601fc5dde76688aa7dae786840141d23e4`  
		Last Modified: Tue, 15 Nov 2022 03:50:11 GMT  
		Size: 26.6 MB (26576195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9882e3666a8ea23dcd83cf24efee4c2bc629f92dcf64bbfb5c9323497a250bd`  
		Last Modified: Tue, 15 Nov 2022 06:04:52 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc118326146d74f82c6277eb8df1029bf3b7f96486d7830fea19631b696893be`  
		Last Modified: Tue, 15 Nov 2022 06:05:05 GMT  
		Size: 69.3 MB (69320668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823b0bab372d5757e3e8f322d5ca5aefbd8984c35bed9771179b5de70ac8aad0`  
		Last Modified: Tue, 15 Nov 2022 06:04:52 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821aad38acd8081587ed34af24add9d0aa67c574e056373044edf7b1429ad4d2`  
		Last Modified: Tue, 15 Nov 2022 06:05:41 GMT  
		Size: 18.0 MB (17998468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee6391212ad86f9de174ba9712196fdf9d7387c2673b491a78fb937af64feadc`  
		Last Modified: Tue, 15 Nov 2022 06:05:38 GMT  
		Size: 434.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06b1d20f19b4c6453c4bc0e3ba102bb3a3daa81fa53828e516ce1838fae1d4e9`  
		Last Modified: Tue, 15 Nov 2022 06:05:38 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7332c9ba03b4af5841716e67cd69ab0091496048e4b45931430e7724556835b0`  
		Last Modified: Tue, 29 Nov 2022 05:24:03 GMT  
		Size: 12.1 MB (12143385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4677392631df9d4ebafbe386dac2e2305a7fc616d6d7ee50f108cddbaa89a8`  
		Last Modified: Tue, 29 Nov 2022 05:24:00 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db91bdd42b012beaac2545ae76d211223b04f7742f0bf0e64e92bf2af7456538`  
		Last Modified: Tue, 29 Nov 2022 05:24:02 GMT  
		Size: 9.5 MB (9537669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e493c94719d0f98e62048624ad8e6aaa2d61273d4d543f4b50344257ec3f6b5`  
		Last Modified: Tue, 29 Nov 2022 05:24:00 GMT  
		Size: 2.5 KB (2462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:453988042e059c08843b95c36ccd6f6f021a29389227e6193ddfc79622f88962`  
		Last Modified: Tue, 29 Nov 2022 05:24:00 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556c2ace849c24d328a557e6045d91ca847e0670d0020b79818810bc37e2dc01`  
		Last Modified: Tue, 29 Nov 2022 05:24:00 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache-bullseye` - linux; arm64 variant v8

```console
$ docker pull php@sha256:765b2fe7eed728da4e5bb4e4699a03e1cd477b7edd72946d4972a62a70c41678
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.4 MB (159418416 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85b8276aaeabfbe27d53005ad9f9821080b0cf867f422d301d59169261e81eb3`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:20 GMT
ADD file:1dad2420090b3d6ef5df8d1f7f2878b22f8687b8dba008a63800f6c74b36dee9 in / 
# Tue, 15 Nov 2022 01:41:20 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 01:58:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 01:58:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 01:58:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 01:58:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 01:58:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 02:01:50 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 15 Nov 2022 02:01:50 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 15 Nov 2022 02:01:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 15 Nov 2022 02:01:58 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 15 Nov 2022 02:01:59 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 15 Nov 2022 02:01:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 02:01:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 02:01:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 02:26:21 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Nov 2022 02:45:16 GMT
ENV PHP_VERSION=8.1.13
# Tue, 29 Nov 2022 02:45:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 29 Nov 2022 02:45:16 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 29 Nov 2022 02:45:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Nov 2022 02:45:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:48:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Nov 2022 02:48:17 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:48:18 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Nov 2022 02:48:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Nov 2022 02:48:18 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Nov 2022 02:48:18 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:48:18 GMT
WORKDIR /var/www/html
# Tue, 29 Nov 2022 02:48:18 GMT
EXPOSE 80
# Tue, 29 Nov 2022 02:48:18 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:f3ac85625e767ee0ec42b5a2ef93880251cd973b86f77124c4ed39bccd2f8bf9`  
		Last Modified: Tue, 15 Nov 2022 01:44:35 GMT  
		Size: 30.1 MB (30060605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:826c69643efc7a2fa413b41d83553f587c092a532d2d6582de3caf323e79a005`  
		Last Modified: Tue, 15 Nov 2022 03:57:53 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c4af7a39c39eedcaf52194d52f333a71017ffe436a4e3725ebeb10f91baccf`  
		Last Modified: Tue, 15 Nov 2022 03:58:04 GMT  
		Size: 86.9 MB (86928187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:946bbe7211684bcd10ae8486cd441fc15f18504b0795e1bbc3b0687b492b215e`  
		Last Modified: Tue, 15 Nov 2022 03:57:53 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48bbb37a166bb998d4d6855dd70df915916376afc2a7eb0646a4453bbd43e8d6`  
		Last Modified: Tue, 15 Nov 2022 03:58:29 GMT  
		Size: 19.2 MB (19166541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ba13601c856716cb7971ee60f01f0138236c05cadff15fd387bd5308610f98`  
		Last Modified: Tue, 15 Nov 2022 03:58:27 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63b292a06a12240a013c7c7fc0ccc4117d2e75937b72ec7aa64b77333157619`  
		Last Modified: Tue, 15 Nov 2022 03:58:27 GMT  
		Size: 510.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1c5061f94f1ee1f30ecd8038284f9501b486588d306db9ce8ddb1264ea31dca`  
		Last Modified: Tue, 29 Nov 2022 04:14:07 GMT  
		Size: 12.1 MB (12144142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e6a592874713ecbb4fcc6bd38f5443d30c759420ea92769de1b002a75dcacd4`  
		Last Modified: Tue, 29 Nov 2022 04:14:03 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c5c8b3df49d3ce74edc9bd9ccf0d52d383bbaafa2a0f33a11909411e5b4ec5`  
		Last Modified: Tue, 29 Nov 2022 04:14:05 GMT  
		Size: 11.1 MB (11113366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ebd0fc920d3cc8cee973d4e131315bf1b66b3743b18f5863ebe1ffb6177611`  
		Last Modified: Tue, 29 Nov 2022 04:14:03 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c653dc18d032da345ab2f8b88f8421d36955fc993985899ec9b16256c4e92b13`  
		Last Modified: Tue, 29 Nov 2022 04:14:03 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5fc3f7a96721c8144be619d809017709596f083ac81c45ba46eb80afdbc1ae`  
		Last Modified: Tue, 29 Nov 2022 04:14:03 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache-bullseye` - linux; 386

```console
$ docker pull php@sha256:437fa73ea5f5af8b8128beeda758f12a0ed1e7d88f3b64cc7e2e5f66994c280a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.6 MB (167625699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30ac24af6827717e6c4079ac57a3fe114218b07d2a6b0d5461402213fabbfdc1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 06 Dec 2022 01:39:52 GMT
ADD file:3912079114d3e8e334fdf795a4793a492f37989804e1148b98fafbd4eaa00b7e in / 
# Tue, 06 Dec 2022 01:39:52 GMT
CMD ["bash"]
# Tue, 06 Dec 2022 02:40:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 06 Dec 2022 02:40:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 06 Dec 2022 02:40:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 06 Dec 2022 02:40:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 06 Dec 2022 02:40:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 06 Dec 2022 02:44:12 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 06 Dec 2022 02:44:13 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 06 Dec 2022 02:44:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 06 Dec 2022 02:44:25 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 06 Dec 2022 02:44:25 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 06 Dec 2022 02:44:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 06 Dec 2022 02:44:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 06 Dec 2022 02:44:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 06 Dec 2022 03:10:39 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 06 Dec 2022 03:10:40 GMT
ENV PHP_VERSION=8.1.13
# Tue, 06 Dec 2022 03:10:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 06 Dec 2022 03:10:42 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 06 Dec 2022 03:10:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 06 Dec 2022 03:10:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 06 Dec 2022 03:13:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 06 Dec 2022 03:13:43 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 06 Dec 2022 03:13:43 GMT
RUN docker-php-ext-enable sodium
# Tue, 06 Dec 2022 03:13:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 06 Dec 2022 03:13:45 GMT
STOPSIGNAL SIGWINCH
# Tue, 06 Dec 2022 03:13:47 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 06 Dec 2022 03:13:47 GMT
WORKDIR /var/www/html
# Tue, 06 Dec 2022 03:13:48 GMT
EXPOSE 80
# Tue, 06 Dec 2022 03:13:49 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:01cb95e209fce595702ddb2b5ed266e2a01b6687efe67d201d74a5aee9595995`  
		Last Modified: Tue, 06 Dec 2022 01:45:41 GMT  
		Size: 32.4 MB (32393046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c18a0da246e8771e541d8d6d1339b6a0fa6ce9a0a8ef9b58d2505080f1828eb3`  
		Last Modified: Tue, 06 Dec 2022 04:04:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca881611a5457bc2a7abbf6bc44a8b4ffe9d0b21f823253921418bc6fec73d6`  
		Last Modified: Tue, 06 Dec 2022 04:04:13 GMT  
		Size: 92.5 MB (92511868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf32450a9988c6cd81671719c2bceb04659d8f13926fe319290b3d80ca3e80f3`  
		Last Modified: Tue, 06 Dec 2022 04:04:01 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3f7465dd13bcfb8e7ef156d90115dae644f78bb09b284b7af0d587da467086`  
		Last Modified: Tue, 06 Dec 2022 04:04:46 GMT  
		Size: 19.5 MB (19515906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2da24facdd6552155a6fdaded67c10b8c1474a77a1132d2fa9b4dedddba7291e`  
		Last Modified: Tue, 06 Dec 2022 04:04:43 GMT  
		Size: 431.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52aa81be52eb049d61327838b0f9c3ed364fae4e15b3d50676751152aa31b979`  
		Last Modified: Tue, 06 Dec 2022 04:04:44 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4ab4050867dca3c67a7d2aa85f5d7945c98167694614517c67c36536afa26b4`  
		Last Modified: Tue, 06 Dec 2022 04:08:08 GMT  
		Size: 11.9 MB (11926994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdef55aa0cc694b27ccb4b77a35e6753007c59d695d792924c2c3ba082522424`  
		Last Modified: Tue, 06 Dec 2022 04:08:05 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf59448e73050f945fbfe5acb53811c5d09791aa27b397f3116854052961f03`  
		Last Modified: Tue, 06 Dec 2022 04:08:07 GMT  
		Size: 11.3 MB (11272434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c077c6ad63222d076d17fece68c0b1c8e4549679f487540519c1f14dfa4bb7d`  
		Last Modified: Tue, 06 Dec 2022 04:08:05 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036cac5237a431e46e043cc4481448ecac825ff02ddf66b28771bda549497f20`  
		Last Modified: Tue, 06 Dec 2022 04:08:05 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a2ae584e044ca9375bb096dab9837bb5ca798fa2a65dee577e2ecf1677e9a0`  
		Last Modified: Tue, 06 Dec 2022 04:08:05 GMT  
		Size: 892.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache-bullseye` - linux; mips64le

```console
$ docker pull php@sha256:e47c88740381990cbc54cedee751a96ad0e3a548e0f22a697ed0deca2cbb9f27
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.5 MB (142516770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e49b0135ad46a925663afc069cf6bce820d328ddfda09f83ec158f24c2b63c6e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 15 Nov 2022 04:13:42 GMT
ADD file:da7bed758c1e8c14583d53792170b6f4133a408ce2966e22ce52905f5c0d55a4 in / 
# Tue, 15 Nov 2022 04:13:46 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 08:47:36 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 08:47:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 08:49:04 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 08:49:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 08:49:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 09:03:55 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 15 Nov 2022 09:03:58 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 15 Nov 2022 09:04:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 15 Nov 2022 09:04:56 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 15 Nov 2022 09:05:02 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 15 Nov 2022 09:05:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 09:05:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 09:05:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 10:02:28 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Nov 2022 03:53:29 GMT
ENV PHP_VERSION=8.1.13
# Tue, 29 Nov 2022 03:53:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 29 Nov 2022 03:53:36 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 29 Nov 2022 03:54:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Nov 2022 03:54:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Nov 2022 04:07:53 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Nov 2022 04:07:57 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Nov 2022 04:08:03 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Nov 2022 04:08:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Nov 2022 04:08:09 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Nov 2022 04:08:12 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Nov 2022 04:08:15 GMT
WORKDIR /var/www/html
# Tue, 29 Nov 2022 04:08:19 GMT
EXPOSE 80
# Tue, 29 Nov 2022 04:08:22 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:27e2cdb4ebe2b6ee11014db328a4a8a055e3dcee2e275bf3aca6f03b39a09ad5`  
		Last Modified: Tue, 15 Nov 2022 04:21:14 GMT  
		Size: 29.6 MB (29635497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9733c932444d371b8ea79e4a346179de7ebf5cc08e7a02e788c2d964ba318a`  
		Last Modified: Tue, 15 Nov 2022 13:18:33 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e5bfa08fc491ee443691797985b59230c10d6f4c1684bf69fd790b1e11aba8`  
		Last Modified: Tue, 15 Nov 2022 13:19:28 GMT  
		Size: 71.8 MB (71813700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd1c7bd207fbbf8e8defa09a29bafd9e56e40ce0a444494a7ddfd528fa9b303b`  
		Last Modified: Tue, 15 Nov 2022 13:18:33 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74fef5d41a635bfa4c5a62f132fd346c7198ce5d0a609c81eb62a8b907b53f85`  
		Last Modified: Tue, 15 Nov 2022 13:20:07 GMT  
		Size: 18.9 MB (18940009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31101283ab7fb2f430b1a51e6860dc361b56f2f812ec6f7b6d473c1d50c9a6a4`  
		Last Modified: Tue, 15 Nov 2022 13:19:54 GMT  
		Size: 438.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e11f4fe3ed709a16b703befab7b206f9562863a0bce158e29bfab71ae09b2d6`  
		Last Modified: Tue, 15 Nov 2022 13:19:54 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21be57f7c20ab45bb4d58e72d8b43f8c2d32e0c1aba02192b2a4447ac421d3c8`  
		Last Modified: Tue, 29 Nov 2022 05:35:30 GMT  
		Size: 11.9 MB (11925753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e90f3ea544359ff59cc6a5f8cba85544c0e2f45562cc46002691067c1adfeb3`  
		Last Modified: Tue, 29 Nov 2022 05:35:25 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2972e2e0980edaa68dfdfca9257baa7d95b30a20033180150ee4e2d6e037198`  
		Last Modified: Tue, 29 Nov 2022 05:35:33 GMT  
		Size: 10.2 MB (10196333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226718a5ade8709755a3e2e636e958fb3741efcb0003d453ca58e98fd162468c`  
		Last Modified: Tue, 29 Nov 2022 05:35:25 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:036270b239c9863003d4082994be3c2ba03c7a041038617b29b2bb9ffc731ebc`  
		Last Modified: Tue, 29 Nov 2022 05:35:25 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3fdcdee57e72d8f83e76440ac3e30df2c817e46f524b47db3c243afc1a1d6a`  
		Last Modified: Tue, 29 Nov 2022 05:35:25 GMT  
		Size: 896.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache-bullseye` - linux; ppc64le

```console
$ docker pull php@sha256:f453dea6663946d9039c9db9c4f9872a93231a4dd232e408f5420826909a845b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.0 MB (165976269 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a583f978946cbd1fad4bdbbaaacbc5736f6f04a074b16ddaadb338aa4037083`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 15 Nov 2022 05:18:45 GMT
ADD file:520926164fdc762143905745329e568c67289232bec450e48645d82a4613dccf in / 
# Tue, 15 Nov 2022 05:18:47 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 05:28:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 05:28:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 05:29:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 05:29:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 05:29:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 05:33:52 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 15 Nov 2022 05:33:52 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 15 Nov 2022 05:34:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 15 Nov 2022 05:34:14 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 15 Nov 2022 05:34:15 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 15 Nov 2022 05:34:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 05:34:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 05:34:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 05:51:35 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Nov 2022 02:21:31 GMT
ENV PHP_VERSION=8.1.13
# Tue, 29 Nov 2022 02:21:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 29 Nov 2022 02:21:32 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 29 Nov 2022 02:21:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Nov 2022 02:21:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:25:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Nov 2022 02:25:52 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:25:53 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Nov 2022 02:25:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Nov 2022 02:25:54 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Nov 2022 02:25:54 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:25:55 GMT
WORKDIR /var/www/html
# Tue, 29 Nov 2022 02:25:55 GMT
EXPOSE 80
# Tue, 29 Nov 2022 02:25:55 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:c57913b7d0318ef1a47f0348ce54d9865316776aa1ffb2c7871b1473b3d29407`  
		Last Modified: Tue, 15 Nov 2022 05:24:22 GMT  
		Size: 35.3 MB (35285140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5f0beaf56e20c42dc99adac83339859a68fe21121e2a97694ccf17bb3d80a1f`  
		Last Modified: Tue, 15 Nov 2022 07:02:41 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb01e5ff921e5a6fdfd50966abf1a71511e1fc3d7c5b93c0f0d23c4b01bde8ad`  
		Last Modified: Tue, 15 Nov 2022 07:03:05 GMT  
		Size: 86.6 MB (86632107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b444ab201aca26c541ce9ce4732f100ccd2fd815497509f4281f39038ecdb838`  
		Last Modified: Tue, 15 Nov 2022 07:02:41 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0fca4b0f24135682d7d43d92cc3e475e3a1f7d0b0685dac72569e8aeb202701`  
		Last Modified: Tue, 15 Nov 2022 07:03:44 GMT  
		Size: 20.5 MB (20465178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f0a8d837f689661b3916dc15531fa63568b8f8dd569bcdf1419e76c70fe957`  
		Last Modified: Tue, 15 Nov 2022 07:03:39 GMT  
		Size: 475.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7270d82c3d39663e1b3ad3a50a772b6757d614fec5eb597256a1c63eb532cc15`  
		Last Modified: Tue, 15 Nov 2022 07:03:39 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d17148f156242f5c4f837d8cd7c77689890543584f9fdb2ac0bd8b7deb21df`  
		Last Modified: Tue, 29 Nov 2022 04:05:51 GMT  
		Size: 12.1 MB (12144818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9247ec937d255fa5bf37d351b8d4fa7751c877ced1865822c6e518ef27c09543`  
		Last Modified: Tue, 29 Nov 2022 04:05:48 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a45774d3fde5fe71f4c7bdeaf3148eb4a6285f761a21874a0cb1ab9c2905bd`  
		Last Modified: Tue, 29 Nov 2022 04:05:51 GMT  
		Size: 11.4 MB (11443443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fca58525c6ee539c3e77e34c692d716fe875f2821f273eda0da1938a70e125e`  
		Last Modified: Tue, 29 Nov 2022 04:05:48 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfddbd709840207ffdd9b9352b331ddad99a0e4405251bd331a3323f3c484ab2`  
		Last Modified: Tue, 29 Nov 2022 04:05:48 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:977d45d8d8c1391ecb5cf6e79a2861ca2106461f8e8a58ea33b1984952009940`  
		Last Modified: Tue, 29 Nov 2022 04:05:48 GMT  
		Size: 894.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache-bullseye` - linux; s390x

```console
$ docker pull php@sha256:710b9b814e04d0b4dc97448ea6cd3bd02eeb21a473214582e4735b5df5489772
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.7 MB (142675298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae1b5cea5130765fb438b8ed3c07fb4a3bbbbde4e65eb3fc7b7a8769fa765d0f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Tue, 15 Nov 2022 01:42:51 GMT
ADD file:af482bbfc85f1f292de8bd5f2751ee2b67ec9e057eab3684f96984f0e4ecf943 in / 
# Tue, 15 Nov 2022 01:42:56 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 02:57:36 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 02:57:36 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 02:58:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 02:58:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 02:58:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 03:02:44 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Tue, 15 Nov 2022 03:02:44 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Tue, 15 Nov 2022 03:03:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Tue, 15 Nov 2022 03:03:05 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Tue, 15 Nov 2022 03:03:06 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Tue, 15 Nov 2022 03:03:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 03:03:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 03:03:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 03:19:35 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 29 Nov 2022 02:23:53 GMT
ENV PHP_VERSION=8.1.13
# Tue, 29 Nov 2022 02:23:53 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.13.tar.xz.asc
# Tue, 29 Nov 2022 02:23:53 GMT
ENV PHP_SHA256=b15ef0ccdd6760825604b3c4e3e73558dcf87c75ef1d68ef4289d8fd261ac856
# Tue, 29 Nov 2022 02:24:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 29 Nov 2022 02:24:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:26:04 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Nov 2022 02:26:04 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:26:05 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Nov 2022 02:26:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Nov 2022 02:26:05 GMT
STOPSIGNAL SIGWINCH
# Tue, 29 Nov 2022 02:26:05 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Tue, 29 Nov 2022 02:26:05 GMT
WORKDIR /var/www/html
# Tue, 29 Nov 2022 02:26:06 GMT
EXPOSE 80
# Tue, 29 Nov 2022 02:26:06 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:a6ad801d746b7bdde3a0ef72107d05694a38101de03b6eed340af802bdf13957`  
		Last Modified: Tue, 15 Nov 2022 01:47:33 GMT  
		Size: 29.6 MB (29643781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d71958e28a746867b0e7cb1c5f031924597b4509a233399a3a3d8968aa95f64`  
		Last Modified: Tue, 15 Nov 2022 04:44:54 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a78b409c9c2463a7e5350cae36b1e7fba6df50cfa44e169bb26a643cd299143e`  
		Last Modified: Tue, 15 Nov 2022 04:45:04 GMT  
		Size: 71.6 MB (71627303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f25a893502757c2fbf006d5887bcc16766dc523c4cac685c2dccf4af8a0ecb7`  
		Last Modified: Tue, 15 Nov 2022 04:44:53 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0515d653f16c8040759be3c29d4f0c2b1036a62349c4e8880020cddb7577440`  
		Last Modified: Tue, 15 Nov 2022 04:45:30 GMT  
		Size: 19.1 MB (19073360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db41f3bdc80a9ab4dac242e3fea7cdfa9920456b16f1c1e282ef531d6f4bda3`  
		Last Modified: Tue, 15 Nov 2022 04:45:28 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afcc8b7a33b20c2381e14440573cd7b4bc7510a6e28de417d2acca44053906f`  
		Last Modified: Tue, 15 Nov 2022 04:45:28 GMT  
		Size: 515.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787869dc0b648bb9e272de366671d95491f30e0cf637a0fc525fb2581b399d08`  
		Last Modified: Tue, 29 Nov 2022 03:28:22 GMT  
		Size: 12.1 MB (12144022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e6c1636cd153c6269618d954006511b476dff2e68a08707dd36e5405e2efe41`  
		Last Modified: Tue, 29 Nov 2022 03:28:20 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef08de5a31baa1f1cb5fe769d6157b9ac123b9f033071d5dbaedfbcd461d150`  
		Last Modified: Tue, 29 Nov 2022 03:28:22 GMT  
		Size: 10.2 MB (10181249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebd703cedc7976dd07f3a09cb28c4cc30f760d38901472485382784c77292f9`  
		Last Modified: Tue, 29 Nov 2022 03:28:20 GMT  
		Size: 2.5 KB (2459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e568b4b861fda431ae55e63636e3e9a3ae55a053bf3dbb4f612d4c1f0c061ae`  
		Last Modified: Tue, 29 Nov 2022 03:28:20 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d1f223604ba710a220ae4b49ec137753cce2d613044777a71a0f7ed8459dab`  
		Last Modified: Tue, 29 Nov 2022 03:28:20 GMT  
		Size: 895.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
