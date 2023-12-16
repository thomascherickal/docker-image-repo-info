## `monica:4-fpm-alpine`

```console
$ docker pull monica@sha256:7762816b8ba2b2bdbcd13cbcd99fcaac6a37587dccedb44a928f795c2a21493f
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

### `monica:4-fpm-alpine` - linux; amd64

```console
$ docker pull monica@sha256:19c285919509b362cc34d89a5ed2bff607f359363d83e9c8eec5ae60b86763b3
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.9 MB (67875018 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf4dc701b151f0568138358047da264f2ff7f872ed1d3dfb403c9b7df07112a4`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 08 Dec 2023 01:20:49 GMT
ADD file:1f4eb46669b5b6275af19eb7471a6899a61c276aa7d925b8ae99310b14b75b92 in / 
# Fri, 08 Dec 2023 01:20:49 GMT
CMD ["/bin/sh"]
# Tue, 12 Dec 2023 20:39:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 12 Dec 2023 20:39:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		openssl 		tar 		xz
# Tue, 12 Dec 2023 20:39:54 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 12 Dec 2023 20:39:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Dec 2023 20:39:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 12 Dec 2023 20:39:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Dec 2023 20:39:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Dec 2023 20:39:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Dec 2023 22:31:11 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 12 Dec 2023 22:58:31 GMT
ENV PHP_VERSION=8.1.26
# Tue, 12 Dec 2023 22:58:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.26.tar.xz.asc
# Tue, 12 Dec 2023 22:58:31 GMT
ENV PHP_SHA256=17f87133596449327451ad4b8d9911bfaea59ff5109f3a6f2bb679f967a8ea0f
# Tue, 12 Dec 2023 22:58:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 12 Dec 2023 22:58:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 16 Dec 2023 06:19:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 		PHP_BUILD_PROVIDER='https://github.com/docker-library/php' 		PHP_UNAME='Linux - Docker' 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 16 Dec 2023 06:19:01 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 16 Dec 2023 06:19:03 GMT
RUN docker-php-ext-enable sodium
# Sat, 16 Dec 2023 06:19:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 16 Dec 2023 06:19:03 GMT
WORKDIR /var/www/html
# Sat, 16 Dec 2023 06:19:03 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 16 Dec 2023 06:19:03 GMT
STOPSIGNAL SIGQUIT
# Sat, 16 Dec 2023 06:19:03 GMT
EXPOSE 9000
# Sat, 16 Dec 2023 06:19:04 GMT
CMD ["php-fpm"]
# Sat, 16 Dec 2023 08:46:07 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 16 Dec 2023 08:46:08 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 16 Dec 2023 08:47:46 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libpq-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         pdo_pgsql         soap     ;     pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-6.0.2;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 16 Dec 2023 08:47:46 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '* * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 16 Dec 2023 08:47:46 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 16 Dec 2023 08:47:46 GMT
ENV PHP_MEMORY_LIMIT=512M PHP_UPLOAD_LIMIT=512M
# Sat, 16 Dec 2023 08:47:47 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > $PHP_INI_DIR/conf.d/limits.ini;
# Sat, 16 Dec 2023 08:47:48 GMT
WORKDIR /var/www/html
# Sat, 16 Dec 2023 08:47:48 GMT
ENV MONICA_VERSION=v4.0.0
# Sat, 16 Dec 2023 08:47:48 GMT
LABEL org.opencontainers.image.revision=e1a3e1315b1a92a5ff0ccab6c22ba9ded77a599e org.opencontainers.image.version=v4.0.0
# Sat, 16 Dec 2023 08:47:57 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 16 Dec 2023 08:47:59 GMT
COPY multi:84468128947ba1749e6048b0956ef2297175650942a70e8e8bc5df81159d8cc7 in /usr/local/bin/ 
# Sat, 16 Dec 2023 08:47:59 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 16 Dec 2023 08:47:59 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:661ff4d9561e3fd050929ee5097067c34bafc523ee60f5294a37fd08056a73ca`  
		Last Modified: Fri, 08 Dec 2023 01:21:10 GMT  
		Size: 3.4 MB (3408480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbc99979baa6760dc40a927f812328a1431e3870d0f166b035365166ef2cf8d4`  
		Last Modified: Tue, 12 Dec 2023 23:24:24 GMT  
		Size: 2.8 MB (2755737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47536423e0797b82f7a737a4efeb29297c96a33e8662ddcd121d728a01eac477`  
		Last Modified: Tue, 12 Dec 2023 23:24:23 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be6d4fc569fcdbdb835c5ee3607367e6ba4779809c0fad97de75045144220f8`  
		Last Modified: Tue, 12 Dec 2023 23:24:23 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce8d290fd902dac7a242000e514dc83802d3e9f64e5842408b8cd6c47e29f76`  
		Last Modified: Tue, 12 Dec 2023 23:35:44 GMT  
		Size: 11.8 MB (11830398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40afc0c478cb19cb1a62ee1dc14d55f2393105f33cc16229431a6bd52c151832`  
		Last Modified: Tue, 12 Dec 2023 23:35:43 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2faba4fae074fc879c02401e8cb3a4e976b21e6bc9b4800cff53e424f7fe3df`  
		Last Modified: Sat, 16 Dec 2023 06:58:47 GMT  
		Size: 12.6 MB (12595082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3937e22c148b901c57efb3717a63526103a98cb3c1760a593b318a52c60bb5c`  
		Last Modified: Sat, 16 Dec 2023 06:58:45 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f7531254e52196ed23ef84413a479ae11b3ddc0372dbb41b004e4b83b2d88d`  
		Last Modified: Sat, 16 Dec 2023 06:58:45 GMT  
		Size: 19.3 KB (19293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b3d91bc2820d30f2e89f3d226d2ddcd007ed6d97cd2d9b181f4f828b9fc8b4`  
		Last Modified: Sat, 16 Dec 2023 06:58:45 GMT  
		Size: 8.9 KB (8879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76e6709ef2a22bf0ed8ca1350815010e63c284d8ff9e8c229f9ad562a56116fc`  
		Last Modified: Sat, 16 Dec 2023 08:49:19 GMT  
		Size: 1.2 MB (1152069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27067f7a1e95df6f9248f22596e2c474726b97755bd50d9c95a81d07f18f5b5b`  
		Last Modified: Sat, 16 Dec 2023 08:49:18 GMT  
		Size: 8.9 MB (8938815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986d23f3dd454daa55da4496ce1356e5ac7bf69457c55a033bed6cdcf387a39a`  
		Last Modified: Sat, 16 Dec 2023 08:49:17 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:011af87a648c91efbd4b0ce5c681890fd4ec668cb6f2c1ea56da3cc4df15237e`  
		Last Modified: Sat, 16 Dec 2023 08:49:17 GMT  
		Size: 27.3 KB (27328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37ae201aaa78f99b8ae4641c8342cafa62599639cfe747fa0499b696b12b78e0`  
		Last Modified: Sat, 16 Dec 2023 08:49:23 GMT  
		Size: 27.1 MB (27132170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:327442f4b88a22fff07196ab91cb464c7c89bf27e0ce796f201c63a0a8273320`  
		Last Modified: Sat, 16 Dec 2023 08:49:17 GMT  
		Size: 2.1 KB (2077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:4-fpm-alpine` - linux; arm variant v6

```console
$ docker pull monica@sha256:c1379e54a5b58dd6bde206d92fc74531b4521ccff00397ec73c1bea26f9d9cc0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.1 MB (66067084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff8b2335c2f05cf0e95752523c6b36beee2f2746647e6670f8164f41eed7bfcf`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 08 Dec 2023 01:49:15 GMT
ADD file:d43ed267a41631ce0e5a4ef5aac821a75300a83f85ecb6259f5616852f89e989 in / 
# Fri, 08 Dec 2023 01:49:15 GMT
CMD ["/bin/sh"]
# Tue, 12 Dec 2023 20:01:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 12 Dec 2023 20:01:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		openssl 		tar 		xz
# Tue, 12 Dec 2023 20:01:51 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 12 Dec 2023 20:01:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Dec 2023 20:01:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 12 Dec 2023 20:01:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Dec 2023 20:01:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Dec 2023 20:01:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Dec 2023 21:30:34 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 12 Dec 2023 21:50:38 GMT
ENV PHP_VERSION=8.1.26
# Tue, 12 Dec 2023 21:50:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.26.tar.xz.asc
# Tue, 12 Dec 2023 21:50:39 GMT
ENV PHP_SHA256=17f87133596449327451ad4b8d9911bfaea59ff5109f3a6f2bb679f967a8ea0f
# Tue, 12 Dec 2023 21:50:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 12 Dec 2023 21:50:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 16 Dec 2023 03:11:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 		PHP_BUILD_PROVIDER='https://github.com/docker-library/php' 		PHP_UNAME='Linux - Docker' 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 16 Dec 2023 03:11:29 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 16 Dec 2023 03:11:30 GMT
RUN docker-php-ext-enable sodium
# Sat, 16 Dec 2023 03:11:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 16 Dec 2023 03:11:30 GMT
WORKDIR /var/www/html
# Sat, 16 Dec 2023 03:11:31 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 16 Dec 2023 03:11:31 GMT
STOPSIGNAL SIGQUIT
# Sat, 16 Dec 2023 03:11:31 GMT
EXPOSE 9000
# Sat, 16 Dec 2023 03:11:31 GMT
CMD ["php-fpm"]
# Sat, 16 Dec 2023 04:48:03 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 16 Dec 2023 04:48:05 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 16 Dec 2023 04:50:01 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libpq-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         pdo_pgsql         soap     ;     pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-6.0.2;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 16 Dec 2023 04:50:02 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '* * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 16 Dec 2023 04:50:02 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 16 Dec 2023 04:50:02 GMT
ENV PHP_MEMORY_LIMIT=512M PHP_UPLOAD_LIMIT=512M
# Sat, 16 Dec 2023 04:50:04 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > $PHP_INI_DIR/conf.d/limits.ini;
# Sat, 16 Dec 2023 04:50:04 GMT
WORKDIR /var/www/html
# Sat, 16 Dec 2023 04:50:04 GMT
ENV MONICA_VERSION=v4.0.0
# Sat, 16 Dec 2023 04:50:04 GMT
LABEL org.opencontainers.image.revision=e1a3e1315b1a92a5ff0ccab6c22ba9ded77a599e org.opencontainers.image.version=v4.0.0
# Sat, 16 Dec 2023 04:50:20 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 16 Dec 2023 04:50:21 GMT
COPY multi:84468128947ba1749e6048b0956ef2297175650942a70e8e8bc5df81159d8cc7 in /usr/local/bin/ 
# Sat, 16 Dec 2023 04:50:21 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 16 Dec 2023 04:50:21 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:0803c38384d9fd0f9afaec8fd13d267547b660dcd46bb92a3d63c5d76e78b04c`  
		Last Modified: Fri, 08 Dec 2023 01:49:33 GMT  
		Size: 3.2 MB (3165143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6157a5053a6ba5646a1361153760014335e77813c8792b60d226dedefbb229`  
		Last Modified: Tue, 12 Dec 2023 22:10:24 GMT  
		Size: 2.8 MB (2761045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2682a06d9f91bef66466bcb1b37715dc344282ac9f062ffff8405cf448d71f51`  
		Last Modified: Tue, 12 Dec 2023 22:10:23 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982a61382f7fcec3d428935d516ac99bf603d105e72ebe0c2952b860f329675f`  
		Last Modified: Tue, 12 Dec 2023 22:10:22 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:746af38a5ce0f5938bfe599dca0bb89e7a31717e478a32976dff78f8c1c53f4c`  
		Last Modified: Tue, 12 Dec 2023 22:19:54 GMT  
		Size: 11.8 MB (11830414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7782f5b0320e7f57bafe4e470b6ffb0c0f59cc8fcf3e988e5c14a9df2cc2e57b`  
		Last Modified: Tue, 12 Dec 2023 22:19:53 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85b9eb869aded52d67714e7a5fed3ac15fc4abdb45672ca67a2844f10e121f9`  
		Last Modified: Sat, 16 Dec 2023 03:41:08 GMT  
		Size: 11.4 MB (11423092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a4e9127c358a27c7a91ed65156f049a3bebf1357495933e23bbf2e0e0c12f9`  
		Last Modified: Sat, 16 Dec 2023 03:41:06 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ffc994f430ddf16b4a7d4209defa40b865a31159432e8eb7b681fe9fcf55cf`  
		Last Modified: Sat, 16 Dec 2023 03:41:06 GMT  
		Size: 19.1 KB (19128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1e9e2d8f33076cc9758b6909fd8d8a9f7cf339bd94461890f3b4447c372d77`  
		Last Modified: Sat, 16 Dec 2023 03:41:05 GMT  
		Size: 8.9 KB (8878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ff170882947dc2e7042fef6562ac3b77d75e644545f3c61cf648253e3f3b6b`  
		Last Modified: Sat, 16 Dec 2023 04:50:34 GMT  
		Size: 1.2 MB (1208494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4f19fbbbb70995409c881fec286eb60df2f092b9a0e62dbfd13211b284733ca`  
		Last Modified: Sat, 16 Dec 2023 04:50:33 GMT  
		Size: 8.5 MB (8484648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48a17c30e6ea10026ed469f4065705792097364baf6b637bd34a55c03caedc20`  
		Last Modified: Sat, 16 Dec 2023 04:50:31 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d7b8bccd5bfc37b7ebe21ea88ad2d435512361d532f06efab44f4afd307af08`  
		Last Modified: Sat, 16 Dec 2023 04:50:31 GMT  
		Size: 27.3 KB (27335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f35daf2358f575455b726b7808299c73947f0bc37e7b7ef6e6a40fddbdbc345c`  
		Last Modified: Sat, 16 Dec 2023 04:50:39 GMT  
		Size: 27.1 MB (27132141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d960c15ff97e9729733f9e738ffaa06a50d95ff7506f2fd83396ed781f2f142b`  
		Last Modified: Sat, 16 Dec 2023 04:50:32 GMT  
		Size: 2.1 KB (2077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:4-fpm-alpine` - linux; arm variant v7

```console
$ docker pull monica@sha256:6a8cf0c8300cd4128a6681fc06cc69416ca1d4524279cb438980ebef4530938c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64653907 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ca325f29afa82853ebc18c1690d886962557015238c14c06404cff8a6506e2b`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 08 Dec 2023 01:57:20 GMT
ADD file:13b9291053208eec61cd7c97bac2fa154380ad8d10182567763eea3e10c5882f in / 
# Fri, 08 Dec 2023 01:57:20 GMT
CMD ["/bin/sh"]
# Tue, 12 Dec 2023 20:17:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 12 Dec 2023 20:17:48 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		openssl 		tar 		xz
# Tue, 12 Dec 2023 20:17:49 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 12 Dec 2023 20:17:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Dec 2023 20:17:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 12 Dec 2023 20:17:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Dec 2023 20:17:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Dec 2023 20:17:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Dec 2023 21:55:39 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 12 Dec 2023 22:16:01 GMT
ENV PHP_VERSION=8.1.26
# Tue, 12 Dec 2023 22:16:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.26.tar.xz.asc
# Tue, 12 Dec 2023 22:16:01 GMT
ENV PHP_SHA256=17f87133596449327451ad4b8d9911bfaea59ff5109f3a6f2bb679f967a8ea0f
# Tue, 12 Dec 2023 22:16:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 12 Dec 2023 22:16:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 16 Dec 2023 05:53:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 		PHP_BUILD_PROVIDER='https://github.com/docker-library/php' 		PHP_UNAME='Linux - Docker' 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 16 Dec 2023 05:53:09 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 16 Dec 2023 05:53:10 GMT
RUN docker-php-ext-enable sodium
# Sat, 16 Dec 2023 05:53:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 16 Dec 2023 05:53:11 GMT
WORKDIR /var/www/html
# Sat, 16 Dec 2023 05:53:11 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 16 Dec 2023 05:53:11 GMT
STOPSIGNAL SIGQUIT
# Sat, 16 Dec 2023 05:53:11 GMT
EXPOSE 9000
# Sat, 16 Dec 2023 05:53:11 GMT
CMD ["php-fpm"]
# Sat, 16 Dec 2023 08:35:19 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 16 Dec 2023 08:35:20 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 16 Dec 2023 08:36:55 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libpq-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         pdo_pgsql         soap     ;     pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-6.0.2;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 16 Dec 2023 08:36:56 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '* * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 16 Dec 2023 08:36:56 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 16 Dec 2023 08:36:56 GMT
ENV PHP_MEMORY_LIMIT=512M PHP_UPLOAD_LIMIT=512M
# Sat, 16 Dec 2023 08:36:57 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > $PHP_INI_DIR/conf.d/limits.ini;
# Sat, 16 Dec 2023 08:36:57 GMT
WORKDIR /var/www/html
# Sat, 16 Dec 2023 08:36:57 GMT
ENV MONICA_VERSION=v4.0.0
# Sat, 16 Dec 2023 08:36:57 GMT
LABEL org.opencontainers.image.revision=e1a3e1315b1a92a5ff0ccab6c22ba9ded77a599e org.opencontainers.image.version=v4.0.0
# Sat, 16 Dec 2023 08:37:08 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 16 Dec 2023 08:37:09 GMT
COPY multi:84468128947ba1749e6048b0956ef2297175650942a70e8e8bc5df81159d8cc7 in /usr/local/bin/ 
# Sat, 16 Dec 2023 08:37:09 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 16 Dec 2023 08:37:09 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:1086c24c41097f090ce847d192c11307e1715eeb563a2cf4f410b2a199ae1942`  
		Last Modified: Fri, 08 Dec 2023 01:57:36 GMT  
		Size: 2.9 MB (2918701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fcdc554dd7b708317247ba5731b0d76bc06dc68a48af57f662820d33c665cc`  
		Last Modified: Tue, 12 Dec 2023 22:36:17 GMT  
		Size: 2.6 MB (2608664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4717604343f2899832c4417228ef3cdb02080f72378a4152eb72083f09c96e`  
		Last Modified: Tue, 12 Dec 2023 22:36:15 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe0a6a05c32e2329e654bc633b417da36b7c74ed6bf626231bf0e900f912838e`  
		Last Modified: Tue, 12 Dec 2023 22:36:15 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11edfcc10f2367a8418ab776a8b19f671127314b7e7c636f6d94ff65d66744f3`  
		Last Modified: Tue, 12 Dec 2023 22:47:36 GMT  
		Size: 11.8 MB (11830409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:485894dc4fc84a0916f46823588fdcb87b39105be32fefa32e62f0b412a15660`  
		Last Modified: Tue, 12 Dec 2023 22:47:35 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:755d7127d30668e20c80952128294bf0ea3a25efe9b4d366a04d866415584cea`  
		Last Modified: Sat, 16 Dec 2023 06:30:23 GMT  
		Size: 10.7 MB (10715079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f400e60b1e33939aed2aab1ba35264d09a8a9d3ff8144a4924eeb00421f711c`  
		Last Modified: Sat, 16 Dec 2023 06:30:20 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:602f628d8045a8af7336e4f6366a42fc1ec003d226efbb0cc63ec7d643a40b56`  
		Last Modified: Sat, 16 Dec 2023 06:30:21 GMT  
		Size: 19.1 KB (19106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb019a95cc0dd536851ac3b544a9dce8710f90e88ff962786b999560cd7502c`  
		Last Modified: Sat, 16 Dec 2023 06:30:21 GMT  
		Size: 8.9 KB (8880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36020f4649229c9ac53697bef9c319f7e3640a45697d2e9b3446a9a25ba2663`  
		Last Modified: Sat, 16 Dec 2023 08:38:20 GMT  
		Size: 1.1 MB (1087949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19f9ffdf0c83d02603e9c2e059eb7ff8bc1ab0783c6c4801dd2eaeac1e94c57`  
		Last Modified: Sat, 16 Dec 2023 08:38:19 GMT  
		Size: 8.3 MB (8298926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec53c49c0d32ef675c1bb775e422fcfce64cb40297a7fb034816f8e545bbd257`  
		Last Modified: Sat, 16 Dec 2023 08:38:18 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1204f8dd1459be532a9d1af255c7980d4db61a6f7c8d76ed2f721eabdc64e8bc`  
		Last Modified: Sat, 16 Dec 2023 08:38:17 GMT  
		Size: 27.3 KB (27300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f00ce77d6c2247b434d150d3155b6c3f6a0ea9cbe14e9a5744245f1adc27cfb`  
		Last Modified: Sat, 16 Dec 2023 08:38:25 GMT  
		Size: 27.1 MB (27132127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a29be67fd313122d2a8f998e788550fc580a23c1d59fb5c8bef07d5995766a`  
		Last Modified: Sat, 16 Dec 2023 08:38:17 GMT  
		Size: 2.1 KB (2076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:4-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull monica@sha256:e12b54ac28e091f1da4b1b07fc21e76b713396949af7c7771458d8538a54b67f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68106375 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4def4cc535dd245a6d720a5d1fae6409f51be248081235936d434dd8e20a55c0`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 08 Dec 2023 01:39:30 GMT
ADD file:8182c73f869a899cf624a59c400acb8226776d15e4d3a0d240a94e65340540d0 in / 
# Fri, 08 Dec 2023 01:39:30 GMT
CMD ["/bin/sh"]
# Tue, 12 Dec 2023 20:09:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 12 Dec 2023 20:09:53 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		openssl 		tar 		xz
# Tue, 12 Dec 2023 20:09:54 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 12 Dec 2023 20:09:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Dec 2023 20:09:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 12 Dec 2023 20:09:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Dec 2023 20:09:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Dec 2023 20:09:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Dec 2023 22:05:06 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 12 Dec 2023 22:33:14 GMT
ENV PHP_VERSION=8.1.26
# Tue, 12 Dec 2023 22:33:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.26.tar.xz.asc
# Tue, 12 Dec 2023 22:33:14 GMT
ENV PHP_SHA256=17f87133596449327451ad4b8d9911bfaea59ff5109f3a6f2bb679f967a8ea0f
# Tue, 12 Dec 2023 22:33:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 12 Dec 2023 22:33:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 16 Dec 2023 05:37:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 		PHP_BUILD_PROVIDER='https://github.com/docker-library/php' 		PHP_UNAME='Linux - Docker' 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 16 Dec 2023 05:37:42 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 16 Dec 2023 05:37:43 GMT
RUN docker-php-ext-enable sodium
# Sat, 16 Dec 2023 05:37:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 16 Dec 2023 05:37:43 GMT
WORKDIR /var/www/html
# Sat, 16 Dec 2023 05:37:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 16 Dec 2023 05:37:43 GMT
STOPSIGNAL SIGQUIT
# Sat, 16 Dec 2023 05:37:43 GMT
EXPOSE 9000
# Sat, 16 Dec 2023 05:37:43 GMT
CMD ["php-fpm"]
# Sat, 16 Dec 2023 08:47:11 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 16 Dec 2023 08:47:13 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 16 Dec 2023 08:48:37 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libpq-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         pdo_pgsql         soap     ;     pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-6.0.2;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 16 Dec 2023 08:48:37 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '* * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 16 Dec 2023 08:48:37 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 16 Dec 2023 08:48:37 GMT
ENV PHP_MEMORY_LIMIT=512M PHP_UPLOAD_LIMIT=512M
# Sat, 16 Dec 2023 08:48:38 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > $PHP_INI_DIR/conf.d/limits.ini;
# Sat, 16 Dec 2023 08:48:38 GMT
WORKDIR /var/www/html
# Sat, 16 Dec 2023 08:48:38 GMT
ENV MONICA_VERSION=v4.0.0
# Sat, 16 Dec 2023 08:48:38 GMT
LABEL org.opencontainers.image.revision=e1a3e1315b1a92a5ff0ccab6c22ba9ded77a599e org.opencontainers.image.version=v4.0.0
# Sat, 16 Dec 2023 08:48:47 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 16 Dec 2023 08:48:48 GMT
COPY multi:84468128947ba1749e6048b0956ef2297175650942a70e8e8bc5df81159d8cc7 in /usr/local/bin/ 
# Sat, 16 Dec 2023 08:48:48 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 16 Dec 2023 08:48:48 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c303524923177661067f7eb378c3dd5277088c2676ebd1cd78e68397bb80fdbf`  
		Last Modified: Fri, 08 Dec 2023 01:39:48 GMT  
		Size: 3.3 MB (3347794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95a19b0853c69aaf4e0a33f42601f1bddea728304bef39e2fc08f66f3d518576`  
		Last Modified: Tue, 12 Dec 2023 23:00:29 GMT  
		Size: 2.8 MB (2810204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872ba87116831a71587816ab8564d1a2b7137e1163524eb7e5abf40966e6882c`  
		Last Modified: Tue, 12 Dec 2023 23:00:28 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3a9508fcdd73dc8c678f841adc3269e9919da38f14917ddaa2162b636d4661c`  
		Last Modified: Tue, 12 Dec 2023 23:00:28 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea00c155286cb0f4427f4b0477fb5cda5a86b42fb52143750fe98b2ed6d19f24`  
		Last Modified: Tue, 12 Dec 2023 23:11:27 GMT  
		Size: 11.8 MB (11830404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d38b47a9c3d181ccf037f8a2955645ed430d0f579dcf6e961730081e8b619d`  
		Last Modified: Tue, 12 Dec 2023 23:11:26 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd536961880b685d38540bab1b9c8b31015c155d346e07d6ecf760d1598a67aa`  
		Last Modified: Sat, 16 Dec 2023 06:15:55 GMT  
		Size: 12.6 MB (12646037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96b92208712c7ba8a6894998d492fc0f9ad42eef3cb48ca7b60d399ab5a370b4`  
		Last Modified: Sat, 16 Dec 2023 06:15:54 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb95dbc9d6216d34d916fcd5bd0483976465d515de096c77fe617d806bad18e`  
		Last Modified: Sat, 16 Dec 2023 06:15:53 GMT  
		Size: 19.1 KB (19075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6d1c806e30d41404bdb4f476f6040813995d4a811ddea248db4ad09d49f765`  
		Last Modified: Sat, 16 Dec 2023 06:15:54 GMT  
		Size: 8.9 KB (8879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015a6b7bfb44c5afc83bb26fc36a269fa56d0e4b9a29c1e7448d3bc4981806d5`  
		Last Modified: Sat, 16 Dec 2023 08:50:05 GMT  
		Size: 1.3 MB (1251004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41beb797f47b140a544eb2563be158582cf9b229a700b37d62279628def29f5`  
		Last Modified: Sat, 16 Dec 2023 08:50:04 GMT  
		Size: 9.0 MB (9026786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f3f9c390b7ff6d3c735380464c44b97bb4c20e98c3bed5930f7ef8c84d7986`  
		Last Modified: Sat, 16 Dec 2023 08:50:03 GMT  
		Size: 218.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9ae86dd3bb8436da7906dc368b0e423dc6bcddc2875015aa37a5c7df366ed0a`  
		Last Modified: Sat, 16 Dec 2023 08:50:03 GMT  
		Size: 27.3 KB (27290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2605bdc8dc91021483dee118292f769bf87555375314066786b1fe0d2490d7cb`  
		Last Modified: Sat, 16 Dec 2023 08:50:08 GMT  
		Size: 27.1 MB (27132129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56334ac6d5a19ee56f423f0cd80d6d304f1fcdbf13268496f18982e352ce9759`  
		Last Modified: Sat, 16 Dec 2023 08:50:03 GMT  
		Size: 2.1 KB (2078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:4-fpm-alpine` - linux; 386

```console
$ docker pull monica@sha256:77eae710d7eea5e6cae95975af469e87ae35f560d82f6b29996328eced7b00c9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68340738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b89984b766cc07dc4bdd3b12b82acb5333552c39733609ac321fd5f6dfd87e5`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 08 Dec 2023 01:38:25 GMT
ADD file:bd52540f209ba362654d795d7893669c819d35011a16f9f319301727a33b3bd9 in / 
# Fri, 08 Dec 2023 01:38:25 GMT
CMD ["/bin/sh"]
# Tue, 12 Dec 2023 20:00:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 12 Dec 2023 20:00:31 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		openssl 		tar 		xz
# Tue, 12 Dec 2023 20:00:32 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 12 Dec 2023 20:00:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Dec 2023 20:00:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 12 Dec 2023 20:00:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Dec 2023 20:00:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Dec 2023 20:00:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Dec 2023 23:05:55 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 12 Dec 2023 23:51:49 GMT
ENV PHP_VERSION=8.1.26
# Tue, 12 Dec 2023 23:51:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.26.tar.xz.asc
# Tue, 12 Dec 2023 23:51:49 GMT
ENV PHP_SHA256=17f87133596449327451ad4b8d9911bfaea59ff5109f3a6f2bb679f967a8ea0f
# Tue, 12 Dec 2023 23:51:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 12 Dec 2023 23:51:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 13 Dec 2023 00:04:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 13 Dec 2023 00:04:48 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 13 Dec 2023 00:04:49 GMT
RUN docker-php-ext-enable sodium
# Wed, 13 Dec 2023 00:04:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 13 Dec 2023 00:04:49 GMT
WORKDIR /var/www/html
# Wed, 13 Dec 2023 00:04:50 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 13 Dec 2023 00:04:50 GMT
STOPSIGNAL SIGQUIT
# Wed, 13 Dec 2023 00:04:50 GMT
EXPOSE 9000
# Wed, 13 Dec 2023 00:04:50 GMT
CMD ["php-fpm"]
# Wed, 13 Dec 2023 02:43:14 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Wed, 13 Dec 2023 02:43:15 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Wed, 13 Dec 2023 02:45:37 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libpq-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         pdo_pgsql         soap     ;     pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-6.0.2;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Wed, 13 Dec 2023 02:45:37 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '* * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Wed, 13 Dec 2023 02:45:37 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Wed, 13 Dec 2023 02:45:37 GMT
ENV PHP_MEMORY_LIMIT=512M PHP_UPLOAD_LIMIT=512M
# Wed, 13 Dec 2023 02:45:39 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > $PHP_INI_DIR/conf.d/limits.ini;
# Wed, 13 Dec 2023 02:45:39 GMT
WORKDIR /var/www/html
# Wed, 13 Dec 2023 02:45:39 GMT
ENV MONICA_VERSION=v4.0.0
# Wed, 13 Dec 2023 02:45:39 GMT
LABEL org.opencontainers.image.revision=e1a3e1315b1a92a5ff0ccab6c22ba9ded77a599e org.opencontainers.image.version=v4.0.0
# Wed, 13 Dec 2023 02:45:53 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Wed, 13 Dec 2023 02:45:55 GMT
COPY multi:84468128947ba1749e6048b0956ef2297175650942a70e8e8bc5df81159d8cc7 in /usr/local/bin/ 
# Wed, 13 Dec 2023 02:45:55 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Wed, 13 Dec 2023 02:45:55 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:9acd8b4c9d4385585f74dabb4bc6b3351888710ae37ec5dbd9ea950281b8f9bb`  
		Last Modified: Fri, 08 Dec 2023 01:38:43 GMT  
		Size: 3.2 MB (3244115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e35c853c51aa63c9f21d6c91fa6948b8160ed6a90764a48e7b1891c38e016590`  
		Last Modified: Wed, 13 Dec 2023 00:34:22 GMT  
		Size: 2.8 MB (2820917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6af7fb9ea0ea850c653027fa7b1b18f1d4c405aade35df3c3ec2151bb8251f`  
		Last Modified: Wed, 13 Dec 2023 00:34:21 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9233674231d3f63e2099e1d4253bf67fd488ef3d4fcd72e3e741ffb7a41f385e`  
		Last Modified: Wed, 13 Dec 2023 00:34:20 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12772cd933eedd51d4e706b490493ce90ee16685bd92a289e1c79799d64b3cbd`  
		Last Modified: Wed, 13 Dec 2023 00:46:51 GMT  
		Size: 11.8 MB (11830409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2f0df9748646b40822395af55981f06180b84d289ab31faf45012027039212a`  
		Last Modified: Wed, 13 Dec 2023 00:46:50 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f446f96deb152d1de19aabc0dac5282e4d0603726d58b0f65aaad32b5e21223`  
		Last Modified: Wed, 13 Dec 2023 00:47:22 GMT  
		Size: 12.9 MB (12921996 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b2a4735b515cb4de8548e21b6f3e48406f222fc26d36faa1ccbe5938f35210e`  
		Last Modified: Wed, 13 Dec 2023 00:47:19 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ca9b69c793b0c4e53bf00d8ca1d5ef8cf69a101370244a72351839bde5c7ea`  
		Last Modified: Wed, 13 Dec 2023 00:47:19 GMT  
		Size: 19.3 KB (19291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6f5b1abfe86c12aefdf96ca1439ea04e971f35856cab03340bb9cb2e630180`  
		Last Modified: Wed, 13 Dec 2023 00:47:19 GMT  
		Size: 8.9 KB (8879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e993ad0cfb8b325ee9b498ad9244c8ba20c61567ae29194f8526012102b96f2c`  
		Last Modified: Wed, 13 Dec 2023 02:46:59 GMT  
		Size: 1.2 MB (1190349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cafa55940dd493ff93a6813706fff73533507498588d09a2f1dd4fc8c4040ec`  
		Last Modified: Wed, 13 Dec 2023 02:46:58 GMT  
		Size: 9.1 MB (9138533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0bff0ab32e0049f5e6c5bbe752ec15a43cfc73e7a64e4c000c256fd3ea6ef61`  
		Last Modified: Wed, 13 Dec 2023 02:46:56 GMT  
		Size: 217.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f407132365f78fbd24b54252b371a01e133b706bf4cb0552012f52078785a87`  
		Last Modified: Wed, 13 Dec 2023 02:46:56 GMT  
		Size: 27.3 KB (27330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f60bb55842681a7c44521d8cd4498df55262423f27ef29eda5d67dd2aaf2e00`  
		Last Modified: Wed, 13 Dec 2023 02:47:06 GMT  
		Size: 27.1 MB (27132144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b2dfbfc1872a4747b635330b8c34adc7f523355f45c53730a16f25e67f4cf6`  
		Last Modified: Wed, 13 Dec 2023 02:46:56 GMT  
		Size: 2.1 KB (2080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:4-fpm-alpine` - linux; ppc64le

```console
$ docker pull monica@sha256:864273c154554900d89ca8cd7980ce125f0bebc9172ac79ed927c68e3ac4f91b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68960398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b313aea92f1549472e7e7ece7d6c320b0838a106993e79104163db9e1300c87`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 08 Dec 2023 01:22:51 GMT
ADD file:052421189f8d269382daaaa8beb63c687e4d8ca908c421abdce53bcc627a40b4 in / 
# Fri, 08 Dec 2023 01:22:51 GMT
CMD ["/bin/sh"]
# Tue, 12 Dec 2023 20:31:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 12 Dec 2023 20:31:18 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		openssl 		tar 		xz
# Tue, 12 Dec 2023 20:31:19 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 12 Dec 2023 20:31:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Dec 2023 20:31:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 12 Dec 2023 20:31:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Dec 2023 20:31:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Dec 2023 20:31:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Dec 2023 22:00:30 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 12 Dec 2023 22:21:51 GMT
ENV PHP_VERSION=8.1.26
# Tue, 12 Dec 2023 22:21:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.26.tar.xz.asc
# Tue, 12 Dec 2023 22:21:51 GMT
ENV PHP_SHA256=17f87133596449327451ad4b8d9911bfaea59ff5109f3a6f2bb679f967a8ea0f
# Tue, 12 Dec 2023 22:21:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 12 Dec 2023 22:21:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 16 Dec 2023 05:46:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 		PHP_BUILD_PROVIDER='https://github.com/docker-library/php' 		PHP_UNAME='Linux - Docker' 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 16 Dec 2023 05:46:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 16 Dec 2023 05:46:36 GMT
RUN docker-php-ext-enable sodium
# Sat, 16 Dec 2023 05:46:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 16 Dec 2023 05:46:36 GMT
WORKDIR /var/www/html
# Sat, 16 Dec 2023 05:46:38 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 16 Dec 2023 05:46:38 GMT
STOPSIGNAL SIGQUIT
# Sat, 16 Dec 2023 05:46:38 GMT
EXPOSE 9000
# Sat, 16 Dec 2023 05:46:39 GMT
CMD ["php-fpm"]
# Sat, 16 Dec 2023 09:50:52 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 16 Dec 2023 09:50:55 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 16 Dec 2023 09:52:58 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libpq-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         pdo_pgsql         soap     ;     pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-6.0.2;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 16 Dec 2023 09:53:00 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '* * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 16 Dec 2023 09:53:01 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 16 Dec 2023 09:53:01 GMT
ENV PHP_MEMORY_LIMIT=512M PHP_UPLOAD_LIMIT=512M
# Sat, 16 Dec 2023 09:53:03 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > $PHP_INI_DIR/conf.d/limits.ini;
# Sat, 16 Dec 2023 09:53:04 GMT
WORKDIR /var/www/html
# Sat, 16 Dec 2023 09:53:05 GMT
ENV MONICA_VERSION=v4.0.0
# Sat, 16 Dec 2023 09:53:05 GMT
LABEL org.opencontainers.image.revision=e1a3e1315b1a92a5ff0ccab6c22ba9ded77a599e org.opencontainers.image.version=v4.0.0
# Sat, 16 Dec 2023 09:53:21 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 16 Dec 2023 09:53:24 GMT
COPY multi:84468128947ba1749e6048b0956ef2297175650942a70e8e8bc5df81159d8cc7 in /usr/local/bin/ 
# Sat, 16 Dec 2023 09:53:25 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 16 Dec 2023 09:53:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:243ac51c334a47917a84be93e972ee6378987e9b3b917a5a8df29025e161c1f3`  
		Last Modified: Fri, 08 Dec 2023 01:23:14 GMT  
		Size: 3.4 MB (3358233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e89935d2f947cbd3585545f82639d347027ef82fbbf413f8684101953ea74bd6`  
		Last Modified: Tue, 12 Dec 2023 22:41:51 GMT  
		Size: 2.8 MB (2838539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b208bea042d5cdcbe6436f88d2f7ea51b03a91df91ae099118f57b644b87bdb2`  
		Last Modified: Tue, 12 Dec 2023 22:41:50 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dcb83a14858379fd485cb474c02417cd209b148b775365e9bae3ab90f5fe798`  
		Last Modified: Tue, 12 Dec 2023 22:41:50 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f42fdc52f2aa69151f0cf954fe506285475267dbbce60c064e5e6bece02a60a`  
		Last Modified: Tue, 12 Dec 2023 22:54:21 GMT  
		Size: 11.8 MB (11830405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147c2ba2e1eace70e1e4ae9e650821725c5cf33b8e493eb31ce57ad401770225`  
		Last Modified: Tue, 12 Dec 2023 22:54:20 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475096f78f89d01ccbfc58b757fd00dacaf264a008bc4fdb8e8fed7e0fdaf6a8`  
		Last Modified: Sat, 16 Dec 2023 06:27:04 GMT  
		Size: 13.0 MB (13038493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24b977ecab04bdb5a75c9dae3b26c49dd01d77c9dcff7af72c49e5d0424642e2`  
		Last Modified: Sat, 16 Dec 2023 06:27:01 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f89f2ad0991fd7ad6e6c5b1ce3bc6354643baaee7f9f598fb29cf52e290ee0`  
		Last Modified: Sat, 16 Dec 2023 06:27:02 GMT  
		Size: 19.1 KB (19095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b9d9e5745ea6ef9cb129d201e15c4d311cd58b61331aa596225ccc5e0c59e8d`  
		Last Modified: Sat, 16 Dec 2023 06:27:02 GMT  
		Size: 8.9 KB (8879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcdb88a3987c9bd260e5652420ed84c0686a5f60c4a550c18164a5d842b34a2`  
		Last Modified: Sat, 16 Dec 2023 09:54:44 GMT  
		Size: 1.2 MB (1246831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1811760a7f3a5f46feeffd68df4d0444c840ff5b9ad385c99b85f80aa882839`  
		Last Modified: Sat, 16 Dec 2023 09:54:43 GMT  
		Size: 9.5 MB (9453723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67867d5d522ba5de3eb572261dd42030987b38ce86a5c25c3795b5f287ba397`  
		Last Modified: Sat, 16 Dec 2023 09:54:41 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4570d5b7717858c5c78c6a0396b14b8189fbadfc40da31ae8ff2880d948eb1`  
		Last Modified: Sat, 16 Dec 2023 09:54:41 GMT  
		Size: 27.3 KB (27312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab828a8afe5d3eca4575424421ac4665b2732b074ec391be8ab01bc5fe47b75`  
		Last Modified: Sat, 16 Dec 2023 09:54:48 GMT  
		Size: 27.1 MB (27132111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cf2ab93938d6c2d96ad6a871253548fa156bb1560235ed1f7a0f17e01c0fc0`  
		Last Modified: Sat, 16 Dec 2023 09:54:41 GMT  
		Size: 2.1 KB (2081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:4-fpm-alpine` - linux; s390x

```console
$ docker pull monica@sha256:3b458ab6ff8c3886b9c77d4d3f4b829a77b8fa811a499833be3315a25969a5cd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.1 MB (68082291 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab959e86255faeed31417771e9e7cbe7085292a39e84de382a9ffcab7101603`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 08 Dec 2023 01:41:50 GMT
ADD file:47e0982fc3ae485c06d46f3c0022afd39ed7ec95fe755c2391e6b0cfcae65dfc in / 
# Fri, 08 Dec 2023 01:41:51 GMT
CMD ["/bin/sh"]
# Tue, 12 Dec 2023 19:58:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 12 Dec 2023 19:58:25 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		openssl 		tar 		xz
# Tue, 12 Dec 2023 19:58:25 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 12 Dec 2023 19:58:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 12 Dec 2023 19:58:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 12 Dec 2023 19:58:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Dec 2023 19:58:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 12 Dec 2023 19:58:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 12 Dec 2023 21:24:49 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 12 Dec 2023 21:45:58 GMT
ENV PHP_VERSION=8.1.26
# Tue, 12 Dec 2023 21:45:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.26.tar.xz.asc
# Tue, 12 Dec 2023 21:45:58 GMT
ENV PHP_SHA256=17f87133596449327451ad4b8d9911bfaea59ff5109f3a6f2bb679f967a8ea0f
# Tue, 12 Dec 2023 21:46:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 12 Dec 2023 21:46:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 16 Dec 2023 04:35:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 		PHP_BUILD_PROVIDER='https://github.com/docker-library/php' 		PHP_UNAME='Linux - Docker' 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 16 Dec 2023 04:35:01 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 16 Dec 2023 04:35:02 GMT
RUN docker-php-ext-enable sodium
# Sat, 16 Dec 2023 04:35:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 16 Dec 2023 04:35:03 GMT
WORKDIR /var/www/html
# Sat, 16 Dec 2023 04:35:03 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 16 Dec 2023 04:35:04 GMT
STOPSIGNAL SIGQUIT
# Sat, 16 Dec 2023 04:35:04 GMT
EXPOSE 9000
# Sat, 16 Dec 2023 04:35:04 GMT
CMD ["php-fpm"]
# Sat, 16 Dec 2023 06:58:46 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 16 Dec 2023 06:58:47 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 16 Dec 2023 07:00:06 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libpq-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         pdo_pgsql         soap     ;     pecl install APCu-5.1.22;     pecl install memcached-3.2.0;     pecl install redis-6.0.2;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 16 Dec 2023 07:00:08 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '* * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 16 Dec 2023 07:00:08 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 16 Dec 2023 07:00:08 GMT
ENV PHP_MEMORY_LIMIT=512M PHP_UPLOAD_LIMIT=512M
# Sat, 16 Dec 2023 07:00:09 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         {         echo 'memory_limit=${PHP_MEMORY_LIMIT}';         echo 'upload_max_filesize=${PHP_UPLOAD_LIMIT}';         echo 'post_max_size=${PHP_UPLOAD_LIMIT}';     } > $PHP_INI_DIR/conf.d/limits.ini;
# Sat, 16 Dec 2023 07:00:10 GMT
WORKDIR /var/www/html
# Sat, 16 Dec 2023 07:00:10 GMT
ENV MONICA_VERSION=v4.0.0
# Sat, 16 Dec 2023 07:00:10 GMT
LABEL org.opencontainers.image.revision=e1a3e1315b1a92a5ff0ccab6c22ba9ded77a599e org.opencontainers.image.version=v4.0.0
# Sat, 16 Dec 2023 07:00:24 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkp://keyserver.ubuntu.com:80 --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 16 Dec 2023 07:00:31 GMT
COPY multi:84468128947ba1749e6048b0956ef2297175650942a70e8e8bc5df81159d8cc7 in /usr/local/bin/ 
# Sat, 16 Dec 2023 07:00:31 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 16 Dec 2023 07:00:31 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:0fca3ee44ced87b7184bc23390283fdf10cfae0e844a25b785dd11c463815227`  
		Last Modified: Fri, 08 Dec 2023 01:42:30 GMT  
		Size: 3.2 MB (3242332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e0180a7268e169fa6dd82fc04f9270dbd4fe716cf09b03fc82f84618025bad4`  
		Last Modified: Tue, 12 Dec 2023 22:07:16 GMT  
		Size: 2.9 MB (2937974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ecaefbf268f4b1e4d9f16c5d67523f3b76e72db0c3fc7a2f3fb6fd7fbdec547`  
		Last Modified: Tue, 12 Dec 2023 22:07:16 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5f0d18e8f1067fcb105dea2ad180f140d138c6d99310025696d1aaa322017db`  
		Last Modified: Tue, 12 Dec 2023 22:07:16 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4add150319cb3d9214bd03b3e2815780d385668eed8c0c981e0c79667b9763`  
		Last Modified: Tue, 12 Dec 2023 22:15:12 GMT  
		Size: 11.8 MB (11830412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d11bc53bc80bbfdee4134007c2ed1071b049bb9877939e8686a797adf33f83e6`  
		Last Modified: Tue, 12 Dec 2023 22:15:11 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80448e61d4ecc1eee3e6393d4eddb262cf230e1e939d476bb3fc790cbedcd21`  
		Last Modified: Sat, 16 Dec 2023 05:05:12 GMT  
		Size: 12.3 MB (12320539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ffdaf693c5c82e5c287d87c65e02e09b28b386e02931b0dc7dd9541c3293f8`  
		Last Modified: Sat, 16 Dec 2023 05:05:10 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e00d882a3b04a38825b1562ea2d5c63da782e83f45982f0d3a6aa0798db97b`  
		Last Modified: Sat, 16 Dec 2023 05:05:10 GMT  
		Size: 19.1 KB (19104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e48cadb218c9f2793d8818c5516b9f6d98b0b5ec89eed0ab347b24066d938d2f`  
		Last Modified: Sat, 16 Dec 2023 05:05:10 GMT  
		Size: 8.9 KB (8877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4777025f5e388711613da27a6e505b3f0369ebf892bd4b99fabb1f7160acb83`  
		Last Modified: Sat, 16 Dec 2023 07:01:23 GMT  
		Size: 1.2 MB (1227850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:488daa7ebab17a8a2c6d795aa8d6146f6ecb63c12a38e7d1a60e51c8642e85a7`  
		Last Modified: Sat, 16 Dec 2023 07:01:23 GMT  
		Size: 9.3 MB (9328973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d5ec23904011d75adb99dfb5930dbf10f4f99c3c7b32d0f074ef9e3e50ecf0e`  
		Last Modified: Sat, 16 Dec 2023 07:01:22 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4c2ed096975fda2b8c3392b9e3a8d1badb1dec50e20c0fd751353ffc08fd7d`  
		Last Modified: Sat, 16 Dec 2023 07:01:22 GMT  
		Size: 27.3 KB (27319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640c517b87534c534a63bb80b2b36c6e795b7714954430d432bf1aecce33a564`  
		Last Modified: Sat, 16 Dec 2023 07:01:28 GMT  
		Size: 27.1 MB (27132136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c199a71982fc39f019bcab92eccd9fd5a6d43ae2cb2286a540db101a0f0fd7ba`  
		Last Modified: Sat, 16 Dec 2023 07:01:22 GMT  
		Size: 2.1 KB (2078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
