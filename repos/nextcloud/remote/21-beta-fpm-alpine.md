## `nextcloud:21-beta-fpm-alpine`

```console
$ docker pull nextcloud@sha256:67accfca483cd7a035edd7ebd6861a216e56988884781a98f7bf275029f01ae3
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

### `nextcloud:21-beta-fpm-alpine` - linux; amd64

```console
$ docker pull nextcloud@sha256:881a78cc68f9d9cc44e53a6295324005e5d67f0edc0f0e2be38d45e49dd104cc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.3 MB (174268908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3017c8362387d94e74791dfd840646810916c1233d67888ad30b87542553d2ec`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:41:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 08:41:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 08:41:55 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 08:41:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 08:41:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 08:48:59 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 08:49:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 08:49:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 08:49:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 09:04:03 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 17:44:01 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 17:44:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 17:44:02 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 17:44:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jan 2021 17:44:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:52:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 20:20:32 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 21 Jan 2021 20:20:35 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 20:20:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 20:20:35 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 20:20:37 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Jan 2021 20:20:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 20:20:38 GMT
EXPOSE 9000
# Thu, 21 Jan 2021 20:20:38 GMT
CMD ["php-fpm"]
# Thu, 21 Jan 2021 23:53:39 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 21 Jan 2021 23:56:00 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.2;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Thu, 21 Jan 2021 23:56:01 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 21 Jan 2021 23:56:01 GMT
VOLUME [/var/www/html]
# Tue, 26 Jan 2021 00:33:29 GMT
ENV NEXTCLOUD_VERSION=21.0.0beta7
# Tue, 26 Jan 2021 00:34:03 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/prereleases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/prereleases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Tue, 26 Jan 2021 00:34:04 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Tue, 26 Jan 2021 00:34:05 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Tue, 26 Jan 2021 00:34:05 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 26 Jan 2021 00:34:06 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e2096094279456885c5847855bddf4d9ac3b5c4f7f0ff73ef92fa69821ff86`  
		Last Modified: Thu, 17 Dec 2020 11:05:30 GMT  
		Size: 1.3 MB (1340903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320f26ee9b1c7b4c2ce0b67550a066ea859fb8796c0ff8de576f7e1b330342da`  
		Last Modified: Thu, 17 Dec 2020 11:05:30 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4612e05a72cfb0fde0de7565baa2660900747122288141d8dba25482f4983fe0`  
		Last Modified: Thu, 17 Dec 2020 11:05:30 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e0e3aa22e445286becccbdab24843c31f01402438adddd0d08b06b35d3e2c2`  
		Last Modified: Thu, 07 Jan 2021 20:31:25 GMT  
		Size: 10.3 MB (10345668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1731c161c4e9fd95a50fcf21c329aa5cd8cc275443b8fba2f313cef1f9022ae3`  
		Last Modified: Thu, 07 Jan 2021 20:31:23 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1297ca4f980950e23e704be0c39c25d9235f63a72e35f285b9b2f81d3611be04`  
		Last Modified: Thu, 07 Jan 2021 20:31:27 GMT  
		Size: 14.3 MB (14259382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf64aa53cc01b96af6d405d1c33e8f532725dac6d70fe01a19b09a2038f0f37c`  
		Last Modified: Thu, 21 Jan 2021 20:32:16 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6308261720a639b2ae3d1d6128c7e72bd26240878191f4817d000b866965e03c`  
		Last Modified: Thu, 21 Jan 2021 20:32:17 GMT  
		Size: 16.9 KB (16901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7295add5d56dbe6c35f5c3edb680729676dd4088ee93ac801d9e402a90362f6`  
		Last Modified: Thu, 21 Jan 2021 20:32:16 GMT  
		Size: 8.5 KB (8451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad9e369809271df8a6bb0c285e9caf2231ebd8054142a678ed82820a987cb08`  
		Last Modified: Fri, 22 Jan 2021 00:05:18 GMT  
		Size: 258.1 KB (258128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29539d5ac781e5f2875659a844dba2bd2b4e39f56a269f9a05bbe6ae9e625b9f`  
		Last Modified: Fri, 22 Jan 2021 00:05:22 GMT  
		Size: 26.6 MB (26560350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208f68851a61bce8c08fdc486cb0763e6df7241add616e995761f3e3ebd2dde4`  
		Last Modified: Fri, 22 Jan 2021 00:05:17 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5169d5197d2e4b87df8460d16b3df78ffda10916230a033b8286c3879c7c668`  
		Last Modified: Tue, 26 Jan 2021 00:42:11 GMT  
		Size: 118.7 MB (118670909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102aa4cc89f76244cb83be7f1812b8598c58ffe8bffc91f625a28911c41a6870`  
		Last Modified: Tue, 26 Jan 2021 00:41:41 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c976f1ee3ebf62b0a4cd83c9a654d09a0c1edee2f26bb24b700b8ba31d0094`  
		Last Modified: Tue, 26 Jan 2021 00:41:48 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:21-beta-fpm-alpine` - linux; arm variant v6

```console
$ docker pull nextcloud@sha256:d2d3d089d8e3f1667689c51a64b2280c4a4183dbc1c6f42d0bd92714bb393972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.2 MB (172194725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7556e5f5007576863de1a09b79e9bfeebfab138490804c24ceb8e552cf633972`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:02:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 04:02:22 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 04:02:27 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 04:02:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 04:02:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 04:07:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 04:07:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 04:07:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 04:07:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 04:17:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 04 Feb 2021 18:21:06 GMT
ENV PHP_VERSION=7.4.15
# Thu, 04 Feb 2021 18:21:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Thu, 04 Feb 2021 18:21:08 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Thu, 04 Feb 2021 18:21:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 04 Feb 2021 18:21:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Feb 2021 18:25:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Feb 2021 18:25:37 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 04 Feb 2021 18:25:40 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Feb 2021 18:25:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Feb 2021 18:25:42 GMT
WORKDIR /var/www/html
# Thu, 04 Feb 2021 18:25:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 04 Feb 2021 18:25:44 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 Feb 2021 18:25:45 GMT
EXPOSE 9000
# Thu, 04 Feb 2021 18:25:46 GMT
CMD ["php-fpm"]
# Thu, 04 Feb 2021 20:14:28 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 04 Feb 2021 20:18:11 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.2;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Thu, 04 Feb 2021 20:18:15 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 04 Feb 2021 20:18:17 GMT
VOLUME [/var/www/html]
# Thu, 04 Feb 2021 20:20:52 GMT
ENV NEXTCLOUD_VERSION=21.0.0beta7
# Thu, 04 Feb 2021 20:21:46 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/prereleases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/prereleases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Thu, 04 Feb 2021 20:21:53 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Thu, 04 Feb 2021 20:21:56 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Thu, 04 Feb 2021 20:21:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 Feb 2021 20:21:59 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16035da780bb4f74637b8f27602f05d4a81886aeea06f603ea7e46dd84d57b6d`  
		Last Modified: Thu, 17 Dec 2020 05:38:57 GMT  
		Size: 1.3 MB (1310288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdfae7d4501031aa09e0c64be274eb95df5740b32cde16be0182bcea9d8a4845`  
		Last Modified: Thu, 17 Dec 2020 05:38:57 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6384065388d88752c6562c2bb76398ecc59f1a03a1c5e4601dc75d768117919`  
		Last Modified: Thu, 17 Dec 2020 05:38:56 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572a0242967d5fcf34acc047da952fdd20dbef26760f6344e354f040354e026f`  
		Last Modified: Thu, 04 Feb 2021 18:56:49 GMT  
		Size: 10.4 MB (10351226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5654afeec92f97b22854e0dc208152a2bc21a0e724c13cef27a14c818c95aaf9`  
		Last Modified: Thu, 04 Feb 2021 18:56:46 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ceb7314c918ecaee7771e14bad0094f28b4666b54b5813a5ed9fce83504821d`  
		Last Modified: Thu, 04 Feb 2021 18:56:50 GMT  
		Size: 13.3 MB (13285729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:736d821f0dd9017572ebe343107767f5e5932792868113e90be4bf81441b37dd`  
		Last Modified: Thu, 04 Feb 2021 18:56:46 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a61715d505c45fc1adf78f507962d77e778260f0fe6d38ea4bbdd3757d4ecf`  
		Last Modified: Thu, 04 Feb 2021 18:56:46 GMT  
		Size: 16.9 KB (16886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee8cf54244c82855be11a60f97abcd3a5bed92a6374b60e0b60af8f4a951c8f6`  
		Last Modified: Thu, 04 Feb 2021 18:56:46 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24913b04f1d9cd8dc1d521edddfb0a3a9bf1cc08e1b16518c25e618b2eba622`  
		Last Modified: Thu, 04 Feb 2021 20:23:09 GMT  
		Size: 268.6 KB (268602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a1df5ef65e5693791b1e07c272c23886abb43291153554992caa5e9da9858b1`  
		Last Modified: Thu, 04 Feb 2021 20:23:15 GMT  
		Size: 25.7 MB (25669400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85644a75bb7e993c6f2b6300019709bfcbe41bdca4e4c45b548cabd4e6879c7`  
		Last Modified: Thu, 04 Feb 2021 20:23:07 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3c8f4184a993c028cc87525d80c2950cf6eab9bd13fab2198e6d60a05316f9`  
		Last Modified: Thu, 04 Feb 2021 20:25:34 GMT  
		Size: 118.7 MB (118670742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7674def9b94e9e88b96213a8d9918017dc12be2e2af05be002542778f49c7ca`  
		Last Modified: Thu, 04 Feb 2021 20:24:53 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9db3195eca1d30776454c2adfbd96c96a66ed22e3398772de75c7e450dfefe4a`  
		Last Modified: Thu, 04 Feb 2021 20:24:53 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:21-beta-fpm-alpine` - linux; arm variant v7

```console
$ docker pull nextcloud@sha256:b762b4d6511ec6165d59347f70afa561b18c9b4f164b060b94f5ea0ed1e0e4b2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.5 MB (170469129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f757b107f77d319704844ef422d148a4b4e8e5303d1ad2d205286e50511d18b3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 03:59:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 03:59:47 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 03:59:49 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 03:59:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 03:59:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 04:04:09 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 04:04:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 04:04:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 04:04:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 04:12:44 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 17:23:57 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 17:23:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 17:23:58 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 17:24:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jan 2021 17:24:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:26:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:13:22 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:13:25 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:13:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:13:27 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 19:13:29 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Jan 2021 19:13:29 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 19:13:30 GMT
EXPOSE 9000
# Thu, 21 Jan 2021 19:13:31 GMT
CMD ["php-fpm"]
# Thu, 21 Jan 2021 23:32:51 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 21 Jan 2021 23:36:01 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.2;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Thu, 21 Jan 2021 23:36:04 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 21 Jan 2021 23:36:05 GMT
VOLUME [/var/www/html]
# Tue, 26 Jan 2021 00:32:02 GMT
ENV NEXTCLOUD_VERSION=21.0.0beta7
# Tue, 26 Jan 2021 00:32:51 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/prereleases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/prereleases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Tue, 26 Jan 2021 00:32:57 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Tue, 26 Jan 2021 00:32:59 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Tue, 26 Jan 2021 00:33:00 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 26 Jan 2021 00:33:01 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb43bb12dd6693d888e6501fba59948c3e894b068d539fbf968aac1638f58847`  
		Last Modified: Thu, 17 Dec 2020 05:28:25 GMT  
		Size: 1.2 MB (1214517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c593d596abc28364a253c99118c3080eec76e91bf5db463e2a66804da18dfa`  
		Last Modified: Thu, 17 Dec 2020 05:28:23 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145a8f86ceab4a34dedf8d4173439cf517eec5c52b3074dea204dce67da7f3ad`  
		Last Modified: Thu, 17 Dec 2020 05:28:23 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d2a8ad2edd92a9062b1a6f88a354e60eeebd125f25241c2c39483ae922eccf`  
		Last Modified: Thu, 07 Jan 2021 18:42:02 GMT  
		Size: 10.3 MB (10345672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:546734c8784e6dcc769b67a3624d6f87f7b9a66afa01115a1aa3f664e08fd527`  
		Last Modified: Thu, 07 Jan 2021 18:41:58 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc52e6f4cbd91919d9b26a09a1996f0a9391b62763f37841509cfe6e511b86e`  
		Last Modified: Thu, 07 Jan 2021 18:42:03 GMT  
		Size: 12.4 MB (12422910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0c65a3e1ae6ef95c1699d005bdd9edd1d99c9476857747f031f327573a1a487`  
		Last Modified: Thu, 21 Jan 2021 19:28:33 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722aca39d0820a5344c33ba85342514a37aa1b47581cc2fb41dc760d0341d5e2`  
		Last Modified: Thu, 21 Jan 2021 19:28:33 GMT  
		Size: 16.9 KB (16864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db56dd8678094d7c7ee1543d761fe97a197e6d905f67dfe2aa808b167fa0a92`  
		Last Modified: Thu, 21 Jan 2021 19:28:33 GMT  
		Size: 8.5 KB (8451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a24b3da67a877505973de8f05fcb0bb86ad4e02dbb784c0ce46e071ea2f36390`  
		Last Modified: Thu, 21 Jan 2021 23:51:16 GMT  
		Size: 243.2 KB (243176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e907ee7c5c2bb9afd241239bc87a79e03ec8b36b489175b5cea0fcd4509e9cc1`  
		Last Modified: Thu, 21 Jan 2021 23:51:22 GMT  
		Size: 25.1 MB (25130434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56d59f3372fb0ec514f51aa0e31befcfb1c79ae319033d84da15b3e283f6ef55`  
		Last Modified: Thu, 21 Jan 2021 23:51:14 GMT  
		Size: 530.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d961b3d80f628f31e4ae3c95b1ff4c5a0ef1b760ec6d93e18091f1dcb254f40e`  
		Last Modified: Tue, 26 Jan 2021 00:44:13 GMT  
		Size: 118.7 MB (118670299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7ef9ced25e7158da0d716a1a3cfce7b21ba36a6b36214457ea331c4e2ac88ed`  
		Last Modified: Tue, 26 Jan 2021 00:43:34 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aecda848be455479f807faa89809f1aada9e60014b8e4943ecf4afcfc2096ce5`  
		Last Modified: Tue, 26 Jan 2021 00:43:34 GMT  
		Size: 1.9 KB (1893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:21-beta-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull nextcloud@sha256:c0f1805dcf273d0542cda4cdffbcea7f25f2927824aa37b8b7822d08aa4299bd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.8 MB (173819362 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5ac63d4321a97392edf1c079f3cb9608a96aa7b7213d63d6ad70908a374253a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:46:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 05:46:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 05:46:55 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 05:46:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 05:47:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 05:51:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 05:51:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 05:51:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 05:51:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 06:01:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 18:10:16 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 18:10:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 18:10:19 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 18:10:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jan 2021 18:10:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 18:14:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:55:04 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:55:09 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:55:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:55:12 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 19:55:14 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Jan 2021 19:55:14 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 19:55:15 GMT
EXPOSE 9000
# Thu, 21 Jan 2021 19:55:16 GMT
CMD ["php-fpm"]
# Fri, 22 Jan 2021 00:31:51 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 22 Jan 2021 00:35:06 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.2;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Fri, 22 Jan 2021 00:35:09 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 22 Jan 2021 00:35:09 GMT
VOLUME [/var/www/html]
# Tue, 26 Jan 2021 01:59:19 GMT
ENV NEXTCLOUD_VERSION=21.0.0beta7
# Tue, 26 Jan 2021 01:59:58 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/prereleases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/prereleases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Tue, 26 Jan 2021 02:00:02 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Tue, 26 Jan 2021 02:00:05 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Tue, 26 Jan 2021 02:00:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 26 Jan 2021 02:00:06 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349511631cc12dc049249fd94f9012c505ccb000f16147091cb84874846fb9b1`  
		Last Modified: Thu, 17 Dec 2020 07:10:16 GMT  
		Size: 1.3 MB (1342931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053bd098149c8419c2b9b5a2702c5d9c4e9de3b2131447e18aacde4047de2d88`  
		Last Modified: Thu, 17 Dec 2020 07:10:15 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00122640c7f935b33a14c9e88b946165e75935d6cd28f9b2d20d783d43c21423`  
		Last Modified: Thu, 17 Dec 2020 07:10:15 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b5acc908a258e5ea1e9e972d38e9c30289ffd2ee6928306144fe083c0d4f8e`  
		Last Modified: Thu, 07 Jan 2021 19:32:43 GMT  
		Size: 10.3 MB (10345707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6f3407f8c8dfce02d9af40a7389c76895567a98e4c301cf32f6e99d77d4903`  
		Last Modified: Thu, 07 Jan 2021 19:32:38 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e56a5f41aef0511951736887d91745c3ce87340112017cdbf06a52c612f55a0`  
		Last Modified: Thu, 07 Jan 2021 19:32:44 GMT  
		Size: 14.1 MB (14069158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5fe49b8dafe2ce1f939504d7eb8bea011ed2b2e8733b1bb51b00e06e48bcf7c`  
		Last Modified: Thu, 21 Jan 2021 20:09:54 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b925f7083f9092f095dac44255a4e0f2816a28c6ed79a86a24c409754baa046`  
		Last Modified: Thu, 21 Jan 2021 20:09:54 GMT  
		Size: 16.9 KB (16912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f1e88358157f786de4ae26838acd1547fcdb51101d8e627f7223b3b1d8dcb57`  
		Last Modified: Thu, 21 Jan 2021 20:09:54 GMT  
		Size: 8.5 KB (8453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a48c66d9b4e6fa2544bd9f218328f15aa4c97831a981dffdc781246273ee59`  
		Last Modified: Fri, 22 Jan 2021 00:47:33 GMT  
		Size: 269.0 KB (269033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46cd7a8374c57e46d886e89f8d5e50f0cb55044fd3eab2a739343a480ec4af58`  
		Last Modified: Fri, 22 Jan 2021 00:47:37 GMT  
		Size: 26.4 MB (26377981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bef0fde85a515d37bb88993176f194440456614b8fb34cdc0d9348e30a5411`  
		Last Modified: Fri, 22 Jan 2021 00:47:31 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ece332b61f6768d5a1f7617f4f584a5dbd2ba35c9e30d23cc12f1cdd4574e48`  
		Last Modified: Tue, 26 Jan 2021 02:09:45 GMT  
		Size: 118.7 MB (118670886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2248244b23b2f00f03dc8ccb28b1e26a7f08566bd75c3753d3dc37a128f58b2a`  
		Last Modified: Tue, 26 Jan 2021 02:09:16 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4e9c5477186f7ad9eefd23903ff8d26f5977c2ca880d28d120a28107870f14`  
		Last Modified: Tue, 26 Jan 2021 02:09:16 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:21-beta-fpm-alpine` - linux; 386

```console
$ docker pull nextcloud@sha256:5355bad9e70adcd972d95a5da0fdee935e9dcfe97f6dbdced083e076221e7dc7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.2 MB (175235098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfedbeaee914c26e90583b0c11ca9f2d45c4884c375579f2361c8c710962263a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 03:34:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 03:34:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 03:34:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 03:34:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 03:34:07 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 03:40:09 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 03:40:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 03:40:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 03:40:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 03:52:35 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 18:21:27 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 18:21:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 18:21:28 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 18:21:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jan 2021 18:21:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 18:31:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:47:29 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:47:31 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:47:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:47:32 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 19:47:33 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Jan 2021 19:47:34 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 19:47:34 GMT
EXPOSE 9000
# Thu, 21 Jan 2021 19:47:34 GMT
CMD ["php-fpm"]
# Thu, 21 Jan 2021 22:52:26 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 21 Jan 2021 22:55:36 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.2;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Thu, 21 Jan 2021 22:55:37 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 21 Jan 2021 22:55:37 GMT
VOLUME [/var/www/html]
# Tue, 26 Jan 2021 00:57:30 GMT
ENV NEXTCLOUD_VERSION=21.0.0beta7
# Tue, 26 Jan 2021 00:58:08 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/prereleases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/prereleases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Tue, 26 Jan 2021 00:58:08 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Tue, 26 Jan 2021 00:58:09 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Tue, 26 Jan 2021 00:58:10 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 26 Jan 2021 00:58:10 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94d120997ac65664d4944fb3d9d4551e8e118f43c788aa67591c2cb54010aed`  
		Last Modified: Thu, 17 Dec 2020 05:43:55 GMT  
		Size: 1.4 MB (1439814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657c96696eb3a101b3148ccc28a870e751ee94e39bb2f3cc1745bdec7655b033`  
		Last Modified: Thu, 17 Dec 2020 05:43:55 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25357089a74d7e4f4ee1bc77cd180c431537e393399785f113a7f2fe4ac7614`  
		Last Modified: Thu, 17 Dec 2020 05:43:52 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a0403170d088ecd930d7283bba2b96eba4f8af70e2683bed18bbce107f3de5`  
		Last Modified: Thu, 07 Jan 2021 21:13:41 GMT  
		Size: 10.3 MB (10345646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5a38b02f7cf978e61b430eb3e6593fe1c12aa329324d6059a56c049bde5d6b`  
		Last Modified: Thu, 07 Jan 2021 21:13:38 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34fb4de243b08ba3f630842f80f7f1230f8e8b6614d2c7448965668cd2c4f4b`  
		Last Modified: Thu, 07 Jan 2021 21:13:41 GMT  
		Size: 14.6 MB (14642409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54676da09d689184289e4a0208cfed3a9d7ab9d6d32c053095c7c7e62ad13f63`  
		Last Modified: Thu, 21 Jan 2021 19:59:41 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ae8a9936d61ff0679edd236e11eb68eeb99f1032ac9131831d483d01a09418`  
		Last Modified: Thu, 21 Jan 2021 19:59:39 GMT  
		Size: 16.9 KB (16894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d4a11e29c458577037adb0effa9ebb42825ac4390a2c673b214e95175dabb2f`  
		Last Modified: Thu, 21 Jan 2021 19:59:40 GMT  
		Size: 8.5 KB (8452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01d67c545aabe30aa450371ac4c5604f52607f9c7177b6834d8f9f302088afa`  
		Last Modified: Thu, 21 Jan 2021 23:07:09 GMT  
		Size: 276.9 KB (276877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76d314900b29b56cce00980443ce514dddf970e0ed7665c2137e30a53611285e`  
		Last Modified: Thu, 21 Jan 2021 23:07:16 GMT  
		Size: 27.0 MB (27030991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6973368bc40128663d13ffceb082808cbc86d9daf4b5a21311748f1ae6ab880`  
		Last Modified: Thu, 21 Jan 2021 23:07:05 GMT  
		Size: 505.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07ef12a840bdae5ba1ae7d44f5b8a8bde79bdbf056630618cb1af30d8b790e4a`  
		Last Modified: Tue, 26 Jan 2021 01:07:02 GMT  
		Size: 118.7 MB (118670726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e99a27281faa655d5263c0489897b241aca0449d232441958b564310239391f0`  
		Last Modified: Tue, 26 Jan 2021 01:06:29 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842f99341ea53cb11d2cdc2c1f257951fb7b86624f8d087a20ee3d9fa4a14f68`  
		Last Modified: Tue, 26 Jan 2021 01:06:29 GMT  
		Size: 1.9 KB (1897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:21-beta-fpm-alpine` - linux; ppc64le

```console
$ docker pull nextcloud@sha256:8ee3aa4056b565a4554e612ad4a011132ba4eba1dc26aa838bc8b58cda316781
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.7 MB (175661045 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37b0680186b645572e658876954eb016eb7c204424ae996c015710d10b086b4f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:02:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 06:02:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 06:03:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 06:03:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 06:03:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 06:09:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 06:09:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 06:09:45 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 06:09:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 06:21:39 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 18:04:06 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 18:04:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 18:04:20 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 18:04:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jan 2021 18:04:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 18:08:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:44:40 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:45:00 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:45:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:45:12 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 19:45:25 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Jan 2021 19:45:37 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 19:45:44 GMT
EXPOSE 9000
# Thu, 21 Jan 2021 19:45:53 GMT
CMD ["php-fpm"]
# Fri, 22 Jan 2021 04:02:07 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Fri, 22 Jan 2021 04:05:13 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.2;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Fri, 22 Jan 2021 04:05:21 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Fri, 22 Jan 2021 04:05:25 GMT
VOLUME [/var/www/html]
# Tue, 26 Jan 2021 02:17:46 GMT
ENV NEXTCLOUD_VERSION=21.0.0beta7
# Tue, 26 Jan 2021 02:19:51 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/prereleases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/prereleases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Tue, 26 Jan 2021 02:19:55 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Tue, 26 Jan 2021 02:19:59 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Tue, 26 Jan 2021 02:20:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 26 Jan 2021 02:20:10 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4878c44618050313be4a5ac046d572683a6e0d371586c31a768e1768423df9a3`  
		Last Modified: Thu, 17 Dec 2020 08:04:10 GMT  
		Size: 1.4 MB (1383302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577c712c96426aadbf75437b4aae5841ed84ba25ee142ec3aaaf86802464d6f9`  
		Last Modified: Thu, 17 Dec 2020 08:04:08 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a10ca736025b1646c79fbd378c22773ccb82df4aadc2cb960dea6eacb8bbb16`  
		Last Modified: Thu, 17 Dec 2020 08:04:08 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b716f68e5de6d72b17c8f89fb302689dc70c27ec1e0fb95eb2a64bf2f6c26`  
		Last Modified: Thu, 07 Jan 2021 19:53:56 GMT  
		Size: 10.3 MB (10345699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795fe2cb0d85f09ac5fd362886605ffe47de33dca98304b0edbb05b43226b05e`  
		Last Modified: Thu, 07 Jan 2021 19:53:49 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a00e93768d44b4d819c0b84d8e36474ed1954df991b0781eca12f4c05c642fd`  
		Last Modified: Thu, 07 Jan 2021 19:53:53 GMT  
		Size: 15.2 MB (15242506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71690ef1ba467e99ddbb7ba8ef07abc17070260d3441921f8e005b2b709ef1dc`  
		Last Modified: Thu, 21 Jan 2021 20:09:49 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bcada07215e9ba10cd5c6df55db6661c6c1ea494c84795faf9ebbfbecad64e`  
		Last Modified: Thu, 21 Jan 2021 20:09:49 GMT  
		Size: 16.9 KB (16940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b24f066acdb0e5b4c8a2ae33ea267ce69e7d0eefc5469913e771cdce832d1c`  
		Last Modified: Thu, 21 Jan 2021 20:09:49 GMT  
		Size: 8.5 KB (8453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55934938f6881ce94a6c1611ce2a5f7c49d2b1657f3c606554d176a0c0ccd7c8`  
		Last Modified: Fri, 22 Jan 2021 04:39:44 GMT  
		Size: 274.4 KB (274394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c10565cc86556af8bd8d85ba2f4cd14a012a5d12e7b8da33ffb36716ff4cd1d`  
		Last Modified: Fri, 22 Jan 2021 04:39:56 GMT  
		Size: 26.9 MB (26904352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b50d1eb6996843a4a67849f0c8eff8e0aec8044ffdcbb9943b1fed3144992421`  
		Last Modified: Fri, 22 Jan 2021 04:39:40 GMT  
		Size: 529.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75ea2bb3f10da1e5cf9211703531e4d477426ff3cecf4e8fa879228b6fad200`  
		Last Modified: Tue, 26 Jan 2021 02:52:53 GMT  
		Size: 118.7 MB (118670918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d3ca23c2ea73b203140fa2e27cd8df849b2284e03e98aa7a1e47a847c8597f`  
		Last Modified: Tue, 26 Jan 2021 02:50:24 GMT  
		Size: 2.5 KB (2531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea5a04b89e9a1d04511438c6b3ffaad32f9e457b1cc9c958993b484ca7f6f9c6`  
		Last Modified: Tue, 26 Jan 2021 02:50:24 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:21-beta-fpm-alpine` - linux; s390x

```console
$ docker pull nextcloud@sha256:83ca46e0fc420a54d91bc37a368236178f54d3323b47837657ca62e262dcef29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **173.2 MB (173246911 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d24fdd9c0d9e674d00c0efbcee3a6b967396666b47640f8e1147adcdbc2dec3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:11:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 06:11:31 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 06:11:33 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 06:11:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 06:11:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 06:17:07 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 06:17:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 06:17:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 06:17:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 06:28:31 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 17:59:00 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 17:59:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 17:59:00 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 17:59:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jan 2021 17:59:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 18:02:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:56:30 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:56:32 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:56:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:56:34 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 19:56:36 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Jan 2021 19:56:36 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 19:56:37 GMT
EXPOSE 9000
# Thu, 21 Jan 2021 19:56:38 GMT
CMD ["php-fpm"]
# Thu, 21 Jan 2021 22:05:48 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 21 Jan 2021 22:08:25 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         bcmath         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-5.3.2;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Thu, 21 Jan 2021 22:08:29 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 21 Jan 2021 22:08:30 GMT
VOLUME [/var/www/html]
# Tue, 26 Jan 2021 01:20:49 GMT
ENV NEXTCLOUD_VERSION=21.0.0beta7
# Tue, 26 Jan 2021 01:21:34 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/prereleases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/prereleases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Tue, 26 Jan 2021 01:21:49 GMT
COPY multi:735a0b44f536c26b775ae5b6d0dc6331e21972d82c38b6571980561dc6f483ee in / 
# Tue, 26 Jan 2021 01:21:51 GMT
COPY multi:69a3d18e5826dcf2a02562f59ec38d4047623d6d537d30e24b29faeb8ea43f9d in /usr/src/nextcloud/config/ 
# Tue, 26 Jan 2021 01:21:51 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 26 Jan 2021 01:21:52 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b33a1a773ad25f9d9c6930913defa3b9196c1fdcd8d5a2d592215cda11cf944`  
		Last Modified: Thu, 17 Dec 2020 08:07:32 GMT  
		Size: 1.4 MB (1382756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4721c450aa935167d123ebc6322a5f753171e457cd26615b6c8cea6dcc8648`  
		Last Modified: Thu, 17 Dec 2020 08:07:31 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17cb6f51130bdca075886a326b2ea4010f9a422c82d02cdb21ff7fb1bcd6936`  
		Last Modified: Thu, 17 Dec 2020 08:07:31 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be36f075387368e209d8070b657d29265f14a5973ff3b1a2e35d25026ed5a5aa`  
		Last Modified: Thu, 07 Jan 2021 18:51:40 GMT  
		Size: 10.3 MB (10345694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb56c83b6fb4b53b79cd6be36dcaad783ca0fb93aff58d5bc032f004cc60e7e6`  
		Last Modified: Thu, 07 Jan 2021 18:51:38 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876922b31665d098cf4c4c3cb30a9c571a5d290b57f1b9195d3e883e471cc4a1`  
		Last Modified: Thu, 07 Jan 2021 18:51:39 GMT  
		Size: 13.6 MB (13555331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2056cab53bbd46b18087ece6e80f2672cca2a6a53409904f2186e9da1790444`  
		Last Modified: Thu, 21 Jan 2021 20:10:59 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34b186682790013c093714b1a689be01d8b67fe8bc0932edfefa75c4c1b1a4ce`  
		Last Modified: Thu, 21 Jan 2021 20:10:59 GMT  
		Size: 16.9 KB (16899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4bdf8e06ea67ff49369259874a92531ea040952dc90d300bde0b1c80cf910dd`  
		Last Modified: Thu, 21 Jan 2021 20:10:59 GMT  
		Size: 8.5 KB (8451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05cb6b4af7fd02d3898487e4d17607b7e3b66e902c358c58f882b39f37231ddd`  
		Last Modified: Thu, 21 Jan 2021 22:23:09 GMT  
		Size: 271.9 KB (271866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326929effc24392485c9cf1fec5975844920b737524147e2aa7a08ab3471444b`  
		Last Modified: Thu, 21 Jan 2021 22:23:09 GMT  
		Size: 26.4 MB (26418592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08bfa70cb15c72595be03cb4700f911e575cd5f76769de0689cba204494b9d21`  
		Last Modified: Thu, 21 Jan 2021 22:23:07 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f83f64d60a2692b2c54a327d093b50851092b9496b7840086c907df6301ded`  
		Last Modified: Tue, 26 Jan 2021 01:29:08 GMT  
		Size: 118.7 MB (118671051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59710edd5c459b67e87fc11edf9525ffc0a8c75ac6ab51b5fcc3f6df241e5e19`  
		Last Modified: Tue, 26 Jan 2021 01:28:53 GMT  
		Size: 2.5 KB (2532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb0c46133cce7cd331bbe0fb857b278e528c8ce6a58a1551b1218f4caa62b4a0`  
		Last Modified: Tue, 26 Jan 2021 01:28:53 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
