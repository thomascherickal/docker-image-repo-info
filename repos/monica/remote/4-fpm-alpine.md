## `monica:4-fpm-alpine`

```console
$ docker pull monica@sha256:5532a12b3a37f17aa4daea58e305805842e544e6c2a20c97f6bd6349f380ced8
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
$ docker pull monica@sha256:3499d6551377e9284af11708a82f55249e60b719598ebeeca2b023e52294a337
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.6 MB (67591532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6b1fe74d843a495054610f098ec0b9079de7687958ab112718965d7f626bc8b`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:53:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 03:53:25 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 03:53:25 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 03:53:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 03:53:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 03:53:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 03:53:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 03:53:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 05:01:14 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 21 Oct 2023 05:36:08 GMT
ENV PHP_VERSION=8.1.24
# Sat, 21 Oct 2023 05:36:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Sat, 21 Oct 2023 05:36:08 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Sat, 21 Oct 2023 05:36:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 21 Oct 2023 05:36:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 21 Oct 2023 05:43:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 21 Oct 2023 05:43:13 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 21 Oct 2023 05:43:14 GMT
RUN docker-php-ext-enable sodium
# Sat, 21 Oct 2023 05:43:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 21 Oct 2023 05:43:14 GMT
WORKDIR /var/www/html
# Sat, 21 Oct 2023 05:43:15 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 21 Oct 2023 05:43:15 GMT
STOPSIGNAL SIGQUIT
# Sat, 21 Oct 2023 05:43:15 GMT
EXPOSE 9000
# Sat, 21 Oct 2023 05:43:15 GMT
CMD ["php-fpm"]
# Sat, 21 Oct 2023 08:50:19 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 21 Oct 2023 08:50:20 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 21 Oct 2023 08:51:44 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;     pecl install APCu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 21 Oct 2023 08:51:45 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 21 Oct 2023 08:51:45 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 21 Oct 2023 08:51:46 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Sat, 21 Oct 2023 08:51:46 GMT
WORKDIR /var/www/html
# Sat, 21 Oct 2023 08:51:46 GMT
ENV MONICA_VERSION=v4.0.0
# Sat, 21 Oct 2023 08:51:46 GMT
LABEL org.opencontainers.image.revision=e1a3e1315b1a92a5ff0ccab6c22ba9ded77a599e org.opencontainers.image.version=v4.0.0
# Sat, 21 Oct 2023 08:51:57 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 21 Oct 2023 08:51:58 GMT
COPY multi:84468128947ba1749e6048b0956ef2297175650942a70e8e8bc5df81159d8cc7 in /usr/local/bin/ 
# Sat, 21 Oct 2023 08:51:58 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 08:51:58 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61eb5622fa41e7d9451865eeadb9858807e2359c9787e86c9084078c65c7367f`  
		Last Modified: Sat, 21 Oct 2023 06:26:15 GMT  
		Size: 2.7 MB (2679351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587160738cca0d7e2afbad4e319bf69a2e5e51250de0bbb96546aa3a8754f814`  
		Last Modified: Sat, 21 Oct 2023 06:26:15 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802431d360de8be26d17059e07cf6636e5d549b0beeb9db464d3a916bc093afc`  
		Last Modified: Sat, 21 Oct 2023 06:26:15 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7085062ba3ba40cd28bbd072a2a50e16db279358a13cb2ed3c7e71d489e2199`  
		Last Modified: Sat, 21 Oct 2023 06:34:53 GMT  
		Size: 11.8 MB (11814630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a651b4b4c0cc4569ecabdb4eab3f659f8aeba397ccf4061525b890a62f649ac`  
		Last Modified: Sat, 21 Oct 2023 06:34:52 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db894a25d01a8b53d907bf247eb66611d3198924541b7b182d5ed2cd49fe3ef`  
		Last Modified: Sat, 21 Oct 2023 06:35:18 GMT  
		Size: 12.8 MB (12819536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b336af589b3bb3911cf33c6c84368e8eb4c12cae41a35012c589a3892b7211b`  
		Last Modified: Sat, 21 Oct 2023 06:35:16 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4115eecbdfe97b4a8fa974c86c40db3ecd1074423257d31ed666aad8204e55`  
		Last Modified: Sat, 21 Oct 2023 06:35:16 GMT  
		Size: 19.0 KB (18984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d7965c05f55ee119b4b52dca7cd6bf8d34f880347e37f7f8e6315ae4d98e0`  
		Last Modified: Sat, 21 Oct 2023 06:35:16 GMT  
		Size: 8.9 KB (8875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d548528a3bd7cd8f1ab58925abb4bc7588b0eaf4755a6d46d89a55f39cd5017`  
		Last Modified: Sat, 21 Oct 2023 08:55:48 GMT  
		Size: 1.1 MB (1139479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083d1d8e0343f75a2966b12d8d224edb9c8bcb6f34ca31b6a6ff222314e40191`  
		Last Modified: Sat, 21 Oct 2023 08:55:47 GMT  
		Size: 8.5 MB (8545377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d2fa9d3b09ca8d672b20ea822af51d602fba78cfaa11d7778d47e39d0ab5a4`  
		Last Modified: Sat, 21 Oct 2023 08:55:45 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c67c5c9b68b95afc778fc9a5cc3178a4bd53a1b51a56c453046495bf9275d96`  
		Last Modified: Sat, 21 Oct 2023 08:55:46 GMT  
		Size: 26.5 KB (26537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a521c907321e85d27f23c79602850b71acfc0cf4d769ea1246611b8b58c820b0`  
		Last Modified: Sat, 21 Oct 2023 08:55:52 GMT  
		Size: 27.1 MB (27130021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45ec45b6ad2b3e1bf646cca438404d7824b19a33af8a66145516955d1c9d656`  
		Last Modified: Sat, 21 Oct 2023 08:55:46 GMT  
		Size: 2.1 KB (2080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:4-fpm-alpine` - linux; arm variant v6

```console
$ docker pull monica@sha256:6c9707b7e4b4e1271c47672199477c3dd5ddd4621ba5a4dc85428fb7ffdf3c6e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.8 MB (65767547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71d33c11f41e747afce01fff315e85f984ad2905574b31f42033c86fd3fd9859`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:12:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 01:12:15 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 01:12:16 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 01:12:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 01:12:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 01:12:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:12:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:12:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 02:12:40 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 21 Oct 2023 02:41:07 GMT
ENV PHP_VERSION=8.1.24
# Sat, 21 Oct 2023 02:41:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Sat, 21 Oct 2023 02:41:07 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Sat, 21 Oct 2023 02:41:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 21 Oct 2023 02:41:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 21 Oct 2023 02:46:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 21 Oct 2023 02:46:52 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 21 Oct 2023 02:46:54 GMT
RUN docker-php-ext-enable sodium
# Sat, 21 Oct 2023 02:46:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 21 Oct 2023 02:46:54 GMT
WORKDIR /var/www/html
# Sat, 21 Oct 2023 02:46:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 21 Oct 2023 02:46:55 GMT
STOPSIGNAL SIGQUIT
# Sat, 21 Oct 2023 02:46:55 GMT
EXPOSE 9000
# Sat, 21 Oct 2023 02:46:55 GMT
CMD ["php-fpm"]
# Sat, 21 Oct 2023 04:07:16 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 21 Oct 2023 04:07:17 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 21 Oct 2023 04:08:44 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;     pecl install APCu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 21 Oct 2023 04:08:44 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 21 Oct 2023 04:08:44 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 21 Oct 2023 04:08:45 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Sat, 21 Oct 2023 04:08:45 GMT
WORKDIR /var/www/html
# Sat, 21 Oct 2023 04:08:45 GMT
ENV MONICA_VERSION=v4.0.0
# Sat, 21 Oct 2023 04:08:46 GMT
LABEL org.opencontainers.image.revision=e1a3e1315b1a92a5ff0ccab6c22ba9ded77a599e org.opencontainers.image.version=v4.0.0
# Sat, 21 Oct 2023 04:08:59 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 21 Oct 2023 04:09:00 GMT
COPY multi:84468128947ba1749e6048b0956ef2297175650942a70e8e8bc5df81159d8cc7 in /usr/local/bin/ 
# Sat, 21 Oct 2023 04:09:00 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 04:09:00 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e612e11521ddc11f4fbafd4815fd061e99bf827b9952ec407d3c976ea4237db`  
		Last Modified: Sat, 21 Oct 2023 03:21:10 GMT  
		Size: 2.7 MB (2685635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01946457dc0771f96a346d9812bad780b01a21b5e87a4574d8485c060782c4f1`  
		Last Modified: Sat, 21 Oct 2023 03:21:09 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db630a9f175c24d8d95bee24189d4d7e3c04d766b096001c7b8dd8cadb299ddd`  
		Last Modified: Sat, 21 Oct 2023 03:21:09 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402a538371c569dccb840dff705b76ec4c601fd7a3cf2fc9f8962201af98b0df`  
		Last Modified: Sat, 21 Oct 2023 03:29:20 GMT  
		Size: 11.8 MB (11814633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8113b4bd4520f8c5f4ca84e5a5d6d30ee7b9f9b75cbf9c151c4c14c5daf9671`  
		Last Modified: Sat, 21 Oct 2023 03:29:19 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6da9c4acf68d7105fe13c43c2c9b915839395e4b19076ab70b49360780d233d`  
		Last Modified: Sat, 21 Oct 2023 03:29:50 GMT  
		Size: 11.7 MB (11724179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e87c362b504575669d948c4a641f37b5be402db38158097cafa0628baf874c`  
		Last Modified: Sat, 21 Oct 2023 03:29:47 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9277213d3e3210071a0cca9402a53354043eb0d3db2c0994b32c47ca18985ac`  
		Last Modified: Sat, 21 Oct 2023 03:29:47 GMT  
		Size: 18.8 KB (18812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a0ddf97075f1b21820b5e0fafee4379deb9ab236fde8966f1ee27029d0ecc22`  
		Last Modified: Sat, 21 Oct 2023 03:29:47 GMT  
		Size: 8.9 KB (8878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b15ce3bfde9b52c65688ec351a002033a1e974033a2c9be0263ef086b7ade76`  
		Last Modified: Sat, 21 Oct 2023 04:09:18 GMT  
		Size: 1.2 MB (1192636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03139e62054af8c610b37f416d42319c2f5c1f9caacf9ae5b05261847eae077d`  
		Last Modified: Sat, 21 Oct 2023 04:09:17 GMT  
		Size: 8.0 MB (8014156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f6ff5703f66c7e3c427b5472347578cd81e5eac50759b6d56cac96509cd879`  
		Last Modified: Sat, 21 Oct 2023 04:09:15 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b6c0258d4304ab856d610b90ed187d656abe23329bd4aceaa460886d284978`  
		Last Modified: Sat, 21 Oct 2023 04:09:15 GMT  
		Size: 26.5 KB (26533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7e74181e5a07ae1116305aa4d8f0fc19fdfe6f3083b05296fac542c5988a70`  
		Last Modified: Sat, 21 Oct 2023 04:09:23 GMT  
		Size: 27.1 MB (27130024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397395f59e13d64c16c2a4d08f2da058572d48619b630648ad3aa0a48424d0d0`  
		Last Modified: Sat, 21 Oct 2023 04:09:15 GMT  
		Size: 2.1 KB (2076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:4-fpm-alpine` - linux; arm variant v7

```console
$ docker pull monica@sha256:13d5ee1091f9c9d0bb83e260d468bdce9bce026d6e12f012d8df3178cb097996
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.3 MB (64335670 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a033d3d2f9bba0c1e93764409ddedb8e21b0c88d2c4c13bc5471cc5c84ac5f74`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 28 Sep 2023 20:59:24 GMT
ADD file:61f54a318ad79861c6177783bb4c604412b5d952f45a9aa12ff97f4dccba7f73 in / 
# Thu, 28 Sep 2023 20:59:24 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:38:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 01:38:30 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 01:38:30 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 01:38:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 01:38:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 01:38:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:38:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:38:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 02:36:04 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 21 Oct 2023 03:05:14 GMT
ENV PHP_VERSION=8.1.24
# Sat, 21 Oct 2023 03:05:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Sat, 21 Oct 2023 03:05:14 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Sat, 21 Oct 2023 03:05:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 21 Oct 2023 03:05:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 21 Oct 2023 03:10:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 21 Oct 2023 03:10:59 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 21 Oct 2023 03:11:00 GMT
RUN docker-php-ext-enable sodium
# Sat, 21 Oct 2023 03:11:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 21 Oct 2023 03:11:01 GMT
WORKDIR /var/www/html
# Sat, 21 Oct 2023 03:11:02 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 21 Oct 2023 03:11:02 GMT
STOPSIGNAL SIGQUIT
# Sat, 21 Oct 2023 03:11:02 GMT
EXPOSE 9000
# Sat, 21 Oct 2023 03:11:02 GMT
CMD ["php-fpm"]
# Sat, 21 Oct 2023 04:54:34 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 21 Oct 2023 04:54:35 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 21 Oct 2023 04:55:59 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;     pecl install APCu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 21 Oct 2023 04:56:00 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 21 Oct 2023 04:56:00 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 21 Oct 2023 04:56:01 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Sat, 21 Oct 2023 04:56:01 GMT
WORKDIR /var/www/html
# Sat, 21 Oct 2023 04:56:01 GMT
ENV MONICA_VERSION=v4.0.0
# Sat, 21 Oct 2023 04:56:01 GMT
LABEL org.opencontainers.image.revision=e1a3e1315b1a92a5ff0ccab6c22ba9ded77a599e org.opencontainers.image.version=v4.0.0
# Sat, 21 Oct 2023 04:56:13 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 21 Oct 2023 04:56:14 GMT
COPY multi:84468128947ba1749e6048b0956ef2297175650942a70e8e8bc5df81159d8cc7 in /usr/local/bin/ 
# Sat, 21 Oct 2023 04:56:15 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 04:56:15 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:622a0779436eb93ceea635e910268f867c2eba47d4f62f0bd45f0bd165af3572`  
		Last Modified: Thu, 28 Sep 2023 21:00:50 GMT  
		Size: 2.9 MB (2899905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b85771de82c52657e20dd48525d4f84f8acc9b0a8e038caa59270b86c697f2`  
		Last Modified: Sat, 21 Oct 2023 03:43:30 GMT  
		Size: 2.5 MB (2524719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9aac39d270b16e3d2ddb731400c6e7d7d75663871e887bcd23f5e8867d4f0b`  
		Last Modified: Sat, 21 Oct 2023 03:43:29 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6906580ddda7fb53704962fe74b174c72d2e1e8f33877ee579c290e1c2bb65a`  
		Last Modified: Sat, 21 Oct 2023 03:43:29 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed93d90e00092a4fb65b975981dff45315aad2382893e3bd70a3e4183e6608c`  
		Last Modified: Sat, 21 Oct 2023 03:52:06 GMT  
		Size: 11.8 MB (11814640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599c8cfc8bab5dc02fcc0aca30a2e6d6573ef97f3905f402e1b590346284d34c`  
		Last Modified: Sat, 21 Oct 2023 03:52:05 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3163cb86b04f7d4059fb73e8c433c927b22c102a7202d2e671f1f806ae2972`  
		Last Modified: Sat, 21 Oct 2023 03:52:31 GMT  
		Size: 11.0 MB (10961298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8697c4a1dbc3b4d98bfaf9ce1df128d56b84ad9deb0204bd99256973bb8acaf`  
		Last Modified: Sat, 21 Oct 2023 03:52:29 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce40d8e71f77dc62873550ac44b3a85f6855eb3735e9aebd24b8d59b2a0440d9`  
		Last Modified: Sat, 21 Oct 2023 03:52:29 GMT  
		Size: 18.8 KB (18818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd8ad59019cea951cb2fd9698cc73f15a1713fe60669d1fb24b5360c868c08a`  
		Last Modified: Sat, 21 Oct 2023 03:52:29 GMT  
		Size: 8.9 KB (8880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158b0fb7efc21434151514e3a1961ea8f55d713ff2a54c4b3ad5b0af43acf767`  
		Last Modified: Sat, 21 Oct 2023 04:59:49 GMT  
		Size: 1.1 MB (1082134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:663c434386dc4d4d6fc452828f9159b8b05796dac5acc6370fc555c476e0c080`  
		Last Modified: Sat, 21 Oct 2023 04:59:49 GMT  
		Size: 7.9 MB (7861971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231731115e6180734434844272cdc6694aee64d15f7d45fe1e8f5ca9a87e580d`  
		Last Modified: Sat, 21 Oct 2023 04:59:47 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e02bfe3f71887ae641acd42e127fe77ef9ca3549a9f76fbff9b19072702dad7c`  
		Last Modified: Sat, 21 Oct 2023 04:59:47 GMT  
		Size: 26.5 KB (26533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c441fc04f47bdf8a34a45ae9560f2aeea4f32397d7b2360a105964c04fe9ff`  
		Last Modified: Sat, 21 Oct 2023 04:59:56 GMT  
		Size: 27.1 MB (27130001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7463550662429e3ff282ada62484462ada084d49ff31a562941e813f1d7789`  
		Last Modified: Sat, 21 Oct 2023 04:59:47 GMT  
		Size: 2.1 KB (2078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:4-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull monica@sha256:78d863ffec445dd24cb285cd56f045861ccfc3b4baf7bc0722734534cf9f5166
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67761125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b738cc0eb17d63824017b73ae8210bc3c43bc243cbbc08500076e46bf981488f`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 03:18:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 03:18:26 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 03:18:27 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 03:18:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 03:18:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 03:18:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 03:18:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 03:18:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 04:26:13 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 21 Oct 2023 05:00:51 GMT
ENV PHP_VERSION=8.1.24
# Sat, 21 Oct 2023 05:00:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Sat, 21 Oct 2023 05:00:51 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Sat, 21 Oct 2023 05:00:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 21 Oct 2023 05:00:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 21 Oct 2023 05:07:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 21 Oct 2023 05:07:53 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 21 Oct 2023 05:07:54 GMT
RUN docker-php-ext-enable sodium
# Sat, 21 Oct 2023 05:07:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 21 Oct 2023 05:07:55 GMT
WORKDIR /var/www/html
# Sat, 21 Oct 2023 05:07:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 21 Oct 2023 05:07:55 GMT
STOPSIGNAL SIGQUIT
# Sat, 21 Oct 2023 05:07:55 GMT
EXPOSE 9000
# Sat, 21 Oct 2023 05:07:55 GMT
CMD ["php-fpm"]
# Sat, 21 Oct 2023 06:56:27 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 21 Oct 2023 06:56:28 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 21 Oct 2023 06:57:41 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;     pecl install APCu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 21 Oct 2023 06:57:41 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 21 Oct 2023 06:57:41 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 21 Oct 2023 06:57:42 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Sat, 21 Oct 2023 06:57:42 GMT
WORKDIR /var/www/html
# Sat, 21 Oct 2023 06:57:42 GMT
ENV MONICA_VERSION=v4.0.0
# Sat, 21 Oct 2023 06:57:42 GMT
LABEL org.opencontainers.image.revision=e1a3e1315b1a92a5ff0ccab6c22ba9ded77a599e org.opencontainers.image.version=v4.0.0
# Sat, 21 Oct 2023 06:57:52 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 21 Oct 2023 06:57:53 GMT
COPY multi:84468128947ba1749e6048b0956ef2297175650942a70e8e8bc5df81159d8cc7 in /usr/local/bin/ 
# Sat, 21 Oct 2023 06:57:53 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 06:57:53 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:586ad9c0520cf94b10cf643fcc476c76d317d9f7fb19ea6664adc39853495259`  
		Last Modified: Sat, 21 Oct 2023 05:46:23 GMT  
		Size: 2.7 MB (2717014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ca4079608bb17975de556b78088351825e86efc0dd9d7e94be500e7aff4c4e`  
		Last Modified: Sat, 21 Oct 2023 05:46:22 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d96350d9b73c214fd82e72b434fb80879d73a1387ad9f7c654a25c99f169907`  
		Last Modified: Sat, 21 Oct 2023 05:46:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af33a1b52205a13414728a809c8f660b1b9193ce1b9ef5954c8a185d5d079d6d`  
		Last Modified: Sat, 21 Oct 2023 05:54:25 GMT  
		Size: 11.8 MB (11814620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:affa24ef9bc6bf27fd6ced4e4bf52bc75597bbed3205f2fb9dcba0492607f2db`  
		Last Modified: Sat, 21 Oct 2023 05:54:25 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb1a50a22443457c05bd06ef07a0264a4540972e2131e20dfb39be917f3b0cd`  
		Last Modified: Sat, 21 Oct 2023 05:54:49 GMT  
		Size: 12.9 MB (12895900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20dd041076ddfeca7ecaa69b963e3fbc6e0253142205096df61ef79efa81076`  
		Last Modified: Sat, 21 Oct 2023 05:54:47 GMT  
		Size: 2.4 KB (2445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75be3ec68fecde05bd2a008e9aa878aa2be94c02beb6d13bb0843ba4f8dffc9`  
		Last Modified: Sat, 21 Oct 2023 05:54:47 GMT  
		Size: 18.8 KB (18767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c466e07bef9824314e5ab03ffb865ca5105db1504b4dbfb226ff4dd322c31814`  
		Last Modified: Sat, 21 Oct 2023 05:54:47 GMT  
		Size: 8.9 KB (8878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8d342bce94595ef73297b7c1ede33f7a5852cff1bd433c38b9580d562d1bcb`  
		Last Modified: Sat, 21 Oct 2023 07:01:04 GMT  
		Size: 1.2 MB (1219867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb07e32275515e8ff453e251eb5c5fc76522e0bc8ef16ffcf8bab3c1b61cc1c4`  
		Last Modified: Sat, 21 Oct 2023 07:01:03 GMT  
		Size: 8.6 MB (8590937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d8c8260e3df4f71cee65722049f0410d83c745223757c00e2fd7fb7fca3c6bd`  
		Last Modified: Sat, 21 Oct 2023 07:01:02 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df0c5aea490b9546ded54fe7d2c1aabab33bf2c8197d4fd755bfaab361926392`  
		Last Modified: Sat, 21 Oct 2023 07:01:02 GMT  
		Size: 26.5 KB (26532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52a00a6991485c8623a8d5c37b7dc30b1f96a10c59a64f61ecd87fdaf5a699eb`  
		Last Modified: Sat, 21 Oct 2023 07:01:07 GMT  
		Size: 27.1 MB (27130009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecce8d0acbb7f41ad14131c280a0d9c2b9192af806a0868f505dc0ca93870805`  
		Last Modified: Sat, 21 Oct 2023 07:01:02 GMT  
		Size: 2.1 KB (2077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:4-fpm-alpine` - linux; 386

```console
$ docker pull monica@sha256:c1904668db5edea7234fa30c6e2be653700555337ad049dbb95a5c5d5158d432
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.8 MB (67832456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5abf39367bd146c8144e0c3055012895ef4e6abf71b9381d9dbc1f19199b229`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 28 Sep 2023 20:38:19 GMT
ADD file:8402753f294e403e92353bd65c86a6428c960be5116c0a15484b663a84f66fcd in / 
# Thu, 28 Sep 2023 20:38:20 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 02:11:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 02:11:14 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 02:11:14 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 02:11:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 02:11:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 02:11:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 02:11:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 02:11:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 04:05:50 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 21 Oct 2023 05:07:17 GMT
ENV PHP_VERSION=8.1.24
# Sat, 21 Oct 2023 05:07:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Sat, 21 Oct 2023 05:07:17 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Sat, 21 Oct 2023 05:07:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 21 Oct 2023 05:07:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 21 Oct 2023 05:19:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 21 Oct 2023 05:19:34 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 21 Oct 2023 05:19:36 GMT
RUN docker-php-ext-enable sodium
# Sat, 21 Oct 2023 05:19:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 21 Oct 2023 05:19:36 GMT
WORKDIR /var/www/html
# Sat, 21 Oct 2023 05:19:36 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 21 Oct 2023 05:19:37 GMT
STOPSIGNAL SIGQUIT
# Sat, 21 Oct 2023 05:19:37 GMT
EXPOSE 9000
# Sat, 21 Oct 2023 05:19:37 GMT
CMD ["php-fpm"]
# Sat, 21 Oct 2023 08:45:06 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 21 Oct 2023 08:45:08 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 21 Oct 2023 08:47:06 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;     pecl install APCu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 21 Oct 2023 08:47:06 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 21 Oct 2023 08:47:06 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 21 Oct 2023 08:47:08 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Sat, 21 Oct 2023 08:47:08 GMT
WORKDIR /var/www/html
# Sat, 21 Oct 2023 08:47:08 GMT
ENV MONICA_VERSION=v4.0.0
# Sat, 21 Oct 2023 08:47:08 GMT
LABEL org.opencontainers.image.revision=e1a3e1315b1a92a5ff0ccab6c22ba9ded77a599e org.opencontainers.image.version=v4.0.0
# Sat, 21 Oct 2023 08:47:22 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 21 Oct 2023 08:47:24 GMT
COPY multi:84468128947ba1749e6048b0956ef2297175650942a70e8e8bc5df81159d8cc7 in /usr/local/bin/ 
# Sat, 21 Oct 2023 08:47:24 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 08:47:24 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:dc95107ad2a031a015320bb397f73ec151d738127175b31ad643120697dc7e90`  
		Last Modified: Thu, 28 Sep 2023 20:39:32 GMT  
		Size: 3.2 MB (3235757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff457a32cf1e27eb13619e9fcf7d730c9b714c0791ec07574b2e0bab00b2a800`  
		Last Modified: Sat, 21 Oct 2023 06:34:21 GMT  
		Size: 2.7 MB (2723262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6599841cbfbc361d822214f5b54f2e29750f96d7fda628907cc716f3c4b8b5d7`  
		Last Modified: Sat, 21 Oct 2023 06:34:20 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae0b29a21ea2a601ab66ba02387f8db8004142686a99f34b871a2a941ebab467`  
		Last Modified: Sat, 21 Oct 2023 06:34:20 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d2963ad66a4333c62522b9e12573e36c8fee174eb1dfffdc9ff53136cdd396`  
		Last Modified: Sat, 21 Oct 2023 06:43:39 GMT  
		Size: 11.8 MB (11814629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c41876722bb89c4ea7d204b48f9836dacd09b4862a9022b1eac0f4207ea311b`  
		Last Modified: Sat, 21 Oct 2023 06:43:37 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f7c04bc0c975b506ca6f812744a62f9ecfc3e757421fdfd6b81a42ad37a3f0`  
		Last Modified: Sat, 21 Oct 2023 06:44:07 GMT  
		Size: 13.0 MB (13008079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acd88a193e61679de352da0c3c87eb2eca6ad5f9e50e1cbe7162245b71084cd`  
		Last Modified: Sat, 21 Oct 2023 06:44:03 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbedb80fef5fa82fcaf99bf1303ec28bb1b7d205b706ba7ca3dd9df203ae0a6a`  
		Last Modified: Sat, 21 Oct 2023 06:44:03 GMT  
		Size: 19.0 KB (18978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb916d4a4f3085f9adf54cce08db848588bca201c1eb73c4e4329ec5e4c90ec`  
		Last Modified: Sat, 21 Oct 2023 06:44:03 GMT  
		Size: 8.9 KB (8880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290111c5b208a8244192e54f9ae3b47a17ee8411f7a9611cadbcf8e4d9c58a05`  
		Last Modified: Sat, 21 Oct 2023 08:52:15 GMT  
		Size: 1.2 MB (1162846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2cba2b5b389ce9e227dd3b527ff055651f53ff1065b5f16a22f76d5e11d9ba`  
		Last Modified: Sat, 21 Oct 2023 08:52:15 GMT  
		Size: 8.7 MB (8696706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257df951c39cf58d89eababb487c83df6a5df1549dabe9f374f28a5a8977fa8c`  
		Last Modified: Sat, 21 Oct 2023 08:52:13 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a1fe857b75f64dd6a46a9f9ff36700e0a55f3bb0c6c18cfc286d4836eafed7`  
		Last Modified: Sat, 21 Oct 2023 08:52:13 GMT  
		Size: 26.5 KB (26533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af313c74d0cd60d1431a6109dfdaffb2506153a97fc4c3c211352213f6a3205`  
		Last Modified: Sat, 21 Oct 2023 08:52:23 GMT  
		Size: 27.1 MB (27130010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcccb9c3bfdf302709e4053a9f8d884ccf328388976ce0c47d11774187d9057a`  
		Last Modified: Sat, 21 Oct 2023 08:52:13 GMT  
		Size: 2.1 KB (2082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:4-fpm-alpine` - linux; ppc64le

```console
$ docker pull monica@sha256:75ef7212b5a8f730e176a44ad4928c778711386e1fc3902cb9968bffa5215be0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.6 MB (68577275 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:291b5318032ada123fbb0e79fca9610fea093e86372e2ed4170a4e87e127bf06`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 28 Sep 2023 21:22:20 GMT
ADD file:a720acb99214334c501363d564d8cae9b90d062ccf8a24a5ba1c831545b783dd in / 
# Thu, 28 Sep 2023 21:22:21 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:19:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 01:19:30 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 01:19:31 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 01:19:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 01:19:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 01:19:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:19:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:19:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 02:09:19 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 21 Oct 2023 02:35:59 GMT
ENV PHP_VERSION=8.1.24
# Sat, 21 Oct 2023 02:36:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Sat, 21 Oct 2023 02:36:00 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Sat, 21 Oct 2023 02:36:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 21 Oct 2023 02:36:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 21 Oct 2023 02:41:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 21 Oct 2023 02:41:04 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 21 Oct 2023 02:41:05 GMT
RUN docker-php-ext-enable sodium
# Sat, 21 Oct 2023 02:41:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 21 Oct 2023 02:41:05 GMT
WORKDIR /var/www/html
# Sat, 21 Oct 2023 02:41:06 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 21 Oct 2023 02:41:06 GMT
STOPSIGNAL SIGQUIT
# Sat, 21 Oct 2023 02:41:07 GMT
EXPOSE 9000
# Sat, 21 Oct 2023 02:41:07 GMT
CMD ["php-fpm"]
# Sat, 21 Oct 2023 06:42:00 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 21 Oct 2023 06:42:02 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 21 Oct 2023 06:43:45 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;     pecl install APCu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 21 Oct 2023 06:43:47 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 21 Oct 2023 06:43:47 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 21 Oct 2023 06:43:49 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Sat, 21 Oct 2023 06:43:49 GMT
WORKDIR /var/www/html
# Sat, 21 Oct 2023 06:43:49 GMT
ENV MONICA_VERSION=v4.0.0
# Sat, 21 Oct 2023 06:43:50 GMT
LABEL org.opencontainers.image.revision=e1a3e1315b1a92a5ff0ccab6c22ba9ded77a599e org.opencontainers.image.version=v4.0.0
# Sat, 21 Oct 2023 06:44:04 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 21 Oct 2023 06:44:08 GMT
COPY multi:84468128947ba1749e6048b0956ef2297175650942a70e8e8bc5df81159d8cc7 in /usr/local/bin/ 
# Sat, 21 Oct 2023 06:44:09 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 06:44:09 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:cd37f9856024d6685ac0233823aded690551c5872d6a27699a96c6a479d20f6f`  
		Last Modified: Thu, 28 Sep 2023 21:23:43 GMT  
		Size: 3.3 MB (3346508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad27196e84bb3ade565a8dd1e6b1058530043ed6f23f3c2b27e177dd9a872c0f`  
		Last Modified: Sat, 21 Oct 2023 03:15:11 GMT  
		Size: 2.8 MB (2766404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af8623e62ddef0a09dade21407c25a1ed872a84bcb0af9cdf932e97f5221e530`  
		Last Modified: Sat, 21 Oct 2023 03:15:10 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:763cf47f2cf8995a5d2a492fab64e7743a5d1b7d942d379bdec3a3dc8130ed53`  
		Last Modified: Sat, 21 Oct 2023 03:15:10 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07bcd5ddb27fdbe29ec451ddb11a0e7e336613ad820205e0e928b8df7fc3c458`  
		Last Modified: Sat, 21 Oct 2023 03:24:28 GMT  
		Size: 11.8 MB (11814614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d9ecca81ab25f93e39bc8d9a459bdc3b6e91b4064f46a50491ed298423f5c3`  
		Last Modified: Sat, 21 Oct 2023 03:24:27 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c8fb112e9c7e8c57e31691ad89fed16fa2486af476d9eaef2b658bea7efe8cf`  
		Last Modified: Sat, 21 Oct 2023 03:24:58 GMT  
		Size: 13.2 MB (13192046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a5556db3f62022575be0b36199b83ebaeb0dea096f1efe44bff96b33cde5cf7`  
		Last Modified: Sat, 21 Oct 2023 03:24:56 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d9f628bbd09ba96eff6bff234d353e2ccdabfb42adfd9a7c9f82557bd2fb4e1`  
		Last Modified: Sat, 21 Oct 2023 03:24:56 GMT  
		Size: 18.8 KB (18786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473fd56768218b23726ebc9d6666acbbd49831e4ea27fec8bf4b6a2db2b0fd06`  
		Last Modified: Sat, 21 Oct 2023 03:24:56 GMT  
		Size: 8.9 KB (8879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac11af8a8d256b8600a181d5cebc2b46545eb1993a6b70786fac23a6b41969c`  
		Last Modified: Sat, 21 Oct 2023 06:48:43 GMT  
		Size: 1.2 MB (1231790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbec4305e9cee80568d52e41e0da543c5a92854e2692bf17b3d4ed05f5e799ff`  
		Last Modified: Sat, 21 Oct 2023 06:48:43 GMT  
		Size: 9.0 MB (9034912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cbb079c681c4af6a92dcc8ca3625e7e755a1dcfd24358cc701d48c69bb8e15a`  
		Last Modified: Sat, 21 Oct 2023 06:48:41 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ff0b8e0676e153487101768f3a96f4a8dba12c3c041781aab4c0031effc32e`  
		Last Modified: Sat, 21 Oct 2023 06:48:41 GMT  
		Size: 26.5 KB (26546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5868fbd91107b5c3ec470aec5ffe00d22696cd8b930f54152393d2112b1f05aa`  
		Last Modified: Sat, 21 Oct 2023 06:48:49 GMT  
		Size: 27.1 MB (27130015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d0ac5536af1d7801ac42d0db23c026c2a70764bf8fc401e255adf950b40d406`  
		Last Modified: Sat, 21 Oct 2023 06:48:41 GMT  
		Size: 2.1 KB (2075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `monica:4-fpm-alpine` - linux; s390x

```console
$ docker pull monica@sha256:ec050dbbb3604c932417aab2888d9e3b4c5bb13149f6f2f474ca9807765e2dab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66850461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3df1d3e8790fd1fbbd8975c5b0b6f6bd9538952eea3ed606d9ddfa7340b81c94`
-	Entrypoint: `["\/usr\/local\/bin\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 28 Sep 2023 20:41:43 GMT
ADD file:fd3808a676fc56c1380e55b2ddbf4014d9371346cf789860b336bc9f00729ed0 in / 
# Thu, 28 Sep 2023 20:41:44 GMT
CMD ["/bin/sh"]
# Sat, 21 Oct 2023 01:18:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 21 Oct 2023 01:18:38 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 21 Oct 2023 01:18:39 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 21 Oct 2023 01:18:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 21 Oct 2023 01:18:40 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Sat, 21 Oct 2023 01:18:40 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:18:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 21 Oct 2023 01:18:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 21 Oct 2023 02:14:23 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Sat, 21 Oct 2023 02:41:49 GMT
ENV PHP_VERSION=8.1.24
# Sat, 21 Oct 2023 02:41:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.24.tar.xz.asc
# Sat, 21 Oct 2023 02:41:50 GMT
ENV PHP_SHA256=ee61f6232bb29bd2e785daf325d2177f2272bf80d086c295a724594e710bce3d
# Sat, 21 Oct 2023 02:41:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 21 Oct 2023 02:41:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 21 Oct 2023 02:47:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 21 Oct 2023 02:47:16 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Sat, 21 Oct 2023 02:47:17 GMT
RUN docker-php-ext-enable sodium
# Sat, 21 Oct 2023 02:47:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 21 Oct 2023 02:47:17 GMT
WORKDIR /var/www/html
# Sat, 21 Oct 2023 02:47:17 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Sat, 21 Oct 2023 02:47:18 GMT
STOPSIGNAL SIGQUIT
# Sat, 21 Oct 2023 02:47:18 GMT
EXPOSE 9000
# Sat, 21 Oct 2023 02:47:18 GMT
CMD ["php-fpm"]
# Sat, 21 Oct 2023 04:10:29 GMT
LABEL org.opencontainers.image.authors=Alexis Saettler <alexis@saettler.org> org.opencontainers.image.title=MonicaHQ, the Personal Relationship Manager org.opencontainers.image.description=This is MonicaHQ, your personal memory! MonicaHQ is like a CRM but for the friends, family, and acquaintances around you. org.opencontainers.image.url=https://monicahq.com org.opencontainers.image.source=https://github.com/monicahq/docker org.opencontainers.image.vendor=Monica
# Sat, 21 Oct 2023 04:10:31 GMT
RUN set -ex;         apk add --no-cache         bash         coreutils
# Sat, 21 Oct 2023 04:11:42 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         icu-dev         zlib-dev         libzip-dev         libxml2-dev         freetype-dev         libpng-dev         libjpeg-turbo-dev         jpeg-dev         gmp-dev         libmemcached-dev         libwebp-dev     ;         docker-php-ext-configure intl;     docker-php-ext-configure gd --with-jpeg --with-freetype --with-webp;     docker-php-ext-configure gmp;     docker-php-ext-install -j "$(nproc)"         intl         zip         bcmath         gd         gmp         pdo_mysql         mysqli         soap     ;     pecl install APCu-5.1.22;     pecl install memcached-3.2.0RC2;     pecl install redis-5.3.7;         docker-php-ext-enable         apcu         memcached         redis     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions         | tr ',' '\n'         | sort -u         | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'         )";     apk add --no-network --virtual .monica-phpext-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 21 Oct 2023 04:11:44 GMT
RUN set -ex;         mkdir -p /var/spool/cron/crontabs;     rm -f /var/spool/cron/crontabs/root;     echo '*/5 * * * * php /var/www/html/artisan schedule:run -v' > /var/spool/cron/crontabs/www-data
# Sat, 21 Oct 2023 04:11:44 GMT
ENV PHP_OPCACHE_VALIDATE_TIMESTAMPS=0 PHP_OPCACHE_MAX_ACCELERATED_FILES=20000 PHP_OPCACHE_MEMORY_CONSUMPTION=192 PHP_OPCACHE_MAX_WASTED_PERCENTAGE=10
# Sat, 21 Oct 2023 04:11:45 GMT
RUN set -ex;         docker-php-ext-enable opcache;     {         echo '[opcache]';         echo 'opcache.enable=1';         echo 'opcache.revalidate_freq=0';         echo 'opcache.validate_timestamps=${PHP_OPCACHE_VALIDATE_TIMESTAMPS}';         echo 'opcache.max_accelerated_files=${PHP_OPCACHE_MAX_ACCELERATED_FILES}';         echo 'opcache.memory_consumption=${PHP_OPCACHE_MEMORY_CONSUMPTION}';         echo 'opcache.max_wasted_percentage=${PHP_OPCACHE_MAX_WASTED_PERCENTAGE}';         echo 'opcache.interned_strings_buffer=16';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> $PHP_INI_DIR/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > $PHP_INI_DIR/conf.d/memory-limit.ini
# Sat, 21 Oct 2023 04:11:45 GMT
WORKDIR /var/www/html
# Sat, 21 Oct 2023 04:11:46 GMT
ENV MONICA_VERSION=v4.0.0
# Sat, 21 Oct 2023 04:11:46 GMT
LABEL org.opencontainers.image.revision=e1a3e1315b1a92a5ff0ccab6c22ba9ded77a599e org.opencontainers.image.version=v4.0.0
# Sat, 21 Oct 2023 04:12:00 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         for ext in tar.bz2 tar.bz2.asc; do         curl -fsSL -o monica-${MONICA_VERSION}.$ext "https://github.com/monicahq/monica/releases/download/${MONICA_VERSION}/monica-${MONICA_VERSION}.$ext";     done;         GPGKEY='BDAB0D0D36A00466A2964E85DE15667131EA6018';     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver hkps://keys.openpgp.org --recv-keys "$GPGKEY";     gpg --batch --verify monica-${MONICA_VERSION}.tar.bz2.asc monica-${MONICA_VERSION}.tar.bz2;         tar -xf monica-${MONICA_VERSION}.tar.bz2 -C /var/www/html --strip-components=1;         gpgconf --kill all;     rm -rf "$GNUPGHOME" monica-${MONICA_VERSION}.tar.bz2 monica-${MONICA_VERSION}.tar.bz2.asc;         cp /var/www/html/.env.example /var/www/html/.env;     chown -R www-data:www-data /var/www/html;         apk del .fetch-deps
# Sat, 21 Oct 2023 04:12:07 GMT
COPY multi:84468128947ba1749e6048b0956ef2297175650942a70e8e8bc5df81159d8cc7 in /usr/local/bin/ 
# Sat, 21 Oct 2023 04:12:07 GMT
ENTRYPOINT ["/usr/local/bin/entrypoint.sh"]
# Sat, 21 Oct 2023 04:12:07 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:47539bffe0f44273ec7731d86be2a6171359b3847c9b60c6ac74c4875c3264af`  
		Last Modified: Thu, 28 Sep 2023 20:43:18 GMT  
		Size: 3.2 MB (3215103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcde857c8cbd1e2f9e4b3bdb1e05a51819df45223c3af3c89c357d02c0683abd`  
		Last Modified: Sat, 21 Oct 2023 03:23:07 GMT  
		Size: 2.8 MB (2789639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3aa1b5985d90d234d5b51288c0ce33de4d2a3f6d3634cd2e6818e9e9a36e8f2`  
		Last Modified: Sat, 21 Oct 2023 03:23:06 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07a26837a8dae33541022d07fbeb175eb6f280a63fe5c2f5b6fdd82525674502`  
		Last Modified: Sat, 21 Oct 2023 03:23:06 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c01eb90f78d6da44386d26813bbb05325c61ccb6a68e5e5708ea60ad7cfea13`  
		Last Modified: Sat, 21 Oct 2023 03:29:53 GMT  
		Size: 11.8 MB (11814626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e90d199bf697761c8c83388e7624d3a30e535d3fd341c1329bd6921545761dc`  
		Last Modified: Sat, 21 Oct 2023 03:29:52 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20af4c1fbcf7172188a204bf962bfcad12ab698af711c738b51ead016082eb45`  
		Last Modified: Sat, 21 Oct 2023 03:30:12 GMT  
		Size: 12.0 MB (11996727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f249210c4435a6af128b8ae8b5c93474547e522c87b1e6ce762d22631b39ccc4`  
		Last Modified: Sat, 21 Oct 2023 03:30:10 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf814d225d5bdc47d559452ad9ed479af42c42834a7355737343a0dfd902410`  
		Last Modified: Sat, 21 Oct 2023 03:30:10 GMT  
		Size: 18.8 KB (18811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29152b0b57e695a3c38f569d306c5772f681d6a9f5e97b74453c1da30f94cde5`  
		Last Modified: Sat, 21 Oct 2023 03:30:10 GMT  
		Size: 8.9 KB (8877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98a46a9a4f44142778fddbdb966c754db529a0cdbead8ee6ad9409bbc3cda78c`  
		Last Modified: Sat, 21 Oct 2023 04:15:12 GMT  
		Size: 1.2 MB (1201922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12f251b86290f26b532f5e5adf940023fa072f423a2794ae6710fa2e7ace2ff2`  
		Last Modified: Sat, 21 Oct 2023 04:15:12 GMT  
		Size: 8.6 MB (8641352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e75b3ea92d4f29c7e4656a588ea39d0cbc6aec3e871aca62db743b1859c8ce6`  
		Last Modified: Sat, 21 Oct 2023 04:15:11 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1b267d6e96c2e72d16d723c743b09de186942b0d4dd41f8e3741dda151a4a9`  
		Last Modified: Sat, 21 Oct 2023 04:15:11 GMT  
		Size: 26.6 KB (26566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42c019973fb1157416e9c83cb085bf4e68b016f5ac813c287f48e98653a4518`  
		Last Modified: Sat, 21 Oct 2023 04:15:16 GMT  
		Size: 27.1 MB (27130064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad3f3ef9dc92f8e75240c0ee4bc6b36627d02577b9a72c4cb556ca72c32341b4`  
		Last Modified: Sat, 21 Oct 2023 04:15:11 GMT  
		Size: 2.1 KB (2076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
