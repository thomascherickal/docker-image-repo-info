## `nextcloud:18-fpm-alpine`

```console
$ docker pull nextcloud@sha256:223cc1dd271efaa93bf5cd445ea331f8ecf32cbd1b3ea28630672ed22860e2e3
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

### `nextcloud:18-fpm-alpine` - linux; amd64

```console
$ docker pull nextcloud@sha256:14a8dffc003f61036d5aacb3425d94b0ce2b51b99a8241f113401f635544516d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.6 MB (159625544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:01de8a72aa48077472f940f5b4142139f0757a00884ee35e656ebb09981ca01b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 06:30:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 22 Oct 2020 06:30:14 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 22 Oct 2020 06:30:15 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 22 Oct 2020 06:30:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Oct 2020 06:30:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Oct 2020 06:37:19 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 22 Oct 2020 06:37:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 06:37:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 06:37:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Oct 2020 07:05:56 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 22 Oct 2020 07:05:56 GMT
ENV PHP_VERSION=7.3.23
# Thu, 22 Oct 2020 07:05:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.23.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.23.tar.xz.asc
# Thu, 22 Oct 2020 07:05:56 GMT
ENV PHP_SHA256=2bdd36176f318f451fb3942bf1e935aabb3c2786cac41a9080f084ad6390e034 PHP_MD5=
# Thu, 22 Oct 2020 07:05:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 22 Oct 2020 07:06:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 22 Oct 2020 07:11:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 22 Oct 2020 07:11:23 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 22 Oct 2020 07:11:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 22 Oct 2020 07:11:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 22 Oct 2020 07:11:24 GMT
WORKDIR /var/www/html
# Thu, 22 Oct 2020 07:11:25 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 22 Oct 2020 07:11:25 GMT
STOPSIGNAL SIGQUIT
# Thu, 22 Oct 2020 07:11:25 GMT
EXPOSE 9000
# Thu, 22 Oct 2020 07:11:25 GMT
CMD ["php-fpm"]
# Thu, 22 Oct 2020 10:06:46 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 22 Oct 2020 10:10:00 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Thu, 22 Oct 2020 10:10:01 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 22 Oct 2020 10:10:01 GMT
VOLUME [/var/www/html]
# Thu, 22 Oct 2020 10:10:54 GMT
ENV NEXTCLOUD_VERSION=18.0.10
# Thu, 22 Oct 2020 10:11:29 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Thu, 22 Oct 2020 10:11:31 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Thu, 22 Oct 2020 10:11:33 GMT
COPY multi:c481008845253a7b26785f1b012d068624b67ddaaefbb62c1931fdf56fd06e2a in /usr/src/nextcloud/config/ 
# Thu, 22 Oct 2020 10:11:33 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Oct 2020 10:11:33 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f8bf6cfdbe614fef94f982905079c16e27b3de2d24eb1ff513d3d83e656ca2`  
		Last Modified: Thu, 22 Oct 2020 07:36:55 GMT  
		Size: 1.3 MB (1340771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5be79740125b9e74a77885bf6ee2b0d25ac7ed9e9432c5aa7210bb3b00458a`  
		Last Modified: Thu, 22 Oct 2020 07:36:55 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99dd6507fe563b66ba35badf706e1bbb2d39eb5d0a3c0d5a86a45d2af7e89c1`  
		Last Modified: Thu, 22 Oct 2020 07:36:55 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2983ef245bc3edcae1e478af4d486f6de1854e309dfe8c4d7cf1016521d7d3e`  
		Last Modified: Thu, 22 Oct 2020 07:38:43 GMT  
		Size: 12.2 MB (12152879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b9b2161b2a2e4b6465ed19b348672ba2718368e48bda5384dc8bf8e5a98a4c`  
		Last Modified: Thu, 22 Oct 2020 07:38:39 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6210a44118c5adfaacadc385d0bdc55d01cecfffe99b4baf117105c9fad613`  
		Last Modified: Thu, 22 Oct 2020 07:38:41 GMT  
		Size: 14.5 MB (14460741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cecf40903dc1a0df30c73bc8b72ef5387aea6144134be380531d4114445bf0c4`  
		Last Modified: Thu, 22 Oct 2020 07:38:38 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e615fbd8fb8f6eac534151151e41780f6b722a82225150d365261209da26fbba`  
		Last Modified: Thu, 22 Oct 2020 07:38:38 GMT  
		Size: 16.7 KB (16703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a2bf4ae57cb2b3b511303233ea39273339fdf7ea2baa12a4ef192388ca19d7a`  
		Last Modified: Thu, 22 Oct 2020 07:38:38 GMT  
		Size: 8.4 KB (8410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4456d2345676e59df443e9c7b9eb83de2186f4f696e0aff787db1d418f3e914b`  
		Last Modified: Thu, 22 Oct 2020 10:18:38 GMT  
		Size: 257.9 KB (257923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8370641481b533e730cbd6779c7073112521640545b2b07fc2325a1e4f2088e`  
		Last Modified: Thu, 22 Oct 2020 10:18:43 GMT  
		Size: 26.4 MB (26365576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a7c3da8ee380192c32f7d3a610f2e956e76d33b8738e17edac2567573c46d0`  
		Last Modified: Thu, 22 Oct 2020 10:18:37 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:706d2c214c001133f86392970575004118fd034c24e4542e1986f90b70bd5fc1`  
		Last Modified: Thu, 22 Oct 2020 10:19:19 GMT  
		Size: 102.2 MB (102216551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a01a969ee1d52d1bdb2f24d22f58527b4f66a5b811b32a009c4dddf78d10d09a`  
		Last Modified: Thu, 22 Oct 2020 10:19:02 GMT  
		Size: 2.5 KB (2525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c888fe91e2f98539a4ef8dcf2d1370de4d3efca16ba1125098cd633186e0e7e7`  
		Last Modified: Thu, 22 Oct 2020 10:19:02 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:18-fpm-alpine` - linux; arm variant v6

```console
$ docker pull nextcloud@sha256:04b07579371df0149e3523d02b81b37a56232005727d102df7f7d0a445df9a70
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.1 MB (158078611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0e3dbb016de13789aebeb595d8ed27bf09e27b9113f705d76ecbee84d07f8e7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:14:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:14:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:14:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:14:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:14:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:20:14 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 11 Jun 2020 18:20:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:20:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:20:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:49:43 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 01 Oct 2020 19:23:14 GMT
ENV PHP_VERSION=7.3.23
# Thu, 01 Oct 2020 19:23:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.23.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.23.tar.xz.asc
# Thu, 01 Oct 2020 19:23:17 GMT
ENV PHP_SHA256=2bdd36176f318f451fb3942bf1e935aabb3c2786cac41a9080f084ad6390e034 PHP_MD5=
# Thu, 01 Oct 2020 19:23:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Oct 2020 19:23:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Oct 2020 19:27:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Oct 2020 19:27:41 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 01 Oct 2020 19:27:45 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Oct 2020 19:27:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Oct 2020 19:27:47 GMT
WORKDIR /var/www/html
# Thu, 01 Oct 2020 19:27:51 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Oct 2020 19:27:52 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Oct 2020 19:27:53 GMT
EXPOSE 9000
# Thu, 01 Oct 2020 19:27:55 GMT
CMD ["php-fpm"]
# Thu, 01 Oct 2020 20:31:24 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 08 Oct 2020 18:54:31 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Thu, 08 Oct 2020 18:54:33 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 08 Oct 2020 18:54:34 GMT
VOLUME [/var/www/html]
# Thu, 08 Oct 2020 19:02:21 GMT
ENV NEXTCLOUD_VERSION=18.0.10
# Thu, 08 Oct 2020 19:10:56 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Thu, 08 Oct 2020 19:11:04 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Thu, 08 Oct 2020 19:11:07 GMT
COPY multi:c481008845253a7b26785f1b012d068624b67ddaaefbb62c1931fdf56fd06e2a in /usr/src/nextcloud/config/ 
# Thu, 08 Oct 2020 19:11:08 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Oct 2020 19:11:09 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72788d65e292354c2ce4b67441d334d0ba534db5ce71d5b8bf78011a256b566f`  
		Last Modified: Thu, 11 Jun 2020 19:29:37 GMT  
		Size: 1.3 MB (1310273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e32d62de43da999aca07cf15fdbe1cd6b03aebc88c15409c3463daadf13e01`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6701e05673b745147608cd1b6eb47a3fbc35bcfd8a65bc536e5b9f919b3d0e77`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:489443dcc73fbbd84c734b0c972fb47570adbe0fd884c17ce75ced52f7fcc604`  
		Last Modified: Thu, 01 Oct 2020 20:24:12 GMT  
		Size: 12.2 MB (12152952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6b13774b88f60049c79c26a3f080253dec7b3b4a3e85126592b6e8b61019d2`  
		Last Modified: Thu, 01 Oct 2020 20:24:08 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f408f7d33b125ea6bd3c52a9ebe9535456bf0631044b657ee30dfdc6b6a7af9f`  
		Last Modified: Thu, 01 Oct 2020 20:24:14 GMT  
		Size: 14.0 MB (14016382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91b79a39bc722e7e25701b916af72b6effe971ac0eb8bcac4b9bb2864025c9b7`  
		Last Modified: Thu, 01 Oct 2020 20:24:09 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fda88aafbc14d1f005e9cf950e86615445192e2fcee44b75402644494f85213`  
		Last Modified: Thu, 01 Oct 2020 20:24:09 GMT  
		Size: 16.8 KB (16822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab61c9396a490dfbf23d0fc4a299fa10efa8e9f4b40c245adf6090f3c06b8f2f`  
		Last Modified: Thu, 01 Oct 2020 20:24:09 GMT  
		Size: 8.4 KB (8414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e95b238242358357267a6b0ab4e1d02fef924a1dac160d0c55d1b71a8f775ae6`  
		Last Modified: Thu, 01 Oct 2020 20:46:34 GMT  
		Size: 268.5 KB (268543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfcffc15d8680184206ba9ea49f2a34bc7975ff0636a6462e4cc71430b5ad0d`  
		Last Modified: Thu, 08 Oct 2020 19:28:46 GMT  
		Size: 25.5 MB (25476019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3235d395ee0057ea58011931e7b56b13b050943189df96d565d01665506ee8`  
		Last Modified: Thu, 08 Oct 2020 19:28:38 GMT  
		Size: 528.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e44bd17e343adcdb887e328394de06b7b2a9a2f12e95bcc872f06ed3d2bb3ae`  
		Last Modified: Thu, 08 Oct 2020 19:29:50 GMT  
		Size: 102.2 MB (102216677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ee11c781559a7634636389ed63b61aa9cf6856a4e7439c457fa8fcc6e1ff1e9`  
		Last Modified: Thu, 08 Oct 2020 19:29:14 GMT  
		Size: 2.5 KB (2524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:598bc6f8dc04b68d70a4ef1547e69393520edf33707a09ea6fec8548a9dd2809`  
		Last Modified: Thu, 08 Oct 2020 19:29:14 GMT  
		Size: 1.9 KB (1891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:18-fpm-alpine` - linux; arm variant v7

```console
$ docker pull nextcloud@sha256:7c68c41b12916c54220aea615ecc4a79938c39de38af1e8bd8d7e7fe546a7e27
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **155.8 MB (155774066 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:856285d78e3aa141ca4e632492f5207b8ca7bd6589d6c790a3ff6bd0eb721c4a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 06:47:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 22 Oct 2020 06:47:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 22 Oct 2020 06:47:45 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 22 Oct 2020 06:47:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Oct 2020 06:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Oct 2020 06:51:33 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 22 Oct 2020 06:51:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 06:51:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 06:51:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Oct 2020 07:14:09 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 22 Oct 2020 07:14:10 GMT
ENV PHP_VERSION=7.3.23
# Thu, 22 Oct 2020 07:14:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.23.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.23.tar.xz.asc
# Thu, 22 Oct 2020 07:14:11 GMT
ENV PHP_SHA256=2bdd36176f318f451fb3942bf1e935aabb3c2786cac41a9080f084ad6390e034 PHP_MD5=
# Thu, 22 Oct 2020 07:14:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 22 Oct 2020 07:14:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 22 Oct 2020 07:17:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 22 Oct 2020 07:17:15 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 22 Oct 2020 07:17:23 GMT
RUN docker-php-ext-enable sodium
# Thu, 22 Oct 2020 07:17:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 22 Oct 2020 07:17:28 GMT
WORKDIR /var/www/html
# Thu, 22 Oct 2020 07:17:38 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 22 Oct 2020 07:17:40 GMT
STOPSIGNAL SIGQUIT
# Thu, 22 Oct 2020 07:17:41 GMT
EXPOSE 9000
# Thu, 22 Oct 2020 07:17:42 GMT
CMD ["php-fpm"]
# Thu, 22 Oct 2020 10:43:23 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 22 Oct 2020 10:46:36 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Thu, 22 Oct 2020 10:46:39 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 22 Oct 2020 10:46:42 GMT
VOLUME [/var/www/html]
# Thu, 22 Oct 2020 10:47:53 GMT
ENV NEXTCLOUD_VERSION=18.0.10
# Thu, 22 Oct 2020 10:48:43 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Thu, 22 Oct 2020 10:48:49 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Thu, 22 Oct 2020 10:48:55 GMT
COPY multi:c481008845253a7b26785f1b012d068624b67ddaaefbb62c1931fdf56fd06e2a in /usr/src/nextcloud/config/ 
# Thu, 22 Oct 2020 10:48:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Oct 2020 10:48:59 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60b50c98f8a8e2c6a27378dfa0f44df1844ac67c6981303675f138a42679f25`  
		Last Modified: Thu, 22 Oct 2020 07:35:57 GMT  
		Size: 1.2 MB (1214265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b472094d673b7c272085505c976192b9aaafa3157c99bade9755fbca18a24071`  
		Last Modified: Thu, 22 Oct 2020 07:35:56 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc39e5d916c11e7eb158e72d14ab981eb45ccc7b6451c1d6d3cb627b71cdbb6`  
		Last Modified: Thu, 22 Oct 2020 07:35:55 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50aa0b5ddfdddb62d168c14d2b8df34b5eb26452cb303c03bc51e3f226191024`  
		Last Modified: Thu, 22 Oct 2020 07:38:25 GMT  
		Size: 12.2 MB (12152900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce2b0915425acb7d227981ef34152b577bf8c1b7d6ceb869bb0dfb4eb06047b9`  
		Last Modified: Thu, 22 Oct 2020 07:38:21 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251023d43999b66aa77b3b4c39b8161fe029bd57d27a4dbfaa36ee8c9ccd5b5e`  
		Last Modified: Thu, 22 Oct 2020 07:38:26 GMT  
		Size: 12.6 MB (12559186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe41f6e6979b804447ee1f4f3d34da2598940e4b5ea8f5787579c30fdd9e182d`  
		Last Modified: Thu, 22 Oct 2020 07:38:21 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6042b2be2aacea7027cf3ecd0c0a9ea4a8d80cbd05ea53533b5026f333923c8`  
		Last Modified: Thu, 22 Oct 2020 07:38:22 GMT  
		Size: 16.7 KB (16690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdbaa539565cb9ec6a4bcaf6cad8f7ad04bd1f9d14bd50d3f70c1273bb2755e3`  
		Last Modified: Thu, 22 Oct 2020 07:38:21 GMT  
		Size: 8.4 KB (8412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce0c00368248c983a7a6bdcf2dda5f19df34eb416f4ee4da01e84d6cd74bffcb`  
		Last Modified: Thu, 22 Oct 2020 10:56:04 GMT  
		Size: 242.9 KB (242867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d723d1454777f75c077e9c94729c3e9ea304b961239b8feb9571d53febbcb0d`  
		Last Modified: Thu, 22 Oct 2020 10:56:09 GMT  
		Size: 24.9 MB (24948410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b247d3eb2c0af31f719fdcf35ef6e8bcdbfae8387b05726f1f79cf3de49e4c71`  
		Last Modified: Thu, 22 Oct 2020 10:56:02 GMT  
		Size: 523.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42fac2a9ecf9d2ba0015afec203995dea560f7ac0609dfd7ae7cee5edac8b150`  
		Last Modified: Thu, 22 Oct 2020 10:57:14 GMT  
		Size: 102.2 MB (102216430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a22fbfc3e672ec1fb03b49d2e14f0c66c159c085a55d5c747f4c176b0548cbbd`  
		Last Modified: Thu, 22 Oct 2020 10:56:40 GMT  
		Size: 2.5 KB (2525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a352075281c65c06966960e73fb04689e2b7e32c6014f7898733eda8d09918c`  
		Last Modified: Thu, 22 Oct 2020 10:56:40 GMT  
		Size: 1.9 KB (1889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:18-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull nextcloud@sha256:8607a7a0e565e9e7684b099b2907500ecfa30a6b5561c6584b334adb560be5d8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **159.1 MB (159100138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f47ced32623021784d7c9448420cb61ebf5636ed59a50f7fd7bca4262e1cc6d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 07:18:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 22 Oct 2020 07:18:56 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 22 Oct 2020 07:18:59 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 22 Oct 2020 07:19:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Oct 2020 07:19:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Oct 2020 07:23:16 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 22 Oct 2020 07:23:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 07:23:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 07:23:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Oct 2020 07:44:56 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 22 Oct 2020 07:44:56 GMT
ENV PHP_VERSION=7.3.23
# Thu, 22 Oct 2020 07:44:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.23.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.23.tar.xz.asc
# Thu, 22 Oct 2020 07:44:58 GMT
ENV PHP_SHA256=2bdd36176f318f451fb3942bf1e935aabb3c2786cac41a9080f084ad6390e034 PHP_MD5=
# Thu, 22 Oct 2020 07:45:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 22 Oct 2020 07:45:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 22 Oct 2020 07:47:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 22 Oct 2020 07:47:54 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 22 Oct 2020 07:47:58 GMT
RUN docker-php-ext-enable sodium
# Thu, 22 Oct 2020 07:48:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 22 Oct 2020 07:48:00 GMT
WORKDIR /var/www/html
# Thu, 22 Oct 2020 07:48:02 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 22 Oct 2020 07:48:03 GMT
STOPSIGNAL SIGQUIT
# Thu, 22 Oct 2020 07:48:04 GMT
EXPOSE 9000
# Thu, 22 Oct 2020 07:48:04 GMT
CMD ["php-fpm"]
# Thu, 22 Oct 2020 10:50:34 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 22 Oct 2020 10:54:05 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Thu, 22 Oct 2020 10:54:08 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 22 Oct 2020 10:54:09 GMT
VOLUME [/var/www/html]
# Thu, 22 Oct 2020 10:55:24 GMT
ENV NEXTCLOUD_VERSION=18.0.10
# Thu, 22 Oct 2020 10:56:00 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Thu, 22 Oct 2020 10:56:03 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Thu, 22 Oct 2020 10:56:06 GMT
COPY multi:c481008845253a7b26785f1b012d068624b67ddaaefbb62c1931fdf56fd06e2a in /usr/src/nextcloud/config/ 
# Thu, 22 Oct 2020 10:56:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Oct 2020 10:56:07 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d57dba23203172f8fffd1379aef0307e782178b62dfc684d43c546f7e874ed`  
		Last Modified: Thu, 22 Oct 2020 08:06:21 GMT  
		Size: 1.3 MB (1342784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8414edb0c9c2f7472bb6228bf691a2ddac19ddad7bad789c7cbdc147aded711`  
		Last Modified: Thu, 22 Oct 2020 08:06:20 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d26eeef0db35b2328adae38a8490c7403844452c3606dd17fbe68216f98e82`  
		Last Modified: Thu, 22 Oct 2020 08:06:19 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d043b147eee71d644d8e5f9b89c136c33f7a711b36c5e547b08bb8bc44abfde7`  
		Last Modified: Thu, 22 Oct 2020 08:08:40 GMT  
		Size: 12.2 MB (12152914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1a3edf60c684d2d303a4b2d5ecf4fd45d0d39a0a2e8b1b47b208e8b2a701c8`  
		Last Modified: Thu, 22 Oct 2020 08:08:37 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0120bb47eea1800a5e39002a13f5efa8b75896985d35156f386f62eaf3e418f7`  
		Last Modified: Thu, 22 Oct 2020 08:08:40 GMT  
		Size: 14.2 MB (14199662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c017f2147e47f9d3101b5a9cb269ba71b6f16d0c058eee52993ad704386d0849`  
		Last Modified: Thu, 22 Oct 2020 08:08:36 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c04e158c324e2bef959dd66d46a542efc00e9bdea2955136e39a62b0f2415e32`  
		Last Modified: Thu, 22 Oct 2020 08:08:36 GMT  
		Size: 16.7 KB (16714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be8d87905d1d436833ac6110a78f2cb12867a4d5202465c265a473e71292ae98`  
		Last Modified: Thu, 22 Oct 2020 08:08:36 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70024380aad4acad63ec93e6f9b2fddcc786b75410c9bfc66e542a04df16109`  
		Last Modified: Thu, 22 Oct 2020 11:02:36 GMT  
		Size: 268.8 KB (268768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e7db933a5cf813aaa6478cc055cc4e287c8a956c13ca761f1d8e2bb1d1eab2`  
		Last Modified: Thu, 22 Oct 2020 11:02:40 GMT  
		Size: 26.2 MB (26178627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c42f642c3c7b356261c9608fc330b6c64977e6275e172a604ed8a982617c79`  
		Last Modified: Thu, 22 Oct 2020 11:02:34 GMT  
		Size: 526.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2375b1ed594d4b958a967d2e902825b544925e9a9ecfa5aa1d65edb90205e979`  
		Last Modified: Thu, 22 Oct 2020 11:03:29 GMT  
		Size: 102.2 MB (102216466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b764e9b8596a27117c058fd0d44c5843c63f36c1b02f2d1ee4749fd13ff0f73`  
		Last Modified: Thu, 22 Oct 2020 11:03:05 GMT  
		Size: 2.5 KB (2524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88764cb6b07e46f4df88a9b3995c44e237820265513a8e23193ee2525d235568`  
		Last Modified: Thu, 22 Oct 2020 11:03:06 GMT  
		Size: 1.9 KB (1888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:18-fpm-alpine` - linux; 386

```console
$ docker pull nextcloud@sha256:547160ac77c4dbb6663d1d7206f14fed6e5c0296f661b2808203cdf0b17100bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.6 MB (160571435 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac6574916926e1973824890a6fa8a8ae2c9d76c0f5843edecdd81e1ae076b70b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:36:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 22 Oct 2020 03:36:26 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 22 Oct 2020 03:36:27 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 22 Oct 2020 03:36:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Oct 2020 03:36:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Oct 2020 03:45:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 22 Oct 2020 03:45:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 03:45:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 03:45:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Oct 2020 04:25:30 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 22 Oct 2020 04:25:31 GMT
ENV PHP_VERSION=7.3.23
# Thu, 22 Oct 2020 04:25:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.23.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.23.tar.xz.asc
# Thu, 22 Oct 2020 04:25:31 GMT
ENV PHP_SHA256=2bdd36176f318f451fb3942bf1e935aabb3c2786cac41a9080f084ad6390e034 PHP_MD5=
# Thu, 22 Oct 2020 04:25:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 22 Oct 2020 04:25:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 22 Oct 2020 04:32:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 22 Oct 2020 04:32:17 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 22 Oct 2020 04:32:18 GMT
RUN docker-php-ext-enable sodium
# Thu, 22 Oct 2020 04:32:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 22 Oct 2020 04:32:18 GMT
WORKDIR /var/www/html
# Thu, 22 Oct 2020 04:32:19 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 22 Oct 2020 04:32:19 GMT
STOPSIGNAL SIGQUIT
# Thu, 22 Oct 2020 04:32:20 GMT
EXPOSE 9000
# Thu, 22 Oct 2020 04:32:20 GMT
CMD ["php-fpm"]
# Thu, 22 Oct 2020 10:56:13 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 22 Oct 2020 10:58:27 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Thu, 22 Oct 2020 10:58:28 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 22 Oct 2020 10:58:28 GMT
VOLUME [/var/www/html]
# Thu, 22 Oct 2020 10:59:22 GMT
ENV NEXTCLOUD_VERSION=18.0.10
# Thu, 22 Oct 2020 10:59:54 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Thu, 22 Oct 2020 10:59:55 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Thu, 22 Oct 2020 10:59:55 GMT
COPY multi:c481008845253a7b26785f1b012d068624b67ddaaefbb62c1931fdf56fd06e2a in /usr/src/nextcloud/config/ 
# Thu, 22 Oct 2020 10:59:56 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Oct 2020 10:59:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30be8ffd290910905a5fb7cbb70252eb0f59edb09db20bdc21f3b65456acc28f`  
		Last Modified: Thu, 22 Oct 2020 05:10:23 GMT  
		Size: 1.4 MB (1439641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d58e2433b13446c863e85b34f8e4c93ca9d5b3b93d2bac415fd9cdf77bcec4`  
		Last Modified: Thu, 22 Oct 2020 05:10:21 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5729dcb8d303f82a7f8cf3df49048e34ce8ee89f79155fb08a475da46b64308`  
		Last Modified: Thu, 22 Oct 2020 05:10:21 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be25704001833c565e517de4a5d64c8af161c9c9d1fb5b08d037b6382349e0f`  
		Last Modified: Thu, 22 Oct 2020 05:13:10 GMT  
		Size: 12.2 MB (12152871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e6fc43b81d2b73a369a6b0b448edde83a51d66a005ea88459e0d4a0b94b3886`  
		Last Modified: Thu, 22 Oct 2020 05:13:06 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f8b979938d2ca05c00a0a19c75111c2ca9fb8582da281ba427188c979ae1bb2`  
		Last Modified: Thu, 22 Oct 2020 05:13:12 GMT  
		Size: 14.8 MB (14829499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa3194fb3bdc8a55005cb9451e65a51d1006c8da69b14dcf803eddaf618134c`  
		Last Modified: Thu, 22 Oct 2020 05:13:06 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06a7821c3d70c250c78ee1e01a170e8f414a492f8d585688f7f0887fd4cda0d`  
		Last Modified: Thu, 22 Oct 2020 05:13:06 GMT  
		Size: 16.7 KB (16699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd372ce2dcad10fed76b4a57ad79e749aaf110a4d489c3009699c77aa3330bb7`  
		Last Modified: Thu, 22 Oct 2020 05:13:06 GMT  
		Size: 8.4 KB (8411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5189d462ead5b1bb7b588273d10e178de11eb98297077e3c5604893f437adf3`  
		Last Modified: Thu, 22 Oct 2020 11:04:41 GMT  
		Size: 276.6 KB (276624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a50e0b9e6dacc4d3baa3840bb20f557af36a5436553398a499940129f40f92`  
		Last Modified: Thu, 22 Oct 2020 11:04:47 GMT  
		Size: 26.8 MB (26830872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25cab4b10d6cadb0893d1a8ba3ce45725682746e44bd652dc4f027f5164fced0`  
		Last Modified: Thu, 22 Oct 2020 11:04:39 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6938767b7408a820c04b9ebfee065d7f145e7347d3d76083173188339d456a`  
		Last Modified: Thu, 22 Oct 2020 11:05:37 GMT  
		Size: 102.2 MB (102216279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae82e22dbe35a72c263de30b32e34b1bb698e57a50915251a3436e1b5b7750a`  
		Last Modified: Thu, 22 Oct 2020 11:05:15 GMT  
		Size: 2.5 KB (2523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea0cdb9c91ceb3d17713af07e02ebca0387d2ca8918f1b4169d18e4ffa6e4daa`  
		Last Modified: Thu, 22 Oct 2020 11:05:14 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:18-fpm-alpine` - linux; ppc64le

```console
$ docker pull nextcloud@sha256:f16885ad99c372a321351ff42a4286a44f816b737c202fb4ae37b63e9621db9c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **161.7 MB (161667823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a84568bed1281bdafeb283c9ed53b42442f483f95eeb365c7aea34750b832266`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:45:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:45:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:45:29 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:45:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:45:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:50:39 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 11 Jun 2020 18:50:43 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:50:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:50:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 20:12:17 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 01 Oct 2020 20:59:22 GMT
ENV PHP_VERSION=7.3.23
# Thu, 01 Oct 2020 20:59:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.23.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.23.tar.xz.asc
# Thu, 01 Oct 2020 20:59:31 GMT
ENV PHP_SHA256=2bdd36176f318f451fb3942bf1e935aabb3c2786cac41a9080f084ad6390e034 PHP_MD5=
# Thu, 01 Oct 2020 20:59:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Oct 2020 20:59:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Oct 2020 21:03:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Oct 2020 21:03:57 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 01 Oct 2020 21:04:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Oct 2020 21:04:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Oct 2020 21:04:14 GMT
WORKDIR /var/www/html
# Thu, 01 Oct 2020 21:04:31 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Oct 2020 21:04:35 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Oct 2020 21:04:39 GMT
EXPOSE 9000
# Thu, 01 Oct 2020 21:04:45 GMT
CMD ["php-fpm"]
# Thu, 01 Oct 2020 23:14:14 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 08 Oct 2020 21:30:44 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Thu, 08 Oct 2020 21:31:07 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 08 Oct 2020 21:31:13 GMT
VOLUME [/var/www/html]
# Thu, 08 Oct 2020 22:17:39 GMT
ENV NEXTCLOUD_VERSION=18.0.10
# Thu, 08 Oct 2020 22:20:28 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Thu, 08 Oct 2020 22:20:42 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Thu, 08 Oct 2020 22:20:46 GMT
COPY multi:c481008845253a7b26785f1b012d068624b67ddaaefbb62c1931fdf56fd06e2a in /usr/src/nextcloud/config/ 
# Thu, 08 Oct 2020 22:20:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 08 Oct 2020 22:20:57 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f98eb9049c4fcbaa1cf16ddb44aaf910a89a5471dc303198251fa25bc2a1ef`  
		Last Modified: Thu, 11 Jun 2020 20:57:07 GMT  
		Size: 1.4 MB (1383311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50cdb8e03fc1b19217cd9f80b86142d090ad3e818795b339ea4d9ef9b74555f`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4466e085b12b265fb47397c7c105fd7d78a5883beef49ab9f386393c4c3dae`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f12ff83f31906267a98a02c4f6dd2e42810221784f256e151fb16a74da5431e`  
		Last Modified: Thu, 01 Oct 2020 22:45:21 GMT  
		Size: 12.2 MB (12152966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d1edd1c9ba42fc153dba2c031acd679ba63761a6ccc79c971d39d5ce2a4028a`  
		Last Modified: Thu, 01 Oct 2020 22:45:14 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aaafa54aebf41e4007318a22012b29e47c460cee34d08ca978e95a1a5806e92`  
		Last Modified: Thu, 01 Oct 2020 22:45:25 GMT  
		Size: 16.1 MB (16097228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b294f6824469300cdaba5a13610a8f4ada7fe7a8de6176e3c840c4890c6558dd`  
		Last Modified: Thu, 01 Oct 2020 22:45:14 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3842402e11253d967c947d1b00b913ef378fb58dcaff8ac92b6df6f00aaaebde`  
		Last Modified: Thu, 01 Oct 2020 22:45:14 GMT  
		Size: 16.8 KB (16836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2f159b28a8c485104a53e20d2162b435c5035de64de7bab031bd6dbbeccc70`  
		Last Modified: Thu, 01 Oct 2020 22:45:15 GMT  
		Size: 8.4 KB (8412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551241666ee93ba84d5b9bbe9e9fcd6a21dc7921f3a3a7c436dc234f308264bf`  
		Last Modified: Fri, 02 Oct 2020 01:00:58 GMT  
		Size: 274.3 KB (274323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a32b248f1da5cf2539181ac02e60687cd0c8665e960f954384f8a77600c8ec`  
		Last Modified: Thu, 08 Oct 2020 23:43:08 GMT  
		Size: 26.7 MB (26703519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c51d552bb53c595b6ecbed95bb83153e95c2e106ab5a7139b7ff9c33cb5289`  
		Last Modified: Thu, 08 Oct 2020 23:42:45 GMT  
		Size: 531.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a9cd5eaf2a7c668429ad3db3be220be882987f7cf17f432d3f6e5479f48e082`  
		Last Modified: Thu, 08 Oct 2020 23:54:32 GMT  
		Size: 102.2 MB (102216781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84e91ec050bd87f586e9fb9f801c429122c8088ae78730256ce78b6e53b05033`  
		Last Modified: Thu, 08 Oct 2020 23:50:58 GMT  
		Size: 2.5 KB (2521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8cadec99d15bcc43a5e9a78d6218b37994534658e4bbcc481068e5c350151c`  
		Last Modified: Thu, 08 Oct 2020 23:50:59 GMT  
		Size: 1.9 KB (1894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nextcloud:18-fpm-alpine` - linux; s390x

```console
$ docker pull nextcloud@sha256:24e3d8ea1a9f8d2a5e33a0335696b8e3176803c8d122c67e50e3aa028bd15683
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.6 MB (158629597 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aee69f48b9a3dc7923d34a6b8b5664959a9eb6c3288f1ea8b12fe6c0183c31e4`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:34:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 22 Oct 2020 04:34:29 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 22 Oct 2020 04:34:31 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 22 Oct 2020 04:34:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Oct 2020 04:34:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Oct 2020 04:39:19 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 22 Oct 2020 04:39:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 04:39:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 04:39:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Oct 2020 05:02:34 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 22 Oct 2020 05:02:34 GMT
ENV PHP_VERSION=7.3.23
# Thu, 22 Oct 2020 05:02:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.23.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.23.tar.xz.asc
# Thu, 22 Oct 2020 05:02:35 GMT
ENV PHP_SHA256=2bdd36176f318f451fb3942bf1e935aabb3c2786cac41a9080f084ad6390e034 PHP_MD5=
# Thu, 22 Oct 2020 05:02:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 22 Oct 2020 05:02:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 22 Oct 2020 05:07:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 22 Oct 2020 05:07:18 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 22 Oct 2020 05:07:20 GMT
RUN docker-php-ext-enable sodium
# Thu, 22 Oct 2020 05:07:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 22 Oct 2020 05:07:21 GMT
WORKDIR /var/www/html
# Thu, 22 Oct 2020 05:07:23 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 22 Oct 2020 05:07:23 GMT
STOPSIGNAL SIGQUIT
# Thu, 22 Oct 2020 05:07:24 GMT
EXPOSE 9000
# Thu, 22 Oct 2020 05:07:24 GMT
CMD ["php-fpm"]
# Thu, 22 Oct 2020 10:44:38 GMT
RUN set -ex;         apk add --no-cache         rsync     ;         rm /var/spool/cron/crontabs/root;     echo '*/5 * * * * php -f /var/www/html/cron.php' > /var/spool/cron/crontabs/www-data
# Thu, 22 Oct 2020 10:47:39 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         $PHPIZE_DEPS         autoconf         freetype-dev         icu-dev         libevent-dev         libjpeg-turbo-dev         libmcrypt-dev         libpng-dev         libmemcached-dev         libxml2-dev         libzip-dev         openldap-dev         pcre-dev         postgresql-dev         imagemagick-dev         libwebp-dev         gmp-dev     ;         docker-php-ext-configure gd --with-freetype-dir=/usr --with-png-dir=/usr --with-jpeg-dir=/usr --with-webp-dir=/usr;     docker-php-ext-configure ldap;     docker-php-ext-install -j "$(nproc)"         exif         gd         intl         ldap         opcache         pcntl         pdo_mysql         pdo_pgsql         zip         gmp     ;         pecl install APCu-5.1.19;     pecl install memcached-3.1.5;     pecl install redis-4.3.0;     pecl install imagick-3.4.4;         docker-php-ext-enable         apcu         memcached         redis         imagick     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .nextcloud-phpext-rundeps $runDeps;     apk del .build-deps
# Thu, 22 Oct 2020 10:47:44 GMT
RUN {         echo 'opcache.enable=1';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=10000';         echo 'opcache.memory_consumption=128';         echo 'opcache.save_comments=1';         echo 'opcache.revalidate_freq=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini;         echo 'apc.enable_cli=1' >> /usr/local/etc/php/conf.d/docker-php-ext-apcu.ini;         echo 'memory_limit=512M' > /usr/local/etc/php/conf.d/memory-limit.ini;         mkdir /var/www/data;     chown -R www-data:root /var/www;     chmod -R g=u /var/www
# Thu, 22 Oct 2020 10:47:45 GMT
VOLUME [/var/www/html]
# Thu, 22 Oct 2020 10:49:07 GMT
ENV NEXTCLOUD_VERSION=18.0.10
# Thu, 22 Oct 2020 10:49:42 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         bzip2         gnupg     ;         curl -fsSL -o nextcloud.tar.bz2         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2";     curl -fsSL -o nextcloud.tar.bz2.asc         "https://download.nextcloud.com/server/releases/nextcloud-${NEXTCLOUD_VERSION}.tar.bz2.asc";     export GNUPGHOME="$(mktemp -d)";     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 28806A878AE423A28372792ED75899B9A724937A;     gpg --batch --verify nextcloud.tar.bz2.asc nextcloud.tar.bz2;     tar -xjf nextcloud.tar.bz2 -C /usr/src/;     gpgconf --kill all;     rm nextcloud.tar.bz2.asc nextcloud.tar.bz2;     rm -rf "$GNUPGHOME" /usr/src/nextcloud/updater;     mkdir -p /usr/src/nextcloud/data;     mkdir -p /usr/src/nextcloud/custom_apps;     chmod +x /usr/src/nextcloud/occ;     apk del .fetch-deps
# Thu, 22 Oct 2020 10:49:53 GMT
COPY multi:7396b0dc331ca301e37b57c4af539d58e09521ec7c723e0739e6eca71f90ffb3 in / 
# Thu, 22 Oct 2020 10:49:55 GMT
COPY multi:c481008845253a7b26785f1b012d068624b67ddaaefbb62c1931fdf56fd06e2a in /usr/src/nextcloud/config/ 
# Thu, 22 Oct 2020 10:49:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 22 Oct 2020 10:49:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18701639c0ce1824d9d9f426e7ad4ccdf2d7598bcb0d03c58a4c0bb7c992e3b7`  
		Last Modified: Thu, 22 Oct 2020 05:29:10 GMT  
		Size: 1.4 MB (1382560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8913bd186df85a9366fb2cdb38fcc79adf2a420106aae8406124ac8d0165e92f`  
		Last Modified: Thu, 22 Oct 2020 05:29:09 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870830cea28d819a5f749933d7ba6ce48296069aed28f02cd4d609284b3944c3`  
		Last Modified: Thu, 22 Oct 2020 05:29:09 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:757ad7955ad2564c04c0f04e313dabb85d3515c8ae7340ea2b2c797c035d6eed`  
		Last Modified: Thu, 22 Oct 2020 05:31:28 GMT  
		Size: 12.2 MB (12152914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4afcae6e05abb0443700d9b453cd25507d50e6c713b5c8a1b6f0b5b69668b2`  
		Last Modified: Thu, 22 Oct 2020 05:31:24 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a59566a70b652dd18fe1849a9c56f989c848e070ce0a7dc1061511fd7be4da6`  
		Last Modified: Thu, 22 Oct 2020 05:31:26 GMT  
		Size: 13.8 MB (13774931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa136016cfb054a69f8b1e549d53aace3a7a0dce2bad3e07e26571a2a84caa8`  
		Last Modified: Thu, 22 Oct 2020 05:31:24 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:719dc292e3364ef2f1fc1f8a3bb1e03b09774412a20c729ee21b7025cc46651d`  
		Last Modified: Thu, 22 Oct 2020 05:31:24 GMT  
		Size: 16.7 KB (16709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7bdbf1764f4913d8c417eb0b77c08c38fba04a69fad1e146893aef118a808b`  
		Last Modified: Thu, 22 Oct 2020 05:31:25 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e376d34815fee8c87c6580ff0bdc24289889103ba07fc96ce961511af79742c`  
		Last Modified: Thu, 22 Oct 2020 10:56:47 GMT  
		Size: 271.7 KB (271659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281e98d1116354fe37f05e63b6c7134a068d8758f4068f98898c13192f703b02`  
		Last Modified: Thu, 22 Oct 2020 10:56:50 GMT  
		Size: 26.2 MB (26230896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e124f2f962a538eeebe1ceb059bf2bce9dd70bbf3d5b15001d1fa94396b8b89`  
		Last Modified: Thu, 22 Oct 2020 10:56:45 GMT  
		Size: 524.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e70f7ab038f7448efc3ef22153953019d796ae0be345ba8a54a1d4428fb032`  
		Last Modified: Thu, 22 Oct 2020 10:57:18 GMT  
		Size: 102.2 MB (102216458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f06a11531b6d2d4307230d319e3806ff905bb43c4336cf85f77ffbf070bba6e4`  
		Last Modified: Thu, 22 Oct 2020 10:57:06 GMT  
		Size: 2.5 KB (2524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40e16dd9cebbbbea4e545811604ff150e78c42939527754dc5f725165cbbc9d`  
		Last Modified: Thu, 22 Oct 2020 10:57:06 GMT  
		Size: 1.9 KB (1890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
