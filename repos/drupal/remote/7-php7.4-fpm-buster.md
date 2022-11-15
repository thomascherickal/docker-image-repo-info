## `drupal:7-php7.4-fpm-buster`

```console
$ docker pull drupal@sha256:a0b0900075163d2ad203667e24121d6a763bc3e9f0d1d0048c77c0ebe6912f52
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `drupal:7-php7.4-fpm-buster` - linux; amd64

```console
$ docker pull drupal@sha256:d5c72b2efb1eb4e8812e482567b9d324cf273ee747190c50f9463f36a7e81052
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.8 MB (144753959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3068259d858d29ff5392bfd3f472ba77cd7f766584172552f62f863505f2b7de`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Nov 2022 04:05:14 GMT
ADD file:9461639b945ced6fb6164491a7e0131261a1b7d69264cce516e75c71e4df22d2 in / 
# Tue, 15 Nov 2022 04:05:14 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 04:26:48 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 04:26:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 04:27:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:27:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 04:27:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 04:27:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 04:27:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 04:27:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 06:08:55 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 15 Nov 2022 06:08:55 GMT
ENV PHP_VERSION=7.4.33
# Tue, 15 Nov 2022 06:08:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.33.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.33.tar.xz.asc
# Tue, 15 Nov 2022 06:08:55 GMT
ENV PHP_SHA256=924846abf93bc613815c55dd3f5809377813ac62a9ec4eb3778675b82a27b927
# Tue, 15 Nov 2022 06:09:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 15 Nov 2022 06:09:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 15 Nov 2022 06:16:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 15 Nov 2022 06:16:12 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 15 Nov 2022 06:16:12 GMT
RUN docker-php-ext-enable sodium
# Tue, 15 Nov 2022 06:16:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 15 Nov 2022 06:16:12 GMT
WORKDIR /var/www/html
# Tue, 15 Nov 2022 06:16:13 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 15 Nov 2022 06:16:13 GMT
STOPSIGNAL SIGQUIT
# Tue, 15 Nov 2022 06:16:13 GMT
EXPOSE 9000
# Tue, 15 Nov 2022 06:16:13 GMT
CMD ["php-fpm"]
# Tue, 15 Nov 2022 08:26:13 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 08:26:13 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 15 Nov 2022 08:30:44 GMT
ENV DRUPAL_VERSION=7.92
# Tue, 15 Nov 2022 08:30:44 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Tue, 15 Nov 2022 08:30:45 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:32820e52a00eb22dc76d70d992be7082cd24b636cfb597ff3951d29a821b46b9`  
		Last Modified: Tue, 15 Nov 2022 04:09:26 GMT  
		Size: 27.1 MB (27140332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a022f9f4db63bdf619d892ab06b0861dc6b1b17b3a137c35093f0937aa7e57`  
		Last Modified: Tue, 15 Nov 2022 06:24:49 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ff96ba8ea962f6736c4fa62505f2aa4b5405f5388b5424727cd3af64cb7cf44`  
		Last Modified: Tue, 15 Nov 2022 06:25:00 GMT  
		Size: 76.7 MB (76687327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b28c78a7e238dc26ddcd2d9ea3c2512abab7fb02db8f343763046433d33bc9c`  
		Last Modified: Tue, 15 Nov 2022 06:24:48 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7381b9c606a76c5d4c0163bbb75847b72767dfb1ebfd03edec9d4f879254ab52`  
		Last Modified: Tue, 15 Nov 2022 06:36:32 GMT  
		Size: 10.7 MB (10742788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d6ad427eb3b8b086dff5f2a996e2b4719f4ac15159e6c171018fc1967318a26`  
		Last Modified: Tue, 15 Nov 2022 06:36:31 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faaa224da81dcd0c6870c0113a5e58f560094d68435729efff0cedfd398c9335`  
		Last Modified: Tue, 15 Nov 2022 06:37:13 GMT  
		Size: 24.9 MB (24897013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3bdf63fa1bea71f69762d9ca019c3f70ccc85c2f6a584856fe4631734d3f1c`  
		Last Modified: Tue, 15 Nov 2022 06:37:08 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3f4ff7f1ae8b0cf1d124b61024c50f2207b686c5df141b71ea699bd457a7df`  
		Last Modified: Tue, 15 Nov 2022 06:37:08 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f44d416d63814a6ce1852578ff0301bc6ec1246cb075401a20d96bcd310618`  
		Last Modified: Tue, 15 Nov 2022 06:37:08 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e14fb152050b7e6b7edfd60381741e5043fd7659aa7de9c3dbb1a68bc4b1ae`  
		Last Modified: Tue, 15 Nov 2022 08:45:27 GMT  
		Size: 1.9 MB (1877190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f0cab869ce5cc4da799364c89a1a858c31e1de1d0f77a2eb2e39f5ecdd0d4f`  
		Last Modified: Tue, 15 Nov 2022 08:45:27 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15322353acf430d582a5d550b16579c3e8ccae24b45c84d464ab1ba2f008077`  
		Last Modified: Tue, 15 Nov 2022 08:52:56 GMT  
		Size: 3.4 MB (3396849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-fpm-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:003cdb60ea7f50bec93d160655b3026c632392f0ee2686e07ea2ff64213639b1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.0 MB (121046043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d306342e6e65ad9e6c6a3a6519336e1f06da22a7e689dd9cbb969d2f0520c53`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Nov 2022 03:43:57 GMT
ADD file:02e51e32df426f4ee14093de5240d396191761b03f60af08b7e920c86c3df725 in / 
# Tue, 15 Nov 2022 03:43:57 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 04:07:37 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 04:07:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 04:07:55 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 04:07:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 04:07:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 04:07:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 04:07:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 04:07:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 05:40:32 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 15 Nov 2022 05:40:32 GMT
ENV PHP_VERSION=7.4.33
# Tue, 15 Nov 2022 05:40:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.33.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.33.tar.xz.asc
# Tue, 15 Nov 2022 05:40:32 GMT
ENV PHP_SHA256=924846abf93bc613815c55dd3f5809377813ac62a9ec4eb3778675b82a27b927
# Tue, 15 Nov 2022 05:40:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 15 Nov 2022 05:40:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 15 Nov 2022 05:47:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 15 Nov 2022 05:47:52 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 15 Nov 2022 05:47:52 GMT
RUN docker-php-ext-enable sodium
# Tue, 15 Nov 2022 05:47:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 15 Nov 2022 05:47:53 GMT
WORKDIR /var/www/html
# Tue, 15 Nov 2022 05:47:53 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 15 Nov 2022 05:47:53 GMT
STOPSIGNAL SIGQUIT
# Tue, 15 Nov 2022 05:47:53 GMT
EXPOSE 9000
# Tue, 15 Nov 2022 05:47:53 GMT
CMD ["php-fpm"]
# Tue, 15 Nov 2022 08:00:14 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 08:00:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 15 Nov 2022 08:09:33 GMT
ENV DRUPAL_VERSION=7.92
# Tue, 15 Nov 2022 08:09:33 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Tue, 15 Nov 2022 08:09:34 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:e14edb06ef42285b9a4c82509f85d76caeb037799d6631d8d272f86af363a045`  
		Last Modified: Tue, 15 Nov 2022 03:51:01 GMT  
		Size: 22.7 MB (22748928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a744950c0c95ea35eac5bd289ec7493aa3d866cb171b0b7b2617100323dafddd`  
		Last Modified: Tue, 15 Nov 2022 06:06:45 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a0c468d8145d2641efffc44b06bbdbbcb730f11fcc94864e28dcc5ab9d69f2`  
		Last Modified: Tue, 15 Nov 2022 06:06:56 GMT  
		Size: 59.5 MB (59542292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cf3287317716a59fab00c89f0f363fdfab61ba1aa6ec645c3ec4b50c904401`  
		Last Modified: Tue, 15 Nov 2022 06:06:45 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a24645442fcb85607749bc4cc718a26b5a82d806bbf919894039df87b0f111`  
		Last Modified: Tue, 15 Nov 2022 06:22:22 GMT  
		Size: 10.7 MB (10740669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26e51bfd53399e59e3152dd6480506d8172bdf6d4dbdc234bbcc8d36c1a744ce`  
		Last Modified: Tue, 15 Nov 2022 06:22:20 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e221cbd25a3b7c1517422234a2afe096f3832e6dfee16c836f895b8e135ddb9f`  
		Last Modified: Tue, 15 Nov 2022 06:23:12 GMT  
		Size: 23.0 MB (23012695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e6c08a0d6510768c0a0696f3eca81d426aebbb857a4b091e545975cce9a780`  
		Last Modified: Tue, 15 Nov 2022 06:23:07 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df04621c73d42d4dee2e1797fea9a9da182463de00423e5a4299a2efabf4733`  
		Last Modified: Tue, 15 Nov 2022 06:23:07 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c949aef6dfae5249022e8be657885d6143cb7ba190b1eeed2cd6bd8883e77e`  
		Last Modified: Tue, 15 Nov 2022 06:23:07 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fcb50c968aa51cd0f22925fc71e9790c7413b587e65bdac6d64886440083d5b`  
		Last Modified: Tue, 15 Nov 2022 08:37:23 GMT  
		Size: 1.6 MB (1592480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636b366a5eb801c9a0df0f2f7a8fb76ca8c808b057ca6620e710e1f1c76b651d`  
		Last Modified: Tue, 15 Nov 2022 08:37:22 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3811cbc3af7df3042c32c5dd775fe47a0cec094b8e5938e21f7be89bfc3e25e8`  
		Last Modified: Tue, 15 Nov 2022 08:46:51 GMT  
		Size: 3.4 MB (3396561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-fpm-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:a8bc7a5be33dbc2dc045d0c5aa7acaaf7b4d461a280b39bb7874d3f9f04cbac5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **137.0 MB (136957193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06c8864572719a4bc8d7bf2646d694d1bfa7203fbe20fcc376e992f1fc95ec5d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 15 Nov 2022 01:41:34 GMT
ADD file:aaead8e4dd08d41c8d1692bbe76b673119289836428e1f713ca550c2468711ac in / 
# Tue, 15 Nov 2022 01:41:34 GMT
CMD ["bash"]
# Tue, 15 Nov 2022 02:10:44 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 15 Nov 2022 02:10:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 15 Nov 2022 02:11:03 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 02:11:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 15 Nov 2022 02:11:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 15 Nov 2022 02:11:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 02:11:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 15 Nov 2022 02:11:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 15 Nov 2022 03:45:25 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 15 Nov 2022 03:45:25 GMT
ENV PHP_VERSION=7.4.33
# Tue, 15 Nov 2022 03:45:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.33.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.33.tar.xz.asc
# Tue, 15 Nov 2022 03:45:25 GMT
ENV PHP_SHA256=924846abf93bc613815c55dd3f5809377813ac62a9ec4eb3778675b82a27b927
# Tue, 15 Nov 2022 03:45:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 15 Nov 2022 03:45:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 15 Nov 2022 03:50:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 15 Nov 2022 03:50:51 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 15 Nov 2022 03:50:51 GMT
RUN docker-php-ext-enable sodium
# Tue, 15 Nov 2022 03:50:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 15 Nov 2022 03:50:51 GMT
WORKDIR /var/www/html
# Tue, 15 Nov 2022 03:50:52 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 15 Nov 2022 03:50:52 GMT
STOPSIGNAL SIGQUIT
# Tue, 15 Nov 2022 03:50:52 GMT
EXPOSE 9000
# Tue, 15 Nov 2022 03:50:52 GMT
CMD ["php-fpm"]
# Tue, 15 Nov 2022 16:11:56 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Tue, 15 Nov 2022 16:11:56 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 15 Nov 2022 16:17:53 GMT
ENV DRUPAL_VERSION=7.92
# Tue, 15 Nov 2022 16:17:53 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Tue, 15 Nov 2022 16:17:54 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:cc457132e077d684a6cecad3331c35341d814c5d364f3cf24d698a6d8e76d0e7`  
		Last Modified: Tue, 15 Nov 2022 01:45:13 GMT  
		Size: 25.9 MB (25914924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a519f5af3edd9577a7d7eecaf5bb04c787a7af6c91565ef581b3c81dffe93b8d`  
		Last Modified: Tue, 15 Nov 2022 03:59:15 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd12efc1398d9588db8c0fe6a81579bd5cf22ddeda1ee4ed50728cb8927b993`  
		Last Modified: Tue, 15 Nov 2022 03:59:23 GMT  
		Size: 70.4 MB (70363086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6a68f17ee8b59b47c2af378bcbc598995c02bb47e3ee4d56eb01cf3a51bdb9`  
		Last Modified: Tue, 15 Nov 2022 03:59:15 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:106e782ea487a2984037e24acbc9a096becbe488c50422b44011fe141de7634b`  
		Last Modified: Tue, 15 Nov 2022 04:11:13 GMT  
		Size: 10.7 MB (10741396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf08d9b95e440199c11bb7447ddebe0a8d75fdee73f2cf3bd0cc459743de1a80`  
		Last Modified: Tue, 15 Nov 2022 04:11:13 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b5a049e46346f83922c55ee937c759b23a6acc115ae5ca5cb7f35641db4a73`  
		Last Modified: Tue, 15 Nov 2022 04:11:49 GMT  
		Size: 24.7 MB (24670869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a777d66d090f5d0505937dc3abfc62f369a20f81d2b2204ef0f3ae2471eccb77`  
		Last Modified: Tue, 15 Nov 2022 04:11:46 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4563deb308c629341d5906a69a9c1e4fe3a103d83a3066a62dae004260cd35c5`  
		Last Modified: Tue, 15 Nov 2022 04:11:46 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48dc24cf49e38e22e24aac98e5216b287dcfc3a484c09b6edc706515c39e980`  
		Last Modified: Tue, 15 Nov 2022 04:11:46 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193f00f90925c2a8d3f8f1b4d8f0b2676db0fccc94b7ea7d54f5c163dbbf97dd`  
		Last Modified: Tue, 15 Nov 2022 16:33:21 GMT  
		Size: 1.9 MB (1857614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c915d99a659ee140e413ad4228540e3631e37fa5f53a69ae9f56251f7198f40c`  
		Last Modified: Tue, 15 Nov 2022 16:33:21 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26c2adecdfa1f802c270828352fa92b67594c5a78eb60df6876f619aa1076eff`  
		Last Modified: Tue, 15 Nov 2022 16:40:47 GMT  
		Size: 3.4 MB (3396846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-fpm-buster` - linux; 386

```console
$ docker pull drupal@sha256:9c0409db2eae8eb1df0e1f426f3ee921f5363a270a962cdde01cc4b0d36499eb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **150.2 MB (150181008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc93377a70525449674e378da90461cbcc00e5f68915575ca2ea6373aea54986`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 25 Oct 2022 02:23:02 GMT
ADD file:49981fa4bc36bce6e4fdd74b2c4429cc4faef5498c3d8fb20fb98b426bbf8c4d in / 
# Tue, 25 Oct 2022 02:23:02 GMT
CMD ["bash"]
# Tue, 25 Oct 2022 07:56:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Tue, 25 Oct 2022 07:56:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Tue, 25 Oct 2022 07:56:40 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Tue, 25 Oct 2022 07:56:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 25 Oct 2022 07:56:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 25 Oct 2022 07:56:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 25 Oct 2022 07:56:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 25 Oct 2022 07:56:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 25 Oct 2022 09:34:56 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Nov 2022 16:52:20 GMT
ENV PHP_VERSION=7.4.33
# Thu, 03 Nov 2022 16:52:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.33.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.33.tar.xz.asc
# Thu, 03 Nov 2022 16:52:22 GMT
ENV PHP_SHA256=924846abf93bc613815c55dd3f5809377813ac62a9ec4eb3778675b82a27b927
# Thu, 03 Nov 2022 16:52:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 03 Nov 2022 16:52:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Nov 2022 16:59:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Nov 2022 16:59:16 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 03 Nov 2022 16:59:16 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Nov 2022 16:59:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Nov 2022 16:59:18 GMT
WORKDIR /var/www/html
# Thu, 03 Nov 2022 16:59:19 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 03 Nov 2022 16:59:20 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Nov 2022 16:59:21 GMT
EXPOSE 9000
# Thu, 03 Nov 2022 16:59:22 GMT
CMD ["php-fpm"]
# Thu, 03 Nov 2022 18:04:59 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 03 Nov 2022 18:05:00 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 03 Nov 2022 18:12:17 GMT
ENV DRUPAL_VERSION=7.92
# Thu, 03 Nov 2022 18:12:18 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Thu, 03 Nov 2022 18:12:20 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:32caca2e9abac2a8ffc2b083d202d57e1970d8adc212be17451a992441fad01b`  
		Last Modified: Tue, 25 Oct 2022 02:29:19 GMT  
		Size: 27.8 MB (27799224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:140e6bcf950ee2d755ce50e370b6647bc357dcbd24dd0ece7e8d7b388f84d94d`  
		Last Modified: Tue, 25 Oct 2022 09:56:51 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d087454ecae3a96210f9074f3beccfe18b333cf212f9946b1aa8a54c4d0c064c`  
		Last Modified: Tue, 25 Oct 2022 09:57:02 GMT  
		Size: 81.2 MB (81234271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2520a6c0f52f7418abcd797a402d8844158c345af1bc2f6a196ef56b0d9b85d6`  
		Last Modified: Tue, 25 Oct 2022 09:56:50 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23ac247a3ec7eefbd66159555ac17e966649f708b436f751d17dcd5453a59441`  
		Last Modified: Thu, 03 Nov 2022 17:37:17 GMT  
		Size: 10.5 MB (10529215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b300039dc1e6db2ce8578a49a945ffc21b85a35c04fce73ae9506237e93784dd`  
		Last Modified: Thu, 03 Nov 2022 17:37:16 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195747d9859f2ea77726a4ec591f627e8c0457e3a38fc2ff977cd849fc0b4862`  
		Last Modified: Thu, 03 Nov 2022 17:38:12 GMT  
		Size: 25.5 MB (25453341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3c96a74d019da422c09b3a094a9ab11c92eb62bd667965016f27fcce6db8af`  
		Last Modified: Thu, 03 Nov 2022 17:38:08 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:879cd24bc0b18c59efbfa317ed03440248a13f7e5f8bd115e0c8a27fb1bed508`  
		Last Modified: Thu, 03 Nov 2022 17:38:08 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec12225cf9ba51e4dadfa10980c9635f2a5cf36b11547ab3ead814fb12501382`  
		Last Modified: Thu, 03 Nov 2022 17:38:08 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c50651d649c564441ec3c20bd64539be1f52f63db3d7181ab01038f1e19b9207`  
		Last Modified: Thu, 03 Nov 2022 18:27:44 GMT  
		Size: 1.8 MB (1755976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60eb4561615d33caaf50e0ef30802a557b524a7950a9b93f22f40ad7cab5ca3`  
		Last Modified: Thu, 03 Nov 2022 18:27:44 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fcb9c5872a8bc08c23169ed511471d5e5c67c3c60bd24972eabb2d5a863dd05`  
		Last Modified: Thu, 03 Nov 2022 18:34:23 GMT  
		Size: 3.4 MB (3396560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
