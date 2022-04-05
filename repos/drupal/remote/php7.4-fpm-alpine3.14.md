## `drupal:php7.4-fpm-alpine3.14`

```console
$ docker pull drupal@sha256:9fb717a9c310b1ceaa4700ab5ac470a27272c5be76ab3b5c793fc637704ea36e
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

### `drupal:php7.4-fpm-alpine3.14` - linux; amd64

```console
$ docker pull drupal@sha256:13608b3a19ce991e820b04eb488df022f0fc9a794d15d767fa7a5b34d70e83fb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50187840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c43390ed05a3445af1cea48c0c3181d8d87afc54dd826b3d1503c06fc7083f9d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 01:11:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 01:11:40 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 01:11:40 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 01:11:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 01:11:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 01:11:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 01:11:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 01:11:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 02:27:21 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 05 Apr 2022 02:27:21 GMT
ENV PHP_VERSION=7.4.28
# Tue, 05 Apr 2022 02:27:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 05 Apr 2022 02:27:21 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 05 Apr 2022 02:27:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 02:27:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 02:37:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 02:37:24 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 02:37:25 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 02:37:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 02:37:26 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 02:37:26 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 02:37:26 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 02:37:26 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 02:37:27 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 11:50:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 05 Apr 2022 11:50:03 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Apr 2022 11:50:03 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:50:03 GMT
ENV DRUPAL_VERSION=9.3.9
# Tue, 05 Apr 2022 11:50:03 GMT
WORKDIR /opt/drupal
# Tue, 05 Apr 2022 11:50:13 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 05 Apr 2022 11:50:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa03774f3e03c326f200279ce7ca2ddf335bd09a519355bf8a0dbf95e5491caa`  
		Last Modified: Tue, 05 Apr 2022 02:49:46 GMT  
		Size: 1.7 MB (1703109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaafb366c9f65869a27c1ae891cf1a8b9fb9be95a65f7d733b5bd38dcad8b9a`  
		Last Modified: Tue, 05 Apr 2022 02:49:46 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff7627ccdb679dac7fbcd955eed5f3c213f86c69ffd5ce9d0316d3af984a2bd0`  
		Last Modified: Tue, 05 Apr 2022 02:49:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8008abac843580c915f1aa61d547e435a3a7d7ba4d20f47a6e1103b0b326fe2f`  
		Last Modified: Tue, 05 Apr 2022 02:55:50 GMT  
		Size: 10.4 MB (10438247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3316d5083a304df95e449abe53629564274fdb60bb927e25da8dfbd647ddeaac`  
		Last Modified: Tue, 05 Apr 2022 02:55:49 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2560001ced5eeccc11153063701f02012662d224e3f20f6678f59ed599c4dc18`  
		Last Modified: Tue, 05 Apr 2022 02:56:14 GMT  
		Size: 11.4 MB (11428745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d013de183c503d6bd06315d93e4a76d9de26120d7b1daccb13fa8132b04ff7e2`  
		Last Modified: Tue, 05 Apr 2022 02:56:12 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4554f854a1084b1b09c38e06745508ee9e8777540575db8b562311384633a350`  
		Last Modified: Tue, 05 Apr 2022 02:56:13 GMT  
		Size: 18.3 KB (18332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2697b0aefff2ff7e533bcf06f0ea840a41ee532504993493f65660b71471bd`  
		Last Modified: Tue, 05 Apr 2022 02:56:12 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db332d9995996f80e9f8f79b34ff15ccda8c32df11803ed0d653f335fa150ac`  
		Last Modified: Tue, 05 Apr 2022 11:58:50 GMT  
		Size: 2.2 MB (2169892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:deb3203939143ab810ba48034dec2456498be80db4e95f6676b3ecbb103da4bb`  
		Last Modified: Tue, 05 Apr 2022 11:58:49 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79570be74731691ac2e5cd085f1817c42d16802df4d539692b7fe34102d2b039`  
		Last Modified: Tue, 05 Apr 2022 11:58:49 GMT  
		Size: 660.1 KB (660095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6335844155a1d676321d219958e3d5402447dff6e1164d3c7d608386cb6cca2`  
		Last Modified: Tue, 05 Apr 2022 11:58:49 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a85d1884eb91fe5474a0dac90ea578621b4fba933f8bab611f2a9f2b5f4cd6e`  
		Last Modified: Tue, 05 Apr 2022 11:58:54 GMT  
		Size: 20.9 MB (20937661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.14` - linux; arm variant v6

```console
$ docker pull drupal@sha256:186ee82f53682db294115a7fbb20f7ac65ae55825ebe9b5c25a615a99edf43d5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49067526 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bc69f006d355dc4b0121a4a57576075d1631b1e8f803d58ff8964faf170e1a1`
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
# Mon, 04 Apr 2022 21:14:01 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Mon, 04 Apr 2022 21:14:01 GMT
ENV DRUPAL_VERSION=9.3.9
# Mon, 04 Apr 2022 21:14:02 GMT
WORKDIR /opt/drupal
# Mon, 04 Apr 2022 21:14:32 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 04 Apr 2022 21:14:34 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
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
	-	`sha256:101154b2b4243f44aed846bcc840279fef7347ad12e66069d10a016cba64fbf7`  
		Last Modified: Mon, 04 Apr 2022 21:29:18 GMT  
		Size: 660.1 KB (660098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb40aa3188659c12e04960368c0b1432b52476a06a5ae5c353f5399b4435562`  
		Last Modified: Mon, 04 Apr 2022 21:29:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6d834409ec3bcee471594493c4b609dd4bc3e767d70e0e265e395168ff0a65`  
		Last Modified: Mon, 04 Apr 2022 21:29:47 GMT  
		Size: 20.9 MB (20937726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.14` - linux; arm variant v7

```console
$ docker pull drupal@sha256:e81f5351a2c4bd137dc9ecea805da01e896629634883898b76f9a30fe82cba09
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.9 MB (47929040 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7adf38db5720a7a31eeaf237024588864935640fe5a4b6555fb468769a2ee3a4`
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
# Mon, 04 Apr 2022 21:42:26 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Mon, 04 Apr 2022 21:42:26 GMT
ENV DRUPAL_VERSION=9.3.9
# Mon, 04 Apr 2022 21:42:27 GMT
WORKDIR /opt/drupal
# Mon, 04 Apr 2022 21:42:55 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 04 Apr 2022 21:42:58 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
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
	-	`sha256:0f09cc47bb9d14e52b34de942caddea963f96de57eca251e54c644c3b089b2f8`  
		Last Modified: Mon, 04 Apr 2022 23:37:40 GMT  
		Size: 660.1 KB (660098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0f9e463deecfc848d5dee751cf0215b7e91009dfce9cd4b1510c321361abd1`  
		Last Modified: Mon, 04 Apr 2022 23:37:39 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3794dd0781627cdec4da4d93cdbce79e0c457c2b100c6263b6c40a574c96cfdb`  
		Last Modified: Mon, 04 Apr 2022 23:38:09 GMT  
		Size: 20.9 MB (20937767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.14` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:7699b51cb5acec54e5bd844394be57ab404b10e7900d7ddce67cdd0b141dc9b4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49877059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f5aeabc6eebbb0097446b6cfcac31ef616b7aff457d7bf28d3c91cb2a198681`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 29 Mar 2022 00:40:12 GMT
ADD file:d0894581cf2fb7d7911ecb25bf0368675197db96d762977964ffc3a7ae8c774c in / 
# Tue, 29 Mar 2022 00:40:13 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 02:55:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 29 Mar 2022 02:55:19 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 29 Mar 2022 02:55:19 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 29 Mar 2022 02:55:20 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 02:55:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 02:55:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:55:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:55:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 05:02:21 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 29 Mar 2022 05:02:22 GMT
ENV PHP_VERSION=7.4.28
# Tue, 29 Mar 2022 05:02:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 29 Mar 2022 05:02:24 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 29 Mar 2022 05:02:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 29 Mar 2022 05:02:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 05:15:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 05:15:28 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 05:15:29 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 05:15:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 05:15:31 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 05:15:32 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 05:15:33 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 05:15:34 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 05:15:35 GMT
CMD ["php-fpm"]
# Wed, 30 Mar 2022 15:31:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 30 Mar 2022 15:31:42 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 04 Apr 2022 21:26:36 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Mon, 04 Apr 2022 21:26:36 GMT
ENV DRUPAL_VERSION=9.3.9
# Mon, 04 Apr 2022 21:26:37 GMT
WORKDIR /opt/drupal
# Mon, 04 Apr 2022 21:26:49 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 04 Apr 2022 21:26:51 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:810d54c7e01bab9975c1fb485c543715b76de7708166132520dfec0fc32c3754`  
		Last Modified: Tue, 29 Mar 2022 00:41:26 GMT  
		Size: 2.7 MB (2717494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d23547051480ea2370b812b539a9689be31bd4f8da8c77cb7dae8567c362e2a`  
		Last Modified: Tue, 29 Mar 2022 05:35:38 GMT  
		Size: 1.7 MB (1699722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94519d769f58083ef844d873bb3dad0e202820cd05de9326b4d6f0e555af95d6`  
		Last Modified: Tue, 29 Mar 2022 05:35:36 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d175b6b77a31ce89a09c5ac0f84caca9af0c8f17c6ee598cf3d506a6f2af6a11`  
		Last Modified: Tue, 29 Mar 2022 05:35:36 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0fc38533b23734855396a20e0073279519d716d31b5f8d54443900e277a62b`  
		Last Modified: Tue, 29 Mar 2022 07:26:11 GMT  
		Size: 10.4 MB (10438010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dfe5bc84b2dd938be75925e9206d2f69477d1f84214ebba60717f3cf2d46e35`  
		Last Modified: Tue, 29 Mar 2022 07:26:10 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b7593a16301fdaaa1e66c436eb6a5e8d2b102d5a1b12b4e56307b4d52daefb`  
		Last Modified: Tue, 29 Mar 2022 07:26:39 GMT  
		Size: 11.3 MB (11263370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c541310f398898a130b7f5c77ccf6a5690f7b4c77d1f70d21599cd75e5a2fe`  
		Last Modified: Tue, 29 Mar 2022 07:26:37 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51ec70360516438b4ccb65d5e9b0da4f60fade0dc62441db7113f6760633bf1`  
		Last Modified: Tue, 29 Mar 2022 07:26:37 GMT  
		Size: 18.3 KB (18259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b4655b341261b1682e47171106de5f5bc7db0523bedc8ddc86dadbe2dc7d41f`  
		Last Modified: Tue, 29 Mar 2022 07:26:37 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06abbea85619e619d430bd05eac47b7f2fade51251afb29e2812db97c3ce9e19`  
		Last Modified: Wed, 30 Mar 2022 15:58:02 GMT  
		Size: 2.1 MB (2128584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a59bab8edc6fb908c7da8f599a5a05152ae26b48b5126708a9e80872a519b8f`  
		Last Modified: Wed, 30 Mar 2022 15:58:02 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cc6fb5c1d8d80b0d8ecbd7a8bab9fbf94f9e458d46875ee013aaa48b971c9bb`  
		Last Modified: Mon, 04 Apr 2022 22:21:57 GMT  
		Size: 660.1 KB (660101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50b3a2b362b633c2bdfd0f8460c57e94b46ab7f654f948e100b4a0c231c8d4f9`  
		Last Modified: Mon, 04 Apr 2022 22:21:57 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e97cf1e8911abcbee51027772fd3634efca68dc5cfb4c839b2c747663c7737ee`  
		Last Modified: Mon, 04 Apr 2022 22:22:02 GMT  
		Size: 20.9 MB (20938238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.14` - linux; 386

```console
$ docker pull drupal@sha256:093111ec82c7cb780d1127fc48cb8896c6a3fc994b5f84e26cc372a47e38c8cd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50717708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c8f884a68ee0e4f8052eae354829bf668393c4446a66f87254d45a8285c9ae8`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:32 GMT
ADD file:6508514d43b69774a3307679ef8f6dba0faf707e62ad6c6c1c8cf40d84e12d1d in / 
# Mon, 04 Apr 2022 23:38:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 00:13:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 00:13:30 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 00:13:31 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 00:13:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 00:13:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 00:13:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:13:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:13:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 01:02:53 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 05 Apr 2022 01:02:54 GMT
ENV PHP_VERSION=7.4.28
# Tue, 05 Apr 2022 01:02:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 05 Apr 2022 01:02:56 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 05 Apr 2022 01:03:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 01:03:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 01:09:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 01:09:20 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 01:09:20 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 01:09:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 01:09:22 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 01:09:23 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 01:09:24 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 01:09:25 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 01:09:26 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 07:43:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 05 Apr 2022 07:43:20 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Apr 2022 07:43:22 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Tue, 05 Apr 2022 07:43:22 GMT
ENV DRUPAL_VERSION=9.3.9
# Tue, 05 Apr 2022 07:43:23 GMT
WORKDIR /opt/drupal
# Tue, 05 Apr 2022 07:43:35 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 05 Apr 2022 07:43:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:c11e5e1035714514f6e237dffd1836a4d03b48af64e55a8e08f9bd9e998e24a9`  
		Last Modified: Mon, 04 Apr 2022 23:39:35 GMT  
		Size: 2.8 MB (2821213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d252c7fc7fdf2acebba22bdce0df2a9b6699d3103f77cd3befcd96c9830dd44d`  
		Last Modified: Tue, 05 Apr 2022 01:25:00 GMT  
		Size: 1.8 MB (1801196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29da06ea807d8f1d3f704ed6147c9f34dbf3dd2c26817a9f8b1ee7643d57a281`  
		Last Modified: Tue, 05 Apr 2022 01:24:59 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7d9b1421b6c940a062a92e05e3ac5394ef9dc0292558b91f73f4d1ced04a14`  
		Last Modified: Tue, 05 Apr 2022 01:24:59 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfa4a62083895ec2b5dcd687af6f956730f36a43449497712bd48f7e0f8fb816`  
		Last Modified: Tue, 05 Apr 2022 01:33:05 GMT  
		Size: 10.4 MB (10437994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d070894d84f1ec537add88389db1c1e6d874aaeec0be0b656b3a44faec4e4e`  
		Last Modified: Tue, 05 Apr 2022 01:33:04 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c468437799ceeaf988314627c87df44d11915e1121785651434ff93ec8263a`  
		Last Modified: Tue, 05 Apr 2022 01:33:35 GMT  
		Size: 11.7 MB (11721163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12e4439ca16d9a648338921bbff4b78ac68d4ac47fbb451ae4932fd0ec79c490`  
		Last Modified: Tue, 05 Apr 2022 01:33:32 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8665ef9bf541291dca6e649a8afdf145de6902d594fd2ba1cf5ab001e41694fb`  
		Last Modified: Tue, 05 Apr 2022 01:33:32 GMT  
		Size: 18.2 KB (18235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9731ee786fcda67d23d1e2ab35e755d38ce5fa25935958676a7ed74dd968dc1`  
		Last Modified: Tue, 05 Apr 2022 01:33:32 GMT  
		Size: 8.4 KB (8439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fb1e78860ed131f6f459b31053806752dd083ec4fb906702fa1257c7d19d75e`  
		Last Modified: Tue, 05 Apr 2022 07:58:47 GMT  
		Size: 2.3 MB (2306285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3794c63b57dc8907ae99eb5178423b7f1b41fb57b2e6e864246c3c59af55fd1b`  
		Last Modified: Tue, 05 Apr 2022 07:58:47 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb5d9e8f12836feed668e3bc93c0e897992c98796af6da98f83cc6e9d88590bd`  
		Last Modified: Tue, 05 Apr 2022 07:58:47 GMT  
		Size: 660.1 KB (660096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b42cc576598f17440d0ee10cc237f7d1f57792864fdba4b30853530e34f48a4`  
		Last Modified: Tue, 05 Apr 2022 07:58:47 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed461f2b65127b193aceb1ef0959a23b0a26c224e438cb05e541a7abcf4175ff`  
		Last Modified: Tue, 05 Apr 2022 07:58:52 GMT  
		Size: 20.9 MB (20938249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.14` - linux; ppc64le

```console
$ docker pull drupal@sha256:93bbe7288543c8deab242a72fb32ebe2115098264141c9200c3aa3c2519f8961
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51076983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eabbdc4a21b7831cd7d0f907dd355769fbf4d35330f4df2377bcf611dc82c7c2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 29 Mar 2022 00:17:09 GMT
ADD file:b8083e0e4f4eed014eb6c7e881671b4c58af2bb5d05d9e60d0e1d217fab852a1 in / 
# Tue, 29 Mar 2022 00:17:12 GMT
CMD ["/bin/sh"]
# Tue, 29 Mar 2022 02:24:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 29 Mar 2022 02:24:22 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 29 Mar 2022 02:24:34 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 29 Mar 2022 02:24:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 29 Mar 2022 02:24:45 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 29 Mar 2022 02:24:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:24:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 29 Mar 2022 02:24:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 29 Mar 2022 04:39:22 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 29 Mar 2022 04:39:23 GMT
ENV PHP_VERSION=7.4.28
# Tue, 29 Mar 2022 04:39:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 29 Mar 2022 04:39:28 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 29 Mar 2022 04:39:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 29 Mar 2022 04:39:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 29 Mar 2022 04:50:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 29 Mar 2022 04:50:15 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 29 Mar 2022 04:50:25 GMT
RUN docker-php-ext-enable sodium
# Tue, 29 Mar 2022 04:50:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 29 Mar 2022 04:50:31 GMT
WORKDIR /var/www/html
# Tue, 29 Mar 2022 04:50:39 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 29 Mar 2022 04:50:40 GMT
STOPSIGNAL SIGQUIT
# Tue, 29 Mar 2022 04:50:42 GMT
EXPOSE 9000
# Tue, 29 Mar 2022 04:50:44 GMT
CMD ["php-fpm"]
# Wed, 30 Mar 2022 18:57:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 30 Mar 2022 18:58:02 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 04 Apr 2022 22:21:06 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Mon, 04 Apr 2022 22:21:09 GMT
ENV DRUPAL_VERSION=9.3.9
# Mon, 04 Apr 2022 22:21:11 GMT
WORKDIR /opt/drupal
# Mon, 04 Apr 2022 22:21:42 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 04 Apr 2022 22:21:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:9b3885e1b82e42fc12e5a6c0b16a783379e4f96c6287d6b56d2aa2120d68c486`  
		Last Modified: Tue, 29 Mar 2022 00:18:44 GMT  
		Size: 2.8 MB (2814183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac47bb21f777673b7d46d5ae2af561e7ee41f8e704fac1c95c7092705ff71575`  
		Last Modified: Tue, 29 Mar 2022 05:12:48 GMT  
		Size: 1.7 MB (1748184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:763b14c5a184a7da21176d18945d140cb7780e4172dbd04171773c21aec7c462`  
		Last Modified: Tue, 29 Mar 2022 05:12:47 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f61e5e97d5a4e8eaa92a458a712cf3deb2c7c2316ef376cd1ee5a8c113cf6cf8`  
		Last Modified: Tue, 29 Mar 2022 05:12:47 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a3ed5c4d59eab7ab2d7224c84e1d9fc9e396fce8ffc79ae2f4f4c38df7045a`  
		Last Modified: Tue, 29 Mar 2022 05:25:34 GMT  
		Size: 10.4 MB (10438249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57650d55b98ff4a2d2cf8f9f61a96e091f38d52e7f019fb6d412c9a7af65ad6a`  
		Last Modified: Tue, 29 Mar 2022 05:25:32 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5977005cce91d3f61ed8c4a82971355e50d5273676049e93b3df5da264192c68`  
		Last Modified: Tue, 29 Mar 2022 05:26:05 GMT  
		Size: 12.1 MB (12149930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4f415b8c3123c38914570692458c8a9d44a7d3dd75f2af555393705d9c125c8`  
		Last Modified: Tue, 29 Mar 2022 05:26:03 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46d9752a3a0b48e993acc6a5be61879f298e585c0a7a9b9708817976426952e6`  
		Last Modified: Tue, 29 Mar 2022 05:26:03 GMT  
		Size: 18.3 KB (18348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10a6743c139bd9df4c62a9b77e4686f796a67f8dc12ae0c639b4cab43d26a677`  
		Last Modified: Tue, 29 Mar 2022 05:26:03 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcf7db0f66900fdd3b447099f270b4c5a222e2f662859f7293310f4d921b648e`  
		Last Modified: Wed, 30 Mar 2022 20:29:43 GMT  
		Size: 2.3 MB (2296865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b18aa31107ecaac404569b68c86576d260477e0c10543ae3193fabe3798d680`  
		Last Modified: Wed, 30 Mar 2022 20:29:41 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab393b33c7c47361f6afd8f233c106f589de64c794bbc4308a0ba667b9608f3a`  
		Last Modified: Mon, 04 Apr 2022 23:22:50 GMT  
		Size: 660.1 KB (660100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4044bcadb1e225ac567ff06ad0020da573cf79391bcc54d69d954da0a04720a`  
		Last Modified: Mon, 04 Apr 2022 23:22:50 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10130bad70f6d4e856b4b26e4462e7c21d26a73da077384d937ce0267c80280e`  
		Last Modified: Mon, 04 Apr 2022 23:24:18 GMT  
		Size: 20.9 MB (20937715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:php7.4-fpm-alpine3.14` - linux; s390x

```console
$ docker pull drupal@sha256:8ec3d66b21d38246a0c089f91f5cca8ccac33b7562067ad63def6f406047d6ec
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49623446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:378dff21f450fa198785c5a9db48906c661ea586e7665900ab5c2b620edc7d37`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:47 GMT
ADD file:0f70e0f0075bee67acb44e5ef01bf6b9df1f69a25b7aa6fd15bd5bb6ec5bcc9f in / 
# Mon, 04 Apr 2022 23:41:48 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 00:08:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 00:08:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 00:08:56 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 00:08:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 00:08:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 00:08:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:08:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:08:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 00:50:59 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 05 Apr 2022 00:51:00 GMT
ENV PHP_VERSION=7.4.28
# Tue, 05 Apr 2022 00:51:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.28.tar.xz.asc
# Tue, 05 Apr 2022 00:51:00 GMT
ENV PHP_SHA256=9cc3b6f6217b60582f78566b3814532c4b71d517876c25013ae51811e65d8fce
# Tue, 05 Apr 2022 00:51:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 00:51:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:56:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 00:56:29 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:56:30 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 00:56:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 00:56:30 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 00:56:30 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 00:56:31 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 00:56:31 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 00:56:31 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 11:53:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 05 Apr 2022 11:53:55 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Apr 2022 11:53:55 GMT
COPY file:9cbc8d461e82cf7c5c8b03ecbb4c9d034d879299c6d43185c2fe17145ed826be in /usr/local/bin/ 
# Tue, 05 Apr 2022 11:53:55 GMT
ENV DRUPAL_VERSION=9.3.9
# Tue, 05 Apr 2022 11:53:56 GMT
WORKDIR /opt/drupal
# Tue, 05 Apr 2022 11:54:11 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 05 Apr 2022 11:54:17 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:6f6a6c77b1bd5dfb3e759efaa292f964f197ae4b96be74d80ef059f87317997a`  
		Last Modified: Mon, 04 Apr 2022 23:42:47 GMT  
		Size: 2.6 MB (2604075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2af9291e8bb0cd2e6ac744794ab2287652d0f0e3b0a1e03feba1ccf6cdc9ef0`  
		Last Modified: Tue, 05 Apr 2022 01:10:11 GMT  
		Size: 1.8 MB (1762717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a6e28b72f7a6dc4fe85e004996700ffc40c5583e3c5b6dc6561c829ac179b2`  
		Last Modified: Tue, 05 Apr 2022 01:10:10 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74a6f63d4dae3713973596b3706bfaa082a0232b19dfb450921a282b03776550`  
		Last Modified: Tue, 05 Apr 2022 01:10:11 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dee25b930e63103db04f466b8d9b84525b8295da1aa973f45f4aea149ebd848`  
		Last Modified: Tue, 05 Apr 2022 02:56:07 GMT  
		Size: 10.4 MB (10438252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba931f97c4ce8631ab507c8e60d90c091657e659fd4b7c3eec5df9db2e296fad`  
		Last Modified: Tue, 05 Apr 2022 02:56:07 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625e77efcc89bb2bb96fca00a52a6f5eff6169261dd6601451e3fd0a85a77000`  
		Last Modified: Tue, 05 Apr 2022 02:56:25 GMT  
		Size: 11.0 MB (11023369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a3b04ba93ff0b26bc6eff1804ad1c279f5028befb7be49b6f174b28a3a5def1`  
		Last Modified: Tue, 05 Apr 2022 02:56:23 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b37fc23d5586a5aa431c2889df4562b216efb2f822ebf3eae21c7db4020f1c1`  
		Last Modified: Tue, 05 Apr 2022 02:56:23 GMT  
		Size: 18.4 KB (18370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df3fcfd586c7df0e66eecc50f3ae27ee9a87859d9b9ca61e06558665e368693`  
		Last Modified: Tue, 05 Apr 2022 02:56:23 GMT  
		Size: 8.4 KB (8441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e909699b400ed90a9b0f4de2ba63c65057e6e7ea8d19275d34e0783626d1db`  
		Last Modified: Tue, 05 Apr 2022 12:09:40 GMT  
		Size: 2.2 MB (2165404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5482f168a8ba36895705017c602f12c5b50fae179ff5bf9bf9d15c9d6f0e7760`  
		Last Modified: Tue, 05 Apr 2022 12:09:40 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876f83422c1eb6d1c10340493438c950c18265570095b20bdbb5db395a984589`  
		Last Modified: Tue, 05 Apr 2022 12:09:40 GMT  
		Size: 660.1 KB (660099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de656b3416a226c7a819c41041a8cd3715d66c48b5756b819baaf2ff11c93f1e`  
		Last Modified: Tue, 05 Apr 2022 12:09:40 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f35726e764c15303467ef3bdb7f417925ab0d0f322b6b6cbe3b1323bf03023`  
		Last Modified: Tue, 05 Apr 2022 12:09:44 GMT  
		Size: 20.9 MB (20937771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
