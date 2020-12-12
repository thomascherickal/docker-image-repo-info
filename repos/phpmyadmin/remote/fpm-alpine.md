## `phpmyadmin:fpm-alpine`

```console
$ docker pull phpmyadmin@sha256:dd237316bd5e5a05f57005791c17d1c9c814b2fd0367999d311a5f956fc58863
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

### `phpmyadmin:fpm-alpine` - linux; amd64

```console
$ docker pull phpmyadmin@sha256:fa2b84dbfc700947f5377cced0ca12c539a7d08bf4ce446a3933d1374ac045d3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47977150 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:55f6673d0d8653db402d406dbc259f08eae1f57b918a76af47a54d49ab36ff5b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 11 Dec 2020 02:04:06 GMT
ADD file:62a1e09319acb6d1bad91ef1c35aabdc7e5e19883a77f30f1951ccfffc812124 in / 
# Fri, 11 Dec 2020 02:04:07 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 07:52:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 11 Dec 2020 07:52:33 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 11 Dec 2020 07:52:34 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 11 Dec 2020 07:52:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Dec 2020 07:52:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Dec 2020 08:02:41 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 11 Dec 2020 08:02:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 08:02:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 08:02:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Dec 2020 08:49:57 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 11 Dec 2020 08:49:57 GMT
ENV PHP_VERSION=7.4.13
# Fri, 11 Dec 2020 08:49:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.13.tar.xz.asc
# Fri, 11 Dec 2020 08:49:58 GMT
ENV PHP_SHA256=aead303e3abac23106529560547baebbedba0bb2943b91d5aa08fff1f41680f4
# Fri, 11 Dec 2020 08:50:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 11 Dec 2020 08:50:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Dec 2020 08:58:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Dec 2020 08:58:37 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Fri, 11 Dec 2020 08:58:39 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Dec 2020 08:58:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Dec 2020 08:58:40 GMT
WORKDIR /var/www/html
# Fri, 11 Dec 2020 08:58:42 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Dec 2020 08:58:42 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Dec 2020 08:58:43 GMT
EXPOSE 9000
# Fri, 11 Dec 2020 08:58:43 GMT
CMD ["php-fpm"]
# Sat, 12 Dec 2020 01:13:36 GMT
RUN apk add --no-cache     bash     tzdata
# Sat, 12 Dec 2020 01:14:51 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         bzip2-dev         freetype-dev         libjpeg-turbo-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .phpmyadmin-phpexts-rundeps $runDeps;     apk del --no-network .build-deps
# Sat, 12 Dec 2020 01:14:52 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly = 1';         echo 'session.use_strict_mode = 1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen = Off';         echo 'max_execution_time = 600';         echo 'memory_limit = 512M';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Sat, 12 Dec 2020 01:14:52 GMT
ENV VERSION=5.0.4
# Sat, 12 Dec 2020 01:14:53 GMT
ENV SHA256=1578c1a08e594da4f4f62e676ccbdbd17784c3de769b094ba42c35bf05c057db
# Sat, 12 Dec 2020 01:14:53 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.0.4/phpMyAdmin-5.0.4-all-languages.tar.xz
# Sat, 12 Dec 2020 01:14:53 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.0.4 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Sat, 12 Dec 2020 01:15:00 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         gnupg     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;     apk del --no-network .fetch-deps
# Sat, 12 Dec 2020 01:15:00 GMT
COPY file:06ad12862a72189c42231c8acdf09dd49cf1544d43e49e2a1cdc3c2e3cea2603 in /etc/phpmyadmin/config.inc.php 
# Sat, 12 Dec 2020 01:15:00 GMT
COPY file:ad4174bf33f482b09f06789b6f1a83c35319165c7da1b86927e9f58fd8b2f0e9 in /docker-entrypoint.sh 
# Sat, 12 Dec 2020 01:15:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Sat, 12 Dec 2020 01:15:01 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:05e7bc50f07f000e9993ec0d264b9ffcbb9a01a4d69c68f556d25e9811a8f7f4`  
		Last Modified: Fri, 11 Dec 2020 02:04:37 GMT  
		Size: 2.8 MB (2796945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d8d8830ff0139fdf244372c3d1967e1f7833e7d0f91838ff0319c0180cc921`  
		Last Modified: Fri, 11 Dec 2020 12:05:53 GMT  
		Size: 1.3 MB (1340834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ac2024c1755529c6798cff1c860e408837634de341e6a258e291e058875d71`  
		Last Modified: Fri, 11 Dec 2020 12:05:51 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cb8735f928abb1eefbd973ae0afa89334a543c2fa6903aa7574d2d7e554376`  
		Last Modified: Fri, 11 Dec 2020 12:05:51 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf66d03b54e7be93055d3c4223cef21f5f2eaabe7e7ea872ebcc0aab5a0b1f42`  
		Last Modified: Fri, 11 Dec 2020 12:08:17 GMT  
		Size: 10.3 MB (10338564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e84b7ea4b2efc3419a428f9b6eb426cce8e27a1d49cc7d3909eee4f8e9e8f0f`  
		Last Modified: Fri, 11 Dec 2020 12:08:14 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057170a556ff13c6f530692ac3ebddd18301d18d36e1ab6d62394ddf49f26cc0`  
		Last Modified: Fri, 11 Dec 2020 12:08:19 GMT  
		Size: 14.3 MB (14256394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5de089cbd8a86f5b2e025df35548573e0007829669f768759f08bb767696db`  
		Last Modified: Fri, 11 Dec 2020 12:08:14 GMT  
		Size: 2.3 KB (2256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa0644635d04be02d909e98ef67717e928f98100a58eb85c822067210552957`  
		Last Modified: Fri, 11 Dec 2020 12:08:14 GMT  
		Size: 16.9 KB (16888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ddd148192263ae03d91317a3f1828dd8827c337aff95d4c2230c94193492ba`  
		Last Modified: Fri, 11 Dec 2020 12:08:14 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47993f4a37e3a8becf4489f570bac27918f85e1ba35f35fa1f7d329ad83af7e0`  
		Last Modified: Sat, 12 Dec 2020 01:16:15 GMT  
		Size: 929.1 KB (929104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:193575cfddcfe38b94bb022f3deaa50b0e1d9a0161b064be66c73d4e94a99b93`  
		Last Modified: Sat, 12 Dec 2020 01:16:14 GMT  
		Size: 5.3 MB (5271623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d01fa8b7a5fef29b3cc16c901d7a6b97e188fddc41616622e80768c6526faf`  
		Last Modified: Sat, 12 Dec 2020 01:16:14 GMT  
		Size: 473.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1f5c99582e875db258ea83948100b032c8799b314f3a22d837b1678962ce6b0`  
		Last Modified: Sat, 12 Dec 2020 01:16:20 GMT  
		Size: 13.0 MB (13011436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a83b1482b3565fe095a2cb43d0f27bcf86a55784211e3a4f80984fba697a717c`  
		Last Modified: Sat, 12 Dec 2020 01:16:13 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d0938e95a341989ac41f478214b7cbcc3215d2892aa11ebfc26a0874026ffbb`  
		Last Modified: Sat, 12 Dec 2020 01:16:12 GMT  
		Size: 834.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:fpm-alpine` - linux; arm variant v6

```console
$ docker pull phpmyadmin@sha256:f14c12b3170a66c259330572160a4e66f33e06829f477a3c62a1adb6b01ae46f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46245891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6d1b9700773accba82cb5279aecca7c52ae984ab8681502d6e9a73cdb7a4ad5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 11 Dec 2020 02:17:15 GMT
ADD file:1a9c0a67560d338c0c0e7005d8915d998fc9cf3e9f53bfd7e42e8391f0a39bce in / 
# Fri, 11 Dec 2020 02:17:15 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 07:04:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 11 Dec 2020 07:04:53 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 11 Dec 2020 07:04:55 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 11 Dec 2020 07:04:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Dec 2020 07:04:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Dec 2020 07:09:12 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 11 Dec 2020 07:09:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 07:09:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 07:09:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Dec 2020 07:17:56 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 11 Dec 2020 07:17:57 GMT
ENV PHP_VERSION=7.4.13
# Fri, 11 Dec 2020 07:17:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.13.tar.xz.asc
# Fri, 11 Dec 2020 07:17:58 GMT
ENV PHP_SHA256=aead303e3abac23106529560547baebbedba0bb2943b91d5aa08fff1f41680f4
# Fri, 11 Dec 2020 07:18:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 11 Dec 2020 07:18:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Dec 2020 07:21:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Dec 2020 07:21:47 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Fri, 11 Dec 2020 07:21:51 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Dec 2020 07:21:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Dec 2020 07:21:53 GMT
WORKDIR /var/www/html
# Fri, 11 Dec 2020 07:21:56 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Dec 2020 07:21:57 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Dec 2020 07:21:58 GMT
EXPOSE 9000
# Fri, 11 Dec 2020 07:21:59 GMT
CMD ["php-fpm"]
# Fri, 11 Dec 2020 08:43:32 GMT
RUN apk add --no-cache     bash     tzdata
# Fri, 11 Dec 2020 08:44:39 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         bzip2-dev         freetype-dev         libjpeg-turbo-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .phpmyadmin-phpexts-rundeps $runDeps;     apk del --no-network .build-deps
# Fri, 11 Dec 2020 08:44:42 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly = 1';         echo 'session.use_strict_mode = 1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen = Off';         echo 'max_execution_time = 600';         echo 'memory_limit = 512M';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Fri, 11 Dec 2020 08:44:43 GMT
ENV VERSION=5.0.4
# Fri, 11 Dec 2020 08:44:44 GMT
ENV SHA256=1578c1a08e594da4f4f62e676ccbdbd17784c3de769b094ba42c35bf05c057db
# Fri, 11 Dec 2020 08:44:45 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.0.4/phpMyAdmin-5.0.4-all-languages.tar.xz
# Fri, 11 Dec 2020 08:44:46 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.0.4 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Fri, 11 Dec 2020 08:44:55 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         gnupg     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;     apk del --no-network .fetch-deps
# Fri, 11 Dec 2020 08:44:58 GMT
COPY file:06ad12862a72189c42231c8acdf09dd49cf1544d43e49e2a1cdc3c2e3cea2603 in /etc/phpmyadmin/config.inc.php 
# Fri, 11 Dec 2020 08:44:59 GMT
COPY file:ad4174bf33f482b09f06789b6f1a83c35319165c7da1b86927e9f58fd8b2f0e9 in /docker-entrypoint.sh 
# Fri, 11 Dec 2020 08:45:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 08:45:01 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f1c16df8fee33d421d08790b17ca2af67a3fe49e77b6b991dd0c30631f5d1baf`  
		Last Modified: Fri, 11 Dec 2020 02:17:57 GMT  
		Size: 2.6 MB (2601992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623cc08cbe035cf15859e57a83e2243620418da06e1905d1875a46bec901e540`  
		Last Modified: Fri, 11 Dec 2020 07:56:49 GMT  
		Size: 1.3 MB (1310156 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3a7aacff9b7ccf646f2bdbbc8d40bbb304550e813876049e721abd35461df9`  
		Last Modified: Fri, 11 Dec 2020 07:56:49 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3d3214ea6f418597f370177309be7728f94481030c9cba6e45c4b74cfd04cc0`  
		Last Modified: Fri, 11 Dec 2020 07:56:49 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff7159949c3c97335dda12e61ad77a87a4125ef93f88655500f4b8057cd38ca`  
		Last Modified: Fri, 11 Dec 2020 07:58:09 GMT  
		Size: 10.3 MB (10338600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c2c2f22a036ec3f2efaed4fd97c10faee4bbf539b56bf2e11b84a7c05b78fa`  
		Last Modified: Fri, 11 Dec 2020 07:58:05 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae33a5a224fa1ee298562bc31d50c9f804652bf619e4836e852c8860c5c49318`  
		Last Modified: Fri, 11 Dec 2020 07:58:09 GMT  
		Size: 13.3 MB (13267849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c09a76a513338db42015101706a8bf9c7309d298d0a3329dee74810ea39db7`  
		Last Modified: Fri, 11 Dec 2020 07:58:05 GMT  
		Size: 2.3 KB (2260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e47c9c32a85f1170c19a3745c3a661a3a3c13e50daddef9919f624a52a70bc30`  
		Last Modified: Fri, 11 Dec 2020 07:58:05 GMT  
		Size: 16.9 KB (16891 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bbe39bbdfd22c5c467c010b89eb9561741273f56a2f378e08f2e055ef9ed919`  
		Last Modified: Fri, 11 Dec 2020 07:58:05 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:597b02236977153012f07752bd6f0803b206f9bd6fa0f715227cf2a4307b915e`  
		Last Modified: Fri, 11 Dec 2020 08:45:25 GMT  
		Size: 912.7 KB (912685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc57dd7c2674042614bd959598ed2864f1979215de8ee25b4fcebec42f19b24`  
		Last Modified: Fri, 11 Dec 2020 08:45:24 GMT  
		Size: 4.8 MB (4770272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a638c8bfcd284b13c6de79e646e83ce45b555294d451b1a044e189ed92f340f`  
		Last Modified: Fri, 11 Dec 2020 08:45:23 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574e6a119db45f3f6ceb0231a4b88a3e6783c74f220baeeb32a4cbac4f511238`  
		Last Modified: Fri, 11 Dec 2020 08:45:28 GMT  
		Size: 13.0 MB (13011980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d364fc013ebca6cbeb42d0adeb2c0d3899dd5ffcc8de1ad9b5dc9437a4562fa`  
		Last Modified: Fri, 11 Dec 2020 08:45:23 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:958f373883d362f4ca114a947dc2031f00d367d864aebdfe2f576344836911d3`  
		Last Modified: Fri, 11 Dec 2020 08:45:23 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:fpm-alpine` - linux; arm variant v7

```console
$ docker pull phpmyadmin@sha256:ddbb93c27d955194ba134af2831900f0280948e26fef219fc2bb00c0fb131fc1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45349145 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fc2500159968d713613e9bd3d273a7cb8e50865229dad03bef50396c41a284c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
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
# Thu, 22 Oct 2020 07:01:44 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 01 Dec 2020 02:43:04 GMT
ENV PHP_VERSION=7.4.13
# Tue, 01 Dec 2020 02:43:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.13.tar.xz.asc
# Tue, 01 Dec 2020 02:43:24 GMT
ENV PHP_SHA256=aead303e3abac23106529560547baebbedba0bb2943b91d5aa08fff1f41680f4
# Tue, 01 Dec 2020 02:43:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 01 Dec 2020 02:43:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Dec 2020 02:46:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Dec 2020 02:46:34 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Tue, 01 Dec 2020 02:46:37 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Dec 2020 02:46:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Dec 2020 02:46:39 GMT
WORKDIR /var/www/html
# Tue, 01 Dec 2020 02:46:42 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 01 Dec 2020 02:46:44 GMT
STOPSIGNAL SIGQUIT
# Tue, 01 Dec 2020 02:46:45 GMT
EXPOSE 9000
# Tue, 01 Dec 2020 02:46:46 GMT
CMD ["php-fpm"]
# Tue, 01 Dec 2020 05:13:03 GMT
RUN apk add --no-cache     bash     tzdata
# Tue, 01 Dec 2020 05:14:07 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         bzip2-dev         freetype-dev         libjpeg-turbo-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .phpmyadmin-phpexts-rundeps $runDeps;     apk del --no-network .build-deps
# Tue, 01 Dec 2020 05:14:12 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly = 1';         echo 'session.use_strict_mode = 1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen = Off';         echo 'max_execution_time = 600';         echo 'memory_limit = 512M';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Tue, 01 Dec 2020 05:14:13 GMT
ENV VERSION=5.0.4
# Tue, 01 Dec 2020 05:14:13 GMT
ENV SHA256=1578c1a08e594da4f4f62e676ccbdbd17784c3de769b094ba42c35bf05c057db
# Tue, 01 Dec 2020 05:14:14 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.0.4/phpMyAdmin-5.0.4-all-languages.tar.xz
# Tue, 01 Dec 2020 05:14:15 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.0.4 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Tue, 01 Dec 2020 05:14:24 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         gnupg     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;     apk del --no-network .fetch-deps
# Tue, 01 Dec 2020 05:14:25 GMT
COPY file:06ad12862a72189c42231c8acdf09dd49cf1544d43e49e2a1cdc3c2e3cea2603 in /etc/phpmyadmin/config.inc.php 
# Tue, 01 Dec 2020 05:14:26 GMT
COPY file:ad4174bf33f482b09f06789b6f1a83c35319165c7da1b86927e9f58fd8b2f0e9 in /docker-entrypoint.sh 
# Tue, 01 Dec 2020 05:14:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 01 Dec 2020 05:14:28 GMT
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
	-	`sha256:ad5979536683af238cd5c6e9e7ee5171a2f468ba42667525bcf73dfbd4442d5c`  
		Last Modified: Tue, 01 Dec 2020 04:01:12 GMT  
		Size: 10.3 MB (10338579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83bfa48b04ad972c7ddc62f60703fd345236339c894ee5e02487d0a6912eec44`  
		Last Modified: Tue, 01 Dec 2020 04:01:08 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d500723729ab98b41c43300141cf87ecedf3122e848cb7f2871a8a18b472c9`  
		Last Modified: Tue, 01 Dec 2020 04:01:12 GMT  
		Size: 12.8 MB (12773054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ffe3faddffbb23fc7ec2b0ac5897aa6700b295f1129a52a58322108a7d7146`  
		Last Modified: Tue, 01 Dec 2020 04:01:08 GMT  
		Size: 2.3 KB (2260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6599d32683be6cd2106e34a046a0a556bffd2baac97299eb69df7408f682be`  
		Last Modified: Tue, 01 Dec 2020 04:01:08 GMT  
		Size: 16.9 KB (16903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7158f5b17b11ddb8f243be54e5fc6112f6017d46780577a568a72e2e7d3f2cb1`  
		Last Modified: Tue, 01 Dec 2020 04:01:08 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa84a801fdba73617fcd8d784eb0973c926bcbb6b983d6408448fd6e247ca0a6`  
		Last Modified: Tue, 01 Dec 2020 05:15:45 GMT  
		Size: 860.7 KB (860743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a00c7a499cbd5e439380c5a65ca6776805c4ba5c7e505d3a04eb9f8270a63b`  
		Last Modified: Tue, 01 Dec 2020 05:15:44 GMT  
		Size: 4.7 MB (4712482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:046a9f23933466e8dfda9cd7f23eb0be5bcdaa08712609326b179772d4049a91`  
		Last Modified: Tue, 01 Dec 2020 05:15:43 GMT  
		Size: 472.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4866abdfbf607daa221f5df14463cc0452db8c9668271885cf190f76b7dee7e3`  
		Last Modified: Tue, 01 Dec 2020 05:15:50 GMT  
		Size: 13.0 MB (13011971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90569c253ff71188a390fa0b32368a8e50f0c3c9b349a44117cfe3b9a2a12f41`  
		Last Modified: Tue, 01 Dec 2020 05:15:43 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c15b26ceaffb4b98c97edd391c942289ef8d9f1bdca0e9bd97f3ab3b508b095`  
		Last Modified: Tue, 01 Dec 2020 05:15:43 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull phpmyadmin@sha256:e34f07a9d605bbd255947991e434eb5df7839e30cdcb2ec503c52ad3e3a78e7b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (48047651 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:227665dd132b64f04f526ca6c587d6659dcb3d7bcd8c02f766651469da2294e5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
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
# Thu, 22 Oct 2020 07:32:38 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 01 Dec 2020 03:31:07 GMT
ENV PHP_VERSION=7.4.13
# Tue, 01 Dec 2020 03:31:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.13.tar.xz.asc
# Tue, 01 Dec 2020 03:31:09 GMT
ENV PHP_SHA256=aead303e3abac23106529560547baebbedba0bb2943b91d5aa08fff1f41680f4
# Tue, 01 Dec 2020 03:31:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 01 Dec 2020 03:31:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Dec 2020 03:34:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Dec 2020 03:35:01 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Tue, 01 Dec 2020 03:35:06 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Dec 2020 03:35:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Dec 2020 03:35:08 GMT
WORKDIR /var/www/html
# Tue, 01 Dec 2020 03:35:10 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 01 Dec 2020 03:35:11 GMT
STOPSIGNAL SIGQUIT
# Tue, 01 Dec 2020 03:35:12 GMT
EXPOSE 9000
# Tue, 01 Dec 2020 03:35:13 GMT
CMD ["php-fpm"]
# Tue, 01 Dec 2020 07:34:51 GMT
RUN apk add --no-cache     bash     tzdata
# Tue, 01 Dec 2020 07:35:46 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         bzip2-dev         freetype-dev         libjpeg-turbo-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .phpmyadmin-phpexts-rundeps $runDeps;     apk del --no-network .build-deps
# Tue, 01 Dec 2020 07:35:49 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly = 1';         echo 'session.use_strict_mode = 1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen = Off';         echo 'max_execution_time = 600';         echo 'memory_limit = 512M';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Tue, 01 Dec 2020 07:35:51 GMT
ENV VERSION=5.0.4
# Tue, 01 Dec 2020 07:35:52 GMT
ENV SHA256=1578c1a08e594da4f4f62e676ccbdbd17784c3de769b094ba42c35bf05c057db
# Tue, 01 Dec 2020 07:35:54 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.0.4/phpMyAdmin-5.0.4-all-languages.tar.xz
# Tue, 01 Dec 2020 07:35:55 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.0.4 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Tue, 01 Dec 2020 07:36:03 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         gnupg     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;     apk del --no-network .fetch-deps
# Tue, 01 Dec 2020 07:36:06 GMT
COPY file:06ad12862a72189c42231c8acdf09dd49cf1544d43e49e2a1cdc3c2e3cea2603 in /etc/phpmyadmin/config.inc.php 
# Tue, 01 Dec 2020 07:36:07 GMT
COPY file:ad4174bf33f482b09f06789b6f1a83c35319165c7da1b86927e9f58fd8b2f0e9 in /docker-entrypoint.sh 
# Tue, 01 Dec 2020 07:36:08 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 01 Dec 2020 07:36:09 GMT
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
	-	`sha256:b747a72bda51ef2a52afed0eef10b56786e7c76ab30913f0e650a83b66935e4f`  
		Last Modified: Tue, 01 Dec 2020 04:54:24 GMT  
		Size: 10.3 MB (10338600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c684293922e5efaae5d67a6b158f6e54284e91081dda97b306a74ce97c9d0738`  
		Last Modified: Tue, 01 Dec 2020 04:54:21 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acdf0cad2cf9d86164e334858db58328dc251f08abe9d0841cc1bf520748163e`  
		Last Modified: Tue, 01 Dec 2020 04:54:25 GMT  
		Size: 14.5 MB (14458713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3417ec8fcb1bd4b4d3f295b89316912d8e33667e645450c3d0a2694887fea5da`  
		Last Modified: Tue, 01 Dec 2020 04:54:21 GMT  
		Size: 2.3 KB (2256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96e2c572c8bf97a5e221afc68cec20acaad7e29b919f242c6cb085234693b08`  
		Last Modified: Tue, 01 Dec 2020 04:54:22 GMT  
		Size: 17.0 KB (16978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732bd773818e9fef29ad5ba55c5ddd1638077be22b0fd0a8f3a8bee4b600da11`  
		Last Modified: Tue, 01 Dec 2020 04:54:21 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f256a2a80d1bf49d1ab5f36c1dd925e45d6c7219c26edf83fe4dadb249b25e24`  
		Last Modified: Tue, 01 Dec 2020 07:37:09 GMT  
		Size: 942.6 KB (942579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaa915b8104ce698fbe93745f7bd36f70588feb72eea9bad09a3b5ff8d9ada3`  
		Last Modified: Tue, 01 Dec 2020 07:37:08 GMT  
		Size: 5.2 MB (5213662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8d2f713cee1f66f1130db075f5d82469e6df41bc42bbec2a39913fb1ca0998`  
		Last Modified: Tue, 01 Dec 2020 07:37:07 GMT  
		Size: 469.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f423f4c52b99c55956d99dacec8e8fd45f2e1b63d34aa1368e64f731356d2940`  
		Last Modified: Tue, 01 Dec 2020 07:37:12 GMT  
		Size: 13.0 MB (13012319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3116e234afce9bf957d69e6cbca97fbf4929fbd3097dac9c7e3cd2c6b789e30e`  
		Last Modified: Tue, 01 Dec 2020 07:37:06 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6371d103e92ce1a1d1f896a6c1bc13648ffef4ced60501cf77e154cea8a952e5`  
		Last Modified: Tue, 01 Dec 2020 07:37:06 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:fpm-alpine` - linux; 386

```console
$ docker pull phpmyadmin@sha256:93706d46e8b7b6a155b400ca0712f72279f39d8c828d5ac0095eb8fd726d4eed
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48997118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc85657dfbda0e5e65a87ce40e58df644d466097f9b68cb70def6e15c2f7c87b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
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
# Thu, 22 Oct 2020 04:01:27 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 01 Dec 2020 04:11:03 GMT
ENV PHP_VERSION=7.4.13
# Tue, 01 Dec 2020 04:11:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.13.tar.xz.asc
# Tue, 01 Dec 2020 04:11:04 GMT
ENV PHP_SHA256=aead303e3abac23106529560547baebbedba0bb2943b91d5aa08fff1f41680f4
# Tue, 01 Dec 2020 04:11:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 01 Dec 2020 04:11:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Dec 2020 04:19:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Dec 2020 04:19:54 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Tue, 01 Dec 2020 04:19:56 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Dec 2020 04:19:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Dec 2020 04:19:56 GMT
WORKDIR /var/www/html
# Tue, 01 Dec 2020 04:19:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 01 Dec 2020 04:19:57 GMT
STOPSIGNAL SIGQUIT
# Tue, 01 Dec 2020 04:19:58 GMT
EXPOSE 9000
# Tue, 01 Dec 2020 04:19:58 GMT
CMD ["php-fpm"]
# Tue, 01 Dec 2020 08:47:04 GMT
RUN apk add --no-cache     bash     tzdata
# Tue, 01 Dec 2020 08:47:54 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         bzip2-dev         freetype-dev         libjpeg-turbo-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .phpmyadmin-phpexts-rundeps $runDeps;     apk del --no-network .build-deps
# Tue, 01 Dec 2020 08:47:54 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly = 1';         echo 'session.use_strict_mode = 1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen = Off';         echo 'max_execution_time = 600';         echo 'memory_limit = 512M';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Tue, 01 Dec 2020 08:47:55 GMT
ENV VERSION=5.0.4
# Tue, 01 Dec 2020 08:47:55 GMT
ENV SHA256=1578c1a08e594da4f4f62e676ccbdbd17784c3de769b094ba42c35bf05c057db
# Tue, 01 Dec 2020 08:47:55 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.0.4/phpMyAdmin-5.0.4-all-languages.tar.xz
# Tue, 01 Dec 2020 08:47:55 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.0.4 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Tue, 01 Dec 2020 08:48:00 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         gnupg     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;     apk del --no-network .fetch-deps
# Tue, 01 Dec 2020 08:48:00 GMT
COPY file:06ad12862a72189c42231c8acdf09dd49cf1544d43e49e2a1cdc3c2e3cea2603 in /etc/phpmyadmin/config.inc.php 
# Tue, 01 Dec 2020 08:48:01 GMT
COPY file:ad4174bf33f482b09f06789b6f1a83c35319165c7da1b86927e9f58fd8b2f0e9 in /docker-entrypoint.sh 
# Tue, 01 Dec 2020 08:48:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 01 Dec 2020 08:48:01 GMT
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
	-	`sha256:d73c975f14cba63719b1acf30eb48c56e9ff5ab3ba3c93cc300551ed40f30ac4`  
		Last Modified: Tue, 01 Dec 2020 07:15:32 GMT  
		Size: 10.3 MB (10338565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8926789263a06364cefc6d6aee50b84a30291d014d2029ca669cb556f4c2bb1`  
		Last Modified: Tue, 01 Dec 2020 07:15:30 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbe8e9cc07ddaae06ed92974d6d0a5249cac41ebb54331b56fc5c9e240eb993`  
		Last Modified: Tue, 01 Dec 2020 07:15:35 GMT  
		Size: 15.0 MB (15012323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e40c7a669cd74ab9dc3e2874416646f823f63c10d9b9a952a55dc1ad5bac9d`  
		Last Modified: Tue, 01 Dec 2020 07:15:30 GMT  
		Size: 2.3 KB (2260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed001fb8127577a70da6914dcf10ccb5d90ed9cf2a1cd3272618748f6b111d03`  
		Last Modified: Tue, 01 Dec 2020 07:15:29 GMT  
		Size: 16.9 KB (16920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90867a60ecf180a61e2ada4f0842adc2c2e44685c28753a5bed45de997db01e7`  
		Last Modified: Tue, 01 Dec 2020 07:15:29 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:513b1da93e3c26c413b26b292d51222e6e513efb7a07aec511bba3a38f2b8346`  
		Last Modified: Tue, 01 Dec 2020 08:48:54 GMT  
		Size: 976.4 KB (976372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5977ec4614e49f7e34041f3327c1b41c818e626c5ac99abf596868cbf06a469b`  
		Last Modified: Tue, 01 Dec 2020 08:48:54 GMT  
		Size: 5.4 MB (5395078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e8c031832ae9287401956de0bf2775cfbd0dfd80ec8520ddf0d181110a6689c`  
		Last Modified: Tue, 01 Dec 2020 08:48:52 GMT  
		Size: 470.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20d16621d46df9d7439eca251712ef84c8789157fd3d18ea2b5e9f589206f35`  
		Last Modified: Tue, 01 Dec 2020 08:48:59 GMT  
		Size: 13.0 MB (13011453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67fd268df463021105c7e3f8299b33630c151fc6f117984fa7626a08a389af88`  
		Last Modified: Tue, 01 Dec 2020 08:48:53 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21686d70202717bc98be2fa93ea60bb036a5298e69bed7a87eefd7cb4aa1e477`  
		Last Modified: Tue, 01 Dec 2020 08:48:53 GMT  
		Size: 834.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:fpm-alpine` - linux; ppc64le

```console
$ docker pull phpmyadmin@sha256:9f8af4dd83e1bf7a67157b7413879bf24818ebfa6a1f936a5f4cb28d6b659fde
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49139492 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e43f430be80c0ceb4b85c0e66ce7b4f682f8c0ecf93a71c7aa06c8a60762fd88`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 11 Dec 2020 03:30:29 GMT
ADD file:9b4b44ee9eaddedc13f114bb55c9abeabceff6abd47f4a660734e431d22fcdce in / 
# Fri, 11 Dec 2020 03:30:32 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 10:06:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 11 Dec 2020 10:06:41 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 11 Dec 2020 10:06:57 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 11 Dec 2020 10:07:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Dec 2020 10:07:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Dec 2020 10:12:38 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 11 Dec 2020 10:12:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 10:12:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 10:12:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Dec 2020 10:52:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 11 Dec 2020 10:52:43 GMT
ENV PHP_VERSION=7.4.13
# Fri, 11 Dec 2020 10:52:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.13.tar.xz.asc
# Fri, 11 Dec 2020 10:52:48 GMT
ENV PHP_SHA256=aead303e3abac23106529560547baebbedba0bb2943b91d5aa08fff1f41680f4
# Fri, 11 Dec 2020 10:53:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 11 Dec 2020 10:53:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Dec 2020 10:56:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Dec 2020 10:56:58 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Fri, 11 Dec 2020 10:57:03 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Dec 2020 10:57:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Dec 2020 10:57:06 GMT
WORKDIR /var/www/html
# Fri, 11 Dec 2020 10:57:14 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Dec 2020 10:57:16 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Dec 2020 10:57:18 GMT
EXPOSE 9000
# Fri, 11 Dec 2020 10:57:21 GMT
CMD ["php-fpm"]
# Fri, 11 Dec 2020 23:04:08 GMT
RUN apk add --no-cache     bash     tzdata
# Fri, 11 Dec 2020 23:05:15 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         bzip2-dev         freetype-dev         libjpeg-turbo-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .phpmyadmin-phpexts-rundeps $runDeps;     apk del --no-network .build-deps
# Fri, 11 Dec 2020 23:05:28 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly = 1';         echo 'session.use_strict_mode = 1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen = Off';         echo 'max_execution_time = 600';         echo 'memory_limit = 512M';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Fri, 11 Dec 2020 23:05:32 GMT
ENV VERSION=5.0.4
# Fri, 11 Dec 2020 23:05:39 GMT
ENV SHA256=1578c1a08e594da4f4f62e676ccbdbd17784c3de769b094ba42c35bf05c057db
# Fri, 11 Dec 2020 23:05:44 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.0.4/phpMyAdmin-5.0.4-all-languages.tar.xz
# Fri, 11 Dec 2020 23:05:49 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.0.4 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Fri, 11 Dec 2020 23:06:16 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         gnupg     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;     apk del --no-network .fetch-deps
# Fri, 11 Dec 2020 23:06:21 GMT
COPY file:06ad12862a72189c42231c8acdf09dd49cf1544d43e49e2a1cdc3c2e3cea2603 in /etc/phpmyadmin/config.inc.php 
# Fri, 11 Dec 2020 23:06:22 GMT
COPY file:ad4174bf33f482b09f06789b6f1a83c35319165c7da1b86927e9f58fd8b2f0e9 in /docker-entrypoint.sh 
# Fri, 11 Dec 2020 23:06:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 23:06:32 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:ed596bc4dd0a0c7ff1952005f6cae53a061e1c7998282289586bbfc17a2fd6db`  
		Last Modified: Fri, 11 Dec 2020 03:31:06 GMT  
		Size: 2.8 MB (2803424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857fb82fb762ef846b2b51d5a207ffbe3d8eaf4d986164e6c60918bdf15d8ada`  
		Last Modified: Fri, 11 Dec 2020 12:46:37 GMT  
		Size: 1.4 MB (1383203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d54be1e5c677b3f9a2f016968368e64061d8e326fad93c8f70c08d7d3e863ef`  
		Last Modified: Fri, 11 Dec 2020 12:46:36 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a04a1ffd499248816e13b35f7a4726fa6f46f4e69ac3130f436b84f23522d5ba`  
		Last Modified: Fri, 11 Dec 2020 12:46:37 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eebf28c61e699e64b43508765b3ac8537df48fb86d9bbe785521c5c8f99e11e`  
		Last Modified: Fri, 11 Dec 2020 12:51:17 GMT  
		Size: 10.3 MB (10338601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b4dc9c61a8c7ad9feebdfcde9f3a5dc83069058f16457b383090d364e96257`  
		Last Modified: Fri, 11 Dec 2020 12:51:01 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba84fe4e9321d59d19264433b4f7e55f6527c2bd9ed3ecacff6334086ce5dfb2`  
		Last Modified: Fri, 11 Dec 2020 12:51:05 GMT  
		Size: 15.2 MB (15242844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fafa72c4ea631792dbdf417cca0dad09cda53df4f2e78eba36f8e14b4c2e85d8`  
		Last Modified: Fri, 11 Dec 2020 12:51:02 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c225fb1ae512d7b455e23fe8cf0a22fde8a7b85cbed624141cb1d10e5dc01b69`  
		Last Modified: Fri, 11 Dec 2020 12:51:01 GMT  
		Size: 16.9 KB (16927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dba2a1f59688349c6e690810536c762cec17b33c05b8d7f7d4bdd29c9874a62a`  
		Last Modified: Fri, 11 Dec 2020 12:51:01 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f715b4eeb3ed55d18add40b5284c6d15e4057ca19a17aa6fafd561cb7427f528`  
		Last Modified: Fri, 11 Dec 2020 23:08:34 GMT  
		Size: 999.8 KB (999793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eacde987c54be34b11b7c7b2db64b8e8a9b70fb883f5c47f88f61d6d2d9269d9`  
		Last Modified: Fri, 11 Dec 2020 23:08:31 GMT  
		Size: 5.3 MB (5326991 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe471cdec8db0c14875e6aff9396de616790a0edbd0405e3b16c74e1e5c20bb`  
		Last Modified: Fri, 11 Dec 2020 23:08:30 GMT  
		Size: 471.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb5dfa5871c59c5a75b09ce6392e326070eaea2fcd537db6be4afb8e1a08e710`  
		Last Modified: Fri, 11 Dec 2020 23:08:34 GMT  
		Size: 13.0 MB (13012243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:818bffa275aa4186bfd67a91984ff9244bca0bcd637c15b39aa04cccc7159761`  
		Last Modified: Fri, 11 Dec 2020 23:08:30 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ca8343db91e008bd65bbe612cb8c1e7fb8ce87803d790d585c6577cd4d2cf9`  
		Last Modified: Fri, 11 Dec 2020 23:08:30 GMT  
		Size: 836.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `phpmyadmin:fpm-alpine` - linux; s390x

```console
$ docker pull phpmyadmin@sha256:1959040841a4294a054f416aa566f6a1942315c03816174ed6b42eb561bbb8b0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.9 MB (46871426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46e37c00650162946cba941c3604aad2694c14d4b9e72c17e18a0fa0702e9533`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 11 Dec 2020 02:09:52 GMT
ADD file:c9395a36a4e03768aabd282eb1f31705cc00181d3147222d9c940eaa5a8fd511 in / 
# Fri, 11 Dec 2020 02:09:53 GMT
CMD ["/bin/sh"]
# Fri, 11 Dec 2020 11:30:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 11 Dec 2020 11:30:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 11 Dec 2020 11:30:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 11 Dec 2020 11:30:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 11 Dec 2020 11:30:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 11 Dec 2020 11:36:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 11 Dec 2020 11:36:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 11:36:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 11 Dec 2020 11:36:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 11 Dec 2020 12:09:03 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 11 Dec 2020 12:09:04 GMT
ENV PHP_VERSION=7.4.13
# Fri, 11 Dec 2020 12:09:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.13.tar.xz.asc
# Fri, 11 Dec 2020 12:09:05 GMT
ENV PHP_SHA256=aead303e3abac23106529560547baebbedba0bb2943b91d5aa08fff1f41680f4
# Fri, 11 Dec 2020 12:09:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 11 Dec 2020 12:09:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Dec 2020 12:13:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Dec 2020 12:13:55 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Fri, 11 Dec 2020 12:13:57 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Dec 2020 12:13:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Dec 2020 12:13:59 GMT
WORKDIR /var/www/html
# Fri, 11 Dec 2020 12:14:00 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Dec 2020 12:14:01 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Dec 2020 12:14:01 GMT
EXPOSE 9000
# Fri, 11 Dec 2020 12:14:02 GMT
CMD ["php-fpm"]
# Fri, 11 Dec 2020 19:52:51 GMT
RUN apk add --no-cache     bash     tzdata
# Fri, 11 Dec 2020 19:53:34 GMT
RUN set -ex;         apk add --no-cache --virtual .build-deps         bzip2-dev         freetype-dev         libjpeg-turbo-dev         libpng-dev         libwebp-dev         libxpm-dev         libzip-dev     ;         docker-php-ext-configure gd --with-freetype --with-jpeg --with-webp --with-xpm;     docker-php-ext-install -j "$(nproc)"         bz2         gd         mysqli         opcache         zip     ;         runDeps="$(         scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions             | tr ',' '\n'             | sort -u             | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";     apk add --virtual .phpmyadmin-phpexts-rundeps $runDeps;     apk del --no-network .build-deps
# Fri, 11 Dec 2020 19:53:36 GMT
RUN set -ex;         {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > $PHP_INI_DIR/conf.d/opcache-recommended.ini;         {         echo 'session.cookie_httponly = 1';         echo 'session.use_strict_mode = 1';     } > $PHP_INI_DIR/conf.d/session-strict.ini;         {         echo 'allow_url_fopen = Off';         echo 'max_execution_time = 600';         echo 'memory_limit = 512M';     } > $PHP_INI_DIR/conf.d/phpmyadmin-misc.ini
# Fri, 11 Dec 2020 19:53:37 GMT
ENV VERSION=5.0.4
# Fri, 11 Dec 2020 19:53:37 GMT
ENV SHA256=1578c1a08e594da4f4f62e676ccbdbd17784c3de769b094ba42c35bf05c057db
# Fri, 11 Dec 2020 19:53:38 GMT
ENV URL=https://files.phpmyadmin.net/phpMyAdmin/5.0.4/phpMyAdmin-5.0.4-all-languages.tar.xz
# Fri, 11 Dec 2020 19:53:38 GMT
LABEL org.opencontainers.image.title=Official phpMyAdmin Docker image org.opencontainers.image.description=Run phpMyAdmin with Alpine, Apache and PHP FPM. org.opencontainers.image.authors=The phpMyAdmin Team <developers@phpmyadmin.net> org.opencontainers.image.vendor=phpMyAdmin org.opencontainers.image.documentation=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.licenses=GPL-2.0-only org.opencontainers.image.version=5.0.4 org.opencontainers.image.url=https://github.com/phpmyadmin/docker#readme org.opencontainers.image.source=https://github.com/phpmyadmin/docker.git
# Fri, 11 Dec 2020 19:53:43 GMT
RUN set -ex;     apk add --no-cache --virtual .fetch-deps         gnupg     ;         export GNUPGHOME="$(mktemp -d)";     export GPGKEY="3D06A59ECE730EB71B511C17CE752F178259BD92";     curl -fsSL -o phpMyAdmin.tar.xz $URL;     curl -fsSL -o phpMyAdmin.tar.xz.asc $URL.asc;     echo "$SHA256 *phpMyAdmin.tar.xz" | sha256sum -c -;     gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver ipv4.pool.sks-keyservers.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver keys.gnupg.net --recv-keys "$GPGKEY"         || gpg --batch --keyserver pgp.mit.edu --recv-keys "$GPGKEY"         || gpg --batch --keyserver keyserver.pgp.com --recv-keys "$GPGKEY";     gpg --batch --verify phpMyAdmin.tar.xz.asc phpMyAdmin.tar.xz;     tar -xf phpMyAdmin.tar.xz -C /var/www/html --strip-components=1;     mkdir -p /var/www/html/tmp;     chown www-data:www-data /var/www/html/tmp;     gpgconf --kill all;     rm -r "$GNUPGHOME" phpMyAdmin.tar.xz phpMyAdmin.tar.xz.asc;     rm -rf /var/www/html/setup/ /var/www/html/examples/ /var/www/html/test/ /var/www/html/po/ /var/www/html/composer.json /var/www/html/RELEASE-DATE-$VERSION;     sed -i "s@define('CONFIG_DIR'.*@define('CONFIG_DIR', '/etc/phpmyadmin/');@" /var/www/html/libraries/vendor_config.php;     apk del --no-network .fetch-deps
# Fri, 11 Dec 2020 19:53:46 GMT
COPY file:06ad12862a72189c42231c8acdf09dd49cf1544d43e49e2a1cdc3c2e3cea2603 in /etc/phpmyadmin/config.inc.php 
# Fri, 11 Dec 2020 19:53:47 GMT
COPY file:ad4174bf33f482b09f06789b6f1a83c35319165c7da1b86927e9f58fd8b2f0e9 in /docker-entrypoint.sh 
# Fri, 11 Dec 2020 19:53:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 11 Dec 2020 19:53:48 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:7c2470fe3d16cb70fca0826168095a96838b1322a8cd1502b28284ee8561b491`  
		Last Modified: Fri, 11 Dec 2020 02:10:27 GMT  
		Size: 2.6 MB (2565988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a23c8359d30ae261ad953f292e6681a71ebc7388607b74d901bbc07f71e1311`  
		Last Modified: Fri, 11 Dec 2020 13:48:01 GMT  
		Size: 1.4 MB (1382587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01422c3e898d3241d4134256bf0d911b0752823227af04614187c79c187e2843`  
		Last Modified: Fri, 11 Dec 2020 13:48:03 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19a0be2077abd44f96e50bdebb1ed93a6e2b8d504761c23fa0e5e9b87045ca38`  
		Last Modified: Fri, 11 Dec 2020 13:48:01 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797fc05bf988e85a5cf643f2d07a0b08a36e3f1529c75c41a2460041b6ee0f43`  
		Last Modified: Fri, 11 Dec 2020 13:50:52 GMT  
		Size: 10.3 MB (10338591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e11bb5dc7804a50c805852fbe653bb133478f5005e8c78c1d712af0d5bd6db4`  
		Last Modified: Fri, 11 Dec 2020 13:50:49 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:311bfe9de08521ea35d7a1520e00de8215315e5a8144a4335f1313ad7f6593de`  
		Last Modified: Fri, 11 Dec 2020 13:50:51 GMT  
		Size: 13.6 MB (13553700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c59a788dffbadef519f959d8de10a3156add64ed4e15c8e96045a3bebf9ef316`  
		Last Modified: Fri, 11 Dec 2020 13:50:49 GMT  
		Size: 2.3 KB (2260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:898ee507348c01a8028e7ad08c8af3edde13cd884ffdfd990ad679df9b004552`  
		Last Modified: Fri, 11 Dec 2020 13:50:49 GMT  
		Size: 16.9 KB (16883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7bec784d5537500a8f385256905e367037e6e1ae365f119cf3a305c384338f`  
		Last Modified: Fri, 11 Dec 2020 13:50:50 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd931bbd56c86fbe8be2b083de0a3520fb5399a78682500ce56296ac6d21afb`  
		Last Modified: Fri, 11 Dec 2020 19:54:52 GMT  
		Size: 954.5 KB (954501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79d27026b558567f50ef4dec4148079327f688aeee9874601426fc39e33da32`  
		Last Modified: Fri, 11 Dec 2020 19:54:50 GMT  
		Size: 5.0 MB (5031625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4367e31da7eb2eb0c567ccc1355ff9d0582ae8830f2e5aa196ec5932e86c1f`  
		Last Modified: Fri, 11 Dec 2020 19:54:50 GMT  
		Size: 474.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cebd5bc320f12adb500f3bcb72f1a818853e608d75de0502a6ada07b37032a1c`  
		Last Modified: Fri, 11 Dec 2020 19:54:52 GMT  
		Size: 13.0 MB (13012084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d48ec757ad91784b83f975f0132ce3726aa7a4d659f554bf6ea37ab018d151a`  
		Last Modified: Fri, 11 Dec 2020 19:54:50 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340dce089fe777072edb3fdb7805f74b3d0b59411c4f110deaa9eef0aa30ca6b`  
		Last Modified: Fri, 11 Dec 2020 19:54:50 GMT  
		Size: 835.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
