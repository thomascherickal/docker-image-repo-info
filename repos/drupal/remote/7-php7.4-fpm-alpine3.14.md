## `drupal:7-php7.4-fpm-alpine3.14`

```console
$ docker pull drupal@sha256:80862d1739f8b34429542a47f813a03b4d54878777df3d36115375ac5c61cef3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `drupal:7-php7.4-fpm-alpine3.14` - linux; amd64

```console
$ docker pull drupal@sha256:241b1e7b163ed33048f11b0778efde315f22081922bdf6ba7638a2a27a7afce0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34630252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:45a6226c0bf0676043e17c18636f9254750ba1858e37e41898bc3d307dc02520`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:48:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 07:48:45 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 07:48:47 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 07:48:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 07:48:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 07:48:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 07:48:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 07:48:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 09:13:39 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Nov 2021 16:53:45 GMT
ENV PHP_VERSION=7.4.26
# Thu, 18 Nov 2021 16:53:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 18 Nov 2021 16:53:46 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 18 Nov 2021 16:54:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Nov 2021 16:54:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 17:12:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 17:12:28 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 18 Nov 2021 17:12:30 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 17:12:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 17:12:31 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 17:12:33 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Nov 2021 17:12:33 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Nov 2021 17:12:34 GMT
EXPOSE 9000
# Thu, 18 Nov 2021 17:12:34 GMT
CMD ["php-fpm"]
# Thu, 18 Nov 2021 21:36:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 18 Nov 2021 21:36:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 03 Dec 2021 17:55:30 GMT
ENV DRUPAL_VERSION=7.83
# Fri, 03 Dec 2021 17:55:30 GMT
ENV DRUPAL_MD5=c8833da8f1ef03a244b4130b71872e26
# Fri, 03 Dec 2021 17:55:31 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67f99012ff9aa7245baebc28963e44f53cc1832fcfaec246f78b5e7e861fbe6`  
		Last Modified: Sat, 13 Nov 2021 10:43:29 GMT  
		Size: 1.7 MB (1712224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db81da314e0b3e7be6d4c80bd6a2cdc1d7f66d6fffc8334a527f6b6e20fca340`  
		Last Modified: Sat, 13 Nov 2021 10:43:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5646ac679ebe77089fb6446f9911a66ae64db7d5b774d356b04c1c911ca0a081`  
		Last Modified: Sat, 13 Nov 2021 10:43:29 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be823f312052566b7ce9a4bd0f842ce5bb4a3eb11a295a0326824ffabb11329`  
		Last Modified: Thu, 18 Nov 2021 19:40:54 GMT  
		Size: 10.4 MB (10440243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bf6fbeb3f2d33e3045b03de8b00c39540b64ff8ade8bbbceaee342cee8de90`  
		Last Modified: Thu, 18 Nov 2021 19:40:53 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81a787dbd1e9ce1abbb601e5097839f68fa0872fcf2b20fe9e08d92706cc3f6`  
		Last Modified: Thu, 18 Nov 2021 19:41:36 GMT  
		Size: 14.4 MB (14365377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c60064d1dcd12774fdd35b08d44c9d8d6c36a2d2d22665d0c9aac5122765bae`  
		Last Modified: Thu, 18 Nov 2021 19:41:33 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad85c2c33f48fea14f6fcc5a45bda37d44c29b176783ba30c4ef8ffaec9579a`  
		Last Modified: Thu, 18 Nov 2021 19:41:33 GMT  
		Size: 18.2 KB (18197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0380c49e03155916174a049701a799d4e3acde985be9ddb835bb401c0c4bc776`  
		Last Modified: Thu, 18 Nov 2021 19:41:33 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4af5bebb6c842681c9e7cff45bd2700372ddb2cac6e3d555a199f24b31233e`  
		Last Modified: Thu, 18 Nov 2021 21:48:59 GMT  
		Size: 1.9 MB (1878059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6e67fc3d81a8db77e1fa335706c6f13ce2b018176de0df31fdd0eddc686f96c`  
		Last Modified: Thu, 18 Nov 2021 21:48:58 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:436e40cd8d34cb2058ace185dac564591a1b07b948eb1209af288c91407cd9d9`  
		Last Modified: Fri, 03 Dec 2021 18:13:13 GMT  
		Size: 3.4 MB (3380071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-fpm-alpine3.14` - linux; arm variant v6

```console
$ docker pull drupal@sha256:07618aad332e7923b2bfd04c37a0bbc56491e236724fa99eea63cfff025042f2
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33304502 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:910f8bd2621adb3cee2adaf2418f729b014d45fcce0ad35c3a17268facd50c1c`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 01:00:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 01:00:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 01:00:57 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 01:00:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 01:00:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 01:01:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 01:01:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 01:01:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 01:41:14 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Nov 2021 15:54:58 GMT
ENV PHP_VERSION=7.4.26
# Thu, 18 Nov 2021 15:54:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 18 Nov 2021 15:54:59 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 18 Nov 2021 15:55:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Nov 2021 15:55:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:04:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 16:04:45 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:04:48 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 16:04:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 16:04:49 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 16:04:51 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Nov 2021 16:04:51 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Nov 2021 16:04:52 GMT
EXPOSE 9000
# Thu, 18 Nov 2021 16:04:52 GMT
CMD ["php-fpm"]
# Thu, 18 Nov 2021 17:30:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 18 Nov 2021 17:30:45 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 02 Dec 2021 19:59:39 GMT
ENV DRUPAL_VERSION=7.83
# Thu, 02 Dec 2021 19:59:39 GMT
ENV DRUPAL_MD5=c8833da8f1ef03a244b4130b71872e26
# Thu, 02 Dec 2021 19:59:43 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fb65eff99d3570be8bbee58e3796b49e0e6fbc64d6c2b55e01eaf1b07709af`  
		Last Modified: Sat, 13 Nov 2021 02:49:22 GMT  
		Size: 1.7 MB (1702248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe18ffa25cea29b8a20ba6c41b7485fd89e792d6d333919ea738dcff33555f`  
		Last Modified: Sat, 13 Nov 2021 02:49:21 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215c6f1ae3409a42a8b2531ec3f19b4dddc77724624fdc7fe72175b53fa03ad0`  
		Last Modified: Sat, 13 Nov 2021 02:49:21 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51043c3368ded4fd963ab642ab064049684d3774825d00295f6ca60cfab1f3a0`  
		Last Modified: Thu, 18 Nov 2021 17:04:34 GMT  
		Size: 10.4 MB (10440263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687f953ec69c43d8ed6b25d8342ad3a9988bfd9ec8b998a3c9150b701281c7e1`  
		Last Modified: Thu, 18 Nov 2021 17:04:32 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af3d8c14828174afaf52ea2d1687ebcae18f6fdc9347eceaea6729d50dab442`  
		Last Modified: Thu, 18 Nov 2021 17:05:43 GMT  
		Size: 13.4 MB (13355049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6b8b2d0a6bd485b05c2660f05a72d3a5e2219859149cc907f5fc3286267f0b`  
		Last Modified: Thu, 18 Nov 2021 17:05:37 GMT  
		Size: 2.3 KB (2300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f11a7caf8be03ecdabf9c5e394252e56c2331c1e5fe80678288415d3edabd04`  
		Last Modified: Thu, 18 Nov 2021 17:05:36 GMT  
		Size: 18.2 KB (18205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b138828e619a0e3c36f93378809eada43426c21ccbad05764660a00bd394ba`  
		Last Modified: Thu, 18 Nov 2021 17:05:36 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbec1a6d8e720d8a0f03026fb03c13563f7e3fe0cae612812d4ab678e3b76b8d`  
		Last Modified: Thu, 18 Nov 2021 17:44:07 GMT  
		Size: 1.8 MB (1760180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:387e1fcaf00281e816f00bfa8870ac5d256275e3626a8141820d09a705a443e7`  
		Last Modified: Thu, 18 Nov 2021 17:44:06 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:138145e9b07511e1b8c76ac1d640e86baa86d29d0572b745598375255d153b90`  
		Last Modified: Thu, 02 Dec 2021 20:11:22 GMT  
		Size: 3.4 MB (3380077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-fpm-alpine3.14` - linux; arm variant v7

```console
$ docker pull drupal@sha256:33e80c41faf14b4c40d2ba7eced4eadca533e46f74afe9009405072e4a31506a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.9 MB (31949614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7b695884ddf41cb928fa507d2f7b9c6dce7f77bde4344a3fdbe262e082657ea`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 02:20:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 02:20:29 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 02:20:30 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 02:20:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 02:20:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 02:20:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 02:20:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 02:20:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 03:03:08 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Nov 2021 17:34:29 GMT
ENV PHP_VERSION=7.4.26
# Thu, 18 Nov 2021 17:34:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 18 Nov 2021 17:34:30 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 18 Nov 2021 17:34:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Nov 2021 17:34:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 17:43:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 17:43:34 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 18 Nov 2021 17:43:36 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 17:43:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 17:43:37 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 17:43:39 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Nov 2021 17:43:39 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Nov 2021 17:43:40 GMT
EXPOSE 9000
# Thu, 18 Nov 2021 17:43:40 GMT
CMD ["php-fpm"]
# Fri, 19 Nov 2021 03:04:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 19 Nov 2021 03:04:18 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 19 Nov 2021 03:18:35 GMT
ENV DRUPAL_VERSION=7.82
# Fri, 19 Nov 2021 03:18:36 GMT
ENV DRUPAL_MD5=51f8515161087935662b9835194a779b
# Fri, 19 Nov 2021 03:18:39 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d591a38553bed13e4644c2ee36cc92a36f4f866265bcec258baef16176c11b`  
		Last Modified: Sat, 13 Nov 2021 04:21:17 GMT  
		Size: 1.6 MB (1571523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a132a38f5266edd87272c20d2129b4448b3dfb530a70424219ddd45fd1d2eb73`  
		Last Modified: Sat, 13 Nov 2021 04:21:16 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a99b8f25382a7fadffc08ae9ebf09b2a2be48a858daf03148035e46335c089a`  
		Last Modified: Sat, 13 Nov 2021 04:21:16 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33572509eb61a00128f39ee9fda81cb699091c67e258241e7006f6a508e94157`  
		Last Modified: Thu, 18 Nov 2021 19:39:10 GMT  
		Size: 10.4 MB (10440242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72afaf8d84251c8c9bb1d3668785c2bce2ef1c270b5f1b16c3fe057f380e8d20`  
		Last Modified: Thu, 18 Nov 2021 19:39:08 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779edc804ece016723b3d8569453951e1eba3770d689a2cbf58191273848167e`  
		Last Modified: Thu, 18 Nov 2021 19:40:20 GMT  
		Size: 12.5 MB (12504986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7d608b067cd591eeb1aeb25e822c5890e6f0852f8fb1dc5989b5e636ed317a`  
		Last Modified: Thu, 18 Nov 2021 19:40:12 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c49ede17d89f8439fbf9a98b9e5e11eb4ffd92ad07c9add13382718835bbb6a`  
		Last Modified: Thu, 18 Nov 2021 19:40:12 GMT  
		Size: 18.2 KB (18192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29cea458fe8e3a0f91069e42c6056acc7769666ee60cf64ad2dc28a258f740b7`  
		Last Modified: Thu, 18 Nov 2021 19:40:12 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ba996a6b50982676d1894db1c5a3dfe2f456dd8da47d5b88c4c52aed6cb3e27`  
		Last Modified: Fri, 19 Nov 2021 03:42:14 GMT  
		Size: 1.6 MB (1588941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75067b44b620210d1c2c4520db54d49639d141eba300246ddf8c792155c54f8`  
		Last Modified: Fri, 19 Nov 2021 03:42:14 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:375a26d0ad98c6a5f9f0988e30ec705444f256f8f95843bc1ce41853d13123e0`  
		Last Modified: Fri, 19 Nov 2021 03:56:44 GMT  
		Size: 3.4 MB (3374014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-fpm-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:6cc5e669093c80b36afaea4dbc58d55f31b9037b1ac176e4bc7040402aac9d62
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34292753 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:628639f8505889f106c989e2fea4f264ae06b458c347e1d1e89ec7f2d2d097b7`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:30:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 12 Nov 2021 19:30:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 12 Nov 2021 19:30:35 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 12 Nov 2021 19:30:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Nov 2021 19:30:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Nov 2021 19:30:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:30:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:30:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Nov 2021 20:22:50 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Nov 2021 16:16:44 GMT
ENV PHP_VERSION=7.4.26
# Thu, 18 Nov 2021 16:16:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 18 Nov 2021 16:16:46 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 18 Nov 2021 16:16:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Nov 2021 16:16:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:24:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 16:24:17 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:24:18 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 16:24:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 16:24:19 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 16:24:20 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Nov 2021 16:24:21 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Nov 2021 16:24:22 GMT
EXPOSE 9000
# Thu, 18 Nov 2021 16:24:23 GMT
CMD ["php-fpm"]
# Thu, 18 Nov 2021 23:50:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 18 Nov 2021 23:50:43 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 03 Dec 2021 12:27:46 GMT
ENV DRUPAL_VERSION=7.83
# Fri, 03 Dec 2021 12:27:47 GMT
ENV DRUPAL_MD5=c8833da8f1ef03a244b4130b71872e26
# Fri, 03 Dec 2021 12:27:49 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9716534ffbe55fb7b1cdc9c51401565113fe78d473379c595bf42e6d05fd5e6e`  
		Last Modified: Fri, 12 Nov 2021 21:25:50 GMT  
		Size: 1.7 MB (1711801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d47cbc9449ef4aab290c562e2d538c1152c89268a02bb026807264d1c3d6da`  
		Last Modified: Fri, 12 Nov 2021 21:25:49 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a654447725655854a94c8af1e17c61ba95c1eb179a627aa323bfd70bfbae408`  
		Last Modified: Fri, 12 Nov 2021 21:25:50 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe8a5cd6e7b96df864899309b2e8c0fa05b123321e61f6af6cbc7d98ce260c8`  
		Last Modified: Thu, 18 Nov 2021 17:35:10 GMT  
		Size: 10.4 MB (10440015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d909104778cbfc0311368bde399e8451a0e2a0d149c22eb42fcb1ac70c3cfc`  
		Last Modified: Thu, 18 Nov 2021 17:35:09 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7da90346c6fbfe105ca5ed861a6d771a222ac2c800f62b145cd08fa636b6f51`  
		Last Modified: Thu, 18 Nov 2021 17:35:57 GMT  
		Size: 14.1 MB (14142606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdef70d9f1a8d1a096749e1610f7529ca4c5f58b6ab6a94de1ad3167f860ba69`  
		Last Modified: Thu, 18 Nov 2021 17:35:55 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a3657fb4056704509e3c814335d219d1f7ddc4c6df8d32975d2a582a383670`  
		Last Modified: Thu, 18 Nov 2021 17:35:55 GMT  
		Size: 18.1 KB (18109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee09c074e685d06c59d3db8fc9c241d78fc68e320fea7ab92c8638d4d44b59f`  
		Last Modified: Thu, 18 Nov 2021 17:35:54 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2992445fb0c0a91b5a77dd2d879c2b23d6d74db07e2d6c6954ea62a9aab6f188`  
		Last Modified: Fri, 19 Nov 2021 00:12:38 GMT  
		Size: 1.9 MB (1869453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987c92fe1ab2a29b3ef462290137bcd287a36da5fc17ba5cd781e5d1ca96d63d`  
		Last Modified: Fri, 19 Nov 2021 00:12:38 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe671daf56fec3ed6f6f26dc8f597779c382297414e6343168209e4ff5588f30`  
		Last Modified: Fri, 03 Dec 2021 12:59:50 GMT  
		Size: 3.4 MB (3380047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-fpm-alpine3.14` - linux; 386

```console
$ docker pull drupal@sha256:79dff2a0c69e245a7fd620b668f1bfab72392133a669d1c2e76f298b5896d5b9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35226879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:408229582120b6936270a005275f8a9380a0ef245029bf243d4c9af16b44a872`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 00:47:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 00:47:24 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 00:47:26 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 00:47:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 00:47:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 00:47:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 00:47:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 00:47:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 02:05:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Nov 2021 16:36:04 GMT
ENV PHP_VERSION=7.4.26
# Thu, 18 Nov 2021 16:36:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 18 Nov 2021 16:36:05 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 18 Nov 2021 16:36:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Nov 2021 16:36:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:53:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 16:53:53 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:53:54 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 16:53:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 16:53:55 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 16:53:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Nov 2021 16:53:56 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Nov 2021 16:53:56 GMT
EXPOSE 9000
# Thu, 18 Nov 2021 16:53:56 GMT
CMD ["php-fpm"]
# Thu, 18 Nov 2021 23:50:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 18 Nov 2021 23:50:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 03 Dec 2021 07:45:54 GMT
ENV DRUPAL_VERSION=7.83
# Fri, 03 Dec 2021 07:45:55 GMT
ENV DRUPAL_MD5=c8833da8f1ef03a244b4130b71872e26
# Fri, 03 Dec 2021 07:45:58 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c05111b719bf0e9c81182879ace55b68244fff3ccaacc6813f9ce740b1adf4d`  
		Last Modified: Sat, 13 Nov 2021 04:00:31 GMT  
		Size: 1.8 MB (1812696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f12e62d2679739a2acadab070b1c7d0f433a8a46d449147d00fa5c4aa0a8753`  
		Last Modified: Sat, 13 Nov 2021 04:00:30 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3e1535943b040497915113f37b46a4ba0dc10f27aabcdb6dbf9d0b594ca8be`  
		Last Modified: Sat, 13 Nov 2021 04:00:30 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e3f24501ef304b64e206982d7aa4664cc7425378028bd85a1d8bec6a61b1fd`  
		Last Modified: Thu, 18 Nov 2021 19:37:10 GMT  
		Size: 10.4 MB (10440236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cceece03507d726abbafc27867570be8fcec456898af998289ca0a5034a71027`  
		Last Modified: Thu, 18 Nov 2021 19:37:09 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed81a5e471a0fb0ac5db3803906d670ff33f24ce191b6d5503a37b724d753592`  
		Last Modified: Thu, 18 Nov 2021 19:38:05 GMT  
		Size: 14.7 MB (14739579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d34c69be3be4d02cde28162b729b0909898059702aee6a6529b76167bae54c4`  
		Last Modified: Thu, 18 Nov 2021 19:38:00 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a719c36dc46411961b026b86c9b6744fc257a4d971e7637af885757b17898f`  
		Last Modified: Thu, 18 Nov 2021 19:38:00 GMT  
		Size: 18.2 KB (18188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f545379a5e98d3ea29f36cd127d7f7e95d2f119e73b1f51eb227c6a98185fc`  
		Last Modified: Thu, 18 Nov 2021 19:38:00 GMT  
		Size: 8.4 KB (8438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6c4db3907b523936b23cd84bdc51343ac883034469a45e8b731c0c5cfdec99`  
		Last Modified: Fri, 19 Nov 2021 00:13:56 GMT  
		Size: 2.0 MB (1992065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc4e3d8578e1db4776d8f4168fb79348f95b7b314a53d64954c9b7eccf9526c`  
		Last Modified: Fri, 19 Nov 2021 00:13:55 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efe321051e490ffb7518ce7f08a678f4e25929c1d9672f857534a70ec55af94`  
		Last Modified: Fri, 03 Dec 2021 08:23:37 GMT  
		Size: 3.4 MB (3380078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-fpm-alpine3.14` - linux; ppc64le

```console
$ docker pull drupal@sha256:24950dc487150f175d6f5b258b94a3d4d5ce3f3450a9b27a8759c5b8c883a693
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35875873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c755cce16c26844192fa63ede0d4e738ddace40aa87c6045ef889020ab6aba4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:56:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 11:56:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 11:56:13 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 11:56:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 11:56:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 11:56:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 11:56:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 11:56:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 12:51:23 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Nov 2021 17:05:30 GMT
ENV PHP_VERSION=7.4.26
# Thu, 18 Nov 2021 17:05:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 18 Nov 2021 17:05:39 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 18 Nov 2021 17:06:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Nov 2021 17:06:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 17:16:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 17:16:35 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 18 Nov 2021 17:16:43 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 17:16:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 17:16:56 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 17:17:03 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Nov 2021 17:17:08 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Nov 2021 17:17:12 GMT
EXPOSE 9000
# Thu, 18 Nov 2021 17:17:14 GMT
CMD ["php-fpm"]
# Fri, 19 Nov 2021 07:46:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 19 Nov 2021 07:46:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 03 Dec 2021 16:47:50 GMT
ENV DRUPAL_VERSION=7.83
# Fri, 03 Dec 2021 16:47:52 GMT
ENV DRUPAL_MD5=c8833da8f1ef03a244b4130b71872e26
# Fri, 03 Dec 2021 16:47:58 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf526002982778a0157923a6219fbadd645d22999e9251af0db89be07d002272`  
		Last Modified: Sat, 13 Nov 2021 14:08:23 GMT  
		Size: 1.8 MB (1759206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b47bb623f5bce1748b7a2c4e16b2726478248c03150000de676a1020aaeada`  
		Last Modified: Sat, 13 Nov 2021 14:08:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f035bbd1b7db7792a68686cccf93b48bd273f6f89375962d7fae46bab690f7ac`  
		Last Modified: Sat, 13 Nov 2021 14:08:23 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ca048d84a232d0369a78f9f5bf66058a7e1c2a028f54aa283b9890a81d0b2d`  
		Last Modified: Thu, 18 Nov 2021 19:08:44 GMT  
		Size: 10.4 MB (10440243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4af54fb1c5fa2e7a563486f08bd776a2e77920493432d57cb1fa9e7f3e2221`  
		Last Modified: Thu, 18 Nov 2021 19:08:42 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22abbb1bfdfab112ca8f4555945d8cc158f898ab6c7082672177729f50bdb9f0`  
		Last Modified: Thu, 18 Nov 2021 19:09:45 GMT  
		Size: 15.4 MB (15400958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85829949ff50cbd0cb85470e897b384e4dfd995a8ef131b2aabd503f78ad44c8`  
		Last Modified: Thu, 18 Nov 2021 19:09:34 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bf287c1d47a86d0a2ef12df4a2d3e23355fe12430d14c89bf932720f79f516`  
		Last Modified: Thu, 18 Nov 2021 19:09:34 GMT  
		Size: 18.2 KB (18200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa20a5b92239e77c1a86c3d4d7fbe9767a0fb8f8393f6c0aad7866bbbc72941`  
		Last Modified: Thu, 18 Nov 2021 19:09:34 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f26d5d983f5eec8faa0fe4a3fafd6dd7ea919a055af7bbcb682ca3b3446be8c`  
		Last Modified: Fri, 19 Nov 2021 08:43:09 GMT  
		Size: 2.0 MB (2046622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898336bc873a43ca3f204684c7e1fb3392fcaa1393dae13404d02c6e05af7445`  
		Last Modified: Fri, 19 Nov 2021 08:43:08 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b446df17ee41491f0ad915fc4aedeeb69b4e3540a15e890ff859cd1b504688ad`  
		Last Modified: Fri, 03 Dec 2021 17:40:16 GMT  
		Size: 3.4 MB (3380072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-php7.4-fpm-alpine3.14` - linux; s390x

```console
$ docker pull drupal@sha256:9c4c3e9b9080b154445249988e330396e651272197a09e653451da0ba7f70376
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33878473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7ae1c557c8a654486813ef010a47c94c4d5cc945cb970c17c63676d586c558ea`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:58:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 12 Nov 2021 19:58:15 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 12 Nov 2021 19:58:15 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 12 Nov 2021 19:58:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Nov 2021 19:58:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Nov 2021 19:58:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:58:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:58:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Nov 2021 20:25:15 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Nov 2021 16:10:18 GMT
ENV PHP_VERSION=7.4.26
# Thu, 18 Nov 2021 16:10:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 18 Nov 2021 16:10:18 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 18 Nov 2021 16:10:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Nov 2021 16:10:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:16:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 16:16:02 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:16:03 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 16:16:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 16:16:03 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 16:16:04 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Nov 2021 16:16:04 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Nov 2021 16:16:04 GMT
EXPOSE 9000
# Thu, 18 Nov 2021 16:16:04 GMT
CMD ["php-fpm"]
# Thu, 18 Nov 2021 17:43:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 18 Nov 2021 17:43:38 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 02 Dec 2021 23:43:06 GMT
ENV DRUPAL_VERSION=7.83
# Thu, 02 Dec 2021 23:43:06 GMT
ENV DRUPAL_MD5=c8833da8f1ef03a244b4130b71872e26
# Thu, 02 Dec 2021 23:43:07 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c6db577f243875f52f246d8a7fdab675a850569d52d6bba314f58258225c1f`  
		Last Modified: Fri, 12 Nov 2021 21:10:48 GMT  
		Size: 1.8 MB (1774038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a472bfa2a1552842a7406f914151af808b4f2a9e245ddbfe7cbc332697f96b12`  
		Last Modified: Fri, 12 Nov 2021 21:10:47 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3cea1835285017465c0df7a510c36971229f7066ec32d2ac436c4f9ac6ebd3`  
		Last Modified: Fri, 12 Nov 2021 21:10:48 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef39893b173d7482549954a8906a84c6259e96aa7a05ce7064736a5e7976e19`  
		Last Modified: Thu, 18 Nov 2021 17:13:23 GMT  
		Size: 10.4 MB (10440256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b49d88c28aa16cbe7e9d20f58f0bd1b057d931184ff26e98cadfbea30f19b63`  
		Last Modified: Thu, 18 Nov 2021 17:13:23 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d7e10db1b37109285a8a55fa59f9b4801a4374a7cf5fd18874511f2a75a8f2`  
		Last Modified: Thu, 18 Nov 2021 17:13:59 GMT  
		Size: 13.7 MB (13726628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5461377de4e6e3348a6e3ff5c6a9a0b84e1788feb5cd8b58b35e6a71258449`  
		Last Modified: Thu, 18 Nov 2021 17:13:57 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09523c5daed1194164f48b562608f20738add5802c9f64a92a92be73d826b868`  
		Last Modified: Thu, 18 Nov 2021 17:13:57 GMT  
		Size: 18.2 KB (18213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e4368bf16410417b043be286103fd2e079fe91e5149d43509b5ef64f060230`  
		Last Modified: Thu, 18 Nov 2021 17:13:57 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:203a568e57153112fac90a11186177d5bc72d1151c26cfc6006fe095c72d152c`  
		Last Modified: Thu, 18 Nov 2021 17:57:32 GMT  
		Size: 1.9 MB (1916896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db1344e4980d93988af78e2cbeaa7856b444bccd65149929e936e465bb100d61`  
		Last Modified: Thu, 18 Nov 2021 17:57:32 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a350e35139350b9d0ffad302fdc6334e6ec1400cea774255f39f538b4b7acff`  
		Last Modified: Thu, 02 Dec 2021 23:59:39 GMT  
		Size: 3.4 MB (3380070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
