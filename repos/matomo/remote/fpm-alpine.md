## `matomo:fpm-alpine`

```console
$ docker pull matomo@sha256:461093b14ed89731df51d5d7f4bff482ff69e4658c9897ea7dd29a7e25a13e4a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `matomo:fpm-alpine` - linux; amd64

```console
$ docker pull matomo@sha256:94c4b504849eb5cf888cabc41c7c61f966b83aaf9559621a31eefa3e6e3d9855
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49673168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ccd37cc5bd0ea379431428aaccfccc8b2acead7378c493f9099db6cd6482760d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 01:18:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 01:18:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 01:18:35 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 01:18:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 01:18:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 01:27:38 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 01:27:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 01:27:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 17 Apr 2020 11:58:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 17 Apr 2020 11:58:21 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 17 Apr 2020 11:58:22 GMT
ENV PHP_VERSION=7.4.5
# Fri, 17 Apr 2020 11:58:22 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.5.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.5.tar.xz.asc/from/this/mirror
# Fri, 17 Apr 2020 11:58:22 GMT
ENV PHP_SHA256=d059fd7f55bdc4d2eada15a00a2976697010d3631ef6f83149cc5289e1f23c2c PHP_MD5=
# Fri, 17 Apr 2020 11:58:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 17 Apr 2020 11:58:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 17 Apr 2020 12:04:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 17 Apr 2020 12:04:21 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 17 Apr 2020 12:04:22 GMT
RUN docker-php-ext-enable sodium
# Fri, 17 Apr 2020 12:04:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 17 Apr 2020 12:04:22 GMT
WORKDIR /var/www/html
# Fri, 17 Apr 2020 12:04:23 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 17 Apr 2020 12:04:23 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Apr 2020 12:04:23 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 12:04:24 GMT
CMD ["php-fpm"]
# Fri, 17 Apr 2020 17:56:55 GMT
LABEL maintainer=pierre@piwik.org
# Fri, 17 Apr 2020 17:58:08 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Fri, 17 Apr 2020 17:58:09 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 17 Apr 2020 17:58:09 GMT
ENV MATOMO_VERSION=3.13.4
# Fri, 17 Apr 2020 17:58:15 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Fri, 17 Apr 2020 17:58:15 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 17 Apr 2020 17:58:15 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Fri, 17 Apr 2020 17:58:15 GMT
VOLUME [/var/www/html]
# Fri, 17 Apr 2020 17:58:16 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 17 Apr 2020 17:58:16 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61c449d5d9102f11bc559aba323f82389b7be6118dea453e8273a7f8cc971ea`  
		Last Modified: Tue, 24 Mar 2020 02:42:25 GMT  
		Size: 1.4 MB (1354647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fde16e1397a31e46a1030c8f769012ebe10f171fc564c77a692053c845975ff`  
		Last Modified: Tue, 24 Mar 2020 02:42:24 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1096698ab2a54e6370c1f2b9c6bb71ae2bb54e306f246aa436b77e1351ff1cf`  
		Last Modified: Tue, 24 Mar 2020 02:42:25 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96de990b7ad3c29b13cc6ff4d6b48464f9eec71db3e4947b055150ee395b905f`  
		Last Modified: Fri, 17 Apr 2020 15:24:29 GMT  
		Size: 10.3 MB (10290383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c280bfe252218fedf4102b5df4856781165cf44864fb701bde0c84f334108a9d`  
		Last Modified: Fri, 17 Apr 2020 15:24:27 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02be9679a029838148ac534e7458d2663b42da65d21eeefc70b8685cf3c051e6`  
		Last Modified: Fri, 17 Apr 2020 15:24:30 GMT  
		Size: 14.2 MB (14188505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01973f6576344f1eb575d90feb857a5bcc902b8f40b17267251a51414cb0bc95`  
		Last Modified: Fri, 17 Apr 2020 15:24:27 GMT  
		Size: 2.2 KB (2217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75924d0578e05181e21c31024e302add9207e7ebe4ddfd5b7b3bb95742b1860e`  
		Last Modified: Fri, 17 Apr 2020 15:24:27 GMT  
		Size: 17.2 KB (17246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7545938f30ed07fa1584df64fedfbcc356147d066b31f8f05b84d63f736d3190`  
		Last Modified: Fri, 17 Apr 2020 15:24:27 GMT  
		Size: 8.4 KB (8441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1154f5917a2bd269053af29565a209a0da567cc9de8e07e70245e698bed4d0fb`  
		Last Modified: Fri, 17 Apr 2020 17:59:01 GMT  
		Size: 5.9 MB (5876506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514560b6fddc02b754ec56e1a432c3aeb9f5e9a03c6c6255ec4c28c921c8abcf`  
		Last Modified: Fri, 17 Apr 2020 17:59:00 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbe44cd561c77fe4df78613f9a00f87ba9cac18f9af208b728604d33fbab76fb`  
		Last Modified: Fri, 17 Apr 2020 17:59:04 GMT  
		Size: 15.1 MB (15129167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:535eb098492c1c40a03096052544622818c0bcb39983e82319791a25985d0d67`  
		Last Modified: Fri, 17 Apr 2020 17:59:00 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb4391cdf484f57db9f06fff9be51948f3d35949dd7a2e1afcf1bfd7511dc66`  
		Last Modified: Fri, 17 Apr 2020 17:59:00 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:fpm-alpine` - linux; arm variant v6

```console
$ docker pull matomo@sha256:3a6d75fe166323b82d2024a2c1c9db1714a7f9e155a373a9d5d9b3fd2537aa9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48157920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46f68ead743a78a4e36961e06615bd853eef4b8ade8cf7be80736a8498d6e2b8`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:40:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 23 Apr 2020 22:40:31 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 23 Apr 2020 22:40:34 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 23 Apr 2020 22:40:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 22:40:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 22:44:52 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 23 Apr 2020 22:44:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 22:44:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 22:44:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 22:44:56 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Apr 2020 22:44:56 GMT
ENV PHP_VERSION=7.4.5
# Thu, 23 Apr 2020 22:44:57 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.5.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.5.tar.xz.asc/from/this/mirror
# Thu, 23 Apr 2020 22:44:58 GMT
ENV PHP_SHA256=d059fd7f55bdc4d2eada15a00a2976697010d3631ef6f83149cc5289e1f23c2c PHP_MD5=
# Thu, 23 Apr 2020 22:45:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 23 Apr 2020 22:45:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:48:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Apr 2020 22:48:46 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 23 Apr 2020 22:48:49 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Apr 2020 22:48:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Apr 2020 22:48:50 GMT
WORKDIR /var/www/html
# Thu, 23 Apr 2020 22:48:52 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 23 Apr 2020 22:48:53 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Apr 2020 22:48:53 GMT
EXPOSE 9000
# Thu, 23 Apr 2020 22:48:54 GMT
CMD ["php-fpm"]
# Fri, 24 Apr 2020 02:06:36 GMT
LABEL maintainer=pierre@piwik.org
# Fri, 24 Apr 2020 02:08:57 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Fri, 24 Apr 2020 02:08:59 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Apr 2020 02:09:00 GMT
ENV MATOMO_VERSION=3.13.4
# Fri, 24 Apr 2020 02:09:15 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Fri, 24 Apr 2020 02:09:16 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 24 Apr 2020 02:09:17 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Fri, 24 Apr 2020 02:09:18 GMT
VOLUME [/var/www/html]
# Fri, 24 Apr 2020 02:09:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 02:09:20 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e4a0b35ae612f97f86d2cb9a5c35d9974c53c9693ed9c503293a2ed4d1f5eb`  
		Last Modified: Thu, 23 Apr 2020 23:53:32 GMT  
		Size: 1.3 MB (1321299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744673dda954515280697917b25c13df9ff57231c28643848fc80b349d6b246b`  
		Last Modified: Thu, 23 Apr 2020 23:53:31 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6829673d00afbe39285f6e4d9977770c99d7bf841436086efa137773c99fd188`  
		Last Modified: Thu, 23 Apr 2020 23:53:31 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14063425f689cd3b759cb0757b947b647f2fb9a606858619858e151a763230ec`  
		Last Modified: Thu, 23 Apr 2020 23:54:07 GMT  
		Size: 10.3 MB (10290396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ad639b6c0b443ef3f09f7f7458936f085163c6ec77f0ca832e1ed88b6777e61`  
		Last Modified: Thu, 23 Apr 2020 23:54:04 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd01e49de56420eee69d8edccfb2fa55a3a2b8bd222bb5437bf3786e14c99cb`  
		Last Modified: Thu, 23 Apr 2020 23:54:10 GMT  
		Size: 13.2 MB (13207739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5b1b62c3349802b2117353af2e83f9c26d6dc22083f8fcdf817e6c87e71376`  
		Last Modified: Thu, 23 Apr 2020 23:54:04 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8554164701513bf1a5d89b7eb0aa99e0d617bf8b8384e4a6503e66b434465078`  
		Last Modified: Thu, 23 Apr 2020 23:54:04 GMT  
		Size: 17.2 KB (17239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055a919b186a6df14a028431931824b4077c077fbca75cbefd8391045c3ed54e`  
		Last Modified: Thu, 23 Apr 2020 23:54:04 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb2a4ccb46ec2e5716aa1ad98437ee040c2b4157303becd6d1cf4dce6c24c23`  
		Last Modified: Fri, 24 Apr 2020 02:09:45 GMT  
		Size: 5.6 MB (5558556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11cf7f916f4ca2c810d6e54e07483830cfe59509641fa9d3f1adf4bd3ab9fc2`  
		Last Modified: Fri, 24 Apr 2020 02:09:44 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2fdf96b97b3f459ebbffada55482f95e9ce07de389d0dbacd3f4812702098fb`  
		Last Modified: Fri, 24 Apr 2020 02:09:50 GMT  
		Size: 15.1 MB (15129219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d8a3c46720fb2466bb39f96e22da11729edff9addd1c00a2680e5387d7f94f`  
		Last Modified: Fri, 24 Apr 2020 02:09:45 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d55f6309a4499533955a485ef7c897a25717017956f9c7777f691b1b68027cc`  
		Last Modified: Fri, 24 Apr 2020 02:09:44 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:fpm-alpine` - linux; arm variant v7

```console
$ docker pull matomo@sha256:6f6378a595c14360bfa8ad9aea7c53c559d92ffcdbe97983d011bfe5a391d8de
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46790479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a1bfde08f03fdfe2ac40740e605d5957b2db4a9d5b134098a3d22981d665600`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 01:36:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 01:36:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 01:36:39 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 01:36:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 01:36:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 01:39:39 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 01:39:40 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 01:39:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 17 Apr 2020 12:34:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 17 Apr 2020 12:34:32 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 17 Apr 2020 12:34:33 GMT
ENV PHP_VERSION=7.4.5
# Fri, 17 Apr 2020 12:34:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.5.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.5.tar.xz.asc/from/this/mirror
# Fri, 17 Apr 2020 12:34:37 GMT
ENV PHP_SHA256=d059fd7f55bdc4d2eada15a00a2976697010d3631ef6f83149cc5289e1f23c2c PHP_MD5=
# Fri, 17 Apr 2020 12:34:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 17 Apr 2020 12:34:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 17 Apr 2020 12:37:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 17 Apr 2020 12:37:18 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 17 Apr 2020 12:37:21 GMT
RUN docker-php-ext-enable sodium
# Fri, 17 Apr 2020 12:37:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 17 Apr 2020 12:37:23 GMT
WORKDIR /var/www/html
# Fri, 17 Apr 2020 12:37:24 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 17 Apr 2020 12:37:25 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Apr 2020 12:37:26 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 12:37:26 GMT
CMD ["php-fpm"]
# Fri, 17 Apr 2020 17:59:11 GMT
LABEL maintainer=pierre@piwik.org
# Fri, 17 Apr 2020 18:01:07 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Fri, 17 Apr 2020 18:01:10 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 17 Apr 2020 18:01:11 GMT
ENV MATOMO_VERSION=3.13.4
# Fri, 17 Apr 2020 18:01:25 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Fri, 17 Apr 2020 18:01:39 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 17 Apr 2020 18:01:42 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Fri, 17 Apr 2020 18:01:45 GMT
VOLUME [/var/www/html]
# Fri, 17 Apr 2020 18:01:47 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 17 Apr 2020 18:01:49 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221e0c8c991c3fdd8db1ec76c1a911aa0f946325ec2cf15d22a25693accc6edc`  
		Last Modified: Tue, 24 Mar 2020 02:07:16 GMT  
		Size: 1.2 MB (1227325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeaee6722c9e078934e8f34fe0dc55d3f3c28d742e92ce6b3e86775beaeeb44`  
		Last Modified: Tue, 24 Mar 2020 02:07:16 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84528978bcc1c0fe1d795bbe412f0a4123fa9119c11c98cd9b1ab8c5db8203f0`  
		Last Modified: Tue, 24 Mar 2020 02:07:16 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a04c3a2941958182817cd6af0c930eb4d94023cd10078e53c357a9d1802224`  
		Last Modified: Fri, 17 Apr 2020 14:38:59 GMT  
		Size: 10.3 MB (10290407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:909af0f5420ee5ea07d8168536567e2561fcf73da46108c4ace0ddf87b7b0573`  
		Last Modified: Fri, 17 Apr 2020 14:38:56 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64e080e6dec253f925d886174ca315815a01bd6c4ab07eb9c63124e7e13d2cb`  
		Last Modified: Fri, 17 Apr 2020 14:39:00 GMT  
		Size: 12.4 MB (12354487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5962388fd5b436335374c710c0235bfe75192ed128309e5bebc10992b2ef1640`  
		Last Modified: Fri, 17 Apr 2020 14:38:56 GMT  
		Size: 2.2 KB (2215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3880e0ae14e835099af2c2cbf00e92aff514b70a67c17558fae0481ccae32468`  
		Last Modified: Fri, 17 Apr 2020 14:38:56 GMT  
		Size: 17.2 KB (17231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:630b13ce5020b227e7d915e25fee6717d4d7b48faa678ef345d95bcf7109e22d`  
		Last Modified: Fri, 17 Apr 2020 14:38:56 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b362efe0a2f60c0d9912657805454a28576950fe8bf7c4309eddf6ab1fa2019a`  
		Last Modified: Fri, 17 Apr 2020 18:03:03 GMT  
		Size: 5.3 MB (5337774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a7ceb1719a85c290ab4bc9815781739f93a26812143363c7c923c9d1bbd4b4`  
		Last Modified: Fri, 17 Apr 2020 18:03:03 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e468d4ae9d767b3bc5234cf30a576b422ba0328b1b38dc9672095069c4c5f528`  
		Last Modified: Fri, 17 Apr 2020 18:03:09 GMT  
		Size: 15.1 MB (15129221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad4b0e04e9dc3ac030d69faa60ca6baaedcf748d224c52b3c6a0f0e44d44cb1b`  
		Last Modified: Fri, 17 Apr 2020 18:03:03 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1105009b73cf9303355f4c9570007041cee63c2fc26f9ab4e26e7355b2e07115`  
		Last Modified: Fri, 17 Apr 2020 18:03:03 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull matomo@sha256:5105069a3445915fb636adf63639d2a7aedde061531d32a8c25fcd013adf2a32
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.4 MB (49371266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57fb4ff1d8bdbe175d524ae116c098eafdd5c1a783eeadc88949cdeeee8a4582`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:27:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 00:27:19 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 00:27:21 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 00:27:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 00:27:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 00:31:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 00:31:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 00:31:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 17 Apr 2020 13:23:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 17 Apr 2020 13:23:43 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 17 Apr 2020 13:23:45 GMT
ENV PHP_VERSION=7.4.5
# Fri, 17 Apr 2020 13:23:46 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.5.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.5.tar.xz.asc/from/this/mirror
# Fri, 17 Apr 2020 13:23:48 GMT
ENV PHP_SHA256=d059fd7f55bdc4d2eada15a00a2976697010d3631ef6f83149cc5289e1f23c2c PHP_MD5=
# Fri, 17 Apr 2020 13:23:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 17 Apr 2020 13:23:53 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 17 Apr 2020 13:27:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 17 Apr 2020 13:27:41 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 17 Apr 2020 13:27:43 GMT
RUN docker-php-ext-enable sodium
# Fri, 17 Apr 2020 13:27:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 17 Apr 2020 13:27:44 GMT
WORKDIR /var/www/html
# Fri, 17 Apr 2020 13:27:46 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 17 Apr 2020 13:27:47 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Apr 2020 13:27:47 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 13:27:48 GMT
CMD ["php-fpm"]
# Fri, 17 Apr 2020 18:44:17 GMT
LABEL maintainer=pierre@piwik.org
# Fri, 17 Apr 2020 18:46:22 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Fri, 17 Apr 2020 18:46:24 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 17 Apr 2020 18:46:24 GMT
ENV MATOMO_VERSION=3.13.4
# Fri, 17 Apr 2020 18:46:34 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Fri, 17 Apr 2020 18:46:36 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 17 Apr 2020 18:46:37 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Fri, 17 Apr 2020 18:46:37 GMT
VOLUME [/var/www/html]
# Fri, 17 Apr 2020 18:46:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 17 Apr 2020 18:46:38 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee501176ea6c9d16dc12649d7c62f4b6466cc96eaf80bfcea3aa261a052ec099`  
		Last Modified: Tue, 24 Mar 2020 01:03:05 GMT  
		Size: 1.4 MB (1359430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876007701d95df62eb874f76916e4d139709812e5e0be471c4107729808d6af`  
		Last Modified: Tue, 24 Mar 2020 01:03:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ed02bd016dcfb57e62d938f46a81237af426353ef7df647b64c3b3a93276a7`  
		Last Modified: Tue, 24 Mar 2020 01:03:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b275d280b9dc4b46388ca0120e75ceaf75c761f5c86fcdbfd52686d30c2fc3`  
		Last Modified: Fri, 17 Apr 2020 15:39:10 GMT  
		Size: 10.3 MB (10290392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f15b9142796e102a19a424d0a3c033f488c607c0ba07eb49095576f30fb2076`  
		Last Modified: Fri, 17 Apr 2020 15:39:07 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4b4e4262df3a946fc982d251f3e9b6bcc56d7928f8c2bbf49b2da0e4f933da`  
		Last Modified: Fri, 17 Apr 2020 15:39:11 GMT  
		Size: 14.0 MB (13985294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0cfe3c1e7d6b40be2eb5fa02e2b3cec4922a13b38e875adf1801544f8bff2be`  
		Last Modified: Fri, 17 Apr 2020 15:39:08 GMT  
		Size: 2.2 KB (2215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f7ff72f3fae1b07630d0e30e0c3fb76ad0a66390fa9df6e53f43cce93a5415`  
		Last Modified: Fri, 17 Apr 2020 15:39:07 GMT  
		Size: 17.2 KB (17230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b129dd0da25f0576e6908dec28e98a9e61854d587ba3cf5472a21ed22c08bb5e`  
		Last Modified: Fri, 17 Apr 2020 15:39:07 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b9820cacaada4e49f8783415bd95498f37379cd2f354878a8c19a283eaaaeb`  
		Last Modified: Fri, 17 Apr 2020 18:47:49 GMT  
		Size: 5.9 MB (5853032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abf6eb29c2810667d252cf6a1786f987e6567f184b41cce0db89758e83c87378`  
		Last Modified: Fri, 17 Apr 2020 18:47:47 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f5e4ec085065206430037bc987e7994f7d6801f643eb768524ebd0b7eb4b12`  
		Last Modified: Fri, 17 Apr 2020 18:47:53 GMT  
		Size: 15.1 MB (15129206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6658279b07d27a79d2129c4e5c10ad652f381896913f822eefac1fdc110e069`  
		Last Modified: Fri, 17 Apr 2020 18:47:47 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e63d8fa00e10e594381fc04362de7fd757c320abb27a4f41eab7cde7946a8f0`  
		Last Modified: Fri, 17 Apr 2020 18:47:47 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:fpm-alpine` - linux; 386

```console
$ docker pull matomo@sha256:e80f4fe03d3bd660da3020ebb7d60260e0224590ce799e1f315039cf100be24b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50253455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1252b29287a3adbfdea3593e7bcb4e628e223b20968671db9bde20a684573d06`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 06:05:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 24 Apr 2020 06:05:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 24 Apr 2020 06:05:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 24 Apr 2020 06:05:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 24 Apr 2020 06:05:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 24 Apr 2020 06:11:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 24 Apr 2020 06:11:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 06:11:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 06:11:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Apr 2020 06:11:35 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 24 Apr 2020 06:11:35 GMT
ENV PHP_VERSION=7.4.5
# Fri, 24 Apr 2020 06:11:36 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.5.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.5.tar.xz.asc/from/this/mirror
# Fri, 24 Apr 2020 06:11:36 GMT
ENV PHP_SHA256=d059fd7f55bdc4d2eada15a00a2976697010d3631ef6f83149cc5289e1f23c2c PHP_MD5=
# Fri, 24 Apr 2020 06:11:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 24 Apr 2020 06:11:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 24 Apr 2020 06:17:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 24 Apr 2020 06:17:09 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 24 Apr 2020 06:17:10 GMT
RUN docker-php-ext-enable sodium
# Fri, 24 Apr 2020 06:17:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 24 Apr 2020 06:17:10 GMT
WORKDIR /var/www/html
# Fri, 24 Apr 2020 06:17:11 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 24 Apr 2020 06:17:11 GMT
STOPSIGNAL SIGQUIT
# Fri, 24 Apr 2020 06:17:12 GMT
EXPOSE 9000
# Fri, 24 Apr 2020 06:17:12 GMT
CMD ["php-fpm"]
# Fri, 24 Apr 2020 10:37:07 GMT
LABEL maintainer=pierre@piwik.org
# Fri, 24 Apr 2020 10:38:28 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Fri, 24 Apr 2020 10:38:29 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Apr 2020 10:38:29 GMT
ENV MATOMO_VERSION=3.13.4
# Fri, 24 Apr 2020 10:38:36 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Fri, 24 Apr 2020 10:38:36 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 24 Apr 2020 10:38:36 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Fri, 24 Apr 2020 10:38:37 GMT
VOLUME [/var/www/html]
# Fri, 24 Apr 2020 10:38:37 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 10:38:37 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990138137e85533c48403b0cd1aee9ac6c5f3fc3be67a74a44a22f1a30e39af6`  
		Last Modified: Fri, 24 Apr 2020 07:59:39 GMT  
		Size: 1.5 MB (1453100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d973cd3524efeb6727b2144c33f96c71896f4ee22b1a55cc0c5aa5756f9b758`  
		Last Modified: Fri, 24 Apr 2020 07:59:37 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f386ab173ce6081c15380f99f906f8ea531e5748425804a21ebb0b5c433e6782`  
		Last Modified: Fri, 24 Apr 2020 07:59:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dbc07d97715867cc0e0b68e35e485477529c00962f9bdcb7de4ca923495631b`  
		Last Modified: Fri, 24 Apr 2020 08:00:09 GMT  
		Size: 10.3 MB (10290393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3212cbec705b88eb67797de6bc6a46461c310ab187a015abf86cd5b0452dfb8`  
		Last Modified: Fri, 24 Apr 2020 08:00:05 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e63d8ca23ba09015af347941104e06548b7c30dda5b05aa6e2538e97796831`  
		Last Modified: Fri, 24 Apr 2020 08:00:14 GMT  
		Size: 14.6 MB (14598012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf76394ae5f9e7a4f5223329ac7280318b0c8330febd62442597e1a97e4ea2f9`  
		Last Modified: Fri, 24 Apr 2020 08:00:06 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0f4f160c9b14975683e4764c697759790d527570f6970d8f93c7b18a345eb7`  
		Last Modified: Fri, 24 Apr 2020 08:00:06 GMT  
		Size: 17.2 KB (17238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7e6bd3b2d978736722929620fce5f4547721bb0f11b0ffd0d510aebd79a9bb`  
		Last Modified: Fri, 24 Apr 2020 08:00:05 GMT  
		Size: 8.4 KB (8441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2af01a85d623e9c519bcc53e2ae9352a14b2f94b6e8688605efd142f02fe29`  
		Last Modified: Fri, 24 Apr 2020 10:39:07 GMT  
		Size: 5.9 MB (5943616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:531d09a4c376e35c3bb7f2d30159cd40af7f7677ad97fe9af3881311be37ad7e`  
		Last Modified: Fri, 24 Apr 2020 10:39:06 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f88ee49d70b19abeded50672f8b9a32f5661426161bd9f8deec48e7ba7bec2f1`  
		Last Modified: Fri, 24 Apr 2020 10:39:11 GMT  
		Size: 15.1 MB (15129218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89f1ba449e89a8b1028259e23fd794a929d85c56ec1f33f95a95bb5baab046b`  
		Last Modified: Fri, 24 Apr 2020 10:39:06 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4886341a1d375b5ff9559441adc84f5e61a25ece23935ca284b0e5e66e8b38b`  
		Last Modified: Fri, 24 Apr 2020 10:39:06 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:fpm-alpine` - linux; ppc64le

```console
$ docker pull matomo@sha256:73fff8c709c91e22a4800e6de3a811ec1b8932c6f40ed168521852986ceef5ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.9 MB (50926058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab20a87bce8ce898c584931d56458b03b63b3a9ccec63075ba4f90a7fb1b87a1`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:21:29 GMT
ADD file:4b35131542b9682214e1c2c72fe3cea215a10e2f775e87befecd80fe2228d5a0 in / 
# Mon, 23 Mar 2020 21:21:32 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:27:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 00:27:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 00:27:38 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 00:27:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 00:27:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 00:32:28 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 00:32:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 00:32:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 17 Apr 2020 16:39:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 17 Apr 2020 16:39:47 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 17 Apr 2020 16:39:49 GMT
ENV PHP_VERSION=7.4.5
# Fri, 17 Apr 2020 16:39:52 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.5.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.5.tar.xz.asc/from/this/mirror
# Fri, 17 Apr 2020 16:39:54 GMT
ENV PHP_SHA256=d059fd7f55bdc4d2eada15a00a2976697010d3631ef6f83149cc5289e1f23c2c PHP_MD5=
# Fri, 17 Apr 2020 16:40:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 17 Apr 2020 16:40:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:44:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 17 Apr 2020 16:44:02 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 17 Apr 2020 16:44:13 GMT
RUN docker-php-ext-enable sodium
# Fri, 17 Apr 2020 16:44:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 17 Apr 2020 16:44:20 GMT
WORKDIR /var/www/html
# Fri, 17 Apr 2020 16:44:29 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 17 Apr 2020 16:44:31 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Apr 2020 16:44:34 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 16:44:37 GMT
CMD ["php-fpm"]
# Sat, 18 Apr 2020 02:53:51 GMT
LABEL maintainer=pierre@piwik.org
# Sat, 18 Apr 2020 02:55:46 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Sat, 18 Apr 2020 02:56:02 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 18 Apr 2020 02:56:07 GMT
ENV MATOMO_VERSION=3.13.4
# Sat, 18 Apr 2020 02:56:28 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Sat, 18 Apr 2020 02:56:37 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Sat, 18 Apr 2020 02:56:44 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Sat, 18 Apr 2020 02:57:03 GMT
VOLUME [/var/www/html]
# Sat, 18 Apr 2020 02:57:24 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 18 Apr 2020 02:57:31 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:bc1c99f4ba60de0d3ca52dc6855483e24c91884e33df71f502bbff6eb909d9b9`  
		Last Modified: Mon, 23 Mar 2020 21:22:12 GMT  
		Size: 2.8 MB (2820052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681c4a6dbdeb5b4877c85db3edbb08e40a877342795a3e7ba7f543a65586c417`  
		Last Modified: Tue, 24 Mar 2020 01:16:24 GMT  
		Size: 1.4 MB (1397873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e23455f025d83291061d4165e722b934e986f58c2b3d71b62a0918166d19db`  
		Last Modified: Tue, 24 Mar 2020 01:16:23 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c3447d90e80a01a72c494bf3563b1379704fcf4fb8b5b207596bbeeac49fc3`  
		Last Modified: Tue, 24 Mar 2020 01:16:22 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ae63940713d9885733c537e8f0fd0422f11b9433c3b5eafd7bbe4fc7974a90`  
		Last Modified: Fri, 17 Apr 2020 20:12:14 GMT  
		Size: 10.3 MB (10290412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aca45ce76c82302d1b72c2e9cc6b33a44da8af3e4b65d1744917f8d7c40ebed9`  
		Last Modified: Fri, 17 Apr 2020 20:12:03 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0270090f70b9129db4ed38496e5ee347aad9a3d4e6d1a0cfc9970c70a9fb4783`  
		Last Modified: Fri, 17 Apr 2020 20:12:09 GMT  
		Size: 15.2 MB (15170133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6637ba614da1090ec48d3cc4c05182fd2c41e48497260a7d0a391ff6ab0033a4`  
		Last Modified: Fri, 17 Apr 2020 20:12:04 GMT  
		Size: 2.2 KB (2216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ad084b177205209bd7d7d996a98d7aeb5ed087852df008b460c03112fd4317`  
		Last Modified: Fri, 17 Apr 2020 20:12:04 GMT  
		Size: 17.2 KB (17236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dfccd5fae65a0a9716cc7fe41314a2c6d90e09db23987f04ccde086f027777a`  
		Last Modified: Fri, 17 Apr 2020 20:12:05 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf8f5c0e3e8cbedd1856b25b5763e4c752972ab4798c8a062f1385ed3b883e5d`  
		Last Modified: Sat, 18 Apr 2020 02:59:17 GMT  
		Size: 6.1 MB (6087639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31489134f40b2fa7ba48cc30faaf403b60d8929fc974bfbb17e13eb2e7ca883`  
		Last Modified: Sat, 18 Apr 2020 02:59:15 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9145199ab3e2af1337fe0858e99a5bf7e7d9574ad0c2f59e6f27a19639076d`  
		Last Modified: Sat, 18 Apr 2020 02:59:19 GMT  
		Size: 15.1 MB (15129176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34198078c3e7c80e2422e3216a253fb00b59a6dba083bb8d01ab063ade1bd421`  
		Last Modified: Sat, 18 Apr 2020 02:59:15 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97891fd7a7f941a37b249ab3a7b66fc11caa0a6e9b1035a2a1de4661f79842ef`  
		Last Modified: Sat, 18 Apr 2020 02:59:15 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:fpm-alpine` - linux; s390x

```console
$ docker pull matomo@sha256:75137f07db33d2dc42e35bcfdb2ec16f707f048c53c26c326f040b0adfd5c73f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.8 MB (48785965 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa7a55ae487b5bc6b85fa2aa92bf2f71cda89fc76ecbff92d55b1c52266411e6`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 23:04:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 23 Apr 2020 23:04:49 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 23 Apr 2020 23:04:50 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 23 Apr 2020 23:04:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 23:04:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 23:07:22 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 23 Apr 2020 23:07:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 23:07:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 23:07:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 23:07:23 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Apr 2020 23:07:23 GMT
ENV PHP_VERSION=7.4.5
# Thu, 23 Apr 2020 23:07:23 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.5.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.5.tar.xz.asc/from/this/mirror
# Thu, 23 Apr 2020 23:07:23 GMT
ENV PHP_SHA256=d059fd7f55bdc4d2eada15a00a2976697010d3631ef6f83149cc5289e1f23c2c PHP_MD5=
# Thu, 23 Apr 2020 23:07:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 23 Apr 2020 23:07:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Apr 2020 23:09:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Apr 2020 23:09:35 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 23 Apr 2020 23:09:36 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Apr 2020 23:09:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Apr 2020 23:09:37 GMT
WORKDIR /var/www/html
# Thu, 23 Apr 2020 23:09:37 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 23 Apr 2020 23:09:37 GMT
STOPSIGNAL SIGQUIT
# Thu, 23 Apr 2020 23:09:38 GMT
EXPOSE 9000
# Thu, 23 Apr 2020 23:09:38 GMT
CMD ["php-fpm"]
# Fri, 24 Apr 2020 09:32:01 GMT
LABEL maintainer=pierre@piwik.org
# Fri, 24 Apr 2020 09:32:53 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Fri, 24 Apr 2020 09:32:54 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 24 Apr 2020 09:32:54 GMT
ENV MATOMO_VERSION=3.13.4
# Fri, 24 Apr 2020 09:33:00 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Fri, 24 Apr 2020 09:33:01 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 24 Apr 2020 09:33:02 GMT
COPY file:5a7e05d095f2d5d960fd43fac9e7317ffe1cd3fb9251933251a337b583272d45 in /entrypoint.sh 
# Fri, 24 Apr 2020 09:33:02 GMT
VOLUME [/var/www/html]
# Fri, 24 Apr 2020 09:33:02 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 24 Apr 2020 09:33:02 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9311aad926b3cb7924b7f1bbfda3972f2b64dca32e8decf8257ba49353a285`  
		Last Modified: Thu, 23 Apr 2020 23:53:51 GMT  
		Size: 1.4 MB (1397092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77861eec55084cb75eb6742ba23b02781c9311acbf6d27f56e08d1323565fe2`  
		Last Modified: Thu, 23 Apr 2020 23:53:50 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628ed6ecb36cf955a18714674b47d5822ae7eb0372cd31f3c2edd4a3c38fce32`  
		Last Modified: Thu, 23 Apr 2020 23:53:48 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4dc93412b4b0c8b58665d8d7262718d1eb97a4c48de5cc586a9bd1922c01ba`  
		Last Modified: Thu, 23 Apr 2020 23:54:21 GMT  
		Size: 10.3 MB (10290399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a8073a252d21986109a95fe67917b35179752aa6348d60d9b150dedca62137`  
		Last Modified: Thu, 23 Apr 2020 23:54:18 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163589be17a53e88a321ee96f470b1643a3cb49446d17f4cf0c8e9d53f23cd4d`  
		Last Modified: Thu, 23 Apr 2020 23:54:21 GMT  
		Size: 13.5 MB (13497767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde35644c7ffb4c973e7e569ccdd7cdc1d9195297760f8edf0b733ce88e5a8b3`  
		Last Modified: Thu, 23 Apr 2020 23:54:18 GMT  
		Size: 2.2 KB (2216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1fd05dfb5c187b6eafdb642b70eda1b1e89e6b46841fd21bb30e2ba1aa3c9b2`  
		Last Modified: Thu, 23 Apr 2020 23:54:18 GMT  
		Size: 17.2 KB (17232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cac1b641d1d14074ae8c68ce95900a6aa88fa24f590db5cca88420a3d17f43d3`  
		Last Modified: Thu, 23 Apr 2020 23:54:18 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77c8b6c13cef04c759c36b1e7d692bdd712e41dcd1746e722054f1c2c735a3eb`  
		Last Modified: Fri, 24 Apr 2020 09:33:24 GMT  
		Size: 5.9 MB (5857883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a895c608b0f110f26278b51ae59bb7098a05e2c6f406305f26942301f546e15`  
		Last Modified: Fri, 24 Apr 2020 09:33:29 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098c5bc92ad8fb5a491ef35a5f7cd84097d335e84b4ca509d025d67384f9e550`  
		Last Modified: Fri, 24 Apr 2020 09:33:27 GMT  
		Size: 15.1 MB (15129203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9b031d705d01a2da5b24563a019779a4ef53fdac0a28d7e5387f4190eb37dc`  
		Last Modified: Fri, 24 Apr 2020 09:33:29 GMT  
		Size: 302.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca49ac0df6d8cfa9bedb9e6897f6bcba94a41a1ae70aeacea3f875768cc9a326`  
		Last Modified: Fri, 24 Apr 2020 09:33:30 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
