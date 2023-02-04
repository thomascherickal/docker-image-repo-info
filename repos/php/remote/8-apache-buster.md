## `php:8-apache-buster`

```console
$ docker pull php@sha256:3a3e6f8a576e469ab17373544a59cbd84477c06c5bba9e240a8adb71d47876c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `php:8-apache-buster` - linux; amd64

```console
$ docker pull php@sha256:2e48bfb9eada75ea8bf950dcc1ea6c1dbfa920f77e723cea7f54980ee8d62b2e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **146.5 MB (146493951 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2cc37f47811d2ec03c1ae5432dbe894dc00058582720b32f07d0542db5ffeecc`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 Jan 2023 02:35:07 GMT
ADD file:67ceb946e54c26c505b5f9f393d77befbd5e9b3b5c069ca301e314ecc74456b0 in / 
# Wed, 11 Jan 2023 02:35:07 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 07:33:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Jan 2023 07:33:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Jan 2023 07:33:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 07:33:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Jan 2023 07:33:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 Jan 2023 07:37:04 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 Jan 2023 07:37:04 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 Jan 2023 07:37:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 Jan 2023 07:37:15 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 Jan 2023 07:37:16 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 Jan 2023 07:37:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 07:37:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 07:37:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Jan 2023 07:37:16 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 03 Feb 2023 00:03:18 GMT
ENV PHP_VERSION=8.2.2
# Fri, 03 Feb 2023 00:03:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.2.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.2.tar.xz.asc
# Fri, 03 Feb 2023 00:03:18 GMT
ENV PHP_SHA256=bdc4aa38e652bac86039601840bae01c0c3653972eaa6f9f93d5f71953a7ee33
# Fri, 03 Feb 2023 00:03:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Fri, 03 Feb 2023 00:03:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 03 Feb 2023 00:06:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 03 Feb 2023 00:06:33 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Fri, 03 Feb 2023 00:06:34 GMT
RUN docker-php-ext-enable sodium
# Fri, 03 Feb 2023 00:06:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 03 Feb 2023 00:06:34 GMT
STOPSIGNAL SIGWINCH
# Fri, 03 Feb 2023 00:06:34 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Fri, 03 Feb 2023 00:06:34 GMT
WORKDIR /var/www/html
# Fri, 03 Feb 2023 00:06:35 GMT
EXPOSE 80
# Fri, 03 Feb 2023 00:06:35 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:548fcab5fe888f589dd092c68b813bfd65359878bd1950d6b753f749e82ebd7c`  
		Last Modified: Wed, 11 Jan 2023 02:39:48 GMT  
		Size: 27.1 MB (27140352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d74ce78967f9140fdc27b9a40d488aa892444f323693e595af68112aa3382947`  
		Last Modified: Wed, 11 Jan 2023 08:46:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7917277b60c64f1dc6c1551881a5b4801a99425ba7a44b9e938670706884bc2`  
		Last Modified: Wed, 11 Jan 2023 08:47:02 GMT  
		Size: 76.7 MB (76687443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e40c0be1c8c0e29a9a0b23d3bc3d8cab104e00bb9602cd31ee58e2c504318193`  
		Last Modified: Wed, 11 Jan 2023 08:46:51 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529d453ff257120704ef78c98f0553897ef830b058d99e26602e5a87cc19399b`  
		Last Modified: Wed, 11 Jan 2023 08:47:29 GMT  
		Size: 18.7 MB (18684921 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b7a4f35f3ffbc1bb356d7a10ea7b0e4d1244641d44d98eb9bef860e5ac1e8b1`  
		Last Modified: Wed, 11 Jan 2023 08:47:26 GMT  
		Size: 478.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57840f7817f4fee07cd5afed77c54505507fdf1f4568c324688bd88d03f72814`  
		Last Modified: Wed, 11 Jan 2023 08:47:26 GMT  
		Size: 514.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f14f7fbd6427ed98deb6d06c4d0d3fd0fbc011bff38ade33a869ea1c009cac6`  
		Last Modified: Fri, 03 Feb 2023 00:44:36 GMT  
		Size: 12.3 MB (12276964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149a89ea9c63cd25b3d59b8b85804de6df3755263db2b23be88b4ab78125f396`  
		Last Modified: Fri, 03 Feb 2023 00:44:34 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593890cf539d16b9ce26c226ff8e98685a9a672b5f87a0e5ab6a10a5e247124d`  
		Last Modified: Fri, 03 Feb 2023 00:44:36 GMT  
		Size: 11.7 MB (11698683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fefb6b68c89e52a6529853d8bbae658087f8a4e6d0cce4851484afd810eaf932`  
		Last Modified: Fri, 03 Feb 2023 00:44:33 GMT  
		Size: 2.5 KB (2460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c95790706dfa4e7680745af5b52bc44e32e90449f53113d30821bc66ef9603`  
		Last Modified: Fri, 03 Feb 2023 00:44:33 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac35aba6e7e936f0c9580b244b2797ef1b6eed6d945cb811aa197fa68b812d8`  
		Last Modified: Fri, 03 Feb 2023 00:44:33 GMT  
		Size: 898.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache-buster` - linux; arm variant v7

```console
$ docker pull php@sha256:146fb5ae1461ae5caffae1a300e8166729361d85e3660549a0c3d365a9993e3f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.2 MB (122174015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6362dee5d8207cb28e98d1548ebb1b9dc582b8e86c85c91a92aaed60d197f481`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 Jan 2023 04:01:11 GMT
ADD file:360ea34974de7bba698a1a4e78149a2da671264dbf02678aef09bcd3f592c229 in / 
# Wed, 11 Jan 2023 04:01:12 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 10:49:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Jan 2023 10:49:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Jan 2023 10:49:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 10:49:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Jan 2023 10:49:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 Jan 2023 10:53:00 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 Jan 2023 10:53:00 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 Jan 2023 10:53:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 Jan 2023 10:53:10 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 Jan 2023 10:53:11 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 Jan 2023 10:53:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 10:53:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 10:53:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Jan 2023 10:53:11 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 02 Feb 2023 23:33:33 GMT
ENV PHP_VERSION=8.2.2
# Thu, 02 Feb 2023 23:33:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.2.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.2.tar.xz.asc
# Thu, 02 Feb 2023 23:33:34 GMT
ENV PHP_SHA256=bdc4aa38e652bac86039601840bae01c0c3653972eaa6f9f93d5f71953a7ee33
# Thu, 02 Feb 2023 23:33:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 02 Feb 2023 23:33:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 02 Feb 2023 23:36:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 02 Feb 2023 23:36:29 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 02 Feb 2023 23:36:30 GMT
RUN docker-php-ext-enable sodium
# Thu, 02 Feb 2023 23:36:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 02 Feb 2023 23:36:30 GMT
STOPSIGNAL SIGWINCH
# Thu, 02 Feb 2023 23:36:30 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 02 Feb 2023 23:36:30 GMT
WORKDIR /var/www/html
# Thu, 02 Feb 2023 23:36:30 GMT
EXPOSE 80
# Thu, 02 Feb 2023 23:36:31 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:75680cfdd833613d913b856d8c584fa88c596b93732050a582a5fe937df3a9e6`  
		Last Modified: Wed, 11 Jan 2023 04:08:41 GMT  
		Size: 22.7 MB (22748873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ed5ebea1659628f295ba410fa8b24cd4ee235c5d22b2d5ea87b4d4757035ec3`  
		Last Modified: Wed, 11 Jan 2023 12:22:30 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb91cd4de312aea95155bd55e405b6e5b71f4cbe5e11669833ff0b019d9d902`  
		Last Modified: Wed, 11 Jan 2023 12:22:40 GMT  
		Size: 59.5 MB (59542505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10feb29d2fa619a45424c2676a475617fade95e0f24d4ee3f66a9e62e7b7db3`  
		Last Modified: Wed, 11 Jan 2023 12:22:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27bf0683b7147ad5e3b9eb7e3a013db171c91753a25debe8cdebafb3642db13c`  
		Last Modified: Wed, 11 Jan 2023 12:23:17 GMT  
		Size: 17.5 MB (17481468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a6dc1450feb0a88caace8c952c8aebcd67f2b36c1392f88fb9647f681e2a5a`  
		Last Modified: Wed, 11 Jan 2023 12:23:13 GMT  
		Size: 432.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d940d534b1be885f87a23290be7df3b473b690ca54e59e5a23e3b98e5bced08`  
		Last Modified: Wed, 11 Jan 2023 12:23:13 GMT  
		Size: 486.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf72f21a38901d10f833d3db6566a9a4bd2fbcc025f969e7041042af97991f8`  
		Last Modified: Fri, 03 Feb 2023 00:20:36 GMT  
		Size: 12.3 MB (12275085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920e288509c6b959d4a56bd00aff6db0a463f63cd2edc1bf6c30cdac73403c46`  
		Last Modified: Fri, 03 Feb 2023 00:20:33 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488af8c10c172b04c3a8a338d16a0d52078733308a4204e2fb74697f55e429c6`  
		Last Modified: Fri, 03 Feb 2023 00:20:35 GMT  
		Size: 10.1 MB (10120626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92a668d76bd930f2208f26b1ccd1deed430050daa4b800ead8482c41dceda0ca`  
		Last Modified: Fri, 03 Feb 2023 00:20:33 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da58435d8b83746b687098511b56509e56ce62a8c1a3c5dbb5a70da83d569f0`  
		Last Modified: Fri, 03 Feb 2023 00:20:33 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8057d9391a645234d5d5a98eb1a5ef105e58ec9d7d5c1224b3a8bc1f568a25`  
		Last Modified: Fri, 03 Feb 2023 00:20:33 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache-buster` - linux; arm64 variant v8

```console
$ docker pull php@sha256:dabbd0421c43f332a5ebcd97f464bd4dc872187cd8061c0531c4c2d00e3c485c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.5 MB (138509569 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf4b96ca7810cc926373e2c2fe73f53216d8c37aa2e86489ee95ef1d75fa8a04`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Sat, 04 Feb 2023 06:17:54 GMT
ADD file:cf6ecb1d6b034b0d4fc309542cb25fff0c997661b323f524ecc258ac323e43f6 in / 
# Sat, 04 Feb 2023 06:17:55 GMT
CMD ["bash"]
# Sat, 04 Feb 2023 12:18:58 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 04 Feb 2023 12:18:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 04 Feb 2023 12:19:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 04 Feb 2023 12:19:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 04 Feb 2023 12:19:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 04 Feb 2023 12:22:21 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Sat, 04 Feb 2023 12:22:21 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Sat, 04 Feb 2023 12:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Sat, 04 Feb 2023 12:22:31 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Sat, 04 Feb 2023 12:22:31 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Sat, 04 Feb 2023 12:22:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 12:22:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Feb 2023 12:22:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 04 Feb 2023 12:22:32 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Sat, 04 Feb 2023 12:22:32 GMT
ENV PHP_VERSION=8.2.2
# Sat, 04 Feb 2023 12:22:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.2.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.2.tar.xz.asc
# Sat, 04 Feb 2023 12:22:32 GMT
ENV PHP_SHA256=bdc4aa38e652bac86039601840bae01c0c3653972eaa6f9f93d5f71953a7ee33
# Sat, 04 Feb 2023 12:22:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 04 Feb 2023 12:22:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 04 Feb 2023 12:25:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 04 Feb 2023 12:25:29 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Sat, 04 Feb 2023 12:25:30 GMT
RUN docker-php-ext-enable sodium
# Sat, 04 Feb 2023 12:25:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 04 Feb 2023 12:25:30 GMT
STOPSIGNAL SIGWINCH
# Sat, 04 Feb 2023 12:25:30 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Sat, 04 Feb 2023 12:25:30 GMT
WORKDIR /var/www/html
# Sat, 04 Feb 2023 12:25:30 GMT
EXPOSE 80
# Sat, 04 Feb 2023 12:25:30 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:bd2853c1424a5596deda2f31e1f82920613a03c667c3ff58cb461340b7bb89cd`  
		Last Modified: Sat, 04 Feb 2023 06:22:04 GMT  
		Size: 25.9 MB (25922631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78a59b8ccf3c868a96ffe9151ff3a1f1a89fee4d0151785e9080a02e8767c46`  
		Last Modified: Sat, 04 Feb 2023 13:18:52 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c974607a8d0be8f9cd77efc0f50a9b22ac01baef575c035f7e8f6cef7654dd`  
		Last Modified: Sat, 04 Feb 2023 13:19:00 GMT  
		Size: 70.4 MB (70361880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0dae2c40cdca83210ffd87d10080044d2271241f03f6ca418351c27703acbeb`  
		Last Modified: Sat, 04 Feb 2023 13:18:51 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c8f0075a627a6b12b30298d5bf854f7411c7d68dae15b528a6f6d3b1fd8080c`  
		Last Modified: Sat, 04 Feb 2023 13:19:26 GMT  
		Size: 18.6 MB (18583775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6296bd37059766b25cf9b0897f32e61829223f7fd097c50663fde2c2751791d`  
		Last Modified: Sat, 04 Feb 2023 13:19:24 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32f1050e799c5b0f54255f9f7bd7821dbe7aeaf9935773004050383fc15b0c7`  
		Last Modified: Sat, 04 Feb 2023 13:19:24 GMT  
		Size: 513.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:745aaf4d7291829ec19cc6f99222c11a418bed6c510125cd9f21bf120326ea32`  
		Last Modified: Sat, 04 Feb 2023 13:19:24 GMT  
		Size: 12.3 MB (12275718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6505419d33cd09b5abfc478ad3afb1d446025f1cc80bf05ae94d0b92555df3`  
		Last Modified: Sat, 04 Feb 2023 13:19:22 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbae161abdf224e319fba009d47b5018a072438ba02e8f4b17ce80d7a1a27864`  
		Last Modified: Sat, 04 Feb 2023 13:19:24 GMT  
		Size: 11.4 MB (11359997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa86de0117d62e6bd6e798722f5e1ab03068afdb32aa0058edd62eebe1d303b`  
		Last Modified: Sat, 04 Feb 2023 13:19:22 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f29059d283ec424fff056fd2989b03aafe612bf4ed456c8850537292a61c176`  
		Last Modified: Sat, 04 Feb 2023 13:19:22 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cab719040440d8bb6099119373fa44b9f0831bdf45a138d74f243b8f5aee5c6`  
		Last Modified: Sat, 04 Feb 2023 13:19:22 GMT  
		Size: 893.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-apache-buster` - linux; 386

```console
$ docker pull php@sha256:623e7f18f2fb18b3ea04b51c3d62f016abf75e2d1df0bc469430fe3179dc19cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.0 MB (151977758 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a001dc71d4d9b81b900b0dfd22f4e939bc1a09d0c9f2a06fc49c52ce5780c5b5`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["apache2-foreground"]`

```dockerfile
# Wed, 11 Jan 2023 03:16:35 GMT
ADD file:9d3bf04d5e729aff5e4261af1fa5560f388c41ddb1cab110433fc60085d332da in / 
# Wed, 11 Jan 2023 03:16:36 GMT
CMD ["bash"]
# Wed, 11 Jan 2023 09:17:21 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 Jan 2023 09:17:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 Jan 2023 09:17:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 Jan 2023 09:17:42 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 Jan 2023 09:17:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 Jan 2023 09:21:34 GMT
ENV APACHE_CONFDIR=/etc/apache2
# Wed, 11 Jan 2023 09:21:34 GMT
ENV APACHE_ENVVARS=/etc/apache2/envvars
# Wed, 11 Jan 2023 09:21:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends apache2; 	rm -rf /var/lib/apt/lists/*; 		sed -ri 's/^export ([^=]+)=(.*)$/: ${\1:=\2}\nexport \1/' "$APACHE_ENVVARS"; 		. "$APACHE_ENVVARS"; 	for dir in 		"$APACHE_LOCK_DIR" 		"$APACHE_RUN_DIR" 		"$APACHE_LOG_DIR" 	; do 		rm -rvf "$dir"; 		mkdir -p "$dir"; 		chown "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$dir"; 		chmod 777 "$dir"; 	done; 		rm -rvf /var/www/html/*; 		ln -sfT /dev/stderr "$APACHE_LOG_DIR/error.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/access.log"; 	ln -sfT /dev/stdout "$APACHE_LOG_DIR/other_vhosts_access.log"; 	chown -R --no-dereference "$APACHE_RUN_USER:$APACHE_RUN_GROUP" "$APACHE_LOG_DIR"
# Wed, 11 Jan 2023 09:21:46 GMT
RUN a2dismod mpm_event && a2enmod mpm_prefork
# Wed, 11 Jan 2023 09:21:47 GMT
RUN { 		echo '<FilesMatch \.php$>'; 		echo '\tSetHandler application/x-httpd-php'; 		echo '</FilesMatch>'; 		echo; 		echo 'DirectoryIndex disabled'; 		echo 'DirectoryIndex index.php index.html'; 		echo; 		echo '<Directory /var/www/>'; 		echo '\tOptions -Indexes'; 		echo '\tAllowOverride All'; 		echo '</Directory>'; 	} | tee "$APACHE_CONFDIR/conf-available/docker-php.conf" 	&& a2enconf docker-php
# Wed, 11 Jan 2023 09:21:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 09:21:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 Jan 2023 09:21:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 Jan 2023 09:21:51 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 02 Feb 2023 22:56:48 GMT
ENV PHP_VERSION=8.2.2
# Thu, 02 Feb 2023 22:56:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.2.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.2.tar.xz.asc
# Thu, 02 Feb 2023 22:56:50 GMT
ENV PHP_SHA256=bdc4aa38e652bac86039601840bae01c0c3653972eaa6f9f93d5f71953a7ee33
# Thu, 02 Feb 2023 22:57:02 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 02 Feb 2023 22:57:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 02 Feb 2023 22:59:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		apache2-dev 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--with-apxs2 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 02 Feb 2023 22:59:49 GMT
COPY multi:e11221d43af7136e4dbad5a74e659bcfa753214a9e615c3daf357f1633d9d3d1 in /usr/local/bin/ 
# Thu, 02 Feb 2023 22:59:49 GMT
RUN docker-php-ext-enable sodium
# Thu, 02 Feb 2023 22:59:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 02 Feb 2023 22:59:51 GMT
STOPSIGNAL SIGWINCH
# Thu, 02 Feb 2023 22:59:53 GMT
COPY file:e3123fcb6566efa979f945bfac1c94c854a559d7b82723e42118882a8ac4de66 in /usr/local/bin/ 
# Thu, 02 Feb 2023 22:59:53 GMT
WORKDIR /var/www/html
# Thu, 02 Feb 2023 22:59:54 GMT
EXPOSE 80
# Thu, 02 Feb 2023 22:59:55 GMT
CMD ["apache2-foreground"]
```

-	Layers:
	-	`sha256:bb9c50683070c3b61ce8fb230515259898ff6a152074a52904cd74d18e287f08`  
		Last Modified: Wed, 11 Jan 2023 03:22:49 GMT  
		Size: 27.8 MB (27798529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4134419930a4fcd0faa93879894eb9dfc61f09526b5d68f9d8dae4a99fe4ba39`  
		Last Modified: Wed, 11 Jan 2023 10:31:47 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9deeaebcc6ab8bd66b3ffd1dac825dafc35ed4dabbe4506680b0a7260e3d959a`  
		Last Modified: Wed, 11 Jan 2023 10:31:58 GMT  
		Size: 81.2 MB (81234459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1075a15bfb339017c56309849301643d886ff2889f02c2c1b67012da0cba84c7`  
		Last Modified: Wed, 11 Jan 2023 10:31:47 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984d9c19bedb856464b9001ef28f7dc41ed4c5ec9f3c59d11b06b06e6dd58c05`  
		Last Modified: Wed, 11 Jan 2023 10:32:31 GMT  
		Size: 18.9 MB (18900845 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3be14dfc1e20623ca9e56b08675644cddfbf28cb21dc1edaeea3cffab2db515`  
		Last Modified: Wed, 11 Jan 2023 10:32:28 GMT  
		Size: 433.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85ba5a6b0e10f39f478323be947141ac9c9d9586bc41a3e646ca22d21ec6c96`  
		Last Modified: Wed, 11 Jan 2023 10:32:28 GMT  
		Size: 487.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f4b2b4d15758d32281f29026a1aea26bb99f5947eae4a91e3d3411152d8e50`  
		Last Modified: Thu, 02 Feb 2023 23:43:08 GMT  
		Size: 12.1 MB (12061794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b4a48e3b3a73856208ef345ddbf6993e41a71d9d7de29fc332e5007cdc0097`  
		Last Modified: Thu, 02 Feb 2023 23:43:05 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fc46387f795454e6ad25029135bf811ccbef8dbb10751c7424971ab297850f2`  
		Last Modified: Thu, 02 Feb 2023 23:43:07 GMT  
		Size: 12.0 MB (11976661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11914366135a218023bdf594c57a4daa173ae13703a0417c341d72ed85cd2bdc`  
		Last Modified: Thu, 02 Feb 2023 23:43:05 GMT  
		Size: 2.5 KB (2462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378ab7da701a718d12cc727ee7868d27682c47b19d12c39573111f56d6665c8e`  
		Last Modified: Thu, 02 Feb 2023 23:43:05 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b82feeaf35aba1497a4db7d706d9a4799ec5b22b243fa368b6645ced3827916`  
		Last Modified: Thu, 02 Feb 2023 23:43:05 GMT  
		Size: 897.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
