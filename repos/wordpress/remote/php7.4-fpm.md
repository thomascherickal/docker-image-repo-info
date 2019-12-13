## `wordpress:php7.4-fpm`

```console
$ docker pull wordpress@sha256:130d603dfb15364df02515857bdabe03ac4c4bbcedad27301e19a68a80b4a7d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `wordpress:php7.4-fpm` - linux; amd64

```console
$ docker pull wordpress@sha256:c01ee6c329d6576141615c4d5116b7e3f6edbbe413ced57f67db577fff4dafc7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **181.4 MB (181402995 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cdd86366035334fef8b4f8bcb81039b89ac27b27a0136ef1dee7c43536f75c11`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:09 GMT
ADD file:bc8179c87c8dbb3d962bed1801f99e7c860ff03797cde6ad19b107d43b973ada in / 
# Fri, 22 Nov 2019 14:55:10 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 15:46:31 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 22 Nov 2019 15:46:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 22 Nov 2019 15:46:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 15:47:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 22 Nov 2019 15:47:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 22 Nov 2019 16:01:22 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 22 Nov 2019 16:01:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 16:01:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 16:01:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Fri, 22 Nov 2019 16:01:23 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 28 Nov 2019 20:36:51 GMT
ENV PHP_VERSION=7.4.0
# Thu, 28 Nov 2019 20:36:51 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.0.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.0.tar.xz.asc/from/this/mirror
# Thu, 28 Nov 2019 20:36:52 GMT
ENV PHP_SHA256=9bb751b20e5d6cc1ea9b1ebf23ef2d5f07f99b2d9cc417bf1d70c04f8b20ec42 PHP_MD5=
# Thu, 28 Nov 2019 20:36:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 28 Nov 2019 20:36:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 28 Nov 2019 20:42:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 01:21:20 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 06 Dec 2019 01:21:21 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 01:21:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 01:21:21 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 01:21:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 06 Dec 2019 01:21:22 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Dec 2019 01:21:22 GMT
EXPOSE 9000
# Fri, 06 Dec 2019 01:21:23 GMT
CMD ["php-fpm"]
# Fri, 06 Dec 2019 03:29:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 03:30:57 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 03:30:58 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 03:30:59 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 03:30:59 GMT
VOLUME [/var/www/html]
# Fri, 06 Dec 2019 03:30:59 GMT
ENV WORDPRESS_VERSION=5.3
# Fri, 06 Dec 2019 03:30:59 GMT
ENV WORDPRESS_SHA1=e3edcb1131e539c2b2e10fed37f8b6683c824a98
# Fri, 06 Dec 2019 03:31:09 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 06 Dec 2019 03:31:09 GMT
COPY file:2413d0c63f9d7b1d114697b18317719a02eadaaa61fc5d0c1edd96c027bc57a4 in /usr/local/bin/ 
# Fri, 06 Dec 2019 03:31:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Dec 2019 03:31:10 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:000eee12ec04cc914bf96e8f5dee7767510c2aca3816af6078bd9fbe3150920c`  
		Last Modified: Fri, 22 Nov 2019 15:02:49 GMT  
		Size: 27.1 MB (27092654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ae4f9fcfeea62b9197d4d4597ac8cc5345bd9da718e89a49509af78476d2e40`  
		Last Modified: Fri, 22 Nov 2019 19:07:37 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f22fbbd07a4ea653467bc27962a5f8afccd9318c8f5c8b3b2afa58d8c9c2db`  
		Last Modified: Fri, 22 Nov 2019 19:07:55 GMT  
		Size: 76.7 MB (76652068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc7a63ad75ffb773427b460e6f531cca45c92111ba8bb214172a53e5e7ceba2`  
		Last Modified: Fri, 22 Nov 2019 19:07:37 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abad41ddce5b53469915c1c830231e321fa2fb00551aafc1ee7be16fc857222`  
		Last Modified: Thu, 28 Nov 2019 21:12:57 GMT  
		Size: 10.6 MB (10553074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd89eed1bd8bf315543d5999292dcde026620e28ff7bb146e40a636ee983a91c`  
		Last Modified: Thu, 28 Nov 2019 21:12:56 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89b8231e936cf61d19295134ba8b5dd4780cf1886c5065cca8aa241e04fa152f`  
		Last Modified: Thu, 28 Nov 2019 21:13:01 GMT  
		Size: 28.5 MB (28518511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6464deb7d652e7a44f8a82f644a713758e467319e26fb3026c6ff39f9667d3`  
		Last Modified: Fri, 06 Dec 2019 01:26:28 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:963ccb985b26c4860bd0ee967ac59cc97eb3147aa67a7671b009b8ceba8f0ef4`  
		Last Modified: Fri, 06 Dec 2019 01:26:28 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b393de0158b33c9319f7ba79eb34bfe869819c1a376e44c5d133b0fbf12398d`  
		Last Modified: Fri, 06 Dec 2019 01:26:28 GMT  
		Size: 8.4 KB (8419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4194422d9d63e3b45c41360ab43bb00fdbc2b5b7cafb14edacb41144e50cabc`  
		Last Modified: Fri, 06 Dec 2019 03:38:41 GMT  
		Size: 16.8 MB (16844806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f062ee3d2338d6d0aaae2d9621d8c5be19679090bf004adc4355d883adde072`  
		Last Modified: Fri, 06 Dec 2019 03:38:39 GMT  
		Size: 9.5 MB (9516095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05ccc4740130d1afb8dc7c4ada0f5b0fb51d1507dfd892003c656be51278f0b`  
		Last Modified: Fri, 06 Dec 2019 03:38:36 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e81bef6372c1433e9a0414d8e7a7adeca07bf61395431b31f3f26287770dfba`  
		Last Modified: Fri, 06 Dec 2019 03:38:36 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb7c3a1d67b1c7bd3202b16d051ba66e3d0c2d3decf6e4ca83de63a6dfe34e89`  
		Last Modified: Fri, 06 Dec 2019 03:38:39 GMT  
		Size: 12.2 MB (12209322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369f740ffaf8a98dce5785133765c6b54a2c03eebb0e2d4ee6dbd0bdc5f3891c`  
		Last Modified: Fri, 06 Dec 2019 03:38:35 GMT  
		Size: 3.9 KB (3897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.4-fpm` - linux; arm variant v5

```console
$ docker pull wordpress@sha256:19f599a974a0687c65d67ae8f77579d57f0153d487b51639e9d2e97110d53850
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.4 MB (158356923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:801314ac93569f1aa710f0a73104e82fba62a63eef6b2b4d4ed9cb3920e3fc7e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 22 Nov 2019 12:13:54 GMT
ADD file:94ed554e445cf749e10644dfa0d836103c120a6ea388bf6dc9f18f7c6b2f095a in / 
# Fri, 22 Nov 2019 12:13:56 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 12:28:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 22 Nov 2019 12:28:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 22 Nov 2019 12:29:17 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 12:29:20 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 22 Nov 2019 12:29:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 22 Nov 2019 12:39:01 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 22 Nov 2019 12:39:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 12:39:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 12:39:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Fri, 22 Nov 2019 12:39:04 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 28 Nov 2019 19:59:54 GMT
ENV PHP_VERSION=7.4.0
# Thu, 28 Nov 2019 19:59:55 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.0.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.0.tar.xz.asc/from/this/mirror
# Thu, 28 Nov 2019 19:59:55 GMT
ENV PHP_SHA256=9bb751b20e5d6cc1ea9b1ebf23ef2d5f07f99b2d9cc417bf1d70c04f8b20ec42 PHP_MD5=
# Thu, 28 Nov 2019 20:00:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 28 Nov 2019 20:00:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 28 Nov 2019 20:04:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 00:49:58 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 06 Dec 2019 00:50:05 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 00:50:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 00:50:28 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 00:50:46 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 06 Dec 2019 00:50:52 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Dec 2019 00:51:03 GMT
EXPOSE 9000
# Fri, 06 Dec 2019 00:51:09 GMT
CMD ["php-fpm"]
# Fri, 06 Dec 2019 03:30:30 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 03:36:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 03:36:33 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 03:36:39 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 03:36:42 GMT
VOLUME [/var/www/html]
# Fri, 13 Dec 2019 22:55:03 GMT
ENV WORDPRESS_VERSION=5.3.1
# Fri, 13 Dec 2019 22:55:03 GMT
ENV WORDPRESS_SHA1=3c635c9f6546782e0bb315784d4663d0e47f872e
# Fri, 13 Dec 2019 22:55:09 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 13 Dec 2019 22:55:10 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 13 Dec 2019 22:55:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Dec 2019 22:55:11 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:45ae7e8aa5bfd9e1b0db11d7fa5a56a8af11b69fc56707d763f89aa2c61b7e8f`  
		Last Modified: Fri, 22 Nov 2019 12:22:20 GMT  
		Size: 24.8 MB (24829480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1058ca8d797488ba0c2d7679f80443f86906e5b266ac3f533defc5be84ba8ee3`  
		Last Modified: Fri, 22 Nov 2019 14:42:32 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d09ee579a05967b60dc35947a1a6eee96a599461e6aab3ef950c5f4fb60825`  
		Last Modified: Fri, 22 Nov 2019 14:42:52 GMT  
		Size: 58.8 MB (58799873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:984298e877a210abb92274d4ba555ba6becc0f83aa91ca5bf71ac7b7edf0dcba`  
		Last Modified: Fri, 22 Nov 2019 14:42:32 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0f780b082a45a79bb9f96c0fe87527017eaccdce0986686775b199af70f024`  
		Last Modified: Thu, 28 Nov 2019 20:15:09 GMT  
		Size: 10.6 MB (10551485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de11225cfb7be357f380fbc53cb206bdc106469e1e1f1fc90a95bef9ebfb3994`  
		Last Modified: Thu, 28 Nov 2019 20:15:06 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10cc4ff9cf61d9c8cc99202930344b0fb0ff54d0b6780d70e49ae2913b408d3e`  
		Last Modified: Thu, 28 Nov 2019 20:15:15 GMT  
		Size: 27.2 MB (27151260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d99d3026da8475e8d5df888106b9f5da9a509dd6c23e1617363f0a4c32acef`  
		Last Modified: Fri, 06 Dec 2019 01:06:42 GMT  
		Size: 2.2 KB (2225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55509c6e72811e49daa4e94956d6051fa329fd0497d66060b6c114bd58e882b6`  
		Last Modified: Fri, 06 Dec 2019 01:06:42 GMT  
		Size: 253.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81a89522e68645cc2275cee2e860b467e51f7d3e121d36e9acd0c29ae8301e23`  
		Last Modified: Fri, 06 Dec 2019 01:06:42 GMT  
		Size: 8.4 KB (8421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1f9cadfd63f73d8f9a626b7d41bb775ba8154b6f0ad7babc15695eca667f356`  
		Last Modified: Fri, 06 Dec 2019 03:40:54 GMT  
		Size: 16.4 MB (16399424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412379ad18236041722c548ff2e0bf1954fd3e992608dc9293af32be714bbade`  
		Last Modified: Fri, 06 Dec 2019 03:40:47 GMT  
		Size: 8.4 MB (8382509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61680425ae562f0f60748e9cd45dbcb3d78ae2ae3c587033fa58d93e41cfa37`  
		Last Modified: Fri, 06 Dec 2019 03:40:45 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0c1070ae77ed25e3d625013abf19ca50a58ebc5aad005ecde97afbcd3a9f77`  
		Last Modified: Fri, 06 Dec 2019 03:40:45 GMT  
		Size: 401.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79796a0f6387b084ca900b5afbef9bbce48497e1327c86239b939684b267a058`  
		Last Modified: Fri, 13 Dec 2019 22:58:19 GMT  
		Size: 12.2 MB (12226378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c657e07025998f52b432d1aae0e95b95dd3124701968cb5b21377e3f306fa133`  
		Last Modified: Fri, 13 Dec 2019 22:58:13 GMT  
		Size: 3.9 KB (3892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.4-fpm` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:a312929f84f1e6b255eaefb968279a07f86d9ef7420f4372a4e5af71ecbe0a3f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.6 MB (154640690 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f91c0c187114156e6cab0064f86047057703c72ace11cceda473a4ead6800f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 22 Nov 2019 13:22:45 GMT
ADD file:85cf6081b7d1948b250d1b3749a65e2561cddafb7cd748db6b7b7420a376a48f in / 
# Fri, 22 Nov 2019 13:22:46 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 15:30:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 22 Nov 2019 15:30:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 22 Nov 2019 15:31:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 15:31:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 22 Nov 2019 15:31:46 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 22 Nov 2019 15:40:25 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 22 Nov 2019 15:40:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 15:40:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 15:40:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Fri, 22 Nov 2019 15:40:28 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 28 Nov 2019 20:11:38 GMT
ENV PHP_VERSION=7.4.0
# Thu, 28 Nov 2019 20:11:38 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.0.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.0.tar.xz.asc/from/this/mirror
# Thu, 28 Nov 2019 20:11:39 GMT
ENV PHP_SHA256=9bb751b20e5d6cc1ea9b1ebf23ef2d5f07f99b2d9cc417bf1d70c04f8b20ec42 PHP_MD5=
# Thu, 28 Nov 2019 20:11:56 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 28 Nov 2019 20:11:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 28 Nov 2019 20:15:33 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 01:16:38 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 06 Dec 2019 01:16:45 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 01:16:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 01:16:47 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 01:16:50 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 06 Dec 2019 01:16:54 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Dec 2019 01:16:58 GMT
EXPOSE 9000
# Fri, 06 Dec 2019 01:17:01 GMT
CMD ["php-fpm"]
# Fri, 06 Dec 2019 03:38:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 03:42:24 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 03:42:30 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 03:42:37 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 03:42:42 GMT
VOLUME [/var/www/html]
# Fri, 13 Dec 2019 23:13:59 GMT
ENV WORDPRESS_VERSION=5.3.1
# Fri, 13 Dec 2019 23:14:00 GMT
ENV WORDPRESS_SHA1=3c635c9f6546782e0bb315784d4663d0e47f872e
# Fri, 13 Dec 2019 23:14:10 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 13 Dec 2019 23:14:11 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 13 Dec 2019 23:14:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Dec 2019 23:14:12 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3cf3d03fb414460b7542c20e72fe29a83f08d22fd2c7a8cab1834eec2976e4b2`  
		Last Modified: Fri, 22 Nov 2019 13:33:25 GMT  
		Size: 22.7 MB (22699053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d332694ad538d1f749e4fdcacbe4a6623985ed44a42e43bce63a9722db08b2f`  
		Last Modified: Fri, 22 Nov 2019 17:35:23 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c8dc0f21f8205464804617dcf082c2798fa80a5e67d2ba4688e5ebaa9e107b`  
		Last Modified: Fri, 22 Nov 2019 17:35:41 GMT  
		Size: 59.5 MB (59501056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efbced36a6afa723160f24df74e373efd1409afd61b9af9d53109c1c8b721c28`  
		Last Modified: Fri, 22 Nov 2019 17:35:22 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f22d28f7e3d824ae9abe307e464ddfcd70c0841f9ea358e4e1198d7f74399583`  
		Last Modified: Thu, 28 Nov 2019 20:36:24 GMT  
		Size: 10.6 MB (10551441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd40f23347e600a3576e3187ff8a0b246bbfe9ccd19a756d6d81ec91a931558f`  
		Last Modified: Thu, 28 Nov 2019 20:36:21 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3770badbadee2541ade69f755a5cde643686d0892bfe082152fbb2fb51722348`  
		Last Modified: Thu, 28 Nov 2019 20:36:29 GMT  
		Size: 26.2 MB (26164294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde916c104b2c9b9b588abe3a955cb37c1257cfa48d909885e7145d115db8b88`  
		Last Modified: Fri, 06 Dec 2019 01:34:49 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd299a4f3faf19b604f42682144fc1e4887a85698defd0caef55782cc9dad156`  
		Last Modified: Fri, 06 Dec 2019 01:34:49 GMT  
		Size: 252.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee13237ef209287254607539bc93d8c4f4c476ad2f4a4f4b5daf371f89e2b976`  
		Last Modified: Fri, 06 Dec 2019 01:34:49 GMT  
		Size: 8.4 KB (8419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a75f2773cde5797de000f0c63d338d5754454cf3a9fafe3507fefc58f32a656`  
		Last Modified: Fri, 06 Dec 2019 03:59:01 GMT  
		Size: 16.0 MB (15951144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785deb7f91c9a755ae69ac7e936bd9794fce17409f5f192e0f98973633a9ac45`  
		Last Modified: Fri, 06 Dec 2019 03:58:53 GMT  
		Size: 7.5 MB (7530805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe49c0547ae47e3edc03865c1009fdac0d31f501ace4089b2707ef3c8aa6c109`  
		Last Modified: Fri, 06 Dec 2019 03:58:50 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e39389a498fdae40f537f4d1a5de11326d900c572f99771214c31ec1bfbdfd`  
		Last Modified: Fri, 06 Dec 2019 03:58:50 GMT  
		Size: 400.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baad798699e40fb1342039468894cbdc78c8f339f12439a322e2954b23c7e24a`  
		Last Modified: Fri, 13 Dec 2019 23:18:57 GMT  
		Size: 12.2 MB (12226383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:816d7da34c9f95e3c87bbe3a21cd2dd15188851ab886e77b1056fd25c40cf079`  
		Last Modified: Fri, 13 Dec 2019 23:18:52 GMT  
		Size: 3.9 KB (3896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.4-fpm` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:56c776063dc59cf309f683f02080da2f432c48cedad0d41db201802906c430e0
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.0 MB (171960160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a56ff452032843f3a55c6767747c6b6f015bf4eb49c9cf0847b9a386e5cb8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 22 Nov 2019 13:41:59 GMT
ADD file:69e0891ef62c74ec5e9bae38f8d2770ab2f0d7ea0d3cf1dc85875763be0b10b7 in / 
# Fri, 22 Nov 2019 13:42:02 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 14:29:54 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 22 Nov 2019 14:30:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 22 Nov 2019 14:30:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 14:30:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 22 Nov 2019 14:30:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 22 Nov 2019 14:39:29 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 22 Nov 2019 14:39:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 14:39:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 14:39:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Fri, 22 Nov 2019 14:39:34 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 28 Nov 2019 19:51:21 GMT
ENV PHP_VERSION=7.4.0
# Thu, 28 Nov 2019 19:51:22 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.0.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.0.tar.xz.asc/from/this/mirror
# Thu, 28 Nov 2019 19:51:23 GMT
ENV PHP_SHA256=9bb751b20e5d6cc1ea9b1ebf23ef2d5f07f99b2d9cc417bf1d70c04f8b20ec42 PHP_MD5=
# Thu, 28 Nov 2019 19:51:45 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 28 Nov 2019 19:51:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 28 Nov 2019 19:56:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 01:12:47 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 06 Dec 2019 01:12:54 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 01:12:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 01:12:57 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 01:12:59 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 06 Dec 2019 01:13:00 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Dec 2019 01:13:02 GMT
EXPOSE 9000
# Fri, 06 Dec 2019 01:13:03 GMT
CMD ["php-fpm"]
# Fri, 06 Dec 2019 03:14:16 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 03:18:30 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 03:18:36 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 03:18:41 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 03:18:44 GMT
VOLUME [/var/www/html]
# Fri, 13 Dec 2019 22:44:20 GMT
ENV WORDPRESS_VERSION=5.3.1
# Fri, 13 Dec 2019 22:44:21 GMT
ENV WORDPRESS_SHA1=3c635c9f6546782e0bb315784d4663d0e47f872e
# Fri, 13 Dec 2019 22:44:26 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 13 Dec 2019 22:44:27 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 13 Dec 2019 22:44:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Dec 2019 22:44:29 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a4f3dd4087f9309af4187e5dda90741441f057da59c2270598e16aa8019b0ca2`  
		Last Modified: Fri, 22 Nov 2019 13:49:50 GMT  
		Size: 25.9 MB (25850802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54f8c59bdaec8c1ab048fd2338d7e3089ffd471db8a7da2fa1b06ac9378eb2d`  
		Last Modified: Fri, 22 Nov 2019 16:35:55 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae19fe01dd7281aa7d623b1511e9f37b42de475fe01580853799b004a3cc54e`  
		Last Modified: Fri, 22 Nov 2019 16:36:16 GMT  
		Size: 70.3 MB (70334484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939a6e43e07c4339d2d353898d5f439d1903e980852de2083f6c0230629bd2e7`  
		Last Modified: Fri, 22 Nov 2019 16:35:56 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62a2727d4c00fc366db9d0fec016ae3e19a1469aa5484020e925418582a3a76d`  
		Last Modified: Thu, 28 Nov 2019 20:22:38 GMT  
		Size: 10.6 MB (10552091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499742f235aa31c3fa7477ec27359b3cd785c97473beba4b730945cb35955e92`  
		Last Modified: Thu, 28 Nov 2019 20:22:35 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f178b5320a4bac3516ddef4733637ad6b9243b206c0a847e2d50253b4180a77e`  
		Last Modified: Thu, 28 Nov 2019 20:22:45 GMT  
		Size: 28.3 MB (28269464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c211f57ac85244f9fab9b83f6bc3bdd66aaae491394c6d40e8515779ff98299`  
		Last Modified: Fri, 06 Dec 2019 01:31:14 GMT  
		Size: 2.2 KB (2222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6388a5c26a390bf3a5a9d257caf42ec3a54530fc00d154c4f4e31870aba696ed`  
		Last Modified: Fri, 06 Dec 2019 01:31:14 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53160e631b605349388c6a8602071da9d09e2d1d4256273522932e4dbc55fca`  
		Last Modified: Fri, 06 Dec 2019 01:31:14 GMT  
		Size: 8.4 KB (8420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98b105eae4339b64c5238a3378b4ffd4e499d395c1e8a0455a10826659eabe03`  
		Last Modified: Fri, 06 Dec 2019 03:33:17 GMT  
		Size: 16.8 MB (16777083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f6c1adf9d4e61a7416b6b40fcb2e88f32030e23fa5dc57d77135a2019d3d35`  
		Last Modified: Fri, 06 Dec 2019 03:33:12 GMT  
		Size: 7.9 MB (7933355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4b2c5f2ae936da5c8d1e4cd2444d135ae04264d9996776be27dfc18f4d261c`  
		Last Modified: Fri, 06 Dec 2019 03:33:10 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379a5d300f2a736eea10853edad2316dea2014a4011e944f1c9e045dcfa3b7a6`  
		Last Modified: Fri, 06 Dec 2019 03:33:09 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c55fd09827cd029ea1556861dfc93c7efc875d5409852cb50ed7b355a36882`  
		Last Modified: Fri, 13 Dec 2019 22:48:54 GMT  
		Size: 12.2 MB (12226376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca470d628bff60ff3f8485921ae1b741ce2d00c5a7fd82fc6e89df058941477`  
		Last Modified: Fri, 13 Dec 2019 22:48:49 GMT  
		Size: 3.9 KB (3890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.4-fpm` - linux; 386

```console
$ docker pull wordpress@sha256:2421702be29393cd050eca30d8fc0ff5855efcf2419489927530b81183165391
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **186.8 MB (186782875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e8f925f560ec0bc92d43e9360dd0df5bfa0c374aa44ef9615864e3c95711d55`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 22 Nov 2019 16:50:19 GMT
ADD file:68f0911eb53ffc655e6a641b4acfb0670c2fd84c7dc34b0128735f0478532a6b in / 
# Fri, 22 Nov 2019 16:50:19 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 19:18:16 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 22 Nov 2019 19:18:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 22 Nov 2019 19:18:46 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 19:18:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 22 Nov 2019 19:18:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 22 Nov 2019 19:29:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 22 Nov 2019 19:29:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 19:29:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 19:29:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Fri, 22 Nov 2019 19:29:35 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 28 Nov 2019 19:52:11 GMT
ENV PHP_VERSION=7.4.0
# Thu, 28 Nov 2019 19:52:11 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.0.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.0.tar.xz.asc/from/this/mirror
# Thu, 28 Nov 2019 19:52:11 GMT
ENV PHP_SHA256=9bb751b20e5d6cc1ea9b1ebf23ef2d5f07f99b2d9cc417bf1d70c04f8b20ec42 PHP_MD5=
# Thu, 28 Nov 2019 19:52:19 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 28 Nov 2019 19:52:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 28 Nov 2019 19:57:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 00:41:22 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 06 Dec 2019 00:41:23 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 00:41:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 00:41:24 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 00:41:24 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 06 Dec 2019 00:41:24 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Dec 2019 00:41:25 GMT
EXPOSE 9000
# Fri, 06 Dec 2019 00:41:25 GMT
CMD ["php-fpm"]
# Fri, 06 Dec 2019 02:47:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 02:49:38 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 02:49:39 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 02:49:40 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 02:49:40 GMT
VOLUME [/var/www/html]
# Fri, 06 Dec 2019 02:49:40 GMT
ENV WORDPRESS_VERSION=5.3
# Fri, 06 Dec 2019 02:49:40 GMT
ENV WORDPRESS_SHA1=e3edcb1131e539c2b2e10fed37f8b6683c824a98
# Fri, 06 Dec 2019 02:49:48 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 06 Dec 2019 02:49:48 GMT
COPY file:2413d0c63f9d7b1d114697b18317719a02eadaaa61fc5d0c1edd96c027bc57a4 in /usr/local/bin/ 
# Fri, 06 Dec 2019 02:49:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Dec 2019 02:49:48 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:ce9b44038a207698571bb0cc0b950ee2a3608cb09b2b20712b353a54ae619111`  
		Last Modified: Fri, 22 Nov 2019 16:58:27 GMT  
		Size: 27.7 MB (27746760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed961f8f7a554aab7872678c1e2706e804ac741f6ab6db08d468f95281c88da`  
		Last Modified: Fri, 22 Nov 2019 22:13:02 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077599002175aec10526395f1b56a347a4e6d6b5a6bd9320c9b42bad0768df3c`  
		Last Modified: Fri, 22 Nov 2019 22:13:27 GMT  
		Size: 81.2 MB (81199104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e59337e9a9db23ff3d6d91ee673a989078459ee463b0e7cd7a9875b071b3ca7b`  
		Last Modified: Fri, 22 Nov 2019 22:13:01 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4f67a15391c9f53ddd8d072e9b4fffb8b3ee40a9067ab14c16c2390e9ea31f`  
		Last Modified: Thu, 28 Nov 2019 20:25:06 GMT  
		Size: 10.6 MB (10552422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bed5e009b7c3054b602d6fa86cc08aeeb69dd73596a5ba27615ab265f6043969`  
		Last Modified: Thu, 28 Nov 2019 20:25:04 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c478e9867227dd0c67f1a9e7de23000b15067c926954be0d2a35b671479fcb`  
		Last Modified: Thu, 28 Nov 2019 20:25:12 GMT  
		Size: 29.1 MB (29104283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9701ec5d4022853706b753a49e901983db1c8687ef799220260425448aa1d52d`  
		Last Modified: Fri, 06 Dec 2019 00:46:12 GMT  
		Size: 2.2 KB (2220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78bdf0e837d5756631567d128ef827a35f479ecf3abd85164b1a84b9668a839`  
		Last Modified: Fri, 06 Dec 2019 00:46:12 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3a1ea98dcbd50f88b9aca0f796e64c8e90c353bf57cef650ce270b63861643`  
		Last Modified: Fri, 06 Dec 2019 00:46:11 GMT  
		Size: 8.4 KB (8421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1988a0994601e0a71fe59ca4a739498596a6cfa3dbaf4848512a4cb83a42925a`  
		Last Modified: Fri, 06 Dec 2019 02:58:07 GMT  
		Size: 17.2 MB (17157938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99539d3350b3a77b2a15b146fd47307c21a2eeca577715fb5e47aca2a155d9f4`  
		Last Modified: Fri, 06 Dec 2019 02:58:00 GMT  
		Size: 8.8 MB (8796583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a19ac78ab5195c1d2636d71bf471b83f164ee6d468157f72d778ffbfdddfd3`  
		Last Modified: Fri, 06 Dec 2019 02:57:55 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37dcf2b1c4693f7ca141a6714994c366fb891ba71194ce0b2581f7b55733ea89`  
		Last Modified: Fri, 06 Dec 2019 02:57:55 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cf6d23be908bb522316939e2039b739bbbd3e3dc14c310e4dfe8ef20ebb8c41`  
		Last Modified: Fri, 06 Dec 2019 02:58:05 GMT  
		Size: 12.2 MB (12209321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454907c5df25ec605734126cd93a09bcdb6212dd940683e971eaa4dc5fe5c078`  
		Last Modified: Fri, 06 Dec 2019 02:57:55 GMT  
		Size: 3.9 KB (3895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.4-fpm` - linux; ppc64le

```console
$ docker pull wordpress@sha256:1e82da82a3baaebdf4c557ca1542cc381a6af7bbffbe4602f4b1c01644357c48
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.8 MB (192770660 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3c6cd71e84bc9df2590b6eccad983e7b56c683b3caf99351ff527a289c39539`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 22 Nov 2019 14:55:33 GMT
ADD file:56ee7f5cc8715d22f4efb9ec5b1c24fac7fdf8f6dc9c07c45625c4f89bdccac3 in / 
# Fri, 22 Nov 2019 14:55:37 GMT
CMD ["bash"]
# Fri, 22 Nov 2019 15:54:24 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Fri, 22 Nov 2019 15:54:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Fri, 22 Nov 2019 15:56:31 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 22 Nov 2019 15:56:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 22 Nov 2019 15:56:40 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 22 Nov 2019 16:08:07 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 22 Nov 2019 16:08:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 16:08:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 22 Nov 2019 16:08:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Fri, 22 Nov 2019 16:08:14 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 28 Nov 2019 20:34:01 GMT
ENV PHP_VERSION=7.4.0
# Thu, 28 Nov 2019 20:34:03 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.0.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.0.tar.xz.asc/from/this/mirror
# Thu, 28 Nov 2019 20:34:09 GMT
ENV PHP_SHA256=9bb751b20e5d6cc1ea9b1ebf23ef2d5f07f99b2d9cc417bf1d70c04f8b20ec42 PHP_MD5=
# Thu, 28 Nov 2019 20:34:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 28 Nov 2019 20:34:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 28 Nov 2019 20:38:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libonig-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 01:21:03 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 06 Dec 2019 01:21:08 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 01:21:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 01:21:12 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 01:21:17 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 06 Dec 2019 01:21:19 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Dec 2019 01:21:20 GMT
EXPOSE 9000
# Fri, 06 Dec 2019 01:21:21 GMT
CMD ["php-fpm"]
# Fri, 06 Dec 2019 06:04:34 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 06:15:24 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 06 Dec 2019 06:15:32 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 06:15:40 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 06:15:43 GMT
VOLUME [/var/www/html]
# Fri, 06 Dec 2019 06:15:47 GMT
ENV WORDPRESS_VERSION=5.3
# Fri, 06 Dec 2019 06:15:54 GMT
ENV WORDPRESS_SHA1=e3edcb1131e539c2b2e10fed37f8b6683c824a98
# Fri, 06 Dec 2019 06:16:10 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 06 Dec 2019 06:16:14 GMT
COPY file:2413d0c63f9d7b1d114697b18317719a02eadaaa61fc5d0c1edd96c027bc57a4 in /usr/local/bin/ 
# Fri, 06 Dec 2019 06:16:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Dec 2019 06:16:19 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:e190211f5678d77388755410611e5e6a755e195e7a1096473c675edc074a2389`  
		Last Modified: Fri, 22 Nov 2019 15:04:10 GMT  
		Size: 30.5 MB (30517327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d2a4c8dd52eee84e0b2c048f8db6f8de263a31df8647418e2ff962d839741d`  
		Last Modified: Fri, 22 Nov 2019 18:52:21 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956265206842c78209185fe0d49498b925db99ec94ffa6658904bc0ac86171e3`  
		Last Modified: Fri, 22 Nov 2019 18:52:54 GMT  
		Size: 82.3 MB (82259548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922b0fcf8aed82cfcadde2a647ede9cae5dce14ec49dfb88d8885bbcef8b152a`  
		Last Modified: Fri, 22 Nov 2019 18:52:20 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb41d180e7e4a5b955f438339be89a84319ab4b74f7c887a7f7c4c19f4b5420e`  
		Last Modified: Thu, 28 Nov 2019 21:09:06 GMT  
		Size: 10.6 MB (10552944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1c2e6031f45d2d4d477dee101c229a91eb42299c099ec120ed3a79405d28d6`  
		Last Modified: Thu, 28 Nov 2019 21:09:01 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42bf9c491e7b60f77f4c73fc394eeec052da869def27ac041e638655c47677c`  
		Last Modified: Thu, 28 Nov 2019 21:09:11 GMT  
		Size: 30.2 MB (30204814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de1946ee1caefd46603f9b95aa4d91afa1c3cedc40ecf5888308dac167163a7f`  
		Last Modified: Fri, 06 Dec 2019 01:39:33 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:869e1846e85fc03936a3f4dfbc331af182217601a3ea13390491930bb3cd695e`  
		Last Modified: Fri, 06 Dec 2019 01:39:33 GMT  
		Size: 250.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e7b50943794c7fa668975efa744d6b03946f1a6156edea4f949dfa0f26b647`  
		Last Modified: Fri, 06 Dec 2019 01:39:33 GMT  
		Size: 8.4 KB (8420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78bb3cb648213cb50dc6dbf35fec660e642f3583023e3262b623efe7099edf4f`  
		Last Modified: Fri, 06 Dec 2019 06:33:11 GMT  
		Size: 17.6 MB (17623488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6544762f8c38ae0d5d8b9cc05897c1eefbc28d8de123bb7d525c5569b60a5712`  
		Last Modified: Fri, 06 Dec 2019 06:33:06 GMT  
		Size: 9.4 MB (9386711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:624cd85cef4cbbab94d31b54d8586660996b0af81b4faa483994c733435929e9`  
		Last Modified: Fri, 06 Dec 2019 06:32:57 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c52cbc049db05a3c905e102571e863a89d0263551bf18d78022ac0189f7f606d`  
		Last Modified: Fri, 06 Dec 2019 06:32:57 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0bb8c1db04c628a6a435e1db5badb727380524a367b28379f823a5ab0fcc38`  
		Last Modified: Fri, 06 Dec 2019 06:33:11 GMT  
		Size: 12.2 MB (12209317 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccf3e846bbadfd1f3afb00b7c545a53ac26de10a1356da68fbe88ed481eabea7`  
		Last Modified: Fri, 06 Dec 2019 06:32:57 GMT  
		Size: 3.9 KB (3897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
