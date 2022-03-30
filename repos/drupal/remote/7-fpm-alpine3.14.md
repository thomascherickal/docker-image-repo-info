## `drupal:7-fpm-alpine3.14`

```console
$ docker pull drupal@sha256:a0c5006631dbfe136e5ce71c57c71e0b6fdccf730982dd9541f1934210adbb4e
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

### `drupal:7-fpm-alpine3.14` - linux; amd64

```console
$ docker pull drupal@sha256:6d560fdbf97c50b648debf0ea85fe35c5b1786fd505bdffc675d462f6d9b8387
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31973174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21fb369b211dd2311579001f44d64f797c9afa70c367af8e2f31dedcc3b01f62`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 29 Mar 2022 00:19:41 GMT
ADD file:900b3c9d6bd18f94bde19b8eb177a55f956f4030deea9171e6c3da797a213636 in / 
# Tue, 29 Mar 2022 00:19:41 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 02:06:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 29 Mar 2022 02:06:33 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 29 Mar 2022 02:06:33 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 29 Mar 2022 02:06:33 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 02:06:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 02:06:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:06:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:06:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 03:58:34 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 29 Mar 2022 03:58:34 GMT
ENV PHP_VERSION=7.4.28
# Tue, 29 Mar 2022 03:58:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 29 Mar 2022 03:58:35 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 29 Mar 2022 03:58:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 29 Mar 2022 03:58:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 04:09:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 04:09:00 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 04:09:01 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 04:09:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 04:09:02 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 04:09:02 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 04:09:02 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 04:09:02 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 04:09:03 GMT
CMD ["php-fpm"]
# Wed, 30 Mar 2022 07:24:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 30 Mar 2022 07:24:07 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 30 Mar 2022 07:27:41 GMT
ENV DRUPAL_VERSION=7.89
# Wed, 30 Mar 2022 07:27:42 GMT
ENV DRUPAL_MD5=924e707e3b1e8269fe623cf2f22ee710
# Wed, 30 Mar 2022 07:27:43 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:cfab2db722092277479ddd659049695fa8081d2a03c31b01d388cc21802de8b4`  
		Last Modified: Tue, 29 Mar 2022 00:20:33 GMT  
		Size: 2.8 MB (2818354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7db1360ca6629c5e82671b970611b689f50275b0a9266b837143de7b176583d1`  
		Last Modified: Tue, 29 Mar 2022 04:23:07 GMT  
		Size: 1.7 MB (1703105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8a7fc89eb93c3c45bf44eaf065da90232608fc171f3188569689f9c3e8ca01`  
		Last Modified: Tue, 29 Mar 2022 04:23:07 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581222eb1f817aa7721035ac6c13a316ac918cdf26eb54966f44f1480011707d`  
		Last Modified: Tue, 29 Mar 2022 04:23:07 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843105d67b9200038853dc6111751db006e4778314b2a0b71dc20fbf2bdce0cf`  
		Last Modified: Tue, 29 Mar 2022 04:32:39 GMT  
		Size: 10.4 MB (10438241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84eb4722e0e8a57171d215f74744b355964d4c9e4809d0db6c0ce3bb6119d005`  
		Last Modified: Tue, 29 Mar 2022 04:32:38 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c9382e16ec9895bf11b39e96fa792646fe186e6575a8fa6a86a8828ca027fbf`  
		Last Modified: Tue, 29 Mar 2022 04:33:02 GMT  
		Size: 11.4 MB (11428665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe80696743b5f063fe77f2162260fd25e90d10b7e36baecf3ca62bdcee638de3`  
		Last Modified: Tue, 29 Mar 2022 04:33:00 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0d1903ef75e6fd6a549e6063b4b968f9d967d14a7ad04cfeade82e70c9e0bc`  
		Last Modified: Tue, 29 Mar 2022 04:33:00 GMT  
		Size: 18.3 KB (18323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50468a85e5161187351785821483471f0509d043b01b3b337fff6fa8605a4e5`  
		Last Modified: Tue, 29 Mar 2022 04:33:00 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a082ff7d1516f693a33d6ab6da2c3bb411a238403d726aed6b1aea7ad1911e89`  
		Last Modified: Wed, 30 Mar 2022 07:42:31 GMT  
		Size: 2.2 MB (2169874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f06756d56a260d861573b5cd78946efc43fbf3c5872a1f41f6ee4cd91c9effc`  
		Last Modified: Wed, 30 Mar 2022 07:42:31 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45fca77cd8bed020eb5964c6897a46a01db0f680fb01540cf88ef61bdd562f3d`  
		Last Modified: Wed, 30 Mar 2022 07:50:06 GMT  
		Size: 3.4 MB (3383373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-fpm-alpine3.14` - linux; arm variant v6

```console
$ docker pull drupal@sha256:c5ba1ff421e88f8d9d6af89f8774bbe2f61e4d4a1203cd3434fe0fb7b68eab8a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30852928 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07d5d0b28746967f18cbdd4f998990f4dca55933388c3e90c2dd479db5f34981`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 29 Mar 2022 00:49:46 GMT
ADD file:9670f4f7de6a9b8eb844e418daedd0dbad90009126790eb65e246b29cac5ea47 in / 
# Tue, 29 Mar 2022 00:49:46 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 01:03:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 29 Mar 2022 01:03:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 29 Mar 2022 01:03:06 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 29 Mar 2022 01:03:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 01:03:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 01:03:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:03:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:03:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 01:47:50 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 29 Mar 2022 01:47:51 GMT
ENV PHP_VERSION=7.4.28
# Tue, 29 Mar 2022 01:47:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 29 Mar 2022 01:47:51 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 29 Mar 2022 01:48:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 29 Mar 2022 01:48:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 01:57:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 01:57:40 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 01:57:43 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 01:57:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 01:57:43 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 01:57:45 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 01:57:45 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 01:57:46 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 01:57:46 GMT
CMD ["php-fpm"]
# Tue, 29 Mar 2022 03:08:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 29 Mar 2022 03:08:27 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 29 Mar 2022 03:12:54 GMT
ENV DRUPAL_VERSION=7.89
# Tue, 29 Mar 2022 03:12:54 GMT
ENV DRUPAL_MD5=924e707e3b1e8269fe623cf2f22ee710
# Tue, 29 Mar 2022 03:12:58 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:79f5c9df0b90097bae07a9861e9e0e3f52a16b0bfde2793c4e14ad033cfb47f4`  
		Last Modified: Tue, 29 Mar 2022 00:51:45 GMT  
		Size: 2.6 MB (2626017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e68acfb8e127d2000623a5b46b3ad33f9390aa70683d5a7e3ac3953342ab3d3d`  
		Last Modified: Tue, 29 Mar 2022 02:11:05 GMT  
		Size: 1.7 MB (1691160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b361518c45781f43fe4762fce5917a961584d0ecc89203bafe481dfada1d0ae1`  
		Last Modified: Tue, 29 Mar 2022 02:11:04 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d1e46eaa8bdfc75786427e73b0f17121c1a7d669842d21e2b4d9bf0915ff29`  
		Last Modified: Tue, 29 Mar 2022 02:11:04 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8997297f857789a5e49981430ac77be2e3a41dd72277cc11e2cfe21896c90a1c`  
		Last Modified: Tue, 29 Mar 2022 02:16:28 GMT  
		Size: 10.4 MB (10438240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681ecdd4d6239307e8ff2d1d457a3c653a587b7e4c55a6ad3ce9f71dc90adc6b`  
		Last Modified: Tue, 29 Mar 2022 02:16:26 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f936abec68e630715e45cf0e4d8cfd6783a0c7f97f9826bafe2e30ea82dca3`  
		Last Modified: Tue, 29 Mar 2022 02:17:12 GMT  
		Size: 10.7 MB (10707867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c106003292e835a933ed69474a3cd1119b8aab85d1507c8ce69c57e0357228`  
		Last Modified: Tue, 29 Mar 2022 02:17:04 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daf8fd04cb350d28c85b4d5a60eafa52c5652be384fbeec75f50b1af2a030eb4`  
		Last Modified: Tue, 29 Mar 2022 02:17:04 GMT  
		Size: 18.3 KB (18343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3837c0f6917f736004c7699d5073f1c302eda89c7af6a98805759f138b516778`  
		Last Modified: Tue, 29 Mar 2022 02:17:04 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:646ff62e4b5f87a0f160bd7d5b5cb62ab85592e7b287693483a08df5f22a3e62`  
		Last Modified: Tue, 29 Mar 2022 03:23:45 GMT  
		Size: 2.0 MB (1974686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8b937a7ec7301ded5fd5bd6d59101ccdd019502b68d793734b8a223a65fec8`  
		Last Modified: Tue, 29 Mar 2022 03:23:44 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d8eede04fdaa500ba81a7d313a2bf778979817f6ca5faad26733a2ebe92123`  
		Last Modified: Tue, 29 Mar 2022 03:28:26 GMT  
		Size: 3.4 MB (3383375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-fpm-alpine3.14` - linux; arm variant v7

```console
$ docker pull drupal@sha256:91a2ce129be1970cf1b5691b55544fb62e17d42a95311e3e6f78b87109af1677
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29714397 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3c8fd8d8eb13dc673344e9ab6a63d735f9eae695e2cd49c134a053989931fe28`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 29 Mar 2022 02:13:44 GMT
ADD file:4c399e6082c49459f8606095d7261eddd2bbaa65359199c3fdc4d2cc068a67f9 in / 
# Tue, 29 Mar 2022 02:13:44 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 07:41:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 29 Mar 2022 07:41:52 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 29 Mar 2022 07:41:54 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 29 Mar 2022 07:41:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 07:41:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 07:41:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 07:41:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 07:41:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 09:54:15 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 29 Mar 2022 09:54:16 GMT
ENV PHP_VERSION=7.4.28
# Tue, 29 Mar 2022 09:54:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 29 Mar 2022 09:54:17 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 29 Mar 2022 09:54:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 29 Mar 2022 09:54:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:04:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 10:04:12 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 10:04:15 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 10:04:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 10:04:17 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 10:04:19 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 10:04:19 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 10:04:20 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 10:04:20 GMT
CMD ["php-fpm"]
# Tue, 29 Mar 2022 11:54:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 29 Mar 2022 11:54:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 29 Mar 2022 12:06:46 GMT
ENV DRUPAL_VERSION=7.89
# Tue, 29 Mar 2022 12:06:47 GMT
ENV DRUPAL_MD5=924e707e3b1e8269fe623cf2f22ee710
# Tue, 29 Mar 2022 12:06:50 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:994307ea7bfd1233222fa14c4fc32b8b85be60f9840c03fba9299eb918066ef3`  
		Last Modified: Tue, 29 Mar 2022 02:15:47 GMT  
		Size: 2.4 MB (2427966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d54f9e882a75e957680bbb788bf5a094e6a788d69b093f489fef69498cf6f7`  
		Last Modified: Tue, 29 Mar 2022 10:38:06 GMT  
		Size: 1.6 MB (1558928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac5ce9becbc99b4ca9ab350939bdb94a5657465e688f0d4e6413d07d0454a27`  
		Last Modified: Tue, 29 Mar 2022 10:38:05 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a430efedf2eda2718b96667efdf683a05edad9eeae68dae93431bd6d008ef291`  
		Last Modified: Tue, 29 Mar 2022 10:38:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7546af505a623060e9720a631828f5744337383a1c7aaa19973cd4781509ca27`  
		Last Modified: Tue, 29 Mar 2022 10:52:12 GMT  
		Size: 10.4 MB (10438226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25304aa20edddac4fc5793b7cce321debf1480d64a531dcb9add8a507ccf3ff7`  
		Last Modified: Tue, 29 Mar 2022 10:52:10 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dccbb4cb1495b46a9d439da7bd489464a0ee2482671b4d553719f9018981c8d`  
		Last Modified: Tue, 29 Mar 2022 10:52:51 GMT  
		Size: 10.1 MB (10064429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb5739e7b7db6eefcf8488b69785a10d2829370960e41db12b7b4a2bfb4f0a7`  
		Last Modified: Tue, 29 Mar 2022 10:52:47 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2384bf07d8ce9065b5c80676a597054904dc2e3f74d3f55cb3fad90c8733980`  
		Last Modified: Tue, 29 Mar 2022 10:52:47 GMT  
		Size: 18.3 KB (18324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f794bef1b2533a2edd8b5f05adfa3f8aba2dffefedd966df97c96b3e2ef5a48`  
		Last Modified: Tue, 29 Mar 2022 10:52:47 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae394586c1d203cb5373afe5941022662a40db2a0493aba82918021ec5208d62`  
		Last Modified: Tue, 29 Mar 2022 14:23:15 GMT  
		Size: 1.8 MB (1809906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1784feb92883b8b3d451830ae1ef48b9aacc5df77ce965ed08f1ab59fdaa9e99`  
		Last Modified: Tue, 29 Mar 2022 14:23:14 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c49d7481c36c92362154d5dd12d946f498a18bbc02bcdb49c6b2c3fca97311`  
		Last Modified: Tue, 29 Mar 2022 14:37:32 GMT  
		Size: 3.4 MB (3383371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-fpm-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:f3989aee2017e402a0da3f89b2483abfd4f096e92ccaeccf5dbbac79bd796aa4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.7 MB (31660082 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ac3d317892466cfec722831c3ef1429c31e0c23193ae398874d8e40b55973bb`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 19:00:08 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 18 Mar 2022 19:00:09 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 18 Mar 2022 19:00:10 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 18 Mar 2022 19:00:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 18 Mar 2022 19:00:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 18 Mar 2022 19:00:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 18 Mar 2022 19:00:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 18 Mar 2022 19:00:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 18 Mar 2022 19:56:09 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 18 Mar 2022 19:56:10 GMT
ENV PHP_VERSION=7.4.28
# Fri, 18 Mar 2022 19:56:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Fri, 18 Mar 2022 19:56:12 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Fri, 18 Mar 2022 19:57:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 18 Mar 2022 19:57:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 20:04:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 20:04:18 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 18 Mar 2022 20:04:18 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 20:04:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 20:04:20 GMT
WORKDIR /var/www/html
# Fri, 18 Mar 2022 20:04:21 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 18 Mar 2022 20:04:22 GMT
STOPSIGNAL SIGQUIT
# Fri, 18 Mar 2022 20:04:23 GMT
EXPOSE 9000
# Fri, 18 Mar 2022 20:04:24 GMT
CMD ["php-fpm"]
# Sat, 19 Mar 2022 18:16:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 19 Mar 2022 18:16:57 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 19 Mar 2022 18:21:29 GMT
ENV DRUPAL_VERSION=7.89
# Sat, 19 Mar 2022 18:21:30 GMT
ENV DRUPAL_MD5=924e707e3b1e8269fe623cf2f22ee710
# Sat, 19 Mar 2022 18:21:32 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6e5521b433fb2737ba096075898c6ba7ae571ce725b0ceaaa56cf3faaea86a`  
		Last Modified: Fri, 18 Mar 2022 20:34:59 GMT  
		Size: 1.7 MB (1699756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcea977862fa31e7c9b4e96bec6528546dbb47ea3237afd6f7692bd2dda18b1`  
		Last Modified: Fri, 18 Mar 2022 20:34:58 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c532b63c5b01bff75aa1b71087bb537095cc31f1f8d360f836ad178e03b6dcc`  
		Last Modified: Fri, 18 Mar 2022 20:34:58 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99e617b2775fead059a53b5b24641eb8e637d5662f6cb3854c72b7cbc18eb289`  
		Last Modified: Fri, 18 Mar 2022 20:40:54 GMT  
		Size: 10.4 MB (10438019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0fd096fe9894a8117ec35fc9389cf6824736e4466b8c89ac0af71309a76b0f`  
		Last Modified: Fri, 18 Mar 2022 20:40:52 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db524ef1c90cbb49f162279617770b803c58566155a4f1c3f4f363e4942f47b`  
		Last Modified: Fri, 18 Mar 2022 20:41:21 GMT  
		Size: 11.3 MB (11263418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1936245b1dcb94cf9131817548072913c7c099038ab1cf30a6f05d71cdb916ca`  
		Last Modified: Fri, 18 Mar 2022 20:41:19 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78365e03b3e92945185d559e4d4e818c4426dc2966f7d1ade5661b8175c5e1b`  
		Last Modified: Fri, 18 Mar 2022 20:41:19 GMT  
		Size: 18.3 KB (18262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45d96454c25e72478bdf9a2ce345039c23986d9bdc6e571fb93872367a4f7fa4`  
		Last Modified: Fri, 18 Mar 2022 20:41:19 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287d7afe100bd6956341e2f98530a1d1e40564c0f5c38c358227a23ce91d53bd`  
		Last Modified: Sat, 19 Mar 2022 18:37:48 GMT  
		Size: 2.1 MB (2128645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3646a176260b79bd7430b4d21d4552dab8ae7cf2c34b928fa7dbe64b1c3cbb0a`  
		Last Modified: Sat, 19 Mar 2022 18:37:48 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ec7d206151617eb4ea3d20bcf7c8494cfa9bd3f9c4a6dfec958af04d8a11e90`  
		Last Modified: Sat, 19 Mar 2022 18:42:35 GMT  
		Size: 3.4 MB (3383072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-fpm-alpine3.14` - linux; 386

```console
$ docker pull drupal@sha256:7753a713e2d572d163d99c1751159845d9595816f2bc70dbe7317aa44fce8d48
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32502062 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8380885380d4ef619e396a4301619baaeeb5ab4b9c91b7dc72f91e1046723570`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 29 Mar 2022 00:38:40 GMT
ADD file:b779b35f4afe33387545e54afc23f09a30d43ad4817cc92ed6b083099748b3cb in / 
# Tue, 29 Mar 2022 00:38:40 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 01:48:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 29 Mar 2022 01:48:19 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 29 Mar 2022 01:48:20 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 29 Mar 2022 01:48:21 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 01:48:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 01:48:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:48:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 01:48:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 03:02:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 29 Mar 2022 03:02:42 GMT
ENV PHP_VERSION=7.4.28
# Tue, 29 Mar 2022 03:02:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 29 Mar 2022 03:02:44 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 29 Mar 2022 03:02:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 29 Mar 2022 03:02:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 03:09:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 03:09:08 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 03:09:08 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 03:09:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 03:09:10 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 03:09:11 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 03:09:12 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 03:09:13 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 03:09:14 GMT
CMD ["php-fpm"]
# Tue, 29 Mar 2022 19:09:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 29 Mar 2022 19:09:17 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 29 Mar 2022 19:15:00 GMT
ENV DRUPAL_VERSION=7.89
# Tue, 29 Mar 2022 19:15:00 GMT
ENV DRUPAL_MD5=924e707e3b1e8269fe623cf2f22ee710
# Tue, 29 Mar 2022 19:15:02 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:ff47816780f28cb5e3d0a86624e638d039b84373892ba3065b1ff9cd4b55b356`  
		Last Modified: Tue, 29 Mar 2022 00:39:52 GMT  
		Size: 2.8 MB (2821065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57e3be10bbaa0d66ca1d31b841c1c444d4764c41835940b522fe328a5ca0fb88`  
		Last Modified: Tue, 29 Mar 2022 03:26:08 GMT  
		Size: 1.8 MB (1801190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce738e996ee853ebe19228c531e54e53913050cea97099fac35e8ede66d8779`  
		Last Modified: Tue, 29 Mar 2022 03:26:07 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7995c153e871b3e4a84c91146df55caa764dc866ac3190ea3658aba7a96cfb1f`  
		Last Modified: Tue, 29 Mar 2022 03:26:07 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad14d9ef5a70229a099180eb7b50917945fd719ce2ea8ea8f65842b026ca7698`  
		Last Modified: Tue, 29 Mar 2022 03:36:49 GMT  
		Size: 10.4 MB (10437988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:397fb61f6ef461ba91649d7eaa6506806595d4e3e23e7fa0ad55cc9215809633`  
		Last Modified: Tue, 29 Mar 2022 03:36:47 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d257a0d99f2a68543d749d32cd99e9d6451f819beddb045fcbe7c665d81b9a66`  
		Last Modified: Tue, 29 Mar 2022 03:37:18 GMT  
		Size: 11.7 MB (11721073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1decf36a798818b2da24aed89db67584f5b385645c2afccf64a5030bd9c6fc04`  
		Last Modified: Tue, 29 Mar 2022 03:37:15 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65425319a3161dd068927eac0cbff93f9cfb848fc574ac2021d71536b35b8e4`  
		Last Modified: Tue, 29 Mar 2022 03:37:16 GMT  
		Size: 18.2 KB (18231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6f48191797a1826c6dd259bb31c7d183c894eb9060649f06fb7f97741b47bd5`  
		Last Modified: Tue, 29 Mar 2022 03:37:15 GMT  
		Size: 8.4 KB (8440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3274cd0334fbadffe821897f3552a384da375aba405a4607783b5ce101cafa27`  
		Last Modified: Tue, 29 Mar 2022 19:34:49 GMT  
		Size: 2.3 MB (2306289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b8ad418ad404e00162581af38a65acff4e4459191ad297f0889bcb3ba56056e`  
		Last Modified: Tue, 29 Mar 2022 19:34:48 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8410e82d0647eed9a029debc13b1841aae8596848b4ea2079ce85ed5cd1ed41d`  
		Last Modified: Tue, 29 Mar 2022 19:43:43 GMT  
		Size: 3.4 MB (3383063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-fpm-alpine3.14` - linux; ppc64le

```console
$ docker pull drupal@sha256:e4b77a1fbdaaffdf16694f4671a00dc92a6ffb8ad159ead35240ed448bf9be72
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32865371 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61c55c8fe10657207ab6c249f5a56269858a8831a7ad266c55385a5cadae662a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 18:18:43 GMT
ADD file:bf9c99d8209e0bed9fd3b62cbe691ebf3829d5a35e63e2b066f1f842577a6d24 in / 
# Thu, 17 Mar 2022 18:18:48 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 14:14:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 18 Mar 2022 14:14:44 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 18 Mar 2022 14:15:00 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 18 Mar 2022 14:15:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 18 Mar 2022 14:15:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 18 Mar 2022 14:15:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 18 Mar 2022 14:15:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 18 Mar 2022 14:15:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 18 Mar 2022 17:11:43 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 18 Mar 2022 17:11:46 GMT
ENV PHP_VERSION=7.4.28
# Fri, 18 Mar 2022 17:11:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Fri, 18 Mar 2022 17:11:57 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Fri, 18 Mar 2022 17:13:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 18 Mar 2022 17:13:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 17:23:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 17:23:12 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 18 Mar 2022 17:23:19 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 17:23:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 17:23:22 GMT
WORKDIR /var/www/html
# Fri, 18 Mar 2022 17:23:28 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 18 Mar 2022 17:23:29 GMT
STOPSIGNAL SIGQUIT
# Fri, 18 Mar 2022 17:23:31 GMT
EXPOSE 9000
# Fri, 18 Mar 2022 17:23:36 GMT
CMD ["php-fpm"]
# Sat, 19 Mar 2022 22:22:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 19 Mar 2022 22:22:10 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 19 Mar 2022 22:36:52 GMT
ENV DRUPAL_VERSION=7.89
# Sat, 19 Mar 2022 22:36:54 GMT
ENV DRUPAL_MD5=924e707e3b1e8269fe623cf2f22ee710
# Sat, 19 Mar 2022 22:37:03 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:8b7e8363a93630a772b70e3cf72231f43c62addae0ee8e507c61d43e3781c4e7`  
		Last Modified: Thu, 17 Mar 2022 18:20:01 GMT  
		Size: 2.8 MB (2817281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877f7777743bc7bd2add2262b34b2f3281189e86a3df534cb64bb3037e637867`  
		Last Modified: Fri, 18 Mar 2022 19:14:06 GMT  
		Size: 1.7 MB (1748164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc00a43798730ff329f01ed8bb2408b6f2a06a4edb64422ea3015b829fd808a7`  
		Last Modified: Fri, 18 Mar 2022 19:14:02 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd7d9bfc0391f0e95e77a59e7cc3e5ece1f7b8c892193e85cf5be005bbb4c45d`  
		Last Modified: Fri, 18 Mar 2022 19:14:02 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0185ba70e32560e45054254652a9fa00497c02a52678824a6f19b415e17cacc2`  
		Last Modified: Fri, 18 Mar 2022 19:27:58 GMT  
		Size: 10.4 MB (10438259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28addc0c1a9d14ccbe45fdbe4c40fb365b18dd533f6bbf0d84f6b496dc90b186`  
		Last Modified: Fri, 18 Mar 2022 19:27:57 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d839a3d81810573ddab86f4ac67c661f3364ffd64811d2a56895800179f7e059`  
		Last Modified: Fri, 18 Mar 2022 19:28:29 GMT  
		Size: 12.1 MB (12149968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f44717c4a90f4cd37d4a51bde91e8a0b2565feabdadf1c8cc8de22c34d801b87`  
		Last Modified: Fri, 18 Mar 2022 19:28:26 GMT  
		Size: 2.3 KB (2300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ad5144492314e8b360bfc5f458a6f6e0fd7179bb9962f431e4ccaa81f2d68f`  
		Last Modified: Fri, 18 Mar 2022 19:28:26 GMT  
		Size: 18.4 KB (18354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182ae76f5c683e7b06b18e7cb5c2b9f859d7bd4d9ac28b9470d887fe135d8b30`  
		Last Modified: Fri, 18 Mar 2022 19:28:26 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30add72759de8454b41baaefccbc31df5f58483402e3b368f03319311b76309d`  
		Last Modified: Sat, 19 Mar 2022 23:19:41 GMT  
		Size: 2.3 MB (2296867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ea07108395194a923818d078eacea697c70eee5051176f3fd31c96ce834b23`  
		Last Modified: Sat, 19 Mar 2022 23:19:40 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fe6687bd167026151fa8325a8e6ef5a4fd52afb910a0a7c05c9b70d13da5a3`  
		Last Modified: Sat, 19 Mar 2022 23:45:20 GMT  
		Size: 3.4 MB (3383374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-fpm-alpine3.14` - linux; s390x

```console
$ docker pull drupal@sha256:3fa06cf670b09be232022f2e37caef3fd4766adc1a8ac522aedbbc2db7dfbf00
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.4 MB (31408788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f823399350ac9dcf505d8c0d1561d3aa277bfb2f5d9aa8cc22571e3e12b3f11`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 29 Mar 2022 00:41:39 GMT
ADD file:7966b18580a674f84c4ff21ab8cffb1be1abafba3a0b270522609851441872aa in / 
# Tue, 29 Mar 2022 00:41:39 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 02:56:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 29 Mar 2022 02:56:09 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 29 Mar 2022 02:56:11 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 29 Mar 2022 02:56:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 02:56:13 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 02:56:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:56:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:56:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 04:08:00 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 29 Mar 2022 04:08:00 GMT
ENV PHP_VERSION=7.4.28
# Tue, 29 Mar 2022 04:08:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 29 Mar 2022 04:08:01 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 29 Mar 2022 04:08:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 29 Mar 2022 04:08:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 04:14:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 04:14:03 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 04:14:04 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 04:14:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 04:14:05 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 04:14:05 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 04:14:05 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 04:14:05 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 04:14:05 GMT
CMD ["php-fpm"]
# Wed, 30 Mar 2022 05:32:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 30 Mar 2022 05:32:21 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 30 Mar 2022 05:39:13 GMT
ENV DRUPAL_VERSION=7.89
# Wed, 30 Mar 2022 05:39:13 GMT
ENV DRUPAL_MD5=924e707e3b1e8269fe623cf2f22ee710
# Wed, 30 Mar 2022 05:39:15 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:91b7491d90d64405ba8401c680bbab3f8f25b600b385adce6abaadf0a4070906`  
		Last Modified: Tue, 29 Mar 2022 00:45:50 GMT  
		Size: 2.6 MB (2604093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb473f0a7dd16b93bd08f172fb87f32864a942d1ff962b9bb398a8743e55cd24`  
		Last Modified: Tue, 29 Mar 2022 05:16:43 GMT  
		Size: 1.8 MB (1762662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd990a92a436d67ee80dad8c334ecdc329a82d925fa974276f59f6ca85ee6e33`  
		Last Modified: Tue, 29 Mar 2022 05:16:43 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3efc08efc3016f133dc98c0331027f4252f13d576c5482be19836b3e83eb089`  
		Last Modified: Tue, 29 Mar 2022 05:16:43 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d090ab5d5daac91945ce8ad25d27a762429bec8dbfadb6790377a622dca75acf`  
		Last Modified: Tue, 29 Mar 2022 08:18:23 GMT  
		Size: 10.4 MB (10438250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce7561d68ff5d20cef9e4d5051a1e6c90d3e1b25eaf6913363e673501757d71`  
		Last Modified: Tue, 29 Mar 2022 08:18:23 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7428a4f75613180877a1629952fb9631df0bcac110ae895042b0b276ecab9f85`  
		Last Modified: Tue, 29 Mar 2022 08:22:21 GMT  
		Size: 11.0 MB (11023407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab7020d3cf98c22571d9cb318599a3e95ee10716b569159073e096147e464fa8`  
		Last Modified: Tue, 29 Mar 2022 08:22:21 GMT  
		Size: 2.4 KB (2445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6a14c30db9139db555ed98aee20fbb6a8f09136754cd889db157b79000ac1d`  
		Last Modified: Tue, 29 Mar 2022 08:22:21 GMT  
		Size: 18.4 KB (18350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0fdaa48eaddce7f6788e7f1c7bfd048d9c92c5a7954fb5df0387437ce01f5e`  
		Last Modified: Tue, 29 Mar 2022 08:22:21 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48589ddcf9a2e5475d6a14f8786608e3f4349ae92ceec45056a7862d9517cad6`  
		Last Modified: Wed, 30 Mar 2022 05:53:29 GMT  
		Size: 2.2 MB (2165415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df0a77f51a3a84880405b4beb924ab9236f7e554d03e8cb21318158084f8860`  
		Last Modified: Wed, 30 Mar 2022 05:53:29 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f07093f533aaa63734fe40a9c3a2566ec20e9712fdeb48e902592bb00228af`  
		Last Modified: Wed, 30 Mar 2022 05:58:28 GMT  
		Size: 3.4 MB (3383374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
