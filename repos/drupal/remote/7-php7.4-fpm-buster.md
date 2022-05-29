## `drupal:7-php7.4-fpm-buster`

```console
$ docker pull drupal@sha256:0dcedb022a20752ca656747fcefa29bd6451ec20c3789600110cbfc540e0d413
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

### `drupal:7-php7.4-fpm-buster` - linux; amd64

```console
$ docker pull drupal@sha256:a70ef1785e3443cecc492606f39dff5bc3d920ce900a8a02a6858005c8988727
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.7 MB (144730130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cd2ec2f56d80e5ac7c44783eae339dad69a4931f0b9eaab803eb77201326bf3`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 May 2022 01:20:43 GMT
ADD file:0513eda9512e010cb9459591b62e0c9d9319750923df091b64250ad6e98c2878 in / 
# Sat, 28 May 2022 01:20:43 GMT
CMD ["bash"]
# Sat, 28 May 2022 08:22:14 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 08:22:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 08:22:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 08:22:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 08:22:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 08:22:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:22:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 08:22:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 09:36:23 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 28 May 2022 09:36:23 GMT
ENV PHP_VERSION=7.4.29
# Sat, 28 May 2022 09:36:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Sat, 28 May 2022 09:36:24 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Sat, 28 May 2022 09:36:35 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 May 2022 09:36:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 May 2022 09:43:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 May 2022 09:43:21 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 May 2022 09:43:21 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 May 2022 09:43:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 May 2022 09:43:21 GMT
WORKDIR /var/www/html
# Sat, 28 May 2022 09:43:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 28 May 2022 09:43:22 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 May 2022 09:43:22 GMT
EXPOSE 9000
# Sat, 28 May 2022 09:43:22 GMT
CMD ["php-fpm"]
# Sun, 29 May 2022 02:34:45 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sun, 29 May 2022 02:34:45 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sun, 29 May 2022 02:37:47 GMT
ENV DRUPAL_VERSION=7.89
# Sun, 29 May 2022 02:37:47 GMT
ENV DRUPAL_MD5=924e707e3b1e8269fe623cf2f22ee710
# Sun, 29 May 2022 02:37:48 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:c1ad9731b2c7bf7fddea67f2f3f553515179a375c489e591e2372700fcaca766`  
		Last Modified: Sat, 28 May 2022 01:26:05 GMT  
		Size: 27.1 MB (27140144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef6a088e191348700971ea8f879b767e613f6e05daab7f01768f01cf4846251`  
		Last Modified: Sat, 28 May 2022 09:52:35 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a462c113a353741726781679186a05d2b658daf6565a2fe88063ff67ba8e94`  
		Last Modified: Sat, 28 May 2022 09:52:46 GMT  
		Size: 76.7 MB (76683812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907da9f0848a2079665195ba8b00fe90ae716b11f614966f4a44c617a642db13`  
		Last Modified: Sat, 28 May 2022 09:52:35 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c320fa654882bd3993d743a0d2ef71f4f2a7d17654fffa694f1148e6e4c8f997`  
		Last Modified: Sat, 28 May 2022 10:01:42 GMT  
		Size: 10.7 MB (10740189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfdaac08a3eb1af1260697185eaa38d9b856c1bd44314026944e36a7fce32950`  
		Last Modified: Sat, 28 May 2022 10:01:42 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27fbdd0203b4d73277ef2cf9a482e62bd863f14faad832c67180a73d7d857b87`  
		Last Modified: Sat, 28 May 2022 10:02:26 GMT  
		Size: 24.9 MB (24894486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c492658c63a07b1e6a3489a3e421fff866aebc566494123ef17c5adc787965d`  
		Last Modified: Sat, 28 May 2022 10:02:22 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6b67ef5b9f18de3a1cd175e93ff94ace4609172946a10bb74379b5e9688c9e`  
		Last Modified: Sat, 28 May 2022 10:02:22 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b19770efc1a5c0535891718fff638e4ae1f03e22026d9d354a9b0eb26dc0e22f`  
		Last Modified: Sat, 28 May 2022 10:02:22 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4cb54e9b91f14beeccae22e8fd8091c1a2ee189f81f03138c63afb976eb642`  
		Last Modified: Sun, 29 May 2022 02:51:18 GMT  
		Size: 1.9 MB (1875885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a002b0f1c769b1da7a6f2b8043fc46251b5eb0d94a10dc2f68dcd2751c21779`  
		Last Modified: Sun, 29 May 2022 02:51:17 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28039b5b10a7ac2cf4e50fcacd93691150ac3b36e5dbfbec846cdbd2f4b40eb`  
		Last Modified: Sun, 29 May 2022 02:56:55 GMT  
		Size: 3.4 MB (3383152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-fpm-buster` - linux; arm variant v5

```console
$ docker pull drupal@sha256:183a620803a8c8c4aa3f1754ff9453986aaf79d850672bd4927b6b72abe802e5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.4 MB (123365460 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a38eb0be8c368769d707e4dee4f542e1a6e6b39d1a0db2e97b3b7982b7eddc62`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 May 2022 00:51:34 GMT
ADD file:c4087f224dff43064778eac76e711d30ca4882a1d3b571b1cd509089166abc0d in / 
# Wed, 11 May 2022 00:51:35 GMT
CMD ["bash"]
# Wed, 11 May 2022 09:24:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 09:24:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 09:25:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 09:25:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 09:25:40 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 09:25:40 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 09:25:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 09:25:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 12:22:05 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 11 May 2022 12:22:06 GMT
ENV PHP_VERSION=7.4.29
# Wed, 11 May 2022 12:22:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Wed, 11 May 2022 12:22:07 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Wed, 11 May 2022 12:22:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 12:22:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 12:37:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 12:37:21 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 May 2022 12:37:23 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 12:37:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 12:37:24 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 12:37:25 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 11 May 2022 12:37:26 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 May 2022 12:37:26 GMT
EXPOSE 9000
# Wed, 11 May 2022 12:37:27 GMT
CMD ["php-fpm"]
# Thu, 12 May 2022 08:39:45 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 08:39:47 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 May 2022 08:39:47 GMT
ENV DRUPAL_VERSION=7.89
# Thu, 12 May 2022 08:39:48 GMT
ENV DRUPAL_MD5=924e707e3b1e8269fe623cf2f22ee710
# Thu, 12 May 2022 08:39:51 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:69d6138017be389335ab570ff643096d0ea914f563d41f238e7ff3520fe8e93f`  
		Last Modified: Wed, 11 May 2022 01:07:20 GMT  
		Size: 24.9 MB (24889917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70615f25d1120ae7d68839b43c0eabd12e7418485e06ab74862abca701eae86`  
		Last Modified: Wed, 11 May 2022 12:58:54 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:988a9e70b4ae550a238f0d27299d0d259f8595f521d243f59765babc667e94a3`  
		Last Modified: Wed, 11 May 2022 12:59:36 GMT  
		Size: 58.8 MB (58826398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d185ed130a961c299528c31c1d21c6de6a245abbded61afb0fb09d9407af674d`  
		Last Modified: Wed, 11 May 2022 12:58:53 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94d08e7057da529155dca341194f8d7d4ee60116a3571d0b9983c52790d3fdc`  
		Last Modified: Wed, 11 May 2022 13:20:09 GMT  
		Size: 10.7 MB (10738462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34e827b550ef22b04df6aa3f90e1ce792f503b7a0742f8c8094c40cd86e75004`  
		Last Modified: Wed, 11 May 2022 13:20:07 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:976bda5b6f0442ff52d878b23f98069649345d165964999c6f866106425bce33`  
		Last Modified: Wed, 11 May 2022 13:21:32 GMT  
		Size: 23.8 MB (23802668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba881e303bda3005af6d5b78879a1ee2f4dffef114a4931ef6c30b15ca94600`  
		Last Modified: Wed, 11 May 2022 13:21:18 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a2c03dbbf84560e244e0247261ecbdf88b344d65efab4d80557fbcbe30838c6`  
		Last Modified: Wed, 11 May 2022 13:21:17 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ab64a25487a1a571dafbf713f1d2be81ce4bdfc3b2152677cefc4243602143`  
		Last Modified: Wed, 11 May 2022 13:21:17 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6dc9d639ac92ba20d3ced5a70ffbad4032d677548b82b4574a1bc18e49884c`  
		Last Modified: Thu, 12 May 2022 08:44:15 GMT  
		Size: 1.7 MB (1712403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3701760904a3531d2b71cead5c7e4cdf332a282742142d89529402edb0b3587`  
		Last Modified: Thu, 12 May 2022 08:44:14 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdb66243f6e7ab6e9086d81a8bc9f8cf571cd68903ec5092a1c4ab718081edd2`  
		Last Modified: Thu, 12 May 2022 08:44:18 GMT  
		Size: 3.4 MB (3383151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-fpm-buster` - linux; arm variant v7

```console
$ docker pull drupal@sha256:d00d12a556949415d3dc01c872c6ebdaba4c7ffa3047162797b2b720730a7312
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **121.0 MB (121023704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecc40de0adddee3018d90fa51719502cfaed44ab41d9a7abb386ec7020f2f77b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 May 2022 01:50:13 GMT
ADD file:bccd1898e72cc79621c20ba59061d318521fbd2a8f10806cc3a1561fcbc9daad in / 
# Wed, 11 May 2022 01:50:14 GMT
CMD ["bash"]
# Wed, 11 May 2022 13:57:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 13:57:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 13:58:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 13:58:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 13:58:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 13:58:40 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 13:58:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 13:58:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 16:43:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 11 May 2022 16:43:59 GMT
ENV PHP_VERSION=7.4.29
# Wed, 11 May 2022 16:43:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Wed, 11 May 2022 16:43:59 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Wed, 11 May 2022 16:44:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 16:44:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 16:58:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 16:58:13 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 May 2022 16:58:15 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 16:58:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 16:58:15 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 16:58:17 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 11 May 2022 16:58:17 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 May 2022 16:58:18 GMT
EXPOSE 9000
# Wed, 11 May 2022 16:58:18 GMT
CMD ["php-fpm"]
# Thu, 12 May 2022 23:10:27 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 23:10:28 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 May 2022 23:23:45 GMT
ENV DRUPAL_VERSION=7.89
# Thu, 12 May 2022 23:23:45 GMT
ENV DRUPAL_MD5=924e707e3b1e8269fe623cf2f22ee710
# Thu, 12 May 2022 23:23:49 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:8f4c08df22a944142862818447616fff8b15d3a7ba383d4eeab678af698c2c43`  
		Last Modified: Wed, 11 May 2022 02:06:00 GMT  
		Size: 22.7 MB (22747864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a35ae60a85d449da971bdbc6d59854e609e55d181d0b965377366967883d93c`  
		Last Modified: Wed, 11 May 2022 17:30:27 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a426817eebdd2c479b3443381e193aa0343bd82393a5cb81e1215846033259`  
		Last Modified: Wed, 11 May 2022 17:31:04 GMT  
		Size: 59.5 MB (59538872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d56a72f8dff231737568a93846b1289fa47b78e57a507860cb5b976c74dc372a`  
		Last Modified: Wed, 11 May 2022 17:30:27 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe9b12fdc9cc9ece7dbae25a2f597c4224d17c53b86f39b0d3318babe1bd9d0`  
		Last Modified: Wed, 11 May 2022 17:58:05 GMT  
		Size: 10.7 MB (10738525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6d5ac58fab0eeacee16d900b5a3c232d7176d8c73bc8cae9e024d79d080681`  
		Last Modified: Wed, 11 May 2022 17:58:02 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f95a92481bc4c34447d11701cce9a27884b19316f6b03d38250ef1a9809eba`  
		Last Modified: Wed, 11 May 2022 17:59:22 GMT  
		Size: 23.0 MB (23011186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f096ca8571a806122d5bc4ad1aac6aa610fee208bea4f0d61891f2f8d6043b`  
		Last Modified: Wed, 11 May 2022 17:59:11 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9311a4d6e15deb0c21ffa4242df70e5fe673d4c0e681ea1f3d96166a71e84950`  
		Last Modified: Wed, 11 May 2022 17:59:12 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc032e46302f6ccef8646440e96df6e360acad13f63c1d420f1a0e6ac7988f56`  
		Last Modified: Wed, 11 May 2022 17:59:11 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4aa6e34c898e509c06e01ba6ad8b8a698d8c4110740850e5e98954c997776fe`  
		Last Modified: Fri, 13 May 2022 00:05:57 GMT  
		Size: 1.6 MB (1591644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f2fb4a12758fa1249d8d21cff60da8c431c2041f328c59dfc7e8bd74c79db1`  
		Last Modified: Fri, 13 May 2022 00:05:56 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b244496000796de65ef1aeea18eb9cf67b8728a5b8b7fed2726463c84733684`  
		Last Modified: Fri, 13 May 2022 00:21:23 GMT  
		Size: 3.4 MB (3383154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-fpm-buster` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:033a2eabc555eaf952215b574a81f988eab2500afb2f1910a4c4d97eefb8f32a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.3 MB (136302257 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48830b4422f4824e7d9758a4891f41c91e6c18b3b662447a0a8bd94d7a368201`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 May 2022 00:41:05 GMT
ADD file:d0e42d603f275c040783ec7b6c051200815492fc35b73110234dfcd584e6cdec in / 
# Sat, 28 May 2022 00:41:05 GMT
CMD ["bash"]
# Sat, 28 May 2022 04:57:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 04:57:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 04:57:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 04:58:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 04:58:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 04:58:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 04:58:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 04:58:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 06:12:23 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 28 May 2022 06:12:23 GMT
ENV PHP_VERSION=7.4.29
# Sat, 28 May 2022 06:12:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Sat, 28 May 2022 06:12:25 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Sat, 28 May 2022 06:12:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 May 2022 06:12:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 May 2022 06:19:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 May 2022 06:19:52 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 May 2022 06:19:52 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 May 2022 06:19:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 May 2022 06:19:54 GMT
WORKDIR /var/www/html
# Sat, 28 May 2022 06:19:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 28 May 2022 06:19:56 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 May 2022 06:19:57 GMT
EXPOSE 9000
# Sat, 28 May 2022 06:19:58 GMT
CMD ["php-fpm"]
# Sat, 28 May 2022 21:49:40 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 21:49:41 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 28 May 2022 21:55:20 GMT
ENV DRUPAL_VERSION=7.89
# Sat, 28 May 2022 21:55:21 GMT
ENV DRUPAL_MD5=924e707e3b1e8269fe623cf2f22ee710
# Sat, 28 May 2022 21:55:23 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:4931fb8ba4223cb35034141162105ee5482122692b2931eb69eec912ce64606d`  
		Last Modified: Sat, 28 May 2022 00:48:26 GMT  
		Size: 25.9 MB (25914033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68aac919b6108af15c6a38f8dfdd7a5b5b821982f907d310254e3ac075564696`  
		Last Modified: Sat, 28 May 2022 06:34:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2f8864a861353b6c73a2d817649ed4affc75b32e821ebfc95289378d5811b5`  
		Last Modified: Sat, 28 May 2022 06:34:14 GMT  
		Size: 70.4 MB (70364250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3379e923dd2ca40e8146b160be28d970495c555641741b4239330dcc0b2d8cb7`  
		Last Modified: Sat, 28 May 2022 06:34:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db12333b5340faa007769afa7d57099aa10343357962afdf2526218cd626f353`  
		Last Modified: Sat, 28 May 2022 06:44:52 GMT  
		Size: 10.5 MB (10527450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83fc0890b460e9cb435797b7783b6dac8fc463c2bc4ed6c1984fadad8d1ef417`  
		Last Modified: Sat, 28 May 2022 06:44:51 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5741a5520fd28d42c30946f5935bab84e5bc5de985d73c9ae0557b837e5ddb80`  
		Last Modified: Sat, 28 May 2022 06:45:41 GMT  
		Size: 24.5 MB (24457087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92850f49ca64afd97a35ceef6da629d27ca71ebb93262ac93a6a7e5da4ef5e5b`  
		Last Modified: Sat, 28 May 2022 06:45:37 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52e6d729eefd74d37763482f1175bd884a1f0c4c6a9a682651257f4f28a4537a`  
		Last Modified: Sat, 28 May 2022 06:45:37 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e1b27add7c102801e25bdc919308ce547cf387906ba19490d5a54dcaa561cd`  
		Last Modified: Sat, 28 May 2022 06:45:37 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10eb27da94ae840221153b7b2056a82af56e25273e46d6960bd048f9091ccc5a`  
		Last Modified: Sat, 28 May 2022 22:16:50 GMT  
		Size: 1.6 MB (1644169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebfc0db131d4f1864225d2523e942a3cf8fae0ffad3c7fa96428c9fa91f8a8a2`  
		Last Modified: Sat, 28 May 2022 22:16:49 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18ae016190c5617b68417d8ba09157da488894530be3a3cf220e75332c2ee01`  
		Last Modified: Sat, 28 May 2022 22:23:15 GMT  
		Size: 3.4 MB (3382853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-fpm-buster` - linux; 386

```console
$ docker pull drupal@sha256:da3f45c4977fd8ade8c869599d7f95346b683f18b2b47aa98962fd1c76ba749c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **149.9 MB (149874097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e819135fe7681420370060556cd1ec8603eae927c99a911135ebc4855a8f4217`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Sat, 28 May 2022 00:40:01 GMT
ADD file:9aea7a35c215cdd778adec1dd5213973ef9b4830110e4550f2ead85679551ee5 in / 
# Sat, 28 May 2022 00:40:01 GMT
CMD ["bash"]
# Sat, 28 May 2022 13:07:46 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Sat, 28 May 2022 13:07:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Sat, 28 May 2022 13:08:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 13:08:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 May 2022 13:08:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 May 2022 13:08:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 13:08:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 May 2022 13:08:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 May 2022 14:20:40 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 28 May 2022 14:20:41 GMT
ENV PHP_VERSION=7.4.29
# Sat, 28 May 2022 14:20:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Sat, 28 May 2022 14:20:43 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Sat, 28 May 2022 14:20:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Sat, 28 May 2022 14:20:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 28 May 2022 14:27:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 28 May 2022 14:27:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 28 May 2022 14:27:34 GMT
RUN docker-php-ext-enable sodium
# Sat, 28 May 2022 14:27:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 28 May 2022 14:27:36 GMT
WORKDIR /var/www/html
# Sat, 28 May 2022 14:27:37 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 28 May 2022 14:27:38 GMT
STOPSIGNAL SIGQUIT
# Sat, 28 May 2022 14:27:39 GMT
EXPOSE 9000
# Sat, 28 May 2022 14:27:40 GMT
CMD ["php-fpm"]
# Sat, 28 May 2022 16:45:50 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 May 2022 16:45:51 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 28 May 2022 16:50:32 GMT
ENV DRUPAL_VERSION=7.89
# Sat, 28 May 2022 16:50:33 GMT
ENV DRUPAL_MD5=924e707e3b1e8269fe623cf2f22ee710
# Sat, 28 May 2022 16:50:35 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:40837b3d848885c0b0c031d6d950b38e6a26962a5ee49704cb3ca2d2db535617`  
		Last Modified: Sat, 28 May 2022 00:47:36 GMT  
		Size: 27.8 MB (27799572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a28d79d5aa87168f78db562f5ed522b4ca6e137827ebc56b5406f690e444f67`  
		Last Modified: Sat, 28 May 2022 14:42:13 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e29d85026bb424319623b6933a017c153d18ee323a49bb6313614946c6b8cb`  
		Last Modified: Sat, 28 May 2022 14:42:28 GMT  
		Size: 81.2 MB (81228806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc3bb47da6bf11574b5f2d9226625a8e1d353b8d852689a648f93c7d91afd1f`  
		Last Modified: Sat, 28 May 2022 14:42:13 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d129e8ef9ed12d600a27d757a4eb8e258af60790c5a90b70f16e955372b75a1`  
		Last Modified: Sat, 28 May 2022 14:53:28 GMT  
		Size: 10.5 MB (10528036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:294105cf695ca56251e0de1d1a850280623040ba4e4aa66576020feb70f46eac`  
		Last Modified: Sat, 28 May 2022 14:53:26 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33a5980eeb6ab3a4c611ab6e829a0dbbd3acca04bf116d5d4a14b69578ed988d`  
		Last Modified: Sat, 28 May 2022 14:54:28 GMT  
		Size: 25.2 MB (25166813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c0cbec177a24700419e2a40926278dcba2922b73f5c241146ce26e090f8532`  
		Last Modified: Sat, 28 May 2022 14:54:24 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d21f31de65077824b591318ff01a6c00c9a63ea4644c881a2ef135b16c861c`  
		Last Modified: Sat, 28 May 2022 14:54:24 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d095aab523361018b576bda2f502a0d0566808121c7f6a10236cccbb5d0fd540`  
		Last Modified: Sat, 28 May 2022 14:54:24 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0549529d7e5cf99b66d06e271c685b7006bfcdc1727d9537da629656f1b3b4`  
		Last Modified: Sat, 28 May 2022 17:11:03 GMT  
		Size: 1.8 MB (1755615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af357a5fccbb22ffb5b1515b842c3f6e0e834644f380c9cbd935d62b00bf04e9`  
		Last Modified: Sat, 28 May 2022 17:11:02 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73d13798599f9409c0f18f37f64864407bab08bcf053993d2a6e71176aecd80`  
		Last Modified: Sat, 28 May 2022 17:17:41 GMT  
		Size: 3.4 MB (3382854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-fpm-buster` - linux; mips64le

```console
$ docker pull drupal@sha256:5e23f82a76c512e43abc4d9ace1fd445d3d2f374a759fe8945e190b0502b029e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.0 MB (126994977 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34c6e0cdd80105bd072528a1eb5fc940b3576d7622536f9b6d8635327a2cbab1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 May 2022 02:24:43 GMT
ADD file:caccabd8a6e13c6bee91558efc76401078239e82c1a4a939aaf89520fab347fd in / 
# Wed, 11 May 2022 02:24:48 GMT
CMD ["bash"]
# Wed, 11 May 2022 14:58:27 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 14:58:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 14:59:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 15:00:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 15:00:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 15:00:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 15:00:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 15:00:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 22:11:06 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 11 May 2022 22:11:09 GMT
ENV PHP_VERSION=7.4.29
# Wed, 11 May 2022 22:11:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Wed, 11 May 2022 22:11:15 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Wed, 11 May 2022 22:11:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 22:12:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 22:43:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 22:43:58 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 May 2022 22:44:05 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 22:44:08 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 22:44:11 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 22:44:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 11 May 2022 22:44:21 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 May 2022 22:44:24 GMT
EXPOSE 9000
# Wed, 11 May 2022 22:44:27 GMT
CMD ["php-fpm"]
# Fri, 13 May 2022 08:18:03 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 13 May 2022 08:18:10 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 13 May 2022 08:18:13 GMT
ENV DRUPAL_VERSION=7.89
# Fri, 13 May 2022 08:18:17 GMT
ENV DRUPAL_MD5=924e707e3b1e8269fe623cf2f22ee710
# Fri, 13 May 2022 08:18:27 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:04988468cf482e6d371e4ebf5a6fb630cd38493fcc79fe45f15650a319a1a0a5`  
		Last Modified: Wed, 11 May 2022 02:35:04 GMT  
		Size: 25.8 MB (25814525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b99cde362b05b002179a926292c510922a5c0df126d888bb83cc6730a39c12`  
		Last Modified: Wed, 11 May 2022 22:58:31 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36cf3757060e28b1f6e27739c3f899a8503a2776793b440fa04dcfc4ae7603e`  
		Last Modified: Wed, 11 May 2022 22:59:15 GMT  
		Size: 61.4 MB (61408108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6c367a64ee731faa2d554502ddef593221c513a05bf429e29ea3eca9a8e40cc`  
		Last Modified: Wed, 11 May 2022 22:58:28 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5d600caf0ed1f1b75db4bac24b61a51a155f94e8ae634264207d32805afda4`  
		Last Modified: Wed, 11 May 2022 23:17:48 GMT  
		Size: 10.5 MB (10526464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d47a6ed86369bfd38b1c36badc73733500303d8895c121fe59d42c96c5b5bc36`  
		Last Modified: Wed, 11 May 2022 23:17:45 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380952ea2dcdfb4ae358a4bcad74ed2c3e287dff635fbc364cb2e0dcbe23e763`  
		Last Modified: Wed, 11 May 2022 23:19:03 GMT  
		Size: 24.2 MB (24227589 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f5090ca7ee75faaf590950bf568c1c20d98a16da7fcaa83a26741ae3d92e310`  
		Last Modified: Wed, 11 May 2022 23:18:49 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:429e1a7629a5620caf6757932ed0847b617a9cd09994672bf2ecc9d52552ecd0`  
		Last Modified: Wed, 11 May 2022 23:18:47 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0116a5d5e9c05241d6aa2de2d713d51011d30ddf344ac40e022f2f7ffdeabc22`  
		Last Modified: Wed, 11 May 2022 23:18:48 GMT  
		Size: 8.4 KB (8449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685db81e62be7179b76f944cc6c9dd930b3de726abb43a853655b45c9401540c`  
		Last Modified: Fri, 13 May 2022 08:20:55 GMT  
		Size: 1.6 MB (1623018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b7543d08e4d6c95d6dff2cf370e177eadec3586f6ced34c06cc72b3e3fcb1e`  
		Last Modified: Fri, 13 May 2022 08:20:54 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb04433915b700e59223ab3fb380885298a2d5e8440bf72a546c41aa05a7a79`  
		Last Modified: Fri, 13 May 2022 08:20:57 GMT  
		Size: 3.4 MB (3382848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-fpm-buster` - linux; ppc64le

```console
$ docker pull drupal@sha256:cde8dfa3b7d752ade840077dea375555e2b42bc6cca727b9b226c77720468169
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.3 MB (155302791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:377437389060c13422c2142bcd8c84221689db1bd41f1f1208774d12757638ea`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 May 2022 01:33:31 GMT
ADD file:57fcc3eadd20c2481e373ef3b56a194006f65b3c7ae29bd1747e625efcd89124 in / 
# Wed, 11 May 2022 01:33:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 16:16:45 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 16:16:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 16:19:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 16:19:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 16:19:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 16:19:28 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 16:19:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 16:19:37 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 19:25:40 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 11 May 2022 19:25:42 GMT
ENV PHP_VERSION=7.4.29
# Wed, 11 May 2022 19:25:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Wed, 11 May 2022 19:25:47 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Wed, 11 May 2022 19:26:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 19:26:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 19:41:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 19:41:03 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 May 2022 19:41:07 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 19:41:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 19:41:12 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 19:41:21 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 11 May 2022 19:41:26 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 May 2022 19:41:31 GMT
EXPOSE 9000
# Wed, 11 May 2022 19:41:34 GMT
CMD ["php-fpm"]
# Thu, 12 May 2022 14:25:41 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Thu, 12 May 2022 14:25:50 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 12 May 2022 14:36:28 GMT
ENV DRUPAL_VERSION=7.89
# Thu, 12 May 2022 14:36:31 GMT
ENV DRUPAL_MD5=924e707e3b1e8269fe623cf2f22ee710
# Thu, 12 May 2022 14:36:38 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:97c4e3bbd0d14c4a194ce9c48b362e1649c341b249c2ad560738b06fe8576dc3`  
		Last Modified: Wed, 11 May 2022 01:44:06 GMT  
		Size: 30.6 MB (30560544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7294fc5b14f6c2a4cfe653cdcf2bc547c17c3054782e9bfe7ee51f153965fd48`  
		Last Modified: Wed, 11 May 2022 20:04:00 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d9f7b323926d8cbf9887c0b380f52ea1d010441e74daec58aaec10ca276e275`  
		Last Modified: Wed, 11 May 2022 20:04:26 GMT  
		Size: 82.3 MB (82293084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f5e905d9e5d088e7c15fe7b7cb57ddade44e1837ba17cea7a66e3342fec270`  
		Last Modified: Wed, 11 May 2022 20:03:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1585579b94440cd4e52e51d576322ae15d03634cf6f8d0caef51269cc9131d72`  
		Last Modified: Wed, 11 May 2022 20:22:47 GMT  
		Size: 10.7 MB (10739964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b51e688606cd5cc28b127a9e59d3e17f1f8811dbba2f706f73241590556a609`  
		Last Modified: Wed, 11 May 2022 20:22:46 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee891a321d29d243d2f0de1b9b4d2706429bb7fbcccd1725bf4823316d77a552`  
		Last Modified: Wed, 11 May 2022 20:23:48 GMT  
		Size: 26.2 MB (26210421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96ab68e7e8e96cda3b547b5c59c3d48d3b2330a705d70df3a89e6219352e498`  
		Last Modified: Wed, 11 May 2022 20:23:44 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00643ab237d1e8f6e99b481d5e20452f9c329b4a41de70d963af1ce79238e25`  
		Last Modified: Wed, 11 May 2022 20:23:43 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fed87e41748c3dbccc77a4bb03f3df285c0d8667f321ab0b504f4fb5df7f26`  
		Last Modified: Wed, 11 May 2022 20:23:43 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30050273ce0464b1ffa7ae674f4bd6de439d36919ab7ffe5ab22a4c24ee1f970`  
		Last Modified: Thu, 12 May 2022 15:21:58 GMT  
		Size: 2.1 MB (2103163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e03e4afd50f72601c021cf0cddf6cb4577859c0eca9245e653c91dd549c81acc`  
		Last Modified: Thu, 12 May 2022 15:21:57 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4865a8d3357bf9ed1fd7facccb123dd46a7f23307564619fb99a05bd7c36c0`  
		Last Modified: Thu, 12 May 2022 15:40:51 GMT  
		Size: 3.4 MB (3383152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-fpm-buster` - linux; s390x

```console
$ docker pull drupal@sha256:47029049c43abc58b05a3fb5d2fb9978da4330ff3b1f4c81f4e889d1d60de293
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **130.7 MB (130711666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a9e9d42c65ee89dbfc208b605e932142d03e5ab9d38660fa710cef046181d4c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 11 May 2022 00:44:47 GMT
ADD file:28b1e60f65391906bebd81248a4da766172138fab99b8b9e6b18bce76afea02d in / 
# Wed, 11 May 2022 00:44:49 GMT
CMD ["bash"]
# Wed, 11 May 2022 09:10:51 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 11 May 2022 09:10:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 11 May 2022 09:11:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 09:11:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 11 May 2022 09:11:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 11 May 2022 09:11:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 09:11:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 11 May 2022 09:11:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 11 May 2022 10:33:36 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 11 May 2022 10:33:36 GMT
ENV PHP_VERSION=7.4.29
# Wed, 11 May 2022 10:33:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.29.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.29.tar.xz.asc
# Wed, 11 May 2022 10:33:36 GMT
ENV PHP_SHA256=7d0f07869f33311ff3fe1138dc0d6c0d673c37fcb737eaed2c6c10a949f1aed6
# Wed, 11 May 2022 10:33:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 11 May 2022 10:33:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 11 May 2022 10:40:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 11 May 2022 10:40:47 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 11 May 2022 10:40:48 GMT
RUN docker-php-ext-enable sodium
# Wed, 11 May 2022 10:40:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 11 May 2022 10:40:48 GMT
WORKDIR /var/www/html
# Wed, 11 May 2022 10:40:49 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 11 May 2022 10:40:49 GMT
STOPSIGNAL SIGQUIT
# Wed, 11 May 2022 10:40:49 GMT
EXPOSE 9000
# Wed, 11 May 2022 10:40:50 GMT
CMD ["php-fpm"]
# Wed, 11 May 2022 17:58:35 GMT
RUN set -eux; 		if command -v a2enmod; then 		a2enmod rewrite; 	fi; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libpng-dev 		libpq-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 17:58:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 11 May 2022 18:04:53 GMT
ENV DRUPAL_VERSION=7.89
# Wed, 11 May 2022 18:04:53 GMT
ENV DRUPAL_MD5=924e707e3b1e8269fe623cf2f22ee710
# Wed, 11 May 2022 18:04:55 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:bf64474a39a67000556a4502abd4584010a062b942cf8e2545d0502d38ffa150`  
		Last Modified: Wed, 11 May 2022 00:50:43 GMT  
		Size: 25.8 MB (25758738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a525bde4054c9188482f1bc960c8dce2d2b7399ff1c138e471f8ac4c20fa099f`  
		Last Modified: Wed, 11 May 2022 10:55:36 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdcd52f3187608b40cd9995c5289500f388c8fdfe08afa7eee1db2c9ea311fa9`  
		Last Modified: Wed, 11 May 2022 10:55:45 GMT  
		Size: 64.7 MB (64726188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:765dbb2648a936aca9898736e993c8703d18a143eea9dce2246bff8004f51403`  
		Last Modified: Wed, 11 May 2022 10:55:36 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0274631e1b0549744f2028d70e6057ea816616afd1f8fd8fbad3aaa4de72fb91`  
		Last Modified: Wed, 11 May 2022 11:05:59 GMT  
		Size: 10.7 MB (10738708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a74e9f9e2f072187305b840e8fc18e4a6ce08c1a0d8e51e65b33d1af31f4b9`  
		Last Modified: Wed, 11 May 2022 11:05:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53cbd2eaaa2776c4c691cef0ed5e93e018ed7f9cfe99587d92d16740031b1fd0`  
		Last Modified: Wed, 11 May 2022 11:06:36 GMT  
		Size: 24.3 MB (24273078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8187d0aa10eb5caf67dad572808c31e5beb0c0ee9609b24e7b4a9949913aa286`  
		Last Modified: Wed, 11 May 2022 11:06:33 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:914aee432e2c4852bea148260de76afa3c4bc5b166ca50bada24e9fbe78ef670`  
		Last Modified: Wed, 11 May 2022 11:06:33 GMT  
		Size: 243.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:167d85caa4b0d11e98576d8fe8772c35fa1f719130d16bd1a1a346e64edc2fd0`  
		Last Modified: Wed, 11 May 2022 11:06:33 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a3878e39dd9557a84e207c2867b61ab72747fa0ad031e2aa42beeda755812d`  
		Last Modified: Wed, 11 May 2022 18:22:47 GMT  
		Size: 1.8 MB (1819364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14271522b0aa03dc00c916c834799f8009ffe3e8f48788aa9913ec5b41ac3df3`  
		Last Modified: Wed, 11 May 2022 18:22:47 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e6c8d26619b09404c6593d8c9962f5cb92a0d25444c22dbac7d6540dc9f3975`  
		Last Modified: Wed, 11 May 2022 18:27:08 GMT  
		Size: 3.4 MB (3383139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
