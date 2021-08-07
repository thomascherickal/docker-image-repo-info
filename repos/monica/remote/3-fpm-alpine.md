## `monica:3-fpm-alpine`

```console
$ docker pull monica@sha256:eb0a095f7530fbcd173bd26d2c614b4240e1e5bc18662187c809f9446aebfe50
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

### `monica:3-fpm-alpine` - linux; amd64

```console
$ docker pull monica@sha256:37a16b5091d687905315280ca6e2bdfba0153e89218ad31e053a21bfe25f5f4d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.9 MB (84879193 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:170d318ed35d6d02a65a77f75866868ac71b6efbd5e415755deee6ffbbdcc5f3`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:50:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 06 Aug 2021 22:50:14 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 06 Aug 2021 22:50:16 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 06 Aug 2021 22:50:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 06 Aug 2021 22:50:19 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 06 Aug 2021 22:59:39 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 06 Aug 2021 22:59:40 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 06 Aug 2021 22:59:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 06 Aug 2021 22:59:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 06 Aug 2021 23:17:47 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 06 Aug 2021 23:17:47 GMT
ENV PHP_VERSION=8.0.9
# Fri, 06 Aug 2021 23:17:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Fri, 06 Aug 2021 23:17:48 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Fri, 06 Aug 2021 23:17:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 06 Aug 2021 23:17:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 06 Aug 2021 23:24:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 06 Aug 2021 23:24:18 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 06 Aug 2021 23:24:19 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Aug 2021 23:24:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Aug 2021 23:24:20 GMT
WORKDIR /var/www/html
# Fri, 06 Aug 2021 23:24:20 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 06 Aug 2021 23:24:20 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Aug 2021 23:24:21 GMT
EXPOSE 9000
# Fri, 06 Aug 2021 23:24:21 GMT
CMD ["php-fpm"]
# Sat, 07 Aug 2021 03:52:37 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 07 Aug 2021 03:52:38 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 07 Aug 2021 03:54:54 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;     pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 07 Aug 2021 03:54:54 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 07 Aug 2021 03:54:55 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 07 Aug 2021 03:54:56 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Sat, 07 Aug 2021 03:54:56 GMT
WORKDIR /var/www/html
# Sat, 07 Aug 2021 03:54:56 GMT
ENV MONICA_VERSION=v3.1.3
# Sat, 07 Aug 2021 03:54:56 GMT
LABEL org.opencontainers.image.revision=cefeb9bdfa74e30ff77ff692c3d14c05ae081bff org.opencontainers.image.version=v3.1.3
# Sat, 07 Aug 2021 03:55:12 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 07 Aug 2021 03:55:13 GMT
COPY multi:5f5b8f46d302c5cdff02d8777e1d9d8f8beff3e1f102442e040e0743e3c62107 in /usr/local/bin/ 
# Sat, 07 Aug 2021 03:55:13 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 07 Aug 2021 03:55:14 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40df5ce4894c4fe544404fe34e6bb75518b0ae8c6b90819795e09750e8023bc5`  
		Last Modified: Sat, 07 Aug 2021 00:01:43 GMT  
		Size: 1.7 MB (1707767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b42904e0b354067c595d0b768fd0ec45eb21ec15058a815b60ade71ee430d732`  
		Last Modified: Sat, 07 Aug 2021 00:01:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49b0bef73260aa884024d4812378dc7458a626d07690e51be1b680ac2ae2dcb4`  
		Last Modified: Sat, 07 Aug 2021 00:01:43 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f20dd09c7ef265cc5dfa019908937ccebd71bb42fb144f41440f5bdf1e4f363`  
		Last Modified: Sat, 07 Aug 2021 00:03:45 GMT  
		Size: 10.7 MB (10698206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1406db6d909e8bacb1bf4dbf24f7edc4573ff0f85d47a36d62193880e1e91d7c`  
		Last Modified: Sat, 07 Aug 2021 00:03:41 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b00981ad58d3654ef47876848fb111ebd74f98b81e3a79e69e4d776fd19e56ee`  
		Last Modified: Sat, 07 Aug 2021 00:03:44 GMT  
		Size: 15.0 MB (15027425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09a365729abe6722f1b3d94177cc8966b12b11d3c469f0de5eb2b70dc730abe`  
		Last Modified: Sat, 07 Aug 2021 00:03:41 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b011327317fe8358a7e745f83dd782c385e007116ccec1b58727a1a47f9b8cb`  
		Last Modified: Sat, 07 Aug 2021 00:03:41 GMT  
		Size: 17.8 KB (17784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18890f9c460ceb1ab9155c263172fb8ab67d63f21aa2aabbfa233680a6259165`  
		Last Modified: Sat, 07 Aug 2021 00:03:41 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1687d8d808142a38b5882815a8f40f532a912830a0bfa103943d879dfb16600`  
		Last Modified: Sat, 07 Aug 2021 03:55:43 GMT  
		Size: 1.2 MB (1235413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48ca731b6847dc6d3583ef2d27aae6a47a3faba595f49cf88fe513ee6cf8582`  
		Last Modified: Sat, 07 Aug 2021 03:55:43 GMT  
		Size: 19.1 MB (19136201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30f4824ae2b5801154ac75e3ae65bcadd17614532394486bf105722e222bfe25`  
		Last Modified: Sat, 07 Aug 2021 03:55:40 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f9530ac6e2ba5ff7fcaad2eb1fe6bbc117b24721bd3cd40e2c4b294d127253`  
		Last Modified: Sat, 07 Aug 2021 03:55:40 GMT  
		Size: 25.8 KB (25752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085d9054fa81ef1d225a14f12ab7c375193f28d5089e99d58ade1ff05b28bde3`  
		Last Modified: Sat, 07 Aug 2021 03:55:49 GMT  
		Size: 34.2 MB (34202836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f17902807185dc0d7aeca1c6957d505443c65a938f627b1d36d02ddb67e2d1`  
		Last Modified: Sat, 07 Aug 2021 03:55:40 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:3-fpm-alpine` - linux; arm variant v6

```console
$ docker pull monica@sha256:8ea7bd1a7361778864d3eb56d3e4b83ec4f8bd9d9f52f224a5d7049a3a3a4148
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.8 MB (82802200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d02062a7123b3b197ecdd003f8cb373e524a651a7278fdfcad33baebd2e659ee`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 06 Aug 2021 17:49:32 GMT
ADD file:7f2c7deda009eabdcbbdccb11e854043d32c498e64e7e1ca02165d7bb4261d39 in / 
# Fri, 06 Aug 2021 17:49:32 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 20:25:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 06 Aug 2021 20:25:29 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 06 Aug 2021 20:25:30 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 06 Aug 2021 20:25:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 06 Aug 2021 20:25:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 06 Aug 2021 20:30:30 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 06 Aug 2021 20:30:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 06 Aug 2021 20:30:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 06 Aug 2021 20:30:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 06 Aug 2021 20:41:04 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 06 Aug 2021 20:41:04 GMT
ENV PHP_VERSION=8.0.9
# Fri, 06 Aug 2021 20:41:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Fri, 06 Aug 2021 20:41:05 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Fri, 06 Aug 2021 20:41:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 06 Aug 2021 20:41:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 06 Aug 2021 20:45:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 06 Aug 2021 20:45:38 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 06 Aug 2021 20:45:41 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Aug 2021 20:45:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Aug 2021 20:45:42 GMT
WORKDIR /var/www/html
# Fri, 06 Aug 2021 20:45:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 06 Aug 2021 20:45:44 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Aug 2021 20:45:44 GMT
EXPOSE 9000
# Fri, 06 Aug 2021 20:45:45 GMT
CMD ["php-fpm"]
# Sat, 07 Aug 2021 02:02:03 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 07 Aug 2021 02:02:05 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 07 Aug 2021 02:06:05 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;     pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 07 Aug 2021 02:06:07 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 07 Aug 2021 02:06:07 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 07 Aug 2021 02:06:10 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Sat, 07 Aug 2021 02:06:11 GMT
WORKDIR /var/www/html
# Sat, 07 Aug 2021 02:06:11 GMT
ENV MONICA_VERSION=v3.1.3
# Sat, 07 Aug 2021 02:06:11 GMT
LABEL org.opencontainers.image.revision=cefeb9bdfa74e30ff77ff692c3d14c05ae081bff org.opencontainers.image.version=v3.1.3
# Sat, 07 Aug 2021 02:06:53 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 07 Aug 2021 02:06:54 GMT
COPY multi:5f5b8f46d302c5cdff02d8777e1d9d8f8beff3e1f102442e040e0743e3c62107 in /usr/local/bin/ 
# Sat, 07 Aug 2021 02:06:55 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 07 Aug 2021 02:06:55 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f465bb3e9fcd0c42f936ecc566c6e40353c00f3089b2b2c2ea1663c30f89d3ab`  
		Last Modified: Fri, 06 Aug 2021 17:51:00 GMT  
		Size: 2.6 MB (2626350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c308e0cc29c44fbd995ee591fe7289bde1e488176fb402318132d40caa05c299`  
		Last Modified: Fri, 06 Aug 2021 21:25:23 GMT  
		Size: 1.7 MB (1696670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983c92fbbed0d3241e2a4aa8f6ec320484791f6923f18c795878fea03971b8bd`  
		Last Modified: Fri, 06 Aug 2021 21:25:22 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f89139d48debd7c21fa5272e8bb4a983181e2f8d1f37a9f65ee5c99086cd7c`  
		Last Modified: Fri, 06 Aug 2021 21:25:22 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1731abf9b63ec78c2cc9a1730af1b5ca19cee8d0e7c3ef28a36c6d750f6844`  
		Last Modified: Fri, 06 Aug 2021 21:28:14 GMT  
		Size: 10.7 MB (10698217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64451af50d9b7791370d14d0a8bdd6cd115dc8bb76cdeed85eaa26fc7f11fabf`  
		Last Modified: Fri, 06 Aug 2021 21:28:09 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ca498196320ee4be66b851d46c8299f5a31b1cbc20108513e26636cd58d393f`  
		Last Modified: Fri, 06 Aug 2021 21:28:19 GMT  
		Size: 13.7 MB (13673306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a663d8c3078984313202c5494f8dddfc4c0675b691d8c79e2dd5950b0edae4`  
		Last Modified: Fri, 06 Aug 2021 21:28:09 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e046def0ccbbc17b9c482364ca78edcdadf475ec52aa17553d0deb32f841fa3c`  
		Last Modified: Fri, 06 Aug 2021 21:28:09 GMT  
		Size: 17.8 KB (17795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c15bb209b403dfb3492a9718d5eb0a1dcd7b9a7640d3d6d42fcd3e96bec6f0a6`  
		Last Modified: Fri, 06 Aug 2021 21:28:09 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85cfa53163cc14a0f35aa50b0fe2cc71d0a53145fe95267389703aa9bf22221`  
		Last Modified: Sat, 07 Aug 2021 02:07:30 GMT  
		Size: 1.3 MB (1263330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8344aa392dab9f61ce890d21acbc43a7db382bffc476275876d3ceea7f64204`  
		Last Modified: Sat, 07 Aug 2021 02:07:38 GMT  
		Size: 18.6 MB (18583168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9f3ba212ca41636992d4ff10bae4c4d379b19af87c87a586087b04f1abdf94`  
		Last Modified: Sat, 07 Aug 2021 02:07:27 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f5ca35ae0e4147626e2539b729ab02904a12f92b89b8db65c349aaecba06fe`  
		Last Modified: Sat, 07 Aug 2021 02:07:27 GMT  
		Size: 25.8 KB (25771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5656e06e5b4f78a6ccbb546daa177d4b2bcb2a5ae7669eb44430aefc1ac464d7`  
		Last Modified: Sat, 07 Aug 2021 02:08:11 GMT  
		Size: 34.2 MB (34202789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51ae055585006313d125e38de5b2fdecb4176a14969e28d11af66ed29e9420de`  
		Last Modified: Sat, 07 Aug 2021 02:07:27 GMT  
		Size: 1.7 KB (1724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:3-fpm-alpine` - linux; arm variant v7

```console
$ docker pull monica@sha256:3281fd031ce9cdbefd4d3494f5d0ae1893406dfa59be7a42e0163507fdf7496a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81150293 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3eef5cd0a4c1f48e690552a04fa64585861664e6937cd4ae7e67354681ce7b1`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 30 Jul 2021 18:36:19 GMT
ADD file:416a8b507abdc6bdcb22997a4be0a4170796c3f9f77e315b2dbff2b0a212bc68 in / 
# Fri, 30 Jul 2021 18:36:20 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 06:33:39 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 31 Jul 2021 06:33:42 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 31 Jul 2021 06:33:44 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 31 Jul 2021 06:33:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 31 Jul 2021 06:33:45 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 31 Jul 2021 06:38:36 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sat, 31 Jul 2021 06:38:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 31 Jul 2021 06:38:37 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 31 Jul 2021 06:38:37 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 31 Jul 2021 06:59:19 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sat, 31 Jul 2021 06:59:19 GMT
ENV PHP_VERSION=8.0.9
# Sat, 31 Jul 2021 06:59:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Sat, 31 Jul 2021 06:59:20 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Sat, 31 Jul 2021 06:59:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 31 Jul 2021 06:59:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 31 Jul 2021 07:03:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 31 Jul 2021 07:03:41 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 31 Jul 2021 07:03:44 GMT
RUN docker-php-ext-enable sodium
# Sat, 31 Jul 2021 07:03:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 31 Jul 2021 07:03:45 GMT
WORKDIR /var/www/html
# Sat, 31 Jul 2021 07:03:46 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 31 Jul 2021 07:03:47 GMT
STOPSIGNAL SIGQUIT
# Sat, 31 Jul 2021 07:03:47 GMT
EXPOSE 9000
# Sat, 31 Jul 2021 07:03:48 GMT
CMD ["php-fpm"]
# Sat, 31 Jul 2021 15:50:13 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 31 Jul 2021 15:50:16 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 31 Jul 2021 15:54:08 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;     pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 31 Jul 2021 15:54:10 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 31 Jul 2021 15:54:11 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 31 Jul 2021 15:54:13 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Sat, 31 Jul 2021 15:54:14 GMT
WORKDIR /var/www/html
# Sat, 31 Jul 2021 15:54:14 GMT
ENV MONICA_VERSION=v3.1.3
# Sat, 31 Jul 2021 15:54:15 GMT
LABEL org.opencontainers.image.revision=cefeb9bdfa74e30ff77ff692c3d14c05ae081bff org.opencontainers.image.version=v3.1.3
# Sat, 31 Jul 2021 15:54:57 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 31 Jul 2021 15:54:59 GMT
COPY multi:5f5b8f46d302c5cdff02d8777e1d9d8f8beff3e1f102442e040e0743e3c62107 in /usr/local/bin/ 
# Sat, 31 Jul 2021 15:55:00 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 31 Jul 2021 15:55:00 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:136482bf81d1fa351b424ebb8c7e34d15f2c5ed3fc0b66b544b8312bda3d52d9`  
		Last Modified: Tue, 15 Jun 2021 23:16:40 GMT  
		Size: 2.4 MB (2427917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c695d54d72235b2a641e5c0e2982ce2288faafa7c7a15cf38314d32eadde549a`  
		Last Modified: Sat, 31 Jul 2021 08:31:05 GMT  
		Size: 1.6 MB (1564631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62bcce9183bdd1bc68e82fa8188ef251388c691dafd2352ad787ddb168450e33`  
		Last Modified: Sat, 31 Jul 2021 08:31:04 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89d6c9a81dd0be6901229c1d2f4adae785f73bf6302ddbd7eb88227ec22de0b`  
		Last Modified: Sat, 31 Jul 2021 08:31:03 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:398f487c2db68e495a678bb67d26995e84e0bbd929b873c712c4ab8eeb45acc4`  
		Last Modified: Sat, 31 Jul 2021 08:35:28 GMT  
		Size: 10.7 MB (10698205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364204ec74954d60a296ca7bbe7c1d6b9004939b091bc71fd8d724f7bbf05182`  
		Last Modified: Sat, 31 Jul 2021 08:35:24 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585379f47b8680e1d56c8091e05d3e8fe814ea77147b70c10550e13fd31b0e70`  
		Last Modified: Sat, 31 Jul 2021 08:35:33 GMT  
		Size: 12.8 MB (12803766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16c79e736efbcd6987134b2fd3da178aa67b9bc40b354fd38325086ed115effa`  
		Last Modified: Sat, 31 Jul 2021 08:35:24 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4272c72e0f68dfbbce77070cec5c40733bf86c52354f1dc951e311f092624151`  
		Last Modified: Sat, 31 Jul 2021 08:35:24 GMT  
		Size: 17.8 KB (17786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bce1f34200ff564d86784cfa1d90c73c861068177c37dbb9991fcbcf268ad0b`  
		Last Modified: Sat, 31 Jul 2021 08:35:24 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7920b49cb1c4fed7f7cc632016fb7bca9b3d20205670972a6daedb5f9a56eec6`  
		Last Modified: Sat, 31 Jul 2021 15:56:46 GMT  
		Size: 1.1 MB (1147794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c21d0a070bf8ca18a9f39cbef15fb19ed38aa017a3d876ede51b2404e31f2be`  
		Last Modified: Sat, 31 Jul 2021 15:56:53 GMT  
		Size: 18.2 MB (18246844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5c13352fd22041284dc4f49e24e26b9f51664546cea9dc23dbfb6a4e7ef405`  
		Last Modified: Sat, 31 Jul 2021 15:56:43 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3dcde7c6fad6ea67b0f3c05e0f5febee2577fac2406e67284577fd189c4c71d`  
		Last Modified: Sat, 31 Jul 2021 15:56:43 GMT  
		Size: 25.7 KB (25741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54e8ff39b2f7399b918b643c019a5bd58202a56502642eb85e49c72469247381`  
		Last Modified: Sat, 31 Jul 2021 15:57:27 GMT  
		Size: 34.2 MB (34202801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7835c0017f2348443490042100b5b485b4df02fff4ed0bcca747001194031b`  
		Last Modified: Sat, 31 Jul 2021 15:56:43 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:3-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull monica@sha256:f95ae6a0214cfc0961db76458f1cf7b7df8087508ba216013a4633e0670be0ed
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84159631 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03876071c4fbbbeafa4c8d3b12f213e4a5efd0952112b03883ad6701ca26e4a0`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 06 Aug 2021 17:39:26 GMT
ADD file:1a8fd1066485e1261462e689c1a072f010c1d3be904b73ef2b84128fac652951 in / 
# Fri, 06 Aug 2021 17:39:27 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 22:13:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 06 Aug 2021 22:13:45 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 06 Aug 2021 22:13:46 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 06 Aug 2021 22:13:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 06 Aug 2021 22:13:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 06 Aug 2021 22:21:12 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 06 Aug 2021 22:21:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 06 Aug 2021 22:21:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 06 Aug 2021 22:21:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 06 Aug 2021 22:34:42 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 06 Aug 2021 22:34:42 GMT
ENV PHP_VERSION=8.0.9
# Fri, 06 Aug 2021 22:34:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Fri, 06 Aug 2021 22:34:42 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Fri, 06 Aug 2021 22:34:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 06 Aug 2021 22:34:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 06 Aug 2021 22:39:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 06 Aug 2021 22:39:45 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 06 Aug 2021 22:39:46 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Aug 2021 22:39:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Aug 2021 22:39:47 GMT
WORKDIR /var/www/html
# Fri, 06 Aug 2021 22:39:47 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 06 Aug 2021 22:39:48 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Aug 2021 22:39:48 GMT
EXPOSE 9000
# Fri, 06 Aug 2021 22:39:48 GMT
CMD ["php-fpm"]
# Sat, 07 Aug 2021 03:26:55 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 07 Aug 2021 03:26:57 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 07 Aug 2021 03:28:43 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;     pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 07 Aug 2021 03:28:44 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 07 Aug 2021 03:28:44 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 07 Aug 2021 03:28:45 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Sat, 07 Aug 2021 03:28:46 GMT
WORKDIR /var/www/html
# Sat, 07 Aug 2021 03:28:46 GMT
ENV MONICA_VERSION=v3.1.3
# Sat, 07 Aug 2021 03:28:46 GMT
LABEL org.opencontainers.image.revision=cefeb9bdfa74e30ff77ff692c3d14c05ae081bff org.opencontainers.image.version=v3.1.3
# Sat, 07 Aug 2021 03:29:00 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 07 Aug 2021 03:29:01 GMT
COPY multi:5f5b8f46d302c5cdff02d8777e1d9d8f8beff3e1f102442e040e0743e3c62107 in /usr/local/bin/ 
# Sat, 07 Aug 2021 03:29:01 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 07 Aug 2021 03:29:01 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:fd3acdcea5682abced546ec19fb6ebee725c5184e5d91614c469c0a79e67f2d0`  
		Last Modified: Fri, 06 Aug 2021 17:40:12 GMT  
		Size: 2.7 MB (2710613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e75c04557b83c6887fa33eb52320a5c1afed1d1b8299d3accdf27cea6b5860`  
		Last Modified: Fri, 06 Aug 2021 23:19:35 GMT  
		Size: 1.7 MB (1710420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd6439bb8bd6ba02680eef64ad51b996399f05a740cd7ab8e62834b24527f60c`  
		Last Modified: Fri, 06 Aug 2021 23:19:35 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d61d6c7061c67dabfce2227dc9665b59eb7c43fd2f927c11e7c76446b50fed3`  
		Last Modified: Fri, 06 Aug 2021 23:19:35 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1dabf8050863e6f4c5d2eb9cfff6d53c0efc71c350288f1f0989d3315a6e13`  
		Last Modified: Fri, 06 Aug 2021 23:22:12 GMT  
		Size: 10.7 MB (10698208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c205d306c5478b8aa48341613f849dcfe357b89df30059188480d36ae905ee79`  
		Last Modified: Fri, 06 Aug 2021 23:22:09 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269869fb5d9d6d2d152bf2acbc1507e1dfbdaffdc8eea9776cbdb265ddcd1fdf`  
		Last Modified: Fri, 06 Aug 2021 23:22:11 GMT  
		Size: 14.5 MB (14467185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57f9889b7bb2d1c6e8c5f410747baf0103998e1d836c4d849597508b399f0247`  
		Last Modified: Fri, 06 Aug 2021 23:22:11 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5501f4d498505479486424658d951e90c6d706a6c06e1a77f39cb9c0c8e41bc`  
		Last Modified: Fri, 06 Aug 2021 23:22:08 GMT  
		Size: 17.8 KB (17789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62ec09d32decdcd15ab155bb3eb27be526ca14f5c6fcb3ec15810d20c57aa0d1`  
		Last Modified: Fri, 06 Aug 2021 23:22:08 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e64b868d2fd0eee20cd4bc2a9081d7245c82e2538793d2be24b161fbdb248b0c`  
		Last Modified: Sat, 07 Aug 2021 03:29:53 GMT  
		Size: 1.3 MB (1258060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b34704ba2a6fe4d510383bcbab558c617bb854c4f867163feabc9593166671f`  
		Last Modified: Sat, 07 Aug 2021 03:29:53 GMT  
		Size: 19.1 MB (19053973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c91ff84935ed2dcff9c6af01398a5beaef27242453ec1d629a1da86ade82a9`  
		Last Modified: Sat, 07 Aug 2021 03:29:50 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24096cd00cf1fe85db537cc9c59ee36c0c2bf0c5df040c139c1f17c528a5daaf`  
		Last Modified: Sat, 07 Aug 2021 03:29:51 GMT  
		Size: 25.7 KB (25740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a69e4cb3b011c6fe5495026746349c669dc92590068988055b4872848f4a0a71`  
		Last Modified: Sat, 07 Aug 2021 03:30:00 GMT  
		Size: 34.2 MB (34202840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1817356bd6b579c2da1cf4cc5c053287dd46a3d5ff0126df82ccba2b4276e0cf`  
		Last Modified: Sat, 07 Aug 2021 03:29:50 GMT  
		Size: 1.7 KB (1721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:3-fpm-alpine` - linux; 386

```console
$ docker pull monica@sha256:f3897bb06fd1763d30d115e29d209f45202bffed442a96ab9b3f79459c5be30f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.7 MB (85721455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71b1a124328310d86b9cee78baac28ce9bd4af681e458e98a3c28d3d6b213f56`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 06 Aug 2021 17:38:26 GMT
ADD file:bafaec4a54d6cef99b5f3660d074a3d2251e4d4bd09df9ea65f33e9bffb7d88d in / 
# Fri, 06 Aug 2021 17:38:26 GMT
CMD ["/bin/sh"]
# Fri, 06 Aug 2021 19:51:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 06 Aug 2021 19:51:53 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 06 Aug 2021 19:51:54 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 06 Aug 2021 19:51:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 06 Aug 2021 19:51:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 06 Aug 2021 20:01:40 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 06 Aug 2021 20:01:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 06 Aug 2021 20:01:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 06 Aug 2021 20:01:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 06 Aug 2021 20:23:46 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 06 Aug 2021 20:23:46 GMT
ENV PHP_VERSION=8.0.9
# Fri, 06 Aug 2021 20:23:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Fri, 06 Aug 2021 20:23:47 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Fri, 06 Aug 2021 20:23:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 06 Aug 2021 20:23:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 06 Aug 2021 20:34:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 06 Aug 2021 20:35:00 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 06 Aug 2021 20:35:02 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Aug 2021 20:35:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Aug 2021 20:35:03 GMT
WORKDIR /var/www/html
# Fri, 06 Aug 2021 20:35:05 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 06 Aug 2021 20:35:05 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Aug 2021 20:35:06 GMT
EXPOSE 9000
# Fri, 06 Aug 2021 20:35:06 GMT
CMD ["php-fpm"]
# Sat, 07 Aug 2021 04:05:20 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 07 Aug 2021 04:05:22 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 07 Aug 2021 04:07:37 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;     pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 07 Aug 2021 04:07:38 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 07 Aug 2021 04:07:38 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 07 Aug 2021 04:07:40 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Sat, 07 Aug 2021 04:07:40 GMT
WORKDIR /var/www/html
# Sat, 07 Aug 2021 04:07:40 GMT
ENV MONICA_VERSION=v3.1.3
# Sat, 07 Aug 2021 04:07:40 GMT
LABEL org.opencontainers.image.revision=cefeb9bdfa74e30ff77ff692c3d14c05ae081bff org.opencontainers.image.version=v3.1.3
# Sat, 07 Aug 2021 04:08:00 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 07 Aug 2021 04:08:01 GMT
COPY multi:5f5b8f46d302c5cdff02d8777e1d9d8f8beff3e1f102442e040e0743e3c62107 in /usr/local/bin/ 
# Sat, 07 Aug 2021 04:08:01 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 07 Aug 2021 04:08:01 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:935703e1179e32e201e4a36d5664d58299dc8e7bcac197b70c295c0a59216db1`  
		Last Modified: Fri, 06 Aug 2021 17:39:15 GMT  
		Size: 2.8 MB (2821910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bc90fe4dc39a7e7f38b6432bdad0e75f77d67e4e3178d9d16f40d1ada5f457`  
		Last Modified: Fri, 06 Aug 2021 21:36:03 GMT  
		Size: 1.8 MB (1805352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:928af557c35f437b637c8d69d4bdd2a15a3b0b67bf9f6787665f71961a34e034`  
		Last Modified: Fri, 06 Aug 2021 21:36:02 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a683f64b78ccf96092b41e5b5ddf8c6e77e27b81a36bf0ecb9636b80b4cf2d4`  
		Last Modified: Fri, 06 Aug 2021 21:36:02 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70f4305236420b0aec17466bddff7246e887f7830fcd003d2da46ed946cc46fe`  
		Last Modified: Fri, 06 Aug 2021 21:39:00 GMT  
		Size: 10.7 MB (10698191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890564ca0ec3a263934fc53f9e4aca8e9da30d565f43393a44221d62c8235765`  
		Last Modified: Fri, 06 Aug 2021 21:38:55 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f09f979827e471973f6fda815572438c447b4068acccd076a13f01993adb3f4`  
		Last Modified: Fri, 06 Aug 2021 21:39:02 GMT  
		Size: 15.4 MB (15369892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4683fc544f2dee3fbd6fe049dde16e001dfd230be77066c3b126fb792040b157`  
		Last Modified: Fri, 06 Aug 2021 21:38:55 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af2687f35c054ac628fde8850a2d489c63ab361861178f9f73c3a35d322ca8de`  
		Last Modified: Fri, 06 Aug 2021 21:38:55 GMT  
		Size: 17.8 KB (17780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9021103ae1aed83d290d4a6addef4e75666e61e26ffb15c6113ccffd3b547c8`  
		Last Modified: Fri, 06 Aug 2021 21:38:55 GMT  
		Size: 8.6 KB (8569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efa5f6e63cfd6e16288e0ed295d40fbefb261a04277ec95529e9e4d9fcaf194`  
		Last Modified: Sat, 07 Aug 2021 04:09:07 GMT  
		Size: 1.3 MB (1333361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0204ef6808b00e9df647334e75b4bea69b8f9a6341670778893467c4c6ef73e0`  
		Last Modified: Sat, 07 Aug 2021 04:09:08 GMT  
		Size: 19.4 MB (19431651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4fa53857a23ecab5883706eb84e83bc44f4b112d39271db2adc4e624fafde1f`  
		Last Modified: Sat, 07 Aug 2021 04:09:03 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712c45ae8c3ea8985970d86f987d1bb965ff6f1ec8e276ccab0dde410e142282`  
		Last Modified: Sat, 07 Aug 2021 04:09:03 GMT  
		Size: 25.7 KB (25729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d9f9b4c47def3ebd52129db7d1c0611982a596f377e178794a4be09cfb150f`  
		Last Modified: Sat, 07 Aug 2021 04:09:16 GMT  
		Size: 34.2 MB (34202783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef9c1f58248b304a3ee83ff0242da6b96d3b83e7091cdaec397ad9c09848d05`  
		Last Modified: Sat, 07 Aug 2021 04:09:03 GMT  
		Size: 1.7 KB (1724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:3-fpm-alpine` - linux; ppc64le

```console
$ docker pull monica@sha256:03b3822e4818337d51123b5ac2ca022356329d96e37a3a392399e925afa4b190
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.1 MB (86100219 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b9eb8846fd6fb95cb8f74926da7ed70a055f5c22120df5e1bec537e63347f278`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 30 Jul 2021 17:24:32 GMT
ADD file:0075aad7a94f0496483442bb2d9fdaa13e9c23087b90638d014b4bc263aa3861 in / 
# Fri, 30 Jul 2021 17:24:37 GMT
CMD ["/bin/sh"]
# Sat, 31 Jul 2021 02:06:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 31 Jul 2021 02:07:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 31 Jul 2021 02:07:21 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 31 Jul 2021 02:07:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 31 Jul 2021 02:07:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 31 Jul 2021 02:13:32 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Sat, 31 Jul 2021 02:13:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 31 Jul 2021 02:13:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 31 Jul 2021 02:13:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 31 Jul 2021 02:40:26 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Sat, 31 Jul 2021 02:40:31 GMT
ENV PHP_VERSION=8.0.9
# Sat, 31 Jul 2021 02:40:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.9.tar.xz.asc
# Sat, 31 Jul 2021 02:40:37 GMT
ENV PHP_SHA256=71a01b2b56544e20e28696ad5b366e431a0984eaa39aa5e35426a4843e172010
# Sat, 31 Jul 2021 02:40:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 31 Jul 2021 02:40:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 31 Jul 2021 02:45:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 31 Jul 2021 02:45:48 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 31 Jul 2021 02:45:59 GMT
RUN docker-php-ext-enable sodium
# Sat, 31 Jul 2021 02:46:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 31 Jul 2021 02:46:04 GMT
WORKDIR /var/www/html
# Sat, 31 Jul 2021 02:46:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 31 Jul 2021 02:46:20 GMT
STOPSIGNAL SIGQUIT
# Sat, 31 Jul 2021 02:46:25 GMT
EXPOSE 9000
# Sat, 31 Jul 2021 02:46:27 GMT
CMD ["php-fpm"]
# Sat, 31 Jul 2021 12:06:24 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 31 Jul 2021 12:06:32 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 31 Jul 2021 12:08:52 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;     pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 31 Jul 2021 12:09:07 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 31 Jul 2021 12:09:11 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 31 Jul 2021 12:09:23 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Sat, 31 Jul 2021 12:09:26 GMT
WORKDIR /var/www/html
# Sat, 31 Jul 2021 12:09:28 GMT
ENV MONICA_VERSION=v3.1.3
# Sat, 31 Jul 2021 12:09:33 GMT
LABEL org.opencontainers.image.revision=cefeb9bdfa74e30ff77ff692c3d14c05ae081bff org.opencontainers.image.version=v3.1.3
# Sat, 31 Jul 2021 12:10:04 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 31 Jul 2021 12:10:12 GMT
COPY multi:5f5b8f46d302c5cdff02d8777e1d9d8f8beff3e1f102442e040e0743e3c62107 in /usr/local/bin/ 
# Sat, 31 Jul 2021 12:10:16 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 31 Jul 2021 12:10:20 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:baf144cfb66ebe9df1969f3b90f1c448beff98edc84de1ccb5d6346195a070d4`  
		Last Modified: Tue, 15 Jun 2021 22:27:38 GMT  
		Size: 2.8 MB (2810478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ccd35cdcd0d2f44750979fa156369560b3d83d0fd6c9b5b6835504233171cbf`  
		Last Modified: Sat, 31 Jul 2021 04:32:59 GMT  
		Size: 1.8 MB (1753665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a0343a7c328a00ea39b214651b5817a2158019d1c2b6acb6ae687007ce40017`  
		Last Modified: Sat, 31 Jul 2021 04:32:58 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13fb577a40a607849a76b566636558cf133d947986988e0a2aac93d0715aece0`  
		Last Modified: Sat, 31 Jul 2021 04:32:58 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51fe78d62df2d766df778b08e8ea485805227e3c35c21047d3467b18171ae577`  
		Last Modified: Sat, 31 Jul 2021 04:35:59 GMT  
		Size: 10.7 MB (10698207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de328cb4959e804d8141a2a5f6e3bd90384b6c53f0881f474f6043586847cfb`  
		Last Modified: Sat, 31 Jul 2021 04:35:56 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1cb88328f85c64ebbce244fe713ca27e4a9396228720235ff28179e65a83c70`  
		Last Modified: Sat, 31 Jul 2021 04:35:59 GMT  
		Size: 15.8 MB (15769014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1046d2c787dd33b51847f51cb5024c7463530bb8f0978eaad1899981df0b0b66`  
		Last Modified: Sat, 31 Jul 2021 04:35:56 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d9fbaf35d7690c81c6a925ed1aaed57a3157dcb9b5a8390ac58a248f9a21713`  
		Last Modified: Sat, 31 Jul 2021 04:35:56 GMT  
		Size: 17.8 KB (17795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d6de3f0ef7fd516a8aaaf894d650041ceba6cec1d02e320e1bb1e45bdc90a79`  
		Last Modified: Sat, 31 Jul 2021 04:35:56 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8956ec42a3bf125e8fa79adc0151637ed0a56c9c3f158b05980fab63a9f863f4`  
		Last Modified: Sat, 31 Jul 2021 12:11:18 GMT  
		Size: 1.3 MB (1343904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0a3ed83d9a0a4fc0f4384ea7a8e284021fe40e9f0c4143ed6082dd698b19ce`  
		Last Modified: Sat, 31 Jul 2021 12:11:20 GMT  
		Size: 19.5 MB (19463746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b54881d5078554ec9abbbeb719277aaa12a93b0b942a63118446ee52fbab1aec`  
		Last Modified: Sat, 31 Jul 2021 12:11:15 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d541221e85b1f04482f71efd448dc4b39fa44b78680cd54781033ad485409f79`  
		Last Modified: Sat, 31 Jul 2021 12:11:15 GMT  
		Size: 25.8 KB (25763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e54ec6c6922e0a067cbc51e2a3b2667aa6fb220cca364c9904de7f1c3b2bec1`  
		Last Modified: Sat, 31 Jul 2021 12:11:25 GMT  
		Size: 34.2 MB (34202834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd1a400fee58f58984ce9ebbe1a9d9b2aefe8133ccbf06fd366adcb85c14f2`  
		Last Modified: Sat, 31 Jul 2021 12:11:15 GMT  
		Size: 1.7 KB (1725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:3-fpm-alpine` - linux; s390x

```console
$ docker pull monica@sha256:f71ee4e872efc6181f5dd0e5b7f4776be1445229ea079155cb7ad2866f49ac76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.6 MB (84645778 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6c5e5988dcf89fc77425a7de60ffd12561517cf383582744cad3234ac886896`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:06:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 14 Apr 2021 19:06:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:06:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:06:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:06:47 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 04 Jun 2021 19:10:54 GMT
ENV PHP_VERSION=8.0.7
# Fri, 04 Jun 2021 19:10:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.7.tar.xz.asc
# Fri, 04 Jun 2021 19:10:55 GMT
ENV PHP_SHA256=d5fc2e4fc780a32404d88c360e3e0009bc725d936459668e9c2ac992f2d83654
# Fri, 04 Jun 2021 19:11:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 04 Jun 2021 19:11:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 04 Jun 2021 19:16:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 04 Jun 2021 19:16:06 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 04 Jun 2021 19:16:07 GMT
RUN docker-php-ext-enable sodium
# Fri, 04 Jun 2021 19:16:08 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 04 Jun 2021 19:16:08 GMT
WORKDIR /var/www/html
# Fri, 04 Jun 2021 19:16:09 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 04 Jun 2021 19:16:10 GMT
STOPSIGNAL SIGQUIT
# Fri, 04 Jun 2021 19:16:11 GMT
EXPOSE 9000
# Fri, 04 Jun 2021 19:16:11 GMT
CMD ["php-fpm"]
# Sun, 27 Jun 2021 14:14:26 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sun, 27 Jun 2021 14:14:28 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sun, 27 Jun 2021 14:16:22 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;     pecl install APCu-5.1.20;     pecl install memcached-3.1.5;     pecl install redis-5.3.4;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sun, 27 Jun 2021 14:16:25 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sun, 27 Jun 2021 14:16:25 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sun, 27 Jun 2021 14:16:27 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Sun, 27 Jun 2021 14:16:27 GMT
WORKDIR /var/www/html
# Tue, 29 Jun 2021 08:57:30 GMT
ENV MONICA_VERSION=v3.1.3
# Tue, 29 Jun 2021 08:57:30 GMT
LABEL org.opencontainers.image.revision=cefeb9bdfa74e30ff77ff692c3d14c05ae081bff org.opencontainers.image.version=v3.1.3
# Tue, 29 Jun 2021 08:58:25 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Tue, 29 Jun 2021 08:58:36 GMT
COPY multi:5f5b8f46d302c5cdff02d8777e1d9d8f8beff3e1f102442e040e0743e3c62107 in /usr/local/bin/ 
# Tue, 29 Jun 2021 08:58:37 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Tue, 29 Jun 2021 08:58:38 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:210f081baa789b8d5f27a61dfc6d3f206e14466299303e5f0aee3b6d7b4563b3`  
		Last Modified: Fri, 04 Jun 2021 19:31:31 GMT  
		Size: 10.8 MB (10788565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90c3fe50f8f6e8e758bf7ef26c3aaec4f4d8a429875bf8b3928b392cb7126621`  
		Last Modified: Fri, 04 Jun 2021 19:31:29 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fcbd135a76f3ca5ca4d5b5b307ac7c584f0e35220a25de10e4b60c9d31df85d`  
		Last Modified: Fri, 04 Jun 2021 19:31:31 GMT  
		Size: 14.3 MB (14298284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8cee214013986ad633af78c9b143ccd768f9e5192d410cfbf43a58ba73aab09`  
		Last Modified: Fri, 04 Jun 2021 19:31:29 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9729d06051e5d1d9fb03306f6bfb995912b2dcfc1b71080f5e40e2f1388094`  
		Last Modified: Fri, 04 Jun 2021 19:31:29 GMT  
		Size: 17.6 KB (17595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb00abf79f65c6ba3cce40770fde21b9394bb0da255f4c191677f13d4fecea0`  
		Last Modified: Fri, 04 Jun 2021 19:31:29 GMT  
		Size: 8.6 KB (8574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fed8f3dad5da5de8598bf2a2f4f7b8f9e25ef97bde091f5de3098acf5455387e`  
		Last Modified: Sun, 27 Jun 2021 14:19:01 GMT  
		Size: 1.3 MB (1290680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd22033de7b62bb8f0906baebb41c53a12342ce44779ff48f1d176d35615c6e1`  
		Last Modified: Sun, 27 Jun 2021 14:19:02 GMT  
		Size: 19.6 MB (19643851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50c1b3dc45deb659a214a2a5185051120c01cbb5e34ea9a9d82ce17c91f6c5b`  
		Last Modified: Sun, 27 Jun 2021 14:18:59 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4ca690ea2378da6163b14da28192cad009a9d3d8b4dba70f0ab4401038a2274`  
		Last Modified: Sun, 27 Jun 2021 14:18:59 GMT  
		Size: 25.7 KB (25664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013fae8622c1126c44d3629effabb3eb0d1b0d9400e702ee0e8c29dff4ddef71`  
		Last Modified: Tue, 29 Jun 2021 09:01:12 GMT  
		Size: 34.2 MB (34202976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6800725a90aec3bf5fe800f1ddbe3f11580c6b633223c88189219e7354a8379`  
		Last Modified: Tue, 29 Jun 2021 09:01:01 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
