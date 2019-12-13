## `wordpress:php7.2-fpm-alpine`

```console
$ docker pull wordpress@sha256:c49e3102403ae178459adbdc73ec5b71d9e86f5a283ad857812d383c1436c65e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `wordpress:php7.2-fpm-alpine` - linux; amd64

```console
$ docker pull wordpress@sha256:e8490c4e9181d60fe610c9923596119e96ea51bfa8fc8f898988a8666cfed1ff
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (68023498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:adbc5075cd7f0e1a4a5b86a51551dbe62e5e51534115dc1edf7b8fff089cfd9c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 20:38:08 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 21 Oct 2019 20:38:09 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 21 Oct 2019 20:38:10 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 21 Oct 2019 20:38:10 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 21 Oct 2019 20:38:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 21 Oct 2019 20:43:24 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 24 Oct 2019 01:15:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 01:15:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 01:15:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 24 Oct 2019 04:25:00 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 22 Nov 2019 13:48:20 GMT
ENV PHP_VERSION=7.2.25
# Fri, 22 Nov 2019 13:48:20 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.25.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.25.tar.xz.asc/from/this/mirror
# Fri, 22 Nov 2019 13:48:21 GMT
ENV PHP_SHA256=746efeedc38e6ff7b1ec1432440f5fa801537adf6cd21e4afb3f040e5b0760a9 PHP_MD5=
# Fri, 22 Nov 2019 13:48:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 22 Nov 2019 13:48:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Nov 2019 13:56:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 01:24:32 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 06 Dec 2019 01:24:34 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 01:24:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 01:24:34 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 01:24:35 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 06 Dec 2019 01:24:35 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Dec 2019 01:24:35 GMT
EXPOSE 9000
# Fri, 06 Dec 2019 01:24:35 GMT
CMD ["php-fpm"]
# Fri, 06 Dec 2019 03:20:29 GMT
RUN apk add --no-cache 		bash 		sed 		ghostscript
# Fri, 06 Dec 2019 03:21:26 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 06 Dec 2019 03:21:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 03:21:28 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 03:21:28 GMT
VOLUME [/var/www/html]
# Fri, 06 Dec 2019 03:21:28 GMT
ENV WORDPRESS_VERSION=5.3
# Fri, 06 Dec 2019 03:21:28 GMT
ENV WORDPRESS_SHA1=e3edcb1131e539c2b2e10fed37f8b6683c824a98
# Fri, 06 Dec 2019 03:21:37 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 06 Dec 2019 03:21:37 GMT
COPY file:2413d0c63f9d7b1d114697b18317719a02eadaaa61fc5d0c1edd96c027bc57a4 in /usr/local/bin/ 
# Fri, 06 Dec 2019 03:21:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Dec 2019 03:21:38 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feea9773e4044a213a29aa77e99239ac5e8f7f56877eab4f96530221d1323dae`  
		Last Modified: Mon, 21 Oct 2019 21:44:19 GMT  
		Size: 1.3 MB (1342556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e8ac5388d32433d5cbb16635a76d609f999bcb3ca7d1e5119e373f8da4de580`  
		Last Modified: Mon, 21 Oct 2019 21:44:19 GMT  
		Size: 1.3 KB (1254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3a226b9fe82df5bbc955b561faf3aa8df8a2faef7d2fd6cc00d95e855d4dd01`  
		Last Modified: Mon, 21 Oct 2019 21:44:18 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0a08ce1b2adeffbae29de68bfd4970552cfaa6392ef66f6a9ddd7bb6321d797`  
		Last Modified: Fri, 22 Nov 2019 14:42:35 GMT  
		Size: 12.3 MB (12298198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6940ed119d735badd9def1926347dee0dad048c295510622856977a8db3a07e`  
		Last Modified: Fri, 22 Nov 2019 14:42:33 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831a6d750410aeacea063fbe7db0e87c626b3019ae8f56be0c9aefd3d6b8af76`  
		Last Modified: Fri, 22 Nov 2019 14:42:38 GMT  
		Size: 14.7 MB (14710722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fb03ed20c72262f7f6b28ec56327512c1097fc8c323e81e96f9bb568740ee9`  
		Last Modified: Fri, 06 Dec 2019 01:30:24 GMT  
		Size: 2.2 KB (2220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179cfc41b10c4b6b55b63fc8822b000e0dcee67a84022ace88863976dbf7fb4b`  
		Last Modified: Fri, 06 Dec 2019 01:30:24 GMT  
		Size: 72.1 KB (72100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10e71220189f82fcb46f04ca5a8939576d08a299038ba9926400f6e03f23770`  
		Last Modified: Fri, 06 Dec 2019 01:30:25 GMT  
		Size: 7.8 KB (7790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43ec1df73236d057797315d88284d82a95f7bf6512483e81a56a764b69dd6f2d`  
		Last Modified: Fri, 06 Dec 2019 03:36:59 GMT  
		Size: 19.1 MB (19100748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:569eac1940f3c21fcd12f5ae9f371aa7d0d469e7772f4307ba418a148c369054`  
		Last Modified: Fri, 06 Dec 2019 03:36:55 GMT  
		Size: 5.5 MB (5485396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b98469b4f12cbf9cc647879b6d6ef9596fa56e18f59864a548ef73f9b7e31cd5`  
		Last Modified: Fri, 06 Dec 2019 03:36:54 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a470fed015dc825a33ee2059a105a3757397bb947534fb6bb353b703168d51a`  
		Last Modified: Fri, 06 Dec 2019 03:36:54 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b339a78e8dd6eb74da40881c35e4fe7a17c457e994be68d036b82dff1d765af9`  
		Last Modified: Fri, 06 Dec 2019 03:36:57 GMT  
		Size: 12.2 MB (12210040 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2219a5d223d53d5c11f7e0795bbb5e4f16aefaba5d0412fbe5b1f90abd34947`  
		Last Modified: Fri, 06 Dec 2019 03:36:54 GMT  
		Size: 3.9 KB (3893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.2-fpm-alpine` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:eaaa458dd11fc1984764a48cf181c93d7df4a0005f79d59a9273334ffe0e1677
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.9 MB (65924523 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5104387c0c8309c94908a6d9e1a93c127a01bda58c6705b067f1f9fd14a19b19`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 19:18:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 21 Oct 2019 19:18:13 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 21 Oct 2019 19:18:15 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 21 Oct 2019 19:18:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 21 Oct 2019 19:18:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 21 Oct 2019 19:21:42 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 23 Oct 2019 23:53:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Oct 2019 23:53:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Oct 2019 23:53:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 24 Oct 2019 00:26:11 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 22 Nov 2019 11:01:09 GMT
ENV PHP_VERSION=7.2.25
# Fri, 22 Nov 2019 11:01:15 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.25.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.25.tar.xz.asc/from/this/mirror
# Fri, 22 Nov 2019 11:01:21 GMT
ENV PHP_SHA256=746efeedc38e6ff7b1ec1432440f5fa801537adf6cd21e4afb3f040e5b0760a9 PHP_MD5=
# Fri, 22 Nov 2019 11:01:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 22 Nov 2019 11:01:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Nov 2019 11:08:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 00:56:49 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 06 Dec 2019 00:57:06 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 00:57:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 00:57:17 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 00:57:31 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 06 Dec 2019 00:57:32 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Dec 2019 00:57:33 GMT
EXPOSE 9000
# Fri, 06 Dec 2019 00:57:34 GMT
CMD ["php-fpm"]
# Fri, 06 Dec 2019 01:54:02 GMT
RUN apk add --no-cache 		bash 		sed 		ghostscript
# Fri, 06 Dec 2019 01:55:43 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 06 Dec 2019 01:55:49 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 01:55:52 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 01:55:53 GMT
VOLUME [/var/www/html]
# Fri, 13 Dec 2019 22:51:49 GMT
ENV WORDPRESS_VERSION=5.3.1
# Fri, 13 Dec 2019 22:51:51 GMT
ENV WORDPRESS_SHA1=3c635c9f6546782e0bb315784d4663d0e47f872e
# Fri, 13 Dec 2019 22:51:58 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 13 Dec 2019 22:51:58 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 13 Dec 2019 22:51:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Dec 2019 22:52:00 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:556f0528fef0a6877c5926ffeb18b55e87dc4776e3fdaede41fb036329a75cc3`  
		Last Modified: Mon, 21 Oct 2019 20:02:17 GMT  
		Size: 1.3 MB (1295196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06dccd8ebd353e14bda266ab0f1ad9c23bd12cc3f45cbb7986c7ae9e76f3050d`  
		Last Modified: Mon, 21 Oct 2019 20:02:16 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3ae71d8a6cd1d296213c9f1cbfc6ef1568f296a38cdd85d9d038b11eebc262`  
		Last Modified: Mon, 21 Oct 2019 20:02:16 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aae5b02cc8042ac38c016723bdf6f68f2860bc689df85087bceb7b8f1f9d443`  
		Last Modified: Fri, 22 Nov 2019 11:35:07 GMT  
		Size: 12.3 MB (12298230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c8fbab35a4895f721a03c417f41abd03064a9aa79149f0b0d5ce9d0b128ceae`  
		Last Modified: Fri, 22 Nov 2019 11:35:01 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ad0fda9b1a154abd61f14cabf23c924516a1df7c53562d0fa94c9e91703277`  
		Last Modified: Fri, 22 Nov 2019 11:35:09 GMT  
		Size: 13.6 MB (13631713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d9402d0775562c1866e0feec0ca56796bae2bd8e996f9249ca97ca61fd91b8`  
		Last Modified: Fri, 06 Dec 2019 01:03:23 GMT  
		Size: 2.2 KB (2223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3e0bd6c88e421f1b8126387458bfc71fad87eb817ce7549e8703101c3a949cc`  
		Last Modified: Fri, 06 Dec 2019 01:03:23 GMT  
		Size: 71.7 KB (71685 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbe5ebba7fa432b90e9b324bb1696b4c0cbb29b977d7e8e4688acd4830e120d`  
		Last Modified: Fri, 06 Dec 2019 01:03:24 GMT  
		Size: 7.8 KB (7790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6be96c2651644ac042abad8d8a267a7fe674037e7ec82b6e5b34436762de4c93`  
		Last Modified: Fri, 06 Dec 2019 02:10:11 GMT  
		Size: 18.5 MB (18507107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29eb2b1f3d249a43cffc9d8f18318963ef49a3b1af003a51780e3b81a19ee62b`  
		Last Modified: Fri, 06 Dec 2019 02:10:02 GMT  
		Size: 5.3 MB (5305128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4e90e6993c9c8bf3fdf95bf76a0331921fccc6ff86f4c557bd42f926085b91`  
		Last Modified: Fri, 06 Dec 2019 02:10:00 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d131afdbb49f83d85e6f06af1445565a3c04482ef20d3d31ec599d08dc011e9a`  
		Last Modified: Fri, 06 Dec 2019 02:10:00 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:247c0214ab62f7f93a65f8b270733278d915701f7fc1e872eedfd13aa1d01046`  
		Last Modified: Fri, 13 Dec 2019 22:53:24 GMT  
		Size: 12.2 MB (12227465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd0bd42442fbf94b892ed99b0c7cf8410c1cbb5177528e173685174012a443db`  
		Last Modified: Fri, 13 Dec 2019 22:53:18 GMT  
		Size: 3.9 KB (3897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.2-fpm-alpine` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:2e811a5b4a16d2dc772d65aa38fe9f6fc3bc6fffb4d963571bb9900716fda24f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63713910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19dd2b94a9ed040c8e60a403a5d1bd92263430c739c44e26d1628ead8abd7068`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 21 Oct 2019 18:15:18 GMT
ADD file:6b2893134302eabeb80e356fc4e5a29d9cd442362c382b3504688c014a734bb9 in / 
# Mon, 21 Oct 2019 18:15:31 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 21:14:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 21 Oct 2019 21:14:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 21 Oct 2019 21:14:53 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 21 Oct 2019 21:14:54 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 21 Oct 2019 21:14:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 21 Oct 2019 21:18:06 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 24 Oct 2019 00:46:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 00:46:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 00:46:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 24 Oct 2019 02:36:03 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 22 Nov 2019 12:50:08 GMT
ENV PHP_VERSION=7.2.25
# Fri, 22 Nov 2019 12:50:10 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.25.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.25.tar.xz.asc/from/this/mirror
# Fri, 22 Nov 2019 12:50:11 GMT
ENV PHP_SHA256=746efeedc38e6ff7b1ec1432440f5fa801537adf6cd21e4afb3f040e5b0760a9 PHP_MD5=
# Fri, 22 Nov 2019 12:50:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 22 Nov 2019 12:50:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Nov 2019 12:53:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 01:30:00 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 06 Dec 2019 01:30:07 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 01:30:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 01:30:11 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 01:30:16 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 06 Dec 2019 01:30:20 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Dec 2019 01:30:23 GMT
EXPOSE 9000
# Fri, 06 Dec 2019 01:30:28 GMT
CMD ["php-fpm"]
# Fri, 06 Dec 2019 03:15:48 GMT
RUN apk add --no-cache 		bash 		sed 		ghostscript
# Fri, 06 Dec 2019 03:17:19 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 06 Dec 2019 03:17:22 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 03:17:30 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 03:17:33 GMT
VOLUME [/var/www/html]
# Fri, 13 Dec 2019 23:12:39 GMT
ENV WORDPRESS_VERSION=5.3.1
# Fri, 13 Dec 2019 23:12:40 GMT
ENV WORDPRESS_SHA1=3c635c9f6546782e0bb315784d4663d0e47f872e
# Fri, 13 Dec 2019 23:12:46 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 13 Dec 2019 23:12:48 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 13 Dec 2019 23:12:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Dec 2019 23:12:49 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:99fc70ac0b64db67086f98ceb3942600816eed98046abd6be5ad66f4614a9ca2`  
		Last Modified: Mon, 21 Oct 2019 18:16:16 GMT  
		Size: 2.4 MB (2378437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da38e013862bbbf80dcededb060890e1056b0a21fb5308d8d1aae6f4add3bc7`  
		Last Modified: Mon, 21 Oct 2019 22:14:03 GMT  
		Size: 1.2 MB (1205015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d960e879727868f38a6a22fb9058a4ee346b2c22f8d1eda7663c2cfbdb499b5e`  
		Last Modified: Mon, 21 Oct 2019 22:14:00 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14285e1740413252e3ef469fc4e2fcd966f5efef93572ad2292b4073e5d8b592`  
		Last Modified: Mon, 21 Oct 2019 22:14:00 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea14c221362b6712c78363dee23191f289967b5e3d820c6b1c1b8d59c7de50b`  
		Last Modified: Fri, 22 Nov 2019 13:19:20 GMT  
		Size: 12.3 MB (12298229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcfac1d26c08226f595d486aadb1b70a61a019d20dd585a73fdbcea9e705f4f9`  
		Last Modified: Fri, 22 Nov 2019 13:19:16 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50cd65132cddb74765850a6c313fa3cd0e3a0ea333b1216b1a7702a04d1b22c`  
		Last Modified: Fri, 22 Nov 2019 13:19:21 GMT  
		Size: 12.7 MB (12712690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6667f3d4e3e5155e705b8bb44a4e2aebb22e76a9a1ea3664bb804bd7231e0cb`  
		Last Modified: Fri, 06 Dec 2019 01:41:23 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02d8f66561ec0761050ef6d064e22f20ba5658ed7351b8b1d6322211ef41e7b`  
		Last Modified: Fri, 06 Dec 2019 01:41:23 GMT  
		Size: 71.7 KB (71678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3322b13da15776e50985ad20b1c4453e48004c711d789d425d2887a12b59f39`  
		Last Modified: Fri, 06 Dec 2019 01:41:23 GMT  
		Size: 7.8 KB (7789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1e8a074f0eb25ebd5f63dbcbb1b197e1aa5924d20de62ec3a3e71d01a3e406`  
		Last Modified: Fri, 06 Dec 2019 03:56:14 GMT  
		Size: 17.7 MB (17714072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd40e5083c223a2b416bf59fedb095020e0be7f7a467cd51490bb83f1cb106b`  
		Last Modified: Fri, 06 Dec 2019 03:56:06 GMT  
		Size: 5.1 MB (5089622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcee48d4a1546690e4b42654089471f2b5da131e6bcee6045598bc3d9254f816`  
		Last Modified: Fri, 06 Dec 2019 03:56:06 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a09c29d9b8be9e5098efc550d33b5eb16787f870e326536f3d2f00ed163edea9`  
		Last Modified: Fri, 06 Dec 2019 03:56:06 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e1dd10138e8b33f4d0f6e1a397f26278b11bd28c0266cf6a121dacca1811f6`  
		Last Modified: Fri, 13 Dec 2019 23:16:35 GMT  
		Size: 12.2 MB (12227483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5309a6f80a5e612e75fb31cd16ada2688b626c07c8e48c21095d64a0eb290687`  
		Last Modified: Fri, 13 Dec 2019 23:16:30 GMT  
		Size: 3.9 KB (3898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.2-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:463ba38ba99cdc34aa43711d845ded8d715167e6e619f402a2832f100377181b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.7 MB (67716574 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d7493feaab181173c4253c7bbc81963b6c491b7a040a4ca74a66385c447fe0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 21:30:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 21 Oct 2019 21:30:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 21 Oct 2019 21:30:42 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 21 Oct 2019 21:30:43 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 21 Oct 2019 21:30:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 21 Oct 2019 21:36:37 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 24 Oct 2019 01:26:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 01:26:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 01:26:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 24 Oct 2019 03:18:59 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 22 Nov 2019 12:52:32 GMT
ENV PHP_VERSION=7.2.25
# Fri, 22 Nov 2019 12:52:33 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.25.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.25.tar.xz.asc/from/this/mirror
# Fri, 22 Nov 2019 12:52:33 GMT
ENV PHP_SHA256=746efeedc38e6ff7b1ec1432440f5fa801537adf6cd21e4afb3f040e5b0760a9 PHP_MD5=
# Fri, 22 Nov 2019 12:52:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 22 Nov 2019 12:52:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Nov 2019 12:55:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 01:25:11 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 06 Dec 2019 01:25:20 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 01:25:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 01:25:21 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 01:25:24 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 06 Dec 2019 01:25:25 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Dec 2019 01:25:26 GMT
EXPOSE 9000
# Fri, 06 Dec 2019 01:25:26 GMT
CMD ["php-fpm"]
# Fri, 06 Dec 2019 02:53:02 GMT
RUN apk add --no-cache 		bash 		sed 		ghostscript
# Fri, 06 Dec 2019 02:55:02 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 06 Dec 2019 02:55:05 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 02:55:09 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 02:55:10 GMT
VOLUME [/var/www/html]
# Fri, 13 Dec 2019 22:42:54 GMT
ENV WORDPRESS_VERSION=5.3.1
# Fri, 13 Dec 2019 22:42:54 GMT
ENV WORDPRESS_SHA1=3c635c9f6546782e0bb315784d4663d0e47f872e
# Fri, 13 Dec 2019 22:43:02 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 13 Dec 2019 22:43:04 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 13 Dec 2019 22:43:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 13 Dec 2019 22:43:06 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f7559d755b5d17673ff70e73b3efc81dd3bd4ce4489eeb38533321f94cc3ebe`  
		Last Modified: Mon, 21 Oct 2019 22:31:02 GMT  
		Size: 1.4 MB (1352864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7bf069919453424b5026db89f0b067a9234f9b089011a96855b488d18020924`  
		Last Modified: Mon, 21 Oct 2019 22:31:01 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d4149d516a6d5226b018c137de79dcd34670a6f862c40f5368bc157de9446a`  
		Last Modified: Mon, 21 Oct 2019 22:31:02 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9868bf2258125b8908781fc9da9891294852e6dcfe4a893d05c6e8ed3e69b52a`  
		Last Modified: Fri, 22 Nov 2019 13:22:33 GMT  
		Size: 12.3 MB (12298231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ecec6c56ad3b1ac5d0a13e3a9d08108516f222711b24f8671dc1f4d91d73be`  
		Last Modified: Fri, 22 Nov 2019 13:22:30 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c1b3b26ba7ff2d4edc90019077018c7a6052ee1849a70b8eae5f1dd47a25d02`  
		Last Modified: Fri, 22 Nov 2019 13:22:35 GMT  
		Size: 14.4 MB (14449639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae286f6fe13ff3322688163263501ab519aeff81d4d375c57dd03fbc165057e7`  
		Last Modified: Fri, 06 Dec 2019 01:37:17 GMT  
		Size: 2.2 KB (2221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b0ec603accf762751b27c0e82cb2b3d60d431d9582eea65ac67a69ddf2c537`  
		Last Modified: Fri, 06 Dec 2019 01:37:17 GMT  
		Size: 71.2 KB (71172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43015f70a0827dac767190f9b88edc8acbb334b0eedaf492315e0221e46accad`  
		Last Modified: Fri, 06 Dec 2019 01:37:17 GMT  
		Size: 7.8 KB (7794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b8ddcb1afa958d488a4cd82a06965ce4bfe190b28215cf49a6140dcd9b0a42f`  
		Last Modified: Fri, 06 Dec 2019 03:30:33 GMT  
		Size: 19.3 MB (19282624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58bb060a9f32608364c0eec13a7a19b9e33c48accf5b3b9d70de2b151533230`  
		Last Modified: Fri, 06 Dec 2019 03:30:26 GMT  
		Size: 5.3 MB (5300103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afc6857db28cd6ad3bffac3e00f21bce2350ab63583d209bb1eb9aa05e76cc7a`  
		Last Modified: Fri, 06 Dec 2019 03:30:24 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d91527dd8face104bcef92c5c34def0d03a1aac2f51c450cb999dc9e1e3006ab`  
		Last Modified: Fri, 06 Dec 2019 03:30:24 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9fc3edee7ac685159b7594769068b8f6b5de67d7496a96bf9ec2e32619ddb34`  
		Last Modified: Fri, 13 Dec 2019 22:46:48 GMT  
		Size: 12.2 MB (12227479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b906e95f73e4a4502fcb4e7ad89132e7b4b3da3b6958d04fecdb16eaecc6ab`  
		Last Modified: Fri, 13 Dec 2019 22:46:43 GMT  
		Size: 3.9 KB (3896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.2-fpm-alpine` - linux; 386

```console
$ docker pull wordpress@sha256:d08cd030b8c4077a179e59d1e7a91a52bdd19e960a57277b69a22fbd79912ecc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68977134 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2dd91a10f13cf30d94813840abb5084059ef2dd41213e4c63f56f4d2c56716ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 21 Oct 2019 16:46:04 GMT
ADD file:dd3b3676fd9c1e0983ade68242b9b9ac5c477f3e4bfc97c2e78fd5db93a441c9 in / 
# Mon, 21 Oct 2019 16:46:04 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 18:36:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 21 Oct 2019 18:36:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 21 Oct 2019 18:36:24 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 21 Oct 2019 18:36:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 21 Oct 2019 18:36:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 21 Oct 2019 18:44:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 24 Oct 2019 03:55:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 03:55:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 03:55:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 24 Oct 2019 10:58:51 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 22 Nov 2019 15:47:13 GMT
ENV PHP_VERSION=7.2.25
# Fri, 22 Nov 2019 15:47:13 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.25.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.25.tar.xz.asc/from/this/mirror
# Fri, 22 Nov 2019 15:47:13 GMT
ENV PHP_SHA256=746efeedc38e6ff7b1ec1432440f5fa801537adf6cd21e4afb3f040e5b0760a9 PHP_MD5=
# Fri, 22 Nov 2019 15:47:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 22 Nov 2019 15:47:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Nov 2019 15:56:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 00:44:21 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 06 Dec 2019 00:44:22 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 00:44:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 00:44:23 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 00:44:23 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 06 Dec 2019 00:44:23 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Dec 2019 00:44:24 GMT
EXPOSE 9000
# Fri, 06 Dec 2019 00:44:24 GMT
CMD ["php-fpm"]
# Fri, 06 Dec 2019 02:36:49 GMT
RUN apk add --no-cache 		bash 		sed 		ghostscript
# Fri, 06 Dec 2019 02:38:12 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 06 Dec 2019 02:38:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 02:38:14 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 02:38:15 GMT
VOLUME [/var/www/html]
# Fri, 06 Dec 2019 02:38:15 GMT
ENV WORDPRESS_VERSION=5.3
# Fri, 06 Dec 2019 02:38:15 GMT
ENV WORDPRESS_SHA1=e3edcb1131e539c2b2e10fed37f8b6683c824a98
# Fri, 06 Dec 2019 02:38:26 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 06 Dec 2019 02:38:26 GMT
COPY file:2413d0c63f9d7b1d114697b18317719a02eadaaa61fc5d0c1edd96c027bc57a4 in /usr/local/bin/ 
# Fri, 06 Dec 2019 02:38:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Dec 2019 02:38:27 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f913bd05bf684aaa4bc173d73cfbb58abb45587962d74f0aa71df36b6b489def`  
		Last Modified: Mon, 21 Oct 2019 16:46:25 GMT  
		Size: 2.8 MB (2785939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb445f03290fbac06f1d4fd8350bdccf0f042078682f16ca78d11decb2072f93`  
		Last Modified: Mon, 21 Oct 2019 20:16:10 GMT  
		Size: 1.4 MB (1433654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35ec15cffb9cdd39c9ce1901ab9a8d40f68a406e79255a5995f04c6eb2ce4496`  
		Last Modified: Mon, 21 Oct 2019 20:16:09 GMT  
		Size: 1.3 KB (1252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d85eba4a24ab26d8a873c36f3caeb67c15ce9d477047194007a6c37a12d7ef`  
		Last Modified: Mon, 21 Oct 2019 20:16:09 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e212660a91f5a96e151250f88962c897d27c3117ae72a85db3d0ec2c128e6d`  
		Last Modified: Fri, 22 Nov 2019 16:46:57 GMT  
		Size: 12.3 MB (12298207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5dfa4d442d920091f906985253a48278e43fd669eb557072605c764d463d74a`  
		Last Modified: Fri, 22 Nov 2019 16:46:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f828fcc965d78efee3fc7012478cb74f16edc68fd3ca02a50202dd30d00c0b0`  
		Last Modified: Fri, 22 Nov 2019 16:47:01 GMT  
		Size: 15.1 MB (15069824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d15cc3c72e92caac0b0e6353ce9c495557d1d94f65a41c86c5636b403861ac5`  
		Last Modified: Fri, 06 Dec 2019 00:49:26 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63fae371c37964d62537f0de4d039f64332e45578e5c6128ca4d2109ed8e12df`  
		Last Modified: Fri, 06 Dec 2019 00:49:26 GMT  
		Size: 71.2 KB (71237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf764f62b6e47c5d32b7899328f1a328a3866c17d71b917cef2877cba259d03`  
		Last Modified: Fri, 06 Dec 2019 00:49:26 GMT  
		Size: 7.8 KB (7785 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65b6c21a8fd738bb03c896625b40022a4d64b66ed2d68530f56b7bf835c9e96`  
		Last Modified: Fri, 06 Dec 2019 02:56:22 GMT  
		Size: 19.6 MB (19591327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad1569554deaec8c71c54b803036932d7e94fe6054c2f22f6e784ab3ca1069e`  
		Last Modified: Fri, 06 Dec 2019 02:56:16 GMT  
		Size: 5.5 MB (5500309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ccc836c291a53d298a50d61ace7a5fbf402ec9e48e8fd07bd9eeca488a53d99`  
		Last Modified: Fri, 06 Dec 2019 02:56:14 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88caf9f41a7c4db3481d6db4e84591f28704fd7cb68746f91de35831f68335e1`  
		Last Modified: Fri, 06 Dec 2019 02:56:14 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0e63fe5d31e313b354097996ec060e84eee2312cd43d51905f7363150955fe`  
		Last Modified: Fri, 06 Dec 2019 02:56:21 GMT  
		Size: 12.2 MB (12210034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e578cd33958d055a727ff68ae5ea2aedc47b6583d6397e6ae89c80795e44c52f`  
		Last Modified: Fri, 06 Dec 2019 02:56:14 GMT  
		Size: 3.9 KB (3896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.2-fpm-alpine` - linux; ppc64le

```console
$ docker pull wordpress@sha256:ec523f2860bcdc5ff3a1e8e32a99999c05ed77419fc73a558d8ba5061863b391
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.8 MB (69805684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:895b23b49e1c17e4dfea3259f04966d6e80a503902cfac3e5a1467ed39b03072`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 21 Oct 2019 17:52:55 GMT
ADD file:11a2dd0058b1642e9ee52239d03223819a53ca346fd42826eead7729c50e1257 in / 
# Mon, 21 Oct 2019 17:53:00 GMT
CMD ["/bin/sh"]
# Mon, 21 Oct 2019 19:21:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 21 Oct 2019 19:21:36 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 21 Oct 2019 19:21:44 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 21 Oct 2019 19:21:46 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 21 Oct 2019 19:21:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 21 Oct 2019 19:26:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 24 Oct 2019 01:21:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 01:21:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 24 Oct 2019 01:22:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 24 Oct 2019 03:29:19 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 22 Nov 2019 13:34:58 GMT
ENV PHP_VERSION=7.2.25
# Fri, 22 Nov 2019 13:35:01 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.25.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.25.tar.xz.asc/from/this/mirror
# Fri, 22 Nov 2019 13:35:06 GMT
ENV PHP_SHA256=746efeedc38e6ff7b1ec1432440f5fa801537adf6cd21e4afb3f040e5b0760a9 PHP_MD5=
# Fri, 22 Nov 2019 13:35:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 22 Nov 2019 13:35:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Nov 2019 13:39:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 06 Dec 2019 01:33:47 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 06 Dec 2019 01:33:53 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Dec 2019 01:33:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Dec 2019 01:33:59 GMT
WORKDIR /var/www/html
# Fri, 06 Dec 2019 01:34:05 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 06 Dec 2019 01:34:09 GMT
STOPSIGNAL SIGQUIT
# Fri, 06 Dec 2019 01:34:11 GMT
EXPOSE 9000
# Fri, 06 Dec 2019 01:34:15 GMT
CMD ["php-fpm"]
# Fri, 06 Dec 2019 05:20:27 GMT
RUN apk add --no-cache 		bash 		sed 		ghostscript
# Fri, 06 Dec 2019 05:21:45 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 06 Dec 2019 05:21:55 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 06 Dec 2019 05:22:01 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Dec 2019 05:22:04 GMT
VOLUME [/var/www/html]
# Fri, 06 Dec 2019 05:22:06 GMT
ENV WORDPRESS_VERSION=5.3
# Fri, 06 Dec 2019 05:22:10 GMT
ENV WORDPRESS_SHA1=e3edcb1131e539c2b2e10fed37f8b6683c824a98
# Fri, 06 Dec 2019 05:22:19 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 06 Dec 2019 05:22:21 GMT
COPY file:2413d0c63f9d7b1d114697b18317719a02eadaaa61fc5d0c1edd96c027bc57a4 in /usr/local/bin/ 
# Fri, 06 Dec 2019 05:22:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Dec 2019 05:22:26 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:cd18d16ea896a0f0eb99be52a9722ffae9a5ac35cf28cb8b96f589352f8e71d6`  
		Last Modified: Mon, 21 Oct 2019 17:53:53 GMT  
		Size: 2.8 MB (2808504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d017d7c8fce6fee939d22f8de103798d1fac32dfbedd09930f5811e4f7cda31d`  
		Last Modified: Mon, 21 Oct 2019 20:21:02 GMT  
		Size: 1.4 MB (1386418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b567e7413433d6d9c79cf4a2dc4d7a1598e8ade914bccc7208d605aac6f74c3f`  
		Last Modified: Mon, 21 Oct 2019 20:21:00 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05644b5a1ce87db12e6dd89e77db169a1b80755f9809cb3b374254737f8d7d51`  
		Last Modified: Mon, 21 Oct 2019 20:21:00 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b253cf611dedbc5836f5e5adf805d4031e61329d2675c0c57d5c4912e42689c`  
		Last Modified: Fri, 22 Nov 2019 14:22:00 GMT  
		Size: 12.3 MB (12298249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c436c2211176ca135bbbd3f24811e2cea76bac98be2c37e9d9d47800c2232a2e`  
		Last Modified: Fri, 22 Nov 2019 14:21:55 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe01d72c8b03df561036bcff5c9c0a75b39f815a083d7fe5cf46fb9d096e7ed4`  
		Last Modified: Fri, 22 Nov 2019 14:21:59 GMT  
		Size: 15.8 MB (15804938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a752e4512b07a56e3375ae8d24d14fd6ccb55474518eab821eaf8de3741054fe`  
		Last Modified: Fri, 06 Dec 2019 01:48:36 GMT  
		Size: 2.2 KB (2222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25567cba21af21cc713a293dcaf3fd3a071b7164f3ff526e17c3ed05f2e53842`  
		Last Modified: Fri, 06 Dec 2019 01:48:36 GMT  
		Size: 71.9 KB (71945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9300f16979a4679e31b7cc465e56b8399a34669b130d7702d5fe3129f4286eae`  
		Last Modified: Fri, 06 Dec 2019 01:48:36 GMT  
		Size: 7.8 KB (7795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:712682eeaccb08c5d4d69dc7df11d2862416bc101020c82e4d5f9b0e9d224a88`  
		Last Modified: Fri, 06 Dec 2019 06:28:39 GMT  
		Size: 19.7 MB (19705558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a9456c6f4683677783ed6340489ca6569ae7bab9da5f50c4b2bc500ded82c8`  
		Last Modified: Fri, 06 Dec 2019 06:28:18 GMT  
		Size: 5.5 MB (5503318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43abbc78ca7b9da0f18379db1cf714b4d286d69eaa66c888c05c78fc0590e1dd`  
		Last Modified: Fri, 06 Dec 2019 06:28:12 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf132bbf219b51b8110b7c0089198f38b541da95567b9cb9c16782d767282d4`  
		Last Modified: Fri, 06 Dec 2019 06:28:12 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a631cfb46bc514eb252996a0b7a650dd8c71aa87a90ec3f570f86c4022e46be4`  
		Last Modified: Fri, 06 Dec 2019 06:28:18 GMT  
		Size: 12.2 MB (12210054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1bc37cc61a8d821626f643badd9fe382dfefbb94f0f5859ed133e5d25d99181`  
		Last Modified: Fri, 06 Dec 2019 06:28:12 GMT  
		Size: 3.9 KB (3894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
