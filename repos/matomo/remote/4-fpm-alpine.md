## `matomo:4-fpm-alpine`

```console
$ docker pull matomo@sha256:8134f3ed95eef4b4f424da339796fd540fe3c5f48490e28cedfa904e71e88b9b
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

### `matomo:4-fpm-alpine` - linux; amd64

```console
$ docker pull matomo@sha256:8c420b11c8e920380b877c9d6debeff71713eb77661ff9061e94d7dadf654ad5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52876469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7bb9b5afd5bba3198a23990a9224d052d62bf3ead662a6cc5fcb09bcdc6e5f18`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 07:06:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 07:06:03 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 07:06:04 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 07:06:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 07:06:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 07:06:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 07:06:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 07:06:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 07:50:54 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 30 Nov 2021 07:50:54 GMT
ENV PHP_VERSION=8.0.13
# Tue, 30 Nov 2021 07:50:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.13.tar.xz.asc
# Tue, 30 Nov 2021 07:50:55 GMT
ENV PHP_SHA256=cd976805ec2e9198417651027dfe16854ba2c2c388151ab9d4d268513d52ed52
# Tue, 30 Nov 2021 07:51:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 30 Nov 2021 07:51:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 30 Nov 2021 08:10:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 30 Nov 2021 08:10:04 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Tue, 30 Nov 2021 08:10:05 GMT
RUN docker-php-ext-enable sodium
# Tue, 30 Nov 2021 08:10:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 30 Nov 2021 08:10:06 GMT
WORKDIR /var/www/html
# Tue, 30 Nov 2021 08:10:07 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 30 Nov 2021 08:10:07 GMT
STOPSIGNAL SIGQUIT
# Tue, 30 Nov 2021 08:10:07 GMT
EXPOSE 9000
# Tue, 30 Nov 2021 08:10:07 GMT
CMD ["php-fpm"]
# Thu, 09 Dec 2021 02:32:23 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 09 Dec 2021 02:32:23 GMT
ENV PHP_MEMORY_LIMIT=256M
# Thu, 09 Dec 2021 02:34:18 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		procps 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 09 Dec 2021 02:34:19 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 10 Dec 2021 20:21:11 GMT
ENV MATOMO_VERSION=4.6.2
# Fri, 10 Dec 2021 20:21:22 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Fri, 10 Dec 2021 20:21:22 GMT
COPY file:f4ea35cff07e183c01b4e508329d1f5c342d9f4d330bda7f28faa530ced0d166 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 10 Dec 2021 20:21:23 GMT
COPY file:ccb778224a0e1f6742127aba2860c245adf24b73ca277e7260c4789883751ccb in /entrypoint.sh 
# Fri, 10 Dec 2021 20:21:23 GMT
VOLUME [/var/www/html]
# Fri, 10 Dec 2021 20:21:23 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Dec 2021 20:21:23 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7da25b2876b1c935b05d7e6efa3e8cd559d031cf30b246d7659ed438726acd`  
		Last Modified: Tue, 30 Nov 2021 09:03:50 GMT  
		Size: 1.7 MB (1709704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc599114627e3bd98e0204b93b161e03065bf9a228bb02ae202469655f12b8d`  
		Last Modified: Tue, 30 Nov 2021 09:03:48 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927a0b37a45a98d7d74a6d7d1567230eca834fb89417274557de7986d1f39401`  
		Last Modified: Tue, 30 Nov 2021 09:03:48 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8279146e52ed2a974f5b5c9beb9ed70e318d47933f75b90ac98b43fa8d2acb90`  
		Last Modified: Tue, 30 Nov 2021 09:06:07 GMT  
		Size: 10.9 MB (10874437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f188883b50e9cfa0b6c53eade32b6bc7ad6c8fb94f54e367cfb12fb51d2c7463`  
		Last Modified: Tue, 30 Nov 2021 09:06:06 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56c64d4e1e1119f9ba45e483f25ed039862777bc357d25d01bfc72b3dc37406b`  
		Last Modified: Tue, 30 Nov 2021 09:06:37 GMT  
		Size: 15.1 MB (15076760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003d402c413f81aeeaf12e6c9216955bdcead8fa9f5973307adac74dd5380085`  
		Last Modified: Tue, 30 Nov 2021 09:06:35 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be58cf002ec573fe20946a0095f58f1c8f740c1222cd634c0707398690c32a6`  
		Last Modified: Tue, 30 Nov 2021 09:06:35 GMT  
		Size: 18.2 KB (18207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944bcdcab902cc1f44eb36d744da209571222ecfb40b2203b5ba4cce191effcc`  
		Last Modified: Tue, 30 Nov 2021 09:06:35 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3444a35645970cf022f52d2ec383075635e416ec362b1761d6fdcff2c38d3855`  
		Last Modified: Thu, 09 Dec 2021 02:37:43 GMT  
		Size: 6.1 MB (6117961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852b467c7632bcfa6fb5b1f068044bb33dc286e21242e6c5738057a814d90e98`  
		Last Modified: Thu, 09 Dec 2021 02:37:42 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719a6dbd64a2b380dcedf65e83386c0bf482802784b4b0f2385123fa82bf0152`  
		Last Modified: Fri, 10 Dec 2021 20:22:45 GMT  
		Size: 16.2 MB (16246793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926da7d388a5aa8be4b0b849137495366397a043cecebae1991118a1121a9af1`  
		Last Modified: Fri, 10 Dec 2021 20:22:42 GMT  
		Size: 342.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad912c8b3b85087c659b052a57ff28a52ce887466320ff4be94c2197c2dc9e03`  
		Last Modified: Fri, 10 Dec 2021 20:22:42 GMT  
		Size: 632.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-fpm-alpine` - linux; arm variant v6

```console
$ docker pull matomo@sha256:e4d296424ec32865973195d35201fb1513281c0af00097eb1b06f42cae7820a3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50458930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a07faa1e058cdeb72abf43fccb406df702b798d59173a71db593358da5bd9d0`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 03:20:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 03:20:06 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 03:20:07 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 03:20:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 03:20:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 03:20:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 03:20:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 03:20:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 03:40:16 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 30 Nov 2021 03:40:17 GMT
ENV PHP_VERSION=8.0.13
# Tue, 30 Nov 2021 03:40:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.13.tar.xz.asc
# Tue, 30 Nov 2021 03:40:18 GMT
ENV PHP_SHA256=cd976805ec2e9198417651027dfe16854ba2c2c388151ab9d4d268513d52ed52
# Tue, 30 Nov 2021 03:40:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 30 Nov 2021 03:40:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 30 Nov 2021 03:49:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 30 Nov 2021 03:49:53 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Tue, 30 Nov 2021 03:49:56 GMT
RUN docker-php-ext-enable sodium
# Tue, 30 Nov 2021 03:49:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 30 Nov 2021 03:49:57 GMT
WORKDIR /var/www/html
# Tue, 30 Nov 2021 03:49:59 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 30 Nov 2021 03:49:59 GMT
STOPSIGNAL SIGQUIT
# Tue, 30 Nov 2021 03:50:00 GMT
EXPOSE 9000
# Tue, 30 Nov 2021 03:50:00 GMT
CMD ["php-fpm"]
# Thu, 09 Dec 2021 02:10:35 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 09 Dec 2021 02:10:35 GMT
ENV PHP_MEMORY_LIMIT=256M
# Thu, 09 Dec 2021 02:14:13 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		procps 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 09 Dec 2021 02:14:15 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 10 Dec 2021 19:52:31 GMT
ENV MATOMO_VERSION=4.6.2
# Fri, 10 Dec 2021 19:53:26 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Fri, 10 Dec 2021 19:53:27 GMT
COPY file:f4ea35cff07e183c01b4e508329d1f5c342d9f4d330bda7f28faa530ced0d166 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 10 Dec 2021 19:53:28 GMT
COPY file:ccb778224a0e1f6742127aba2860c245adf24b73ca277e7260c4789883751ccb in /entrypoint.sh 
# Fri, 10 Dec 2021 19:53:28 GMT
VOLUME [/var/www/html]
# Fri, 10 Dec 2021 19:53:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Dec 2021 19:53:29 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289be6d758ff0faa38d64732e5736031f2250cbf78d1ca4b32abba4accd6a3fa`  
		Last Modified: Tue, 30 Nov 2021 04:29:36 GMT  
		Size: 1.7 MB (1698826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0b442a0f679dba79aa838c408cf49916ca26d27e1252e26f3904d7c5b83d6c`  
		Last Modified: Tue, 30 Nov 2021 04:29:33 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef02b1cade59fbcc24c0ee972dd15d8caa89dda554cdb8aa742de1c6f3d5b7c`  
		Last Modified: Tue, 30 Nov 2021 04:29:33 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c6a247480ef130c8325f9be1fbe1ef2047e23510e25f9d5f225aa541df8f573`  
		Last Modified: Tue, 30 Nov 2021 04:33:02 GMT  
		Size: 10.9 MB (10874432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:262d37c9213794bc797b5852779610048f5977dcbf668151bb98ca8f72ce251c`  
		Last Modified: Tue, 30 Nov 2021 04:32:59 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a37532eefa1deb82e161df2f79889b1358d843171b29c1aeac23b1e050895c4`  
		Last Modified: Tue, 30 Nov 2021 04:33:55 GMT  
		Size: 13.7 MB (13709715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876acb7b0ac81144668793897c2461d25a7792ef3b0966e5b5c8db35d2c39a03`  
		Last Modified: Tue, 30 Nov 2021 04:33:45 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe58f3927080d7d6307681f68274be25b9227d5131615907ec25dcd19e428272`  
		Last Modified: Tue, 30 Nov 2021 04:33:45 GMT  
		Size: 18.2 KB (18203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72c236ec9a62d08919d756e382b75e76b80792d5b6772e56ef7e095a54ba7a0`  
		Last Modified: Tue, 30 Nov 2021 04:33:45 GMT  
		Size: 8.6 KB (8569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b379ef7bc6759d9efa03a7e93c05b5a76d4d3a549e089965eb03d19412dbddb0`  
		Last Modified: Thu, 09 Dec 2021 02:15:36 GMT  
		Size: 5.3 MB (5265361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07c7e4429c18ea10ffae7c275b996a84dedf96d17a60035b16c8045a6ab2c1e7`  
		Last Modified: Thu, 09 Dec 2021 02:15:34 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87ab9d61df4d7fd9013fd5e7108f49ff0af12bb035838c9109294fa39dff6909`  
		Last Modified: Fri, 10 Dec 2021 19:54:20 GMT  
		Size: 16.2 MB (16246773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64e032ca774e87aeaee06deef22112801385697665a022c13c1168af097dfc6e`  
		Last Modified: Fri, 10 Dec 2021 19:54:04 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ddf03f9613e5d2264f1fce93734767092b2a4e0167f50366106c4eb7200730`  
		Last Modified: Fri, 10 Dec 2021 19:54:04 GMT  
		Size: 629.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-fpm-alpine` - linux; arm variant v7

```console
$ docker pull matomo@sha256:df1e730b945ba517c5b52424ed62794fb9a232b3a6b08bb46a2e0690cfc72ad1
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49313912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91a9d106f34bbf98923b624e8880e25cc66efd9a48d7295fde3c86bc6f8e177a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 05:27:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 05:27:16 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 05:27:18 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 05:27:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 05:27:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 05:27:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 05:27:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 05:27:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 05:48:42 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 30 Nov 2021 05:48:43 GMT
ENV PHP_VERSION=8.0.13
# Tue, 30 Nov 2021 05:48:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.13.tar.xz.asc
# Tue, 30 Nov 2021 05:48:44 GMT
ENV PHP_SHA256=cd976805ec2e9198417651027dfe16854ba2c2c388151ab9d4d268513d52ed52
# Tue, 30 Nov 2021 05:49:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 30 Nov 2021 05:49:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 30 Nov 2021 05:57:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 30 Nov 2021 05:57:46 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Tue, 30 Nov 2021 05:57:49 GMT
RUN docker-php-ext-enable sodium
# Tue, 30 Nov 2021 05:57:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 30 Nov 2021 05:57:50 GMT
WORKDIR /var/www/html
# Tue, 30 Nov 2021 05:57:51 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 30 Nov 2021 05:57:52 GMT
STOPSIGNAL SIGQUIT
# Tue, 30 Nov 2021 05:57:52 GMT
EXPOSE 9000
# Tue, 30 Nov 2021 05:57:53 GMT
CMD ["php-fpm"]
# Thu, 09 Dec 2021 02:37:41 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 09 Dec 2021 02:37:41 GMT
ENV PHP_MEMORY_LIMIT=256M
# Thu, 09 Dec 2021 02:41:08 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		procps 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 09 Dec 2021 02:41:10 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 10 Dec 2021 20:07:33 GMT
ENV MATOMO_VERSION=4.6.2
# Fri, 10 Dec 2021 20:08:16 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Fri, 10 Dec 2021 20:08:18 GMT
COPY file:f4ea35cff07e183c01b4e508329d1f5c342d9f4d330bda7f28faa530ced0d166 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 10 Dec 2021 20:08:18 GMT
COPY file:ccb778224a0e1f6742127aba2860c245adf24b73ca277e7260c4789883751ccb in /entrypoint.sh 
# Fri, 10 Dec 2021 20:08:19 GMT
VOLUME [/var/www/html]
# Fri, 10 Dec 2021 20:08:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Dec 2021 20:08:19 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484fe107211badcebee7c4211e5ed91c7e5212cdd6d7edbb292a63ec60572bdd`  
		Last Modified: Tue, 30 Nov 2021 06:57:00 GMT  
		Size: 1.6 MB (1568802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93353d0a7113f37ba224b9ee296684e49f27c1c9440d3a3c5d310749213da97f`  
		Last Modified: Tue, 30 Nov 2021 06:56:59 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137db50a58959a68358c190d2a143088b82ab25d97cb889876fbc0728e446058`  
		Last Modified: Tue, 30 Nov 2021 06:57:00 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4c87492896d37a070cd671acdeddc35fa626c16b56042ccbe125ae386d61b81`  
		Last Modified: Tue, 30 Nov 2021 07:01:07 GMT  
		Size: 10.9 MB (10874434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c951b2578fc00c76c8737687c283fc7850ef1e891c7b7f34e1b9ddbf24699bb`  
		Last Modified: Tue, 30 Nov 2021 07:01:04 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e92b7f731fd73059ae08235b93d3d7d63ab19c500989a37daa4400c950b710f`  
		Last Modified: Tue, 30 Nov 2021 07:01:58 GMT  
		Size: 12.8 MB (12844206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556a6819e7cb3132b97d67cf20a7c895464b4101e4649cc296b0cf46f77c332b`  
		Last Modified: Tue, 30 Nov 2021 07:01:50 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59413402f0cb78e1f80439e3030778455a33f86e1b953e836d7f0e91adf4094e`  
		Last Modified: Tue, 30 Nov 2021 07:01:50 GMT  
		Size: 18.2 KB (18208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe08dab18dec084b093b9958fb18865e8c25423e2049179988a2c09d541eaf1`  
		Last Modified: Tue, 30 Nov 2021 07:01:50 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535eb641cde6a50595a18fb121f2135e4f99053afc8fe7bc37a395f2df108a9c`  
		Last Modified: Thu, 09 Dec 2021 02:44:54 GMT  
		Size: 5.3 MB (5312473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b211203853081b21c379e8b61ecf977323a97a2e595496b18f7681712614959`  
		Last Modified: Thu, 09 Dec 2021 02:44:52 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c6280bb026f4e0b0b9c5a52517589cf447b6c9581acc63f301a48a2fecdfdd`  
		Last Modified: Fri, 10 Dec 2021 20:11:37 GMT  
		Size: 16.2 MB (16246826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffe353fe27f334d4c4403df7566d3236fde1007ab238e62e128dde34b8cd759d`  
		Last Modified: Fri, 10 Dec 2021 20:11:21 GMT  
		Size: 345.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ac39c3e1aea9eef9158a0488a2538a1be4ec3fc8fd2a00252b31c285a46856c`  
		Last Modified: Fri, 10 Dec 2021 20:11:21 GMT  
		Size: 631.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull matomo@sha256:4f3e054e18f808099196f8c1ae1cdd5fb50b5a5d1a2cdea5f7f71668a22948ea
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51806108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:420125abb1f0a7163bbda687e1d667b1229f98d488b4a05f8c4d633c902fa345`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 02:50:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 02:50:47 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 02:50:48 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 02:50:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 02:50:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 02:50:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 02:50:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 02:50:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 03:15:23 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 30 Nov 2021 03:15:24 GMT
ENV PHP_VERSION=8.0.13
# Tue, 30 Nov 2021 03:15:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.13.tar.xz.asc
# Tue, 30 Nov 2021 03:15:26 GMT
ENV PHP_SHA256=cd976805ec2e9198417651027dfe16854ba2c2c388151ab9d4d268513d52ed52
# Tue, 30 Nov 2021 03:15:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 30 Nov 2021 03:15:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 30 Nov 2021 03:23:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 30 Nov 2021 03:23:09 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Tue, 30 Nov 2021 03:23:10 GMT
RUN docker-php-ext-enable sodium
# Tue, 30 Nov 2021 03:23:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 30 Nov 2021 03:23:12 GMT
WORKDIR /var/www/html
# Tue, 30 Nov 2021 03:23:13 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 30 Nov 2021 03:23:14 GMT
STOPSIGNAL SIGQUIT
# Tue, 30 Nov 2021 03:23:15 GMT
EXPOSE 9000
# Tue, 30 Nov 2021 03:23:16 GMT
CMD ["php-fpm"]
# Thu, 09 Dec 2021 01:48:37 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 09 Dec 2021 01:48:37 GMT
ENV PHP_MEMORY_LIMIT=256M
# Thu, 09 Dec 2021 01:50:14 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		procps 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 09 Dec 2021 01:50:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 10 Dec 2021 19:46:44 GMT
ENV MATOMO_VERSION=4.6.2
# Fri, 10 Dec 2021 19:47:18 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Fri, 10 Dec 2021 19:47:19 GMT
COPY file:f4ea35cff07e183c01b4e508329d1f5c342d9f4d330bda7f28faa530ced0d166 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 10 Dec 2021 19:47:20 GMT
COPY file:ccb778224a0e1f6742127aba2860c245adf24b73ca277e7260c4789883751ccb in /entrypoint.sh 
# Fri, 10 Dec 2021 19:47:20 GMT
VOLUME [/var/www/html]
# Fri, 10 Dec 2021 19:47:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Dec 2021 19:47:22 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd720d9f53003155e4cfe3f1974fc0e4d74a622ea8c61cfccb00ee8b842c09b6`  
		Last Modified: Tue, 30 Nov 2021 03:59:34 GMT  
		Size: 1.7 MB (1708308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680efee530f3c970c3140b358d3dc583ded463f9adbadb737ca64c765cf997ee`  
		Last Modified: Tue, 30 Nov 2021 03:59:33 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643d01251bc949843dbd734a37e7cf28a01af4ea11443738b8b92d17e1e438de`  
		Last Modified: Tue, 30 Nov 2021 03:59:33 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5d2dd2e9744cc40d2b42c18613e2045ba6b72c922c37c8cda231e7cfcfff09`  
		Last Modified: Tue, 30 Nov 2021 04:02:18 GMT  
		Size: 10.9 MB (10874209 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09868cbd5e70feef55023ec2d20dfd178cc2fc4c1b875775b8578dd3758e22f1`  
		Last Modified: Tue, 30 Nov 2021 04:02:16 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53351e4c31dc5141df9db4d7140445d4bd36434a8bd19f404a0a5fe14e64511d`  
		Last Modified: Tue, 30 Nov 2021 04:02:52 GMT  
		Size: 14.5 MB (14499313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359d93e99a2d2d16a6674242af5c29f150e03fa02dd960efdd018b5240054cc9`  
		Last Modified: Tue, 30 Nov 2021 04:02:50 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c37a5bbbecdfaf97f30eeb1a45f69bf653de48477df4e877fec2a9e17f57419`  
		Last Modified: Tue, 30 Nov 2021 04:02:49 GMT  
		Size: 18.1 KB (18117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9e8df1efcce2c2808d6442e9f16bb02c6f2c72a3a940c3a90f6a4eeb2a798f`  
		Last Modified: Tue, 30 Nov 2021 04:02:49 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a302fb34fb3889ca65eb92067699fc160364d4bee956a1c8b09e8681b6a8a518`  
		Last Modified: Thu, 09 Dec 2021 01:52:35 GMT  
		Size: 5.7 MB (5731128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df1475cfb06903735d3f87ce20763641a6f473117d5950a0e53e0b2fc6dd96b`  
		Last Modified: Thu, 09 Dec 2021 01:52:35 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:198cc01c352070bf576faee61a753ca84bdb143091513ebd5a3e2dfb58e801f0`  
		Last Modified: Fri, 10 Dec 2021 19:49:05 GMT  
		Size: 16.2 MB (16245474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8f0ec065d03e3eeaef0af26e635cedd0abd5c6c19ff924ad476c5445aa91b9`  
		Last Modified: Fri, 10 Dec 2021 19:49:01 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cd5bada952cde540076dc635f02d535efe04ef6161127791db765807483e02`  
		Last Modified: Fri, 10 Dec 2021 19:49:01 GMT  
		Size: 631.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-fpm-alpine` - linux; 386

```console
$ docker pull matomo@sha256:3581627976953b4f2ca1f4847cdc831e6238d61ce3ad00f75b775092e2149acd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.2 MB (53242701 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa382af998acc7791a930e66397e2edbc91fc6b5eaa2a0d30ba60a803cb798a9`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 05:59:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 05:59:06 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 05:59:07 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 05:59:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 05:59:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 05:59:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 05:59:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 05:59:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 06:44:18 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 30 Nov 2021 06:44:19 GMT
ENV PHP_VERSION=8.0.13
# Tue, 30 Nov 2021 06:44:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.13.tar.xz.asc
# Tue, 30 Nov 2021 06:44:19 GMT
ENV PHP_SHA256=cd976805ec2e9198417651027dfe16854ba2c2c388151ab9d4d268513d52ed52
# Tue, 30 Nov 2021 06:44:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 30 Nov 2021 06:44:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 30 Nov 2021 07:04:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 30 Nov 2021 07:04:55 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Tue, 30 Nov 2021 07:04:57 GMT
RUN docker-php-ext-enable sodium
# Tue, 30 Nov 2021 07:04:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 30 Nov 2021 07:04:57 GMT
WORKDIR /var/www/html
# Tue, 30 Nov 2021 07:04:58 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 30 Nov 2021 07:04:59 GMT
STOPSIGNAL SIGQUIT
# Tue, 30 Nov 2021 07:04:59 GMT
EXPOSE 9000
# Tue, 30 Nov 2021 07:04:59 GMT
CMD ["php-fpm"]
# Thu, 09 Dec 2021 01:50:23 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 09 Dec 2021 01:50:23 GMT
ENV PHP_MEMORY_LIMIT=256M
# Thu, 09 Dec 2021 01:52:27 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		procps 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 09 Dec 2021 01:52:28 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 10 Dec 2021 19:42:53 GMT
ENV MATOMO_VERSION=4.6.2
# Fri, 10 Dec 2021 19:43:04 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Fri, 10 Dec 2021 19:43:05 GMT
COPY file:f4ea35cff07e183c01b4e508329d1f5c342d9f4d330bda7f28faa530ced0d166 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 10 Dec 2021 19:43:05 GMT
COPY file:ccb778224a0e1f6742127aba2860c245adf24b73ca277e7260c4789883751ccb in /entrypoint.sh 
# Fri, 10 Dec 2021 19:43:06 GMT
VOLUME [/var/www/html]
# Fri, 10 Dec 2021 19:43:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Dec 2021 19:43:06 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d6acd3b6e4278a7b3ef37d3525813808468237f086215b68594b244dbd1fba`  
		Last Modified: Tue, 30 Nov 2021 08:26:15 GMT  
		Size: 1.8 MB (1810453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc53af545b93519336bed63b8765255ac8280e27c8e3a17c336f92526b3f290`  
		Last Modified: Tue, 30 Nov 2021 08:26:14 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d406b6d62c3d67bec5f638d47d2b1b49c0ee41d80a791a1b90eaec776cf4fd`  
		Last Modified: Tue, 30 Nov 2021 08:26:13 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d123df95de9a3ba60290c45615f21dff954698e79ef5e253db235ba41d8d1c2`  
		Last Modified: Tue, 30 Nov 2021 08:29:53 GMT  
		Size: 10.9 MB (10874428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5a10462765fcacdbd3d2c18968e7d5506f5f0e6745b0438ebeb60ccbec7e5b`  
		Last Modified: Tue, 30 Nov 2021 08:29:52 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c903faf8dcaad895edb1b385229163879ed82404b121730414686b91043f7e`  
		Last Modified: Tue, 30 Nov 2021 08:30:35 GMT  
		Size: 15.4 MB (15406849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58b3e79e53f2bf68a958705590fc46dcfb95425e0313645c6ad7497e6e8cfd83`  
		Last Modified: Tue, 30 Nov 2021 08:30:30 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd4edbca43c36e4658f92b1d0fac568fdd44afc759e45cd31764aabe5f5df5e`  
		Last Modified: Tue, 30 Nov 2021 08:30:30 GMT  
		Size: 18.2 KB (18204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32eeccf2c2ad29ed15d933b633ece5ee569a8a814ec52a8e3a8726a41d3d3687`  
		Last Modified: Tue, 30 Nov 2021 08:30:31 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1aca6a0451f0e3fa3f77fa70eaf2abd5c51888dae393f7bd6181718d0a21e0`  
		Last Modified: Thu, 09 Dec 2021 01:58:25 GMT  
		Size: 6.0 MB (6044668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc3cc172bebb22823ae9e8ba8fdedb350878c9938c8ab737050a9195232857f1`  
		Last Modified: Thu, 09 Dec 2021 01:58:23 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d92f2c20a4c4b70f054e55fc53208522c06c05d61684fc54db2a9804d8e526fd`  
		Last Modified: Fri, 10 Dec 2021 19:44:59 GMT  
		Size: 16.2 MB (16246788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7512dc6658a9489d0fd313236af152eb375d0f88ad178a418a0be52c3137fd7e`  
		Last Modified: Fri, 10 Dec 2021 19:44:55 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6288ae5e5806cb7da280f2d253d1df58de963c378de0c43356010393da7d95b`  
		Last Modified: Fri, 10 Dec 2021 19:44:54 GMT  
		Size: 631.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-fpm-alpine` - linux; ppc64le

```console
$ docker pull matomo@sha256:4a3cb3a023d03047e7a98bded7c665e5d2a4e558dfe380aa45ba7d3e26badf7c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.4 MB (53441236 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ecfc11cf904da36d1f8200fd49a5918a22e71b2f32fe1da14cea69bec762761`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 06:02:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 06:03:14 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 06:03:32 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 06:03:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 06:03:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 06:03:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 06:03:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 06:04:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 06:28:05 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 30 Nov 2021 06:28:07 GMT
ENV PHP_VERSION=8.0.13
# Tue, 30 Nov 2021 06:28:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.13.tar.xz.asc
# Tue, 30 Nov 2021 06:28:10 GMT
ENV PHP_SHA256=cd976805ec2e9198417651027dfe16854ba2c2c388151ab9d4d268513d52ed52
# Tue, 30 Nov 2021 06:28:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 30 Nov 2021 06:28:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 30 Nov 2021 06:39:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 30 Nov 2021 06:39:07 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Tue, 30 Nov 2021 06:39:15 GMT
RUN docker-php-ext-enable sodium
# Tue, 30 Nov 2021 06:39:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 30 Nov 2021 06:39:22 GMT
WORKDIR /var/www/html
# Tue, 30 Nov 2021 06:39:29 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 30 Nov 2021 06:39:32 GMT
STOPSIGNAL SIGQUIT
# Tue, 30 Nov 2021 06:39:34 GMT
EXPOSE 9000
# Tue, 30 Nov 2021 06:39:39 GMT
CMD ["php-fpm"]
# Thu, 09 Dec 2021 02:59:10 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 09 Dec 2021 02:59:13 GMT
ENV PHP_MEMORY_LIMIT=256M
# Thu, 09 Dec 2021 03:01:32 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		procps 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 09 Dec 2021 03:01:37 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 10 Dec 2021 20:21:52 GMT
ENV MATOMO_VERSION=4.6.2
# Fri, 10 Dec 2021 20:22:19 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Fri, 10 Dec 2021 20:22:25 GMT
COPY file:f4ea35cff07e183c01b4e508329d1f5c342d9f4d330bda7f28faa530ced0d166 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 10 Dec 2021 20:22:26 GMT
COPY file:ccb778224a0e1f6742127aba2860c245adf24b73ca277e7260c4789883751ccb in /entrypoint.sh 
# Fri, 10 Dec 2021 20:22:28 GMT
VOLUME [/var/www/html]
# Fri, 10 Dec 2021 20:22:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Dec 2021 20:22:32 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603762061fb50079a4b6eb13347fd9a84cc1456d628cf781c89924a54bc419c1`  
		Last Modified: Tue, 30 Nov 2021 07:26:39 GMT  
		Size: 1.8 MB (1756276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645c08440cfaddc2735de2e28697acff0bc71db4cc7242494a44f92c94134e32`  
		Last Modified: Tue, 30 Nov 2021 07:26:39 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5de97a9a329d566f48c2edce253e4ccda6f021041e92326728b7499d13c823b`  
		Last Modified: Tue, 30 Nov 2021 07:26:39 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4479252694b8af910b4be2db9a7d699e99920590df6365ead58741b05f161bef`  
		Last Modified: Tue, 30 Nov 2021 07:29:25 GMT  
		Size: 10.9 MB (10874433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1389516e7bc1f0f56c59866a28554410910aae2e6b7d0539eddd2f7fd64f04ae`  
		Last Modified: Tue, 30 Nov 2021 07:29:24 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a780112bb524d896186b290192c20d93f5731b6d09b7fb2308697aad36fc66`  
		Last Modified: Tue, 30 Nov 2021 07:30:02 GMT  
		Size: 15.8 MB (15811717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e1b7ffc89aa69ebf9a59156af423be12fddf991bd576a3500ddd414785faf4`  
		Last Modified: Tue, 30 Nov 2021 07:29:58 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653164caf5a0d2d40df063fa50bbc1c9553b46c496893af6408d3cbf81e1f0a3`  
		Last Modified: Tue, 30 Nov 2021 07:29:58 GMT  
		Size: 18.2 KB (18199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa87745ae92ffe2c0deecf3c1461fd5d949f613731ab632a118f1bad0dc2028`  
		Last Modified: Tue, 30 Nov 2021 07:29:58 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0b14142b5171582b569a31ce603c9b219d0c9cc265d83610ae318e6c67262ca`  
		Last Modified: Thu, 09 Dec 2021 03:04:38 GMT  
		Size: 5.9 MB (5904840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c325c65abd3a5c510ee96e2e4a5a41aa3adfdd2e79a6600e5643f82a78c5472`  
		Last Modified: Thu, 09 Dec 2021 03:04:37 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf26f8a73770c40940ad5834188a80495f884a1fd777378b03a51bd463f3c67c`  
		Last Modified: Fri, 10 Dec 2021 20:24:24 GMT  
		Size: 16.2 MB (16246794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d68272124547da2b4789c87a2aa760e3c974fbcbebe0fa63f861f385a1fd22`  
		Last Modified: Fri, 10 Dec 2021 20:24:20 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:528bad8c09d758abfefd4d62a9939683e1ab6787158f43c18930104fd5510251`  
		Last Modified: Fri, 10 Dec 2021 20:24:20 GMT  
		Size: 631.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:4-fpm-alpine` - linux; s390x

```console
$ docker pull matomo@sha256:c0a1ea5524ce19aa2fdf237c670d9ec195e44cad546bac8def0502bdc87e1155
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.0 MB (50983261 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88747d85376178684ba846c99968e5ac564e7f36f272652642dd28cbbb941948`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:50:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 04:50:01 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 04:50:02 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 04:50:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 04:50:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 04:50:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 04:50:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 04:50:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 05:03:16 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Tue, 30 Nov 2021 05:03:16 GMT
ENV PHP_VERSION=8.0.13
# Tue, 30 Nov 2021 05:03:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.13.tar.xz.asc
# Tue, 30 Nov 2021 05:03:17 GMT
ENV PHP_SHA256=cd976805ec2e9198417651027dfe16854ba2c2c388151ab9d4d268513d52ed52
# Tue, 30 Nov 2021 05:03:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 30 Nov 2021 05:03:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 30 Nov 2021 05:09:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 30 Nov 2021 05:09:11 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Tue, 30 Nov 2021 05:09:12 GMT
RUN docker-php-ext-enable sodium
# Tue, 30 Nov 2021 05:09:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 30 Nov 2021 05:09:12 GMT
WORKDIR /var/www/html
# Tue, 30 Nov 2021 05:09:12 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 30 Nov 2021 05:09:12 GMT
STOPSIGNAL SIGQUIT
# Tue, 30 Nov 2021 05:09:13 GMT
EXPOSE 9000
# Tue, 30 Nov 2021 05:09:13 GMT
CMD ["php-fpm"]
# Thu, 09 Dec 2021 01:47:23 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 09 Dec 2021 01:47:23 GMT
ENV PHP_MEMORY_LIMIT=256M
# Thu, 09 Dec 2021 01:48:29 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		procps 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		bcmath 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.21; 	pecl install redis-5.3.4; 		docker-php-ext-enable 		apcu 		redis 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 09 Dec 2021 01:48:29 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 10 Dec 2021 19:46:09 GMT
ENV MATOMO_VERSION=4.6.2
# Fri, 10 Dec 2021 19:46:18 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Fri, 10 Dec 2021 19:46:20 GMT
COPY file:f4ea35cff07e183c01b4e508329d1f5c342d9f4d330bda7f28faa530ced0d166 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 10 Dec 2021 19:46:20 GMT
COPY file:ccb778224a0e1f6742127aba2860c245adf24b73ca277e7260c4789883751ccb in /entrypoint.sh 
# Fri, 10 Dec 2021 19:46:20 GMT
VOLUME [/var/www/html]
# Fri, 10 Dec 2021 19:46:21 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 10 Dec 2021 19:46:21 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079fbafa3afc04920b17b503e5d173a44e68fa743eddc7a0eca5e81c7572b8a2`  
		Last Modified: Tue, 30 Nov 2021 08:33:50 GMT  
		Size: 1.8 MB (1771410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ea1ee8ecbda317521ca15da3d8e45a369d74d9b70a0070ebd705cb9aaf88a2`  
		Last Modified: Tue, 30 Nov 2021 08:33:49 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abad577e66a4ab93646ed4a4aefb0579d577932add0d28121e5aece37cfc08dd`  
		Last Modified: Tue, 30 Nov 2021 08:33:49 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ea87a2caf3efacfd6163cd632a41aac71423742de7f52d4c0635e61d8c4905`  
		Last Modified: Tue, 30 Nov 2021 08:35:43 GMT  
		Size: 10.9 MB (10874446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37a713981b32d62b43ac0776106c363b80d7ae7dcc8f6bf53fcdcb0b37a58c9c`  
		Last Modified: Tue, 30 Nov 2021 08:35:43 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdad54750e409f4e1d9727c0b28c562da7c8f6e15bfb2761e30354430265208c`  
		Last Modified: Tue, 30 Nov 2021 08:36:03 GMT  
		Size: 14.1 MB (14093937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6268c54bed6cac052c500137573bfff1b75932fdb2aa814b43a13460aec88460`  
		Last Modified: Tue, 30 Nov 2021 08:36:01 GMT  
		Size: 2.3 KB (2301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bc27e5d85b2c81c6da68cc1d1894ba0af32345ecd8dfa97c9fec15e0cfb536`  
		Last Modified: Tue, 30 Nov 2021 08:36:01 GMT  
		Size: 18.2 KB (18230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c726c8dcbdc78ea1f58bf2c53f60bf190d2d96338b320ca6534ab35ed7c799`  
		Last Modified: Tue, 30 Nov 2021 08:36:01 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1156a09e1322d123ca9858049bb1b8714850279f4cab90e200b2e32e7233985`  
		Last Modified: Thu, 09 Dec 2021 01:51:58 GMT  
		Size: 5.4 MB (5358254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f88d310a9957b8aa2984fb32714804004128afb014ca6649ad0c6cb5031def3`  
		Last Modified: Thu, 09 Dec 2021 01:51:58 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8f12daf027f9fb48c0c3b5f116ae80d0138af216453ebd65fdabe561b3a823`  
		Last Modified: Fri, 10 Dec 2021 19:47:43 GMT  
		Size: 16.2 MB (16246846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0edb0b577488c5e5aa1c3382ebc0bde75d0f5725bcd52d7feef92a66c648b78d`  
		Last Modified: Fri, 10 Dec 2021 19:47:41 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca04a0ee0e6d108863c2bac024b1dbc5560e51e0e9cf30d4b20409c6a97ce49`  
		Last Modified: Fri, 10 Dec 2021 19:47:40 GMT  
		Size: 630.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
