## `yourls:fpm-alpine`

```console
$ docker pull yourls@sha256:363f238f76b3022ea77a905ac8245b6265ec07cae015e338c924645e9397f8ff
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

### `yourls:fpm-alpine` - linux; amd64

```console
$ docker pull yourls@sha256:07f1cf6cf62936153b3c2586c50d3e6e8df2e3c88f452e372a4e74e6003fd8c0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34210120 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d9d4dd9d57ff31b575a57ed955d83b2419e1adbfbd021c6b0208d975d25cb6cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 15:23:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 15:23:12 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 15:23:13 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 15:23:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 15:23:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 15:29:08 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 15:29:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 15:29:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 15:29:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 15:29:08 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Apr 2021 15:29:09 GMT
ENV PHP_VERSION=8.0.3
# Thu, 01 Apr 2021 15:29:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 01 Apr 2021 15:29:09 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 01 Apr 2021 15:29:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 15:29:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 15:35:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 15:35:00 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 15:35:02 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 15:35:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 15:35:02 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 15:35:03 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 15:35:03 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 15:35:04 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 15:35:04 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 20:24:43 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 01 Apr 2021 20:24:44 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 20:24:45 GMT
RUN apk add --no-cache bash
# Thu, 01 Apr 2021 20:24:45 GMT
ENV YOURLS_VERSION=1.8.1
# Thu, 01 Apr 2021 20:24:45 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Thu, 01 Apr 2021 20:24:47 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 01 Apr 2021 20:24:48 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Thu, 01 Apr 2021 20:24:48 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Thu, 01 Apr 2021 20:24:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 20:24:48 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047b7ad6600bd2809fe552fabb09e2ed32a5f37e0308062b241603f33d64d070`  
		Last Modified: Thu, 01 Apr 2021 16:52:20 GMT  
		Size: 1.7 MB (1694860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590887918baf4908a9d380f8ea1b4ee9595564e8b69cc89d7545e3b6677ee933`  
		Last Modified: Thu, 01 Apr 2021 16:52:20 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63facc7722cc65600a457d7a4f4790059217214d0437029357e996412b38124e`  
		Last Modified: Thu, 01 Apr 2021 16:52:20 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf608d30a80a36f77b56c2c8872d8fd55edaf02e77a31fee2f4e560c7d786dfd`  
		Last Modified: Thu, 01 Apr 2021 16:53:20 GMT  
		Size: 10.8 MB (10775188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aab0da525cba34e30481e0c0230bfa24c6d437df5a38a09bbe29f22e18ce220`  
		Last Modified: Thu, 01 Apr 2021 16:53:15 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d98d37a56a38202136639e112e00641fbce5e384179c87cc6ee462369bafc46`  
		Last Modified: Thu, 01 Apr 2021 16:53:19 GMT  
		Size: 15.0 MB (15021147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf22c3b28cf430c1de5dcdb6b7cd0fe70a8c650263ca08a4cca15393965db92`  
		Last Modified: Thu, 01 Apr 2021 16:53:15 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efd12cf38afa4fc2c4152c3e8c15ebd2464d60eba97ac77290b88718b70537d1`  
		Last Modified: Thu, 01 Apr 2021 16:53:15 GMT  
		Size: 17.5 KB (17511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29abce8c9efe34d9937b7729df46939a539b46995039b4934275e0f5a42affe`  
		Last Modified: Thu, 01 Apr 2021 16:53:15 GMT  
		Size: 8.6 KB (8569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5002865a83c8cea2fbd892753808e942919acf85de98132ef2dfad0df292f1b9`  
		Last Modified: Thu, 01 Apr 2021 20:25:21 GMT  
		Size: 710.3 KB (710272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7abf0b5097a01825d75e9ebf973bea1408cf6a7040d06012caeb556def51771`  
		Last Modified: Thu, 01 Apr 2021 20:25:19 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d8af42e121ae7a950286bdda93b2f2b80b92402d42bac848921a21f3870772`  
		Last Modified: Thu, 01 Apr 2021 20:25:21 GMT  
		Size: 590.6 KB (590640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:770ff56661f9a2d27f48527cc5f62698b5cbec70b15608043572854084a7d188`  
		Last Modified: Thu, 01 Apr 2021 20:25:19 GMT  
		Size: 2.6 MB (2572151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2c0d1fdda9a787c9d996a595f297df174d1cb7dfc2a960d0427cdafed835efb`  
		Last Modified: Thu, 01 Apr 2021 20:25:19 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:271969896c9a96c8cac540f94b9359b0ed8a6230520ab2684f95d63eed5268fa`  
		Last Modified: Thu, 01 Apr 2021 20:25:18 GMT  
		Size: 2.0 KB (2039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; arm variant v6

```console
$ docker pull yourls@sha256:0827b712abf642ef53ff45f93613d9e4499e7076f5e92a12fc589dc66f2ead47
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32271367 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b13f49063eb5c5459444abffff213783423c389e1afbf11f725a18a2a68a237c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:37:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 31 Mar 2021 22:37:10 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 31 Mar 2021 22:37:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 31 Mar 2021 22:37:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 31 Mar 2021 22:37:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 31 Mar 2021 22:43:03 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 31 Mar 2021 22:43:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 22:43:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 22:43:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 31 Mar 2021 22:43:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 31 Mar 2021 22:43:10 GMT
ENV PHP_VERSION=8.0.3
# Wed, 31 Mar 2021 22:43:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 31 Mar 2021 22:43:12 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 31 Mar 2021 22:43:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 31 Mar 2021 22:43:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 22:47:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 22:47:08 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 31 Mar 2021 22:47:12 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 22:47:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 22:47:14 GMT
WORKDIR /var/www/html
# Wed, 31 Mar 2021 22:47:17 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 31 Mar 2021 22:47:18 GMT
STOPSIGNAL SIGQUIT
# Wed, 31 Mar 2021 22:47:19 GMT
EXPOSE 9000
# Wed, 31 Mar 2021 22:47:19 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 05:55:27 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 01 Apr 2021 05:55:30 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 05:55:33 GMT
RUN apk add --no-cache bash
# Thu, 01 Apr 2021 05:55:34 GMT
ENV YOURLS_VERSION=1.8.1
# Thu, 01 Apr 2021 05:55:35 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Thu, 01 Apr 2021 05:55:39 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 01 Apr 2021 05:55:40 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Thu, 01 Apr 2021 05:55:41 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Thu, 01 Apr 2021 05:55:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 05:55:43 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6e43e67e5babad459f6f197992a26d77e745ef3b9a9ffac78e944ac250c167`  
		Last Modified: Thu, 01 Apr 2021 00:01:46 GMT  
		Size: 1.7 MB (1684700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a574a3d26078380134181643d6542608f6e510e2cce4119361f1df09b617dcb2`  
		Last Modified: Thu, 01 Apr 2021 00:01:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90716c38f3f1c30424f0b486ba18c8c8c630b62f6858c89513c20968dfb91bd`  
		Last Modified: Thu, 01 Apr 2021 00:01:43 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f10247c507a96af7229085b0eeb6928a8ff4998f4f53d63cb5d943c99e5695b`  
		Last Modified: Thu, 01 Apr 2021 00:02:47 GMT  
		Size: 10.8 MB (10775172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a01536081adff240608b9c7791d57b2679be8d5fafdb720ade244cd3c21868`  
		Last Modified: Thu, 01 Apr 2021 00:02:40 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4557b7ff52df19aef8099eccccecfda8cb6e23065f8839a056c23f809eedf87e`  
		Last Modified: Thu, 01 Apr 2021 00:02:50 GMT  
		Size: 13.7 MB (13653551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:038feb1f276a5f7eb6dc678f15136ef215da63c94afa990881d8818a48a9531c`  
		Last Modified: Thu, 01 Apr 2021 00:02:40 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af1959d4289ec8a607848f6e848509925ac74183fd6a00bfff30d169f84b0bc1`  
		Last Modified: Thu, 01 Apr 2021 00:02:40 GMT  
		Size: 17.5 KB (17504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e10cad8566869a49d934f5824e3f30d7c03d8735335156d3501b79db23b1e2`  
		Last Modified: Thu, 01 Apr 2021 00:02:41 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:582408ac2b213be597e5ebca0e209e865f5dadf81cb52984107f7286609dd861`  
		Last Modified: Thu, 01 Apr 2021 05:56:09 GMT  
		Size: 359.4 KB (359374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c88506fc7a22cc0bca5e318cf41e42d6ddd08611b18cb369941b1b4ed94b28`  
		Last Modified: Thu, 01 Apr 2021 05:56:07 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421ed9273d0247c8902da24aeb49cddc461adffa479c6844133ae9e51bcda265`  
		Last Modified: Thu, 01 Apr 2021 05:56:07 GMT  
		Size: 570.4 KB (570383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:debc4064fe984ac5176140253b3cd517880a278c25b4939a2cf89942c685a254`  
		Last Modified: Thu, 01 Apr 2021 05:56:08 GMT  
		Size: 2.6 MB (2572153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a25245f4bb02cafa43d4029cbe2e29050d3ceb196f80d7c89e09dd066f5a9f16`  
		Last Modified: Thu, 01 Apr 2021 05:56:07 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6340a8f87b58529d0cdf304dba7c77ce59080ddbb2cf7bf6d4b417186c4ffb56`  
		Last Modified: Thu, 01 Apr 2021 05:56:07 GMT  
		Size: 2.0 KB (2037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; arm variant v7

```console
$ docker pull yourls@sha256:bad1aed2c2021441d64ddbf9df76206476aafe7a67a1874156ac6b049f70faba
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31010534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:978204cd3e499c3f8111081a72164ea4659ea7a0e476e8d10831b132a6994034`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:27 GMT
ADD file:56e92c06393237a87e0a1ff475e9c9dc80e897d69ec20f45359b587906da345b in / 
# Wed, 31 Mar 2021 18:13:31 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 10:30:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 10:30:57 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 10:31:00 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 10:31:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 10:31:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 10:34:16 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 10:34:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 10:34:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 10:34:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 10:34:19 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Apr 2021 10:34:20 GMT
ENV PHP_VERSION=8.0.3
# Thu, 01 Apr 2021 10:34:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 01 Apr 2021 10:34:22 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 01 Apr 2021 10:34:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 10:34:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 10:37:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 10:37:24 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 10:37:31 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 10:37:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 10:37:34 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 10:37:41 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 10:37:43 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 10:37:44 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 10:37:45 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 16:28:33 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 01 Apr 2021 16:28:36 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 16:28:41 GMT
RUN apk add --no-cache bash
# Thu, 01 Apr 2021 16:28:42 GMT
ENV YOURLS_VERSION=1.8.1
# Thu, 01 Apr 2021 16:28:43 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Thu, 01 Apr 2021 16:28:48 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 01 Apr 2021 16:28:49 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Thu, 01 Apr 2021 16:28:51 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Thu, 01 Apr 2021 16:28:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 16:28:53 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:07389e51ea05e1c9a3cb0ef92d31181f2afa1e445207ad99ffd8a94d6d6af295`  
		Last Modified: Wed, 31 Mar 2021 18:14:57 GMT  
		Size: 2.4 MB (2424108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666e972adac2d89789c65311d5fa79b86ccca10bba7ba162a4867317aeda31d8`  
		Last Modified: Thu, 01 Apr 2021 11:28:25 GMT  
		Size: 1.6 MB (1555129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577388c2383035f4d1e21e88cd7e24171330947439ec55a7c61cc69d96757504`  
		Last Modified: Thu, 01 Apr 2021 11:28:25 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f9ffa02fa172c0624511859b54b0fed84d5c012c089a5291763728fc215d70`  
		Last Modified: Thu, 01 Apr 2021 11:28:25 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b2c8cb63fd2e4f4b640e172c7f8a3fd61ca472a90c5f4d368612e46a7bea221`  
		Last Modified: Thu, 01 Apr 2021 11:29:02 GMT  
		Size: 10.8 MB (10775171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07f30975ff91c0b82d3d0c1a239e223eb98793b7e0c7f2f462d82d998203dc30`  
		Last Modified: Thu, 01 Apr 2021 11:28:59 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e161555a2b66092acb12044267bb36fbbd8a21f5187f2f31019ddade63ac653f`  
		Last Modified: Thu, 01 Apr 2021 11:29:04 GMT  
		Size: 12.8 MB (12797646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2369cca14a0ebb6a14311b4edcb08291085eddf8e8e1db57919b6439143bd462`  
		Last Modified: Thu, 01 Apr 2021 11:28:59 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57160b88b461258c5f2f3e96d55cb746bcac2dbaa207511f82f8c93eda1553c6`  
		Last Modified: Thu, 01 Apr 2021 11:28:59 GMT  
		Size: 17.5 KB (17519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13172d271825ec8a16c4b066bf0d92c3bfcd6f830723d24e6aeee23b5b4046bd`  
		Last Modified: Thu, 01 Apr 2021 11:28:59 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bfb6e78ecc686ba3df9b6e559129d0866af985d9f485362c9b3e63debe6cdd0`  
		Last Modified: Thu, 01 Apr 2021 16:29:24 GMT  
		Size: 333.0 KB (332985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae13980ce6d68752c0fa85aa1d89bbe40dd386be1193cd03ad3c0d61d6106e9`  
		Last Modified: Thu, 01 Apr 2021 16:29:22 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4653ae1a39f98312544c7661835b8e8af462a1cab633c9b33189b02f1ab6172`  
		Last Modified: Thu, 01 Apr 2021 16:29:22 GMT  
		Size: 519.4 KB (519415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7134c3e81e91002ddf100731f9cda3bedff59adabb1551c7db091ab9d2635da7`  
		Last Modified: Thu, 01 Apr 2021 16:29:23 GMT  
		Size: 2.6 MB (2572150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd85d12ef45d518a1407c115eb2be9c044625df19e999f0e267f28e0304b918`  
		Last Modified: Thu, 01 Apr 2021 16:29:22 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a201ac2f382cda3eabf05ddef321503b1ed40ed61dc02a12431518333f673c2f`  
		Last Modified: Thu, 01 Apr 2021 16:29:22 GMT  
		Size: 2.0 KB (2039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:d600a368ce032c216b9bc0b1a5a7af0fd74f11d71d1ae10451a8a0ed5c048209
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.2 MB (33201605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd20cd126dec2c151aed93d35ee1ddc5b2e3608bff75393d6e279367a900b758`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 14:17:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 14:17:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 14:17:54 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 14:17:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 14:17:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 14:22:39 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 14:22:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 14:22:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 14:22:43 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 14:22:44 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Apr 2021 14:22:45 GMT
ENV PHP_VERSION=8.0.3
# Thu, 01 Apr 2021 14:22:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 01 Apr 2021 14:22:48 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 01 Apr 2021 14:22:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 14:22:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 14:26:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 14:26:58 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 14:27:03 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 14:27:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 14:27:06 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 14:27:08 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 14:27:09 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 14:27:11 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 14:27:12 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 20:35:18 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 01 Apr 2021 20:35:20 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 20:35:23 GMT
RUN apk add --no-cache bash
# Thu, 01 Apr 2021 20:35:24 GMT
ENV YOURLS_VERSION=1.8.1
# Thu, 01 Apr 2021 20:35:25 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Thu, 01 Apr 2021 20:35:28 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 01 Apr 2021 20:35:29 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Thu, 01 Apr 2021 20:35:30 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Thu, 01 Apr 2021 20:35:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 20:35:32 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68148511d312111e170da734bba39b160e6ca92976f410effb2b7122e2d2992d`  
		Last Modified: Thu, 01 Apr 2021 15:27:48 GMT  
		Size: 1.7 MB (1694540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2098b55e85688425b39195714604b23533ff01167635ec114a88bd28292c33c4`  
		Last Modified: Thu, 01 Apr 2021 15:27:48 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e694ac18ee7ae9ba3a85bd272d1feae8bfcf166d4ea6bea3de67d9199e7569a0`  
		Last Modified: Thu, 01 Apr 2021 15:27:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4f37ad14d57243ea05d832f51d48b17349bfa772aaf884e2cd94fbd76e4fe9`  
		Last Modified: Thu, 01 Apr 2021 15:28:26 GMT  
		Size: 10.8 MB (10775186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e70feb1e899aa45f6b82696695af648ff5eab6418dc799463989b8daa97a81e`  
		Last Modified: Thu, 01 Apr 2021 15:28:23 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46e195218d5ed27751c169607a830b9ccb2b2fbbc38f442068b5bef3a9499d29`  
		Last Modified: Thu, 01 Apr 2021 15:28:27 GMT  
		Size: 14.4 MB (14444669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9c406e09743186c68e3419e3285c7ba36b52bb9ee5ebd7117f3db04676807d`  
		Last Modified: Thu, 01 Apr 2021 15:28:23 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb385d6f9a5e1f2cd2c6f44023cf57b6e9f1c90f9e09661a013eec4079350fbb`  
		Last Modified: Thu, 01 Apr 2021 15:28:23 GMT  
		Size: 17.5 KB (17525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2517c868d7dd544abe862166b41d0f42b8996c81b9959f4435f8e79279d0020`  
		Last Modified: Thu, 01 Apr 2021 15:28:23 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2d5e43710a65300fb205bdfd24b715d7fa7d128ae2c1284774b4281e942ada`  
		Last Modified: Thu, 01 Apr 2021 20:36:00 GMT  
		Size: 368.9 KB (368903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3d1bcdc93a9f170db5dd3b096ae19cd4f07183976d385822697c797a54747d`  
		Last Modified: Thu, 01 Apr 2021 20:35:58 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793818d584528e913497f41fada5664b2de4559ccde45c41f152b5b5e248b04b`  
		Last Modified: Thu, 01 Apr 2021 20:35:58 GMT  
		Size: 600.3 KB (600305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc2b07fd458cb709ef8802767b0fbfac257e94eaf9a6d72d511998b44019f8c`  
		Last Modified: Thu, 01 Apr 2021 20:35:59 GMT  
		Size: 2.6 MB (2572154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2566c638fc1fc5e828e0283159daa162472621369804191602f2088a5ffb72f6`  
		Last Modified: Thu, 01 Apr 2021 20:35:58 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee33b090f3429bee8e80a428d01dd568825bee83c1d760a5d4c297d836bdb1dc`  
		Last Modified: Thu, 01 Apr 2021 20:35:58 GMT  
		Size: 2.0 KB (2037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; 386

```console
$ docker pull yourls@sha256:24034a5bfed6d92dc897e0f8cf03ee3a9125c0232aefcb7633fbf48922c398cb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34069646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:452ea384acd84423799b540874401de95997888cf2df5917419a2777a21a4482`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 02:49:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 02:49:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 02:49:03 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 02:49:03 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 02:49:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 02:55:53 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 02:55:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 02:55:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 02:55:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 02:55:54 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Apr 2021 02:55:55 GMT
ENV PHP_VERSION=8.0.3
# Thu, 01 Apr 2021 02:55:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 01 Apr 2021 02:55:55 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 01 Apr 2021 02:56:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 02:56:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:02:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 03:02:34 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:02:36 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 03:02:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 03:02:36 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 03:02:37 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 03:02:37 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 03:02:38 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 03:02:38 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 09:13:56 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 01 Apr 2021 09:13:58 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 09:14:00 GMT
RUN apk add --no-cache bash
# Thu, 01 Apr 2021 09:14:00 GMT
ENV YOURLS_VERSION=1.8.1
# Thu, 01 Apr 2021 09:14:00 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Thu, 01 Apr 2021 09:14:03 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 01 Apr 2021 09:14:03 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Thu, 01 Apr 2021 09:14:03 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Thu, 01 Apr 2021 09:14:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 09:14:04 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4303b3cd022ad91251e7495aeed4896d9bb7f6fa0dcb18e18234a628ef5cfeec`  
		Last Modified: Thu, 01 Apr 2021 04:41:12 GMT  
		Size: 1.8 MB (1793710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526e185ad2b26faab26d003f328b965c1bbcb1058eae28cb5cb132c7ea7f0c09`  
		Last Modified: Thu, 01 Apr 2021 04:41:11 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e9b82cb292af1dd42fbdda274111233ed643f3515fe3b67e1c212c10f26daa`  
		Last Modified: Thu, 01 Apr 2021 04:41:11 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9428b4cff16222c521f92097bf9b89992104beee3d108a2a7beea9947c425154`  
		Last Modified: Thu, 01 Apr 2021 04:42:24 GMT  
		Size: 10.8 MB (10775166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cdb84a1295b5612ccfc3be7e64054d792ed8873944d2656fbeee538aa781b2`  
		Last Modified: Thu, 01 Apr 2021 04:42:22 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7646fe88db7c4355f7c6493417bec660bcd2b276e3f8afa9be14111c1118ca`  
		Last Modified: Thu, 01 Apr 2021 04:42:23 GMT  
		Size: 15.1 MB (15052269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfba9b93f24716821d6788d4f15500dfa69990ca30b186c39074617524b1a110`  
		Last Modified: Thu, 01 Apr 2021 04:42:18 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79013804856a0c77403f9d8c30f82e43ee202088874e8818264f9d740693e27f`  
		Last Modified: Thu, 01 Apr 2021 04:42:18 GMT  
		Size: 17.5 KB (17504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45793c76738df4904e2801090307aadb449674cc8f7dda58893ec3da1d0ae9e8`  
		Last Modified: Thu, 01 Apr 2021 04:42:18 GMT  
		Size: 8.6 KB (8568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1f04d9f701874f2139a55ed480b38b6f880181d7521e1bdea9bf6397e6a27f`  
		Last Modified: Thu, 01 Apr 2021 09:15:15 GMT  
		Size: 391.0 KB (391008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0408076db82a005ae49e0d90b92049798a53aad75a5a48649c051f2a40620751`  
		Last Modified: Thu, 01 Apr 2021 09:15:10 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecc66e2cf9e6f0d794bb9104f13ff7c2704218c9c8409505ca5b7ff03717f1c0`  
		Last Modified: Thu, 01 Apr 2021 09:15:11 GMT  
		Size: 632.6 KB (632640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a26ed2f71f36467afc099ff539b578a97c49f58733511e9c7898e7b6db98bf88`  
		Last Modified: Thu, 01 Apr 2021 09:15:13 GMT  
		Size: 2.6 MB (2572151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:619195a3f71fb7f7f50b8c94d70447455f4a15dacfa3b033541f74cf050057c0`  
		Last Modified: Thu, 01 Apr 2021 09:15:11 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ff1e075de8c0f40c88cc1c9a76ab166625040300d21fa6a6db025fac96e97f3`  
		Last Modified: Thu, 01 Apr 2021 09:15:11 GMT  
		Size: 2.0 KB (2037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; ppc64le

```console
$ docker pull yourls@sha256:609f430449982290335c5c8bc04cb0ebddede33e717b97bbc3f072a7fe3c0582
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34775195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8ed591e9e880f78c265df93f25e7c2918b8449f7e9e1aaae4e8c23e0541659e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 12:16:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 26 Mar 2021 12:17:00 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 26 Mar 2021 12:17:20 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 26 Mar 2021 12:17:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 26 Mar 2021 12:17:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 26 Mar 2021 12:24:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 26 Mar 2021 12:24:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 12:24:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 12:24:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 26 Mar 2021 12:25:02 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 26 Mar 2021 12:25:06 GMT
ENV PHP_VERSION=8.0.3
# Fri, 26 Mar 2021 12:25:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Fri, 26 Mar 2021 12:25:18 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Fri, 26 Mar 2021 12:25:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 26 Mar 2021 12:25:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:30:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 26 Mar 2021 12:30:42 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:30:52 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Mar 2021 12:31:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Mar 2021 12:31:08 GMT
WORKDIR /var/www/html
# Fri, 26 Mar 2021 12:31:30 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 26 Mar 2021 12:31:36 GMT
STOPSIGNAL SIGQUIT
# Fri, 26 Mar 2021 12:31:38 GMT
EXPOSE 9000
# Fri, 26 Mar 2021 12:31:41 GMT
CMD ["php-fpm"]
# Sat, 27 Mar 2021 04:48:25 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 27 Mar 2021 04:48:36 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 27 Mar 2021 04:48:45 GMT
RUN apk add --no-cache bash
# Sat, 27 Mar 2021 04:48:47 GMT
ENV YOURLS_VERSION=1.8.1
# Sat, 27 Mar 2021 04:48:50 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Sat, 27 Mar 2021 04:48:56 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 27 Mar 2021 04:48:58 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Sat, 27 Mar 2021 04:48:58 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Sat, 27 Mar 2021 04:49:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 04:49:03 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daca8c363f7712061682fe7d66e2ffc7b799dc3eeda331a052371fb1d4e035f4`  
		Last Modified: Fri, 26 Mar 2021 14:03:41 GMT  
		Size: 1.7 MB (1741748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424805b3da287757ac21e21b913464a51a7f769315aa3d315509d358f2abe2d9`  
		Last Modified: Fri, 26 Mar 2021 14:03:40 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264372d3d9e7f169e6bae54417834eaa26d51761308cbd903403393d376a6e94`  
		Last Modified: Fri, 26 Mar 2021 14:03:39 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e94f3e6259ca9ba3fc5bd9afdeb1a4940a1c4d742f76abbde6bdfdb42840217`  
		Last Modified: Fri, 26 Mar 2021 14:04:45 GMT  
		Size: 10.8 MB (10775160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef3f6583cf2c35ce64b6efb0ca100764a6d7f0591911fb1772cd0b4a8ae6b58`  
		Last Modified: Fri, 26 Mar 2021 14:04:40 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3492ef84ca892efc76c479f0785381dc566cf4b662edcada02245e5b1d013028`  
		Last Modified: Fri, 26 Mar 2021 14:04:44 GMT  
		Size: 15.8 MB (15753970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2e45019092cd7d14148964ce017ad33420711de462c50d2c1faba189941161`  
		Last Modified: Fri, 26 Mar 2021 14:04:40 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83f010a2b5e46873add78250324e72df93f6f29a19f4905244df60eeb6493c0c`  
		Last Modified: Fri, 26 Mar 2021 14:04:40 GMT  
		Size: 17.5 KB (17528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:122fce25e0fd7982b68f0f40062d4b84c7df4ef55b4b8ae50feb464135118f37`  
		Last Modified: Fri, 26 Mar 2021 14:04:40 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824a224d66d4831297f1f84fc225d2f427eb091db0873de698e66755b82ea6f3`  
		Last Modified: Sat, 27 Mar 2021 04:49:35 GMT  
		Size: 422.5 KB (422504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2152c136f5d3c2817bfa872c2eca3118bfdce18b1e0a8e7b20d7d25a5fc3633b`  
		Last Modified: Sat, 27 Mar 2021 04:49:31 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fb880646bd8ea794447494c9517d0cf59153280a949f000deb27b8b9d6f489`  
		Last Modified: Sat, 27 Mar 2021 04:49:32 GMT  
		Size: 662.6 KB (662595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc7bfcb2ae1528ae67f11427d05c032614f0e156237928c9be115a219c36659`  
		Last Modified: Sat, 27 Mar 2021 04:49:33 GMT  
		Size: 2.6 MB (2572157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74708016a2b6383719bbe89012e81250cc6c5428c7338811242971a38207dc0c`  
		Last Modified: Sat, 27 Mar 2021 04:49:31 GMT  
		Size: 1.2 KB (1188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bd83772ae8aaf922ba391125b879dc92d20c3c89a06625ad964563d43c297bc`  
		Last Modified: Sat, 27 Mar 2021 04:49:31 GMT  
		Size: 2.0 KB (2035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; s390x

```console
$ docker pull yourls@sha256:f18b9107c06f4e813e2176ff61e60da75968c0c72a68a199127ad5e123cb620b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.8 MB (32770240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:04d1bda3e93deda220ae5e00ca5dc9216c538e563bedfeafadffb287cbfd9000`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 17:14:58 GMT
ADD file:3f5fe04867af3c9f2cfc5b315d97097145ae11343399985386321a8db21d7786 in / 
# Wed, 31 Mar 2021 17:14:58 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 01:11:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 01:11:52 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 01:11:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 01:11:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 01:11:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 01:16:12 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 01:16:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 01:16:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 01:16:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 01:16:13 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Apr 2021 01:16:13 GMT
ENV PHP_VERSION=8.0.3
# Thu, 01 Apr 2021 01:16:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 01 Apr 2021 01:16:13 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 01 Apr 2021 01:16:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 01:16:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 01:20:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 01:20:14 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 01:20:15 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 01:20:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 01:20:15 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 01:20:16 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 01:20:16 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 01:20:17 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 01:20:17 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 05:26:26 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 01 Apr 2021 05:26:26 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 05:26:27 GMT
RUN apk add --no-cache bash
# Thu, 01 Apr 2021 05:26:28 GMT
ENV YOURLS_VERSION=1.8.1
# Thu, 01 Apr 2021 05:26:28 GMT
ENV YOURLS_SHA256=92b0666af3e3ad4a783e78cba93687e9a24acf216606a6d457819c5d36d2cfe4
# Thu, 01 Apr 2021 05:26:29 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 01 Apr 2021 05:26:30 GMT
COPY file:7bfc5a435dd9f76b0c1d23545b13f25bad15f4271d687c1a76bb5d10a41af1eb in /usr/local/bin/ 
# Thu, 01 Apr 2021 05:26:30 GMT
COPY file:0bcfdfe0566007e7477c55552a1341b82b958e95879a5314f411d2188da2429e in /usr/src/yourls/user/ 
# Thu, 01 Apr 2021 05:26:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 05:26:30 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:1d4058bbeedf5296bcaf5ae8f37c8cd58152acad3ec45a536e08b83f5d3abe83`  
		Last Modified: Wed, 31 Mar 2021 17:15:36 GMT  
		Size: 2.6 MB (2602591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4c07ec00cdaafa92f3d601111e0e944457d2558ae06e4ce2e67960618fc651`  
		Last Modified: Thu, 01 Apr 2021 02:24:49 GMT  
		Size: 1.8 MB (1756492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5489cbeafa33cd33ad47e4fd6c7340503c898fb03a500adea4bb365316c28b9`  
		Last Modified: Thu, 01 Apr 2021 02:24:48 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1315fe5c5d5b17d21ea40b00f7ec9504f46655b7a4b0d3ca770546a572162af`  
		Last Modified: Thu, 01 Apr 2021 02:24:48 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b71a6d861b02c2300758b177e344fec34179d167da8bf35181dece005a4bf7ab`  
		Last Modified: Thu, 01 Apr 2021 02:25:31 GMT  
		Size: 10.8 MB (10775167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07dede899b886e26c83c648050491b8ccd19f79d47c629cd1b8558050e6f63a`  
		Last Modified: Thu, 01 Apr 2021 02:25:28 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be656fe18a3c4ec608323890d7f40f15ea463146c640df019a0bcd26f6409485`  
		Last Modified: Thu, 01 Apr 2021 02:25:31 GMT  
		Size: 14.0 MB (14039326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f59540ee1a048cb3510f9d9af7b210cd3c8e09d9e287dcd299d7b8a681ef633b`  
		Last Modified: Thu, 01 Apr 2021 02:25:28 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7c63ab71d932b7713555683d1f38550f9c7bd9ba00b69b879959aeb1d5673d`  
		Last Modified: Thu, 01 Apr 2021 02:25:28 GMT  
		Size: 17.5 KB (17514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4573900651b1f5f52ab3f68a7a0dd389a10c53e6360bb8feac32d9fbc7fa78c2`  
		Last Modified: Thu, 01 Apr 2021 02:25:30 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c01e127bdcccd61a0b4a025b5838142e62fb8239d396a7db132ac6624778c6f`  
		Last Modified: Thu, 01 Apr 2021 05:26:54 GMT  
		Size: 375.4 KB (375380 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62eef6375455d040c1edd6e2a0d9937ed53cbcb6c8b68c23c6c4d5742c6629de`  
		Last Modified: Thu, 01 Apr 2021 05:26:52 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed2ba910473af095ad4e70768acc9b6df7fa1e86c8ca1437915dacba27822feb`  
		Last Modified: Thu, 01 Apr 2021 05:26:52 GMT  
		Size: 615.2 KB (615219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ac28c4e61f0c16fc5280abe299ced6fed40af92a0a57dc3800aa8892a61048`  
		Last Modified: Thu, 01 Apr 2021 05:26:53 GMT  
		Size: 2.6 MB (2572150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2591087de275c36bc631be1836d0476af624b1d98be884608f2a4e0a85bbd7a6`  
		Last Modified: Thu, 01 Apr 2021 05:26:52 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ad8dd5de2f5cea73aeed5de2da21abe79eb2f49a50b602a0cdb2711acb4f23e`  
		Last Modified: Thu, 01 Apr 2021 05:26:52 GMT  
		Size: 2.0 KB (2038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
