## `drupal:fpm-alpine`

```console
$ docker pull drupal@sha256:bc62c354989f3aeeaa51a897af39f4240057760a3ffe436748435f0b0224c1b9
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

### `drupal:fpm-alpine` - linux; amd64

```console
$ docker pull drupal@sha256:9fb3e2c28321362a63a1840e7e99cd42d203f89f6fac16c4325e0c27862f2727
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52505245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cae7387b461507b752c6316425f63ec1676a135dc7e1a7234570325bfec0acf`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:13 GMT
ADD file:f77db8e5b937d8ebb7e254eccd4d311798ea9f4dd5081ea2a7e2b1d3790300c2 in / 
# Wed, 31 Mar 2021 20:10:13 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 15:35:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 15:35:22 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 15:35:23 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 15:35:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 15:35:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 15:40:48 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 15:40:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 15:40:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 15:40:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 15:40:49 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Apr 2021 15:40:49 GMT
ENV PHP_VERSION=8.0.3
# Thu, 01 Apr 2021 15:40:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 01 Apr 2021 15:40:49 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 01 Apr 2021 15:40:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 15:40:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 15:45:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 15:45:51 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 15:45:53 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 15:45:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 15:45:53 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 15:45:54 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 15:45:54 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 15:45:54 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 15:45:54 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 19:29:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 19:29:19 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 20:48:22 GMT
COPY file:fcdd9873d1016333cd6a1e73b637568a047577950b59a36536176b39a60c66cf in /usr/local/bin/ 
# Thu, 01 Apr 2021 20:48:22 GMT
ENV DRUPAL_VERSION=9.1.5
# Thu, 01 Apr 2021 20:48:23 GMT
WORKDIR /opt/drupal
# Thu, 01 Apr 2021 20:48:35 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 01 Apr 2021 20:48:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:532819f3e44cebad88c82f5393801acb876b7a61d36b84bce646561789bb2018`  
		Last Modified: Wed, 31 Mar 2021 20:11:03 GMT  
		Size: 2.8 MB (2799712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aff8d50decdf72ea74c5f261dc5027350a4d32b7c326e4696042548e89a9cf1`  
		Last Modified: Thu, 01 Apr 2021 16:53:59 GMT  
		Size: 1.3 MB (1340902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a17e65b2c2a5419af1354742266ba010b1f9274700addf98c557da542df413b`  
		Last Modified: Thu, 01 Apr 2021 16:53:57 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5babbc773bdaab8d8228e4ea1eb6a10e9e7d62e48fff14cf0d90914bace56cf`  
		Last Modified: Thu, 01 Apr 2021 16:54:00 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4db1c5832fdf7dc5848bce29abbe3588aa01201c1f9f152deb2ff72b3142490`  
		Last Modified: Thu, 01 Apr 2021 16:54:32 GMT  
		Size: 10.8 MB (10774619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47062a3eeee7aeea59f72673ac619259371271f30c3120263ccd871a116b740`  
		Last Modified: Thu, 01 Apr 2021 16:54:31 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:074f9404f286f2270e7be71d558e08acd95986d8df4fbdb1dbcd0b9205d2aed1`  
		Last Modified: Thu, 01 Apr 2021 16:54:33 GMT  
		Size: 15.0 MB (14967870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40e0f9cf896e5373a09f6389afa4fa3950cf874408e4723b86fb02f952de778d`  
		Last Modified: Thu, 01 Apr 2021 16:54:28 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1361c9857b91a2a229e3c41038fad495f302499df548dfe0858b486b24f6d5d3`  
		Last Modified: Thu, 01 Apr 2021 16:54:30 GMT  
		Size: 16.9 KB (16885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a522dbc2bc0cf4262c96c515fd70080c537876d9cfcaec036d899104c425b423`  
		Last Modified: Thu, 01 Apr 2021 16:54:28 GMT  
		Size: 8.6 KB (8567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d0d2b42db796ae4bedd6d887170fdb2360b2c55cb10c4f4f35bcad67cca8de`  
		Last Modified: Thu, 01 Apr 2021 19:35:30 GMT  
		Size: 3.2 MB (3211674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c93e284391a07e18308208175debf57678519c9c8b0fc5bc8fa95945efe11e5`  
		Last Modified: Thu, 01 Apr 2021 19:35:29 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7670566fadb847e69213b189d0444d8955bfa8249eeaa50131d802a427c19b58`  
		Last Modified: Thu, 01 Apr 2021 20:59:17 GMT  
		Size: 553.0 KB (553013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c527d92e6f553d27c9cefd700a078a587236ab0bd69149a3c50142bff1f7addf`  
		Last Modified: Thu, 01 Apr 2021 20:59:15 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715de249c90c68155dda5b0f9688dae8cfc8e5db09de9883c399c452a1d1d0fd`  
		Last Modified: Thu, 01 Apr 2021 20:59:19 GMT  
		Size: 18.8 MB (18827241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-alpine` - linux; arm variant v6

```console
$ docker pull drupal@sha256:005804ce075851ae162c62ff25a401e6f25c6868f091450a15e59eefe1e71ef2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50495311 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4aa09056227d357eb9bc5d4619f9a105f1b8fece8285f60f6c3f0dee483deed6`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:11 GMT
ADD file:00ac3d0df16779e7564cda9cbf94eef90ffa8043778a867272ff0135a1fb537f in / 
# Wed, 31 Mar 2021 17:19:12 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:47:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 31 Mar 2021 22:47:48 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 31 Mar 2021 22:47:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 31 Mar 2021 22:47:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 31 Mar 2021 22:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 31 Mar 2021 22:54:04 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 31 Mar 2021 22:54:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 22:54:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 22:54:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 31 Mar 2021 22:54:08 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 31 Mar 2021 22:54:09 GMT
ENV PHP_VERSION=8.0.3
# Wed, 31 Mar 2021 22:54:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 31 Mar 2021 22:54:10 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 31 Mar 2021 22:54:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 31 Mar 2021 22:54:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 22:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 22:58:19 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Wed, 31 Mar 2021 22:58:25 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 22:58:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 22:58:28 GMT
WORKDIR /var/www/html
# Wed, 31 Mar 2021 22:58:31 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 31 Mar 2021 22:58:32 GMT
STOPSIGNAL SIGQUIT
# Wed, 31 Mar 2021 22:58:33 GMT
EXPOSE 9000
# Wed, 31 Mar 2021 22:58:34 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 05:17:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 05:17:51 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 19:06:04 GMT
COPY file:fcdd9873d1016333cd6a1e73b637568a047577950b59a36536176b39a60c66cf in /usr/local/bin/ 
# Thu, 01 Apr 2021 19:06:06 GMT
ENV DRUPAL_VERSION=9.1.5
# Thu, 01 Apr 2021 19:06:06 GMT
WORKDIR /opt/drupal
# Thu, 01 Apr 2021 19:06:36 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 01 Apr 2021 19:06:49 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:66e54586dae0889b30da12f7a66838d9b86511b58696c83c3b9166ff1a534bbe`  
		Last Modified: Wed, 31 Mar 2021 17:20:05 GMT  
		Size: 2.6 MB (2604658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529c015d2eaf8e9ab8eacefeae519999e683b3a0ed18a191adb3a65a562ce8eb`  
		Last Modified: Thu, 01 Apr 2021 00:03:16 GMT  
		Size: 1.3 MB (1310217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54b442c2bebdb19fcc3177f200ff8ae47793c870b284148b7ae3d32e4b7d1cb0`  
		Last Modified: Thu, 01 Apr 2021 00:03:14 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d9a8d897698cf053dbf182ba7fd6339c136e27795724845908701a3b49aa6f`  
		Last Modified: Thu, 01 Apr 2021 00:03:14 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857d972360567c09200b44a0ce03a99aba512b643d8112ec35ad7fd556c04fb1`  
		Last Modified: Thu, 01 Apr 2021 00:03:53 GMT  
		Size: 10.8 MB (10774625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5dd4cb7d7efae3f00a7164fbd81be76f46ebd2b01ae011782cbce6e684f94d7`  
		Last Modified: Thu, 01 Apr 2021 00:03:48 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b44e6000677cc58f556878480e4f725e99a8dd3cd6ff25bc20aecaf248d399`  
		Last Modified: Thu, 01 Apr 2021 00:03:58 GMT  
		Size: 13.6 MB (13646556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:225029ebaad952b3421bf0b0f10c7a1d14f9b10a1bd411fbcc89f0cce6210c13`  
		Last Modified: Thu, 01 Apr 2021 00:03:48 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3673b8b354b028f2d0bd2d0a5c700ccd141f692354f4045bad761feca36be8e6`  
		Last Modified: Thu, 01 Apr 2021 00:03:48 GMT  
		Size: 16.9 KB (16886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ecf9bc8cd957a22e9f07cd19b8167145061ab8fe1aeace0b18c75d747a3ae8`  
		Last Modified: Thu, 01 Apr 2021 00:03:48 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af3d7f58226457fee663a8866ae7f958a6f6828c221e8d5cd53a19a89cd5989b`  
		Last Modified: Thu, 01 Apr 2021 05:24:09 GMT  
		Size: 2.7 MB (2748672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3059d80856763e51ab8fbfb0a491e23bf92ce0b82706165469d11041028bfdb9`  
		Last Modified: Thu, 01 Apr 2021 05:24:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79d2695f2ca4ba6a8f0dc4fb033ffe11e38b5f9f674790693a5f26da3b9440f9`  
		Last Modified: Thu, 01 Apr 2021 19:11:11 GMT  
		Size: 553.0 KB (553015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c58b4474b67761abc7e5ec268b4c49db625aec2a19f16347361d1463f8a6e5`  
		Last Modified: Thu, 01 Apr 2021 19:11:09 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec6ab001f04f257fc1cb07ea513919a3f28e20e7702a80c94c2054ea6a20cbee`  
		Last Modified: Thu, 01 Apr 2021 19:11:21 GMT  
		Size: 18.8 MB (18827351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-alpine` - linux; arm variant v7

```console
$ docker pull drupal@sha256:0c1d0b4fc259b0d601014185321a94a4efd3250a044895a3b4c4d3259f816e17
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.1 MB (49091984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2f810ce3095ddc95c832d29b5e9e8490199c2cd105d61dd37335afda67933acf`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 18:13:45 GMT
ADD file:1270a9135e4e3d6bcd51f9c8bb7a5129c493366412591f1a6885db98056a572e in / 
# Wed, 31 Mar 2021 18:13:47 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 10:37:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 10:37:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 10:38:05 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 10:38:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 10:38:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 10:41:44 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 10:41:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 10:41:46 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 10:41:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 10:41:48 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Apr 2021 10:41:49 GMT
ENV PHP_VERSION=8.0.3
# Thu, 01 Apr 2021 10:41:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 01 Apr 2021 10:41:52 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 01 Apr 2021 10:42:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 10:42:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 10:44:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 10:44:48 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 10:44:51 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 10:44:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 10:44:53 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 10:44:56 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 10:44:56 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 10:44:57 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 10:44:58 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 15:20:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 15:21:02 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 19:46:54 GMT
COPY file:fcdd9873d1016333cd6a1e73b637568a047577950b59a36536176b39a60c66cf in /usr/local/bin/ 
# Thu, 01 Apr 2021 19:46:54 GMT
ENV DRUPAL_VERSION=9.1.5
# Thu, 01 Apr 2021 19:46:56 GMT
WORKDIR /opt/drupal
# Thu, 01 Apr 2021 19:47:30 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 01 Apr 2021 19:47:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b04429a2165487924dcbfedfff74fa262e6828327d04bb4b1c6a477096f5010e`  
		Last Modified: Wed, 31 Mar 2021 18:15:12 GMT  
		Size: 2.4 MB (2408269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c014c2a1c880d4c4829e5eaf7cf0ec560d6196afc6217656cc6de4c4e133a607`  
		Last Modified: Thu, 01 Apr 2021 11:29:22 GMT  
		Size: 1.2 MB (1214329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acd9f9112566d47aee3c66982e8b96e01743dbfdf373e19aedff96dc560d782`  
		Last Modified: Thu, 01 Apr 2021 11:29:25 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:817d5333294d06a092009820dfa37d07ff76bc101437d4c10f617903b8ebd070`  
		Last Modified: Thu, 01 Apr 2021 11:29:22 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb62458f22b4f678d4040bb5d6bdc18b1d17f5c879e740c6038b9735da09da0`  
		Last Modified: Thu, 01 Apr 2021 11:29:44 GMT  
		Size: 10.8 MB (10774610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1768a8c1283360a067ffdfa476e9f3ddc0d819545261e067e8c741358bc4b86e`  
		Last Modified: Thu, 01 Apr 2021 11:29:43 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7dd486f285dc234574087b99ec7f8f4aa1c31b81ffd4df02cacbb78f3fc28d`  
		Last Modified: Thu, 01 Apr 2021 11:29:44 GMT  
		Size: 12.8 MB (12790945 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43863f93bcf84123097afcea2e5b289bf5d7d564d6f9d60a422df7509c5110cc`  
		Last Modified: Thu, 01 Apr 2021 11:29:42 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:383c9096c95e65f69415578ab03dec6721de8ff1c98d40c9deca7e0856727976`  
		Last Modified: Thu, 01 Apr 2021 11:29:43 GMT  
		Size: 16.9 KB (16866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:142475037caf1d6651490851fad0353f8f91f8ae8a974a21d92e90a30945f23a`  
		Last Modified: Thu, 01 Apr 2021 11:29:40 GMT  
		Size: 8.6 KB (8569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7b8309a46038dc97ad5bf55acd44c99847db7ffdcf37e08d7c94745db0ede5`  
		Last Modified: Thu, 01 Apr 2021 15:30:27 GMT  
		Size: 2.5 MB (2493375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0541b97862c369583f3b5779162c790b440e37a106cd7afc27c2a17b17980e41`  
		Last Modified: Thu, 01 Apr 2021 15:30:26 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c061eefd6017b5038175bd4d22668585a314e8eb9fbcf293dc88c8c65b7f59a7`  
		Last Modified: Thu, 01 Apr 2021 20:04:17 GMT  
		Size: 553.0 KB (553013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c24cac07a4636b70b0ee747af7eb1db1999abe54e008ccf1f002fc181e3701`  
		Last Modified: Thu, 01 Apr 2021 20:04:17 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55efcf93ce3a96e91b306a6c60bc6138b7ceb73f196eeee2cc39adfedc33db87`  
		Last Modified: Thu, 01 Apr 2021 20:04:30 GMT  
		Size: 18.8 MB (18827246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:cd5092f76b745b2e28bbf219060740923750a8b64202088c0747711ee0d292f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51566080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75695780ddace5b6399e413f0611a6a58bb790d5adeda6c09bb1057a16fe84b1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:48 GMT
ADD file:dd1db8a59e36aac513488fa97629360c665b6079fb7c6b3cd09065ef993f6675 in / 
# Wed, 31 Mar 2021 17:21:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 14:27:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 14:27:36 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 14:27:39 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 14:27:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 14:27:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 14:31:38 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 14:31:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 14:31:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 14:31:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 14:31:41 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Apr 2021 14:31:42 GMT
ENV PHP_VERSION=8.0.3
# Thu, 01 Apr 2021 14:31:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 01 Apr 2021 14:31:44 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 01 Apr 2021 14:31:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 14:31:50 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 14:35:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 14:35:11 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 14:35:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 14:35:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 14:35:15 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 14:35:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 14:35:19 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 14:35:19 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 14:35:20 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 19:36:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 19:36:06 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 19:36:07 GMT
COPY file:fcdd9873d1016333cd6a1e73b637568a047577950b59a36536176b39a60c66cf in /usr/local/bin/ 
# Thu, 01 Apr 2021 19:36:08 GMT
ENV DRUPAL_VERSION=9.1.5
# Thu, 01 Apr 2021 19:36:09 GMT
WORKDIR /opt/drupal
# Thu, 01 Apr 2021 19:36:29 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 01 Apr 2021 19:36:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:9a219e8acc52b4071b6121a1e4d4ecbce48f38113fbbcfe026c26768ce76bcc0`  
		Last Modified: Wed, 31 Mar 2021 17:22:52 GMT  
		Size: 2.7 MB (2709852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92dba67ea2fd5816dd837ab3462f2eb2eaa8f5b1de107ec82c8825805955830c`  
		Last Modified: Thu, 01 Apr 2021 15:28:52 GMT  
		Size: 1.3 MB (1342973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84790c433c4c7efb40e084d3fff815c4bc175c07e527e3fc6103758d5118dd4`  
		Last Modified: Thu, 01 Apr 2021 15:28:52 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed570efd768c764ea5c77c43a405863ea75c89092d334a29d0644c807e4798c8`  
		Last Modified: Thu, 01 Apr 2021 15:28:52 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a5793702a146f2d9cacfff4ae4618b570e4b3e8b992c6bf34eb046a58970956`  
		Last Modified: Thu, 01 Apr 2021 15:29:19 GMT  
		Size: 10.8 MB (10774611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47af04c0c667021f60b8487130ad9018ccd50d0da4e44a4b312e82eed9cafc0`  
		Last Modified: Thu, 01 Apr 2021 15:29:13 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cbc21d81a741a15a85308f9f30b19fc59f2d5fec587e5667bd63cb41fb5fe1`  
		Last Modified: Thu, 01 Apr 2021 15:29:18 GMT  
		Size: 14.4 MB (14438753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc2d8b7a66a726fb5b519a6ae207f9e9cd3e39124442eafe587cf6b297916de`  
		Last Modified: Thu, 01 Apr 2021 15:29:16 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67c6f43d454db78414b2140decec57260e07dea9c7acb12901c59dd4ad1f2d2d`  
		Last Modified: Thu, 01 Apr 2021 15:29:17 GMT  
		Size: 16.9 KB (16881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4dac6513ee5f40002c95edb61fb9dcf30601887cf896b212ad0ee2f8bf6713`  
		Last Modified: Thu, 01 Apr 2021 15:29:13 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b60c9e6518223547682b9d559a8b9a59467e4268d2bb946d4c55ab468e514c16`  
		Last Modified: Thu, 01 Apr 2021 19:49:42 GMT  
		Size: 2.9 MB (2889270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d0789aa92d2a4142147092f08e44e5c933547475db4920558a9f677a15ad547`  
		Last Modified: Thu, 01 Apr 2021 19:49:42 GMT  
		Size: 322.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4a8f0eb1df9123fe829b52fc6edbb85d07823ab2fe8cc9913aa5290919a679c`  
		Last Modified: Thu, 01 Apr 2021 19:49:42 GMT  
		Size: 553.0 KB (552997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a46f45859c4251d01808c4882093429b18993e08b655659cb26d494ac857198`  
		Last Modified: Thu, 01 Apr 2021 19:49:42 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed8bb1216cc8642d43e446511cdbe703200175d8262f0cd3b435b62cfc41dd69`  
		Last Modified: Thu, 01 Apr 2021 19:49:49 GMT  
		Size: 18.8 MB (18827415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-alpine` - linux; 386

```console
$ docker pull drupal@sha256:7f5c04975b807863fe692b11e0fadd181d8f2d836f5b28cec13c837222d17e34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52512450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b566dee368151204bbddc0c2d3d4305cae69e49de5da3942ba851cff89bb2184`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:08 GMT
ADD file:053c3a6154e80758106cbf0fec936c3b41dabf24a9f5eda36416caa90556810c in / 
# Wed, 31 Mar 2021 17:43:09 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:02:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 03:02:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 03:02:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 03:02:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 03:02:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 03:08:53 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 03:08:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 03:08:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 03:08:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 03:08:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Apr 2021 03:08:54 GMT
ENV PHP_VERSION=8.0.3
# Thu, 01 Apr 2021 03:08:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 01 Apr 2021 03:08:54 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 01 Apr 2021 03:09:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 03:09:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:14:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 03:14:47 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:14:48 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 03:14:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 03:14:49 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 03:14:50 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 03:14:50 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 03:14:50 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 03:14:50 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 09:18:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 09:18:05 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 18:56:25 GMT
COPY file:fcdd9873d1016333cd6a1e73b637568a047577950b59a36536176b39a60c66cf in /usr/local/bin/ 
# Thu, 01 Apr 2021 18:56:25 GMT
ENV DRUPAL_VERSION=9.1.5
# Thu, 01 Apr 2021 18:56:25 GMT
WORKDIR /opt/drupal
# Thu, 01 Apr 2021 18:56:37 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 01 Apr 2021 18:56:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:8eca83e4805e4c5e7b071425a4603bc4b02885b817aa7c1bba9605bd2cb9125a`  
		Last Modified: Wed, 31 Mar 2021 17:44:26 GMT  
		Size: 2.8 MB (2794977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca80016dbb16befd5aa82b9149d37c6577450d173d66fb0b638d8377822407d4`  
		Last Modified: Thu, 01 Apr 2021 04:43:07 GMT  
		Size: 1.4 MB (1439817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fafae2eed22e4f4b7c690e28391ddf1a273067a5b12e3c4f32827774dd5bdc15`  
		Last Modified: Thu, 01 Apr 2021 04:43:05 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db45b483048b084820a30ce08c132efa2cbc029b60de461a4e5b5e897e48299f`  
		Last Modified: Thu, 01 Apr 2021 04:43:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7695750d537f67a5401bd95f6e2b9cc91482bc3d69291678258057ed542e468`  
		Last Modified: Thu, 01 Apr 2021 04:43:45 GMT  
		Size: 10.8 MB (10774605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200423445e20eb5c286e0144749694b1ef51a31143d32e2ee4d0f4a8deb4edf4`  
		Last Modified: Thu, 01 Apr 2021 04:43:41 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:595dea1e1852f9999c6a5825de7f128dfd4872281df4b31e7d36f52bacef4c4a`  
		Last Modified: Thu, 01 Apr 2021 04:43:46 GMT  
		Size: 15.0 MB (15014195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d9e3a253c8453d60c5eadf6cb196101b6c71ea9c73738eaeac8b659e31e40e`  
		Last Modified: Thu, 01 Apr 2021 04:43:41 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b15d92de38ce36aba3b45351116c4a4a1791f72d7e416b58cc3107592700ae`  
		Last Modified: Thu, 01 Apr 2021 04:43:41 GMT  
		Size: 16.9 KB (16878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c022dc4f04dd3b52072ca62c2748b8057570a573574b5f703f19634f3d4328`  
		Last Modified: Thu, 01 Apr 2021 04:43:41 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0013f70a540fd2abd69e6d8b6da5860a37bc4c815ac56ff4ad5e38c07b8cef01`  
		Last Modified: Thu, 01 Apr 2021 09:33:11 GMT  
		Size: 3.1 MB (3078236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff819dcc0ed43dcec75f43fcd23337da4eca7c95e946bcaa40f7f3a12332c53`  
		Last Modified: Thu, 01 Apr 2021 09:33:10 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e20e1a087ced6b7059ff163764447e86aa1a10ceb741ad83ed977a1cd1dba8`  
		Last Modified: Thu, 01 Apr 2021 19:12:55 GMT  
		Size: 553.0 KB (553013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b75936f4faab10904785f4b689a874c89a5840d75cd10bd0982224bf68d2e6`  
		Last Modified: Thu, 01 Apr 2021 19:12:54 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9cdd135cfebec068d037e9fafe2262a80f51b8cb850757d237645adc5e597c`  
		Last Modified: Thu, 01 Apr 2021 19:13:02 GMT  
		Size: 18.8 MB (18827396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-alpine` - linux; ppc64le

```console
$ docker pull drupal@sha256:98d61a94a8faa4ffdd1e1329b2ebe25df3ff3eab423e99a8ecbe43c293ce36ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53099125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5bc4cba1c002d58378bc0c4f3a2b0077726ab4e0c6ef9cbdbcb3ab07bf520c91`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 18:56:11 GMT
ADD file:d51af61c5955c980d18387ab532110c3874f95a87768be84dfd1eeb3e701d3a4 in / 
# Wed, 31 Mar 2021 18:56:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 22:04:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 22:05:09 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 22:05:25 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 22:05:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 22:05:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 22:11:50 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 22:11:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 22:12:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 22:12:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 22:12:14 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Apr 2021 22:12:17 GMT
ENV PHP_VERSION=8.0.3
# Thu, 01 Apr 2021 22:12:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 01 Apr 2021 22:12:27 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 01 Apr 2021 22:12:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 22:12:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 22:16:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 22:16:46 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 22:17:04 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 22:17:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 22:17:17 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 22:17:30 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 22:17:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 22:17:45 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 22:17:51 GMT
CMD ["php-fpm"]
# Fri, 02 Apr 2021 05:14:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 02 Apr 2021 05:14:45 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 02 Apr 2021 05:14:46 GMT
COPY file:fcdd9873d1016333cd6a1e73b637568a047577950b59a36536176b39a60c66cf in /usr/local/bin/ 
# Fri, 02 Apr 2021 05:14:48 GMT
ENV DRUPAL_VERSION=9.1.5
# Fri, 02 Apr 2021 05:14:51 GMT
WORKDIR /opt/drupal
# Fri, 02 Apr 2021 05:15:22 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 02 Apr 2021 05:15:33 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:d6d4557865d9cec3513c1a5e744cb1073a563d464b8d546911289b9df9998f1b`  
		Last Modified: Wed, 31 Mar 2021 18:57:36 GMT  
		Size: 2.8 MB (2806070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9419926485e714786eb20b7eb5cddc3574a440af1413622feea82302dd7d50eb`  
		Last Modified: Thu, 01 Apr 2021 23:47:54 GMT  
		Size: 1.4 MB (1383186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f862a619e55f20cb796df3edd9f18562b5ddf486d1b216aae0b99287bef1a9`  
		Last Modified: Thu, 01 Apr 2021 23:47:53 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cd54117ef328fe730dd1cb898fb4c4d348136267dc726c3595c65d680f06ff`  
		Last Modified: Thu, 01 Apr 2021 23:47:53 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00daad187e330451ca0600aa8394d69d3eae3917ec382b70cdbf2da5b506548`  
		Last Modified: Thu, 01 Apr 2021 23:48:24 GMT  
		Size: 10.8 MB (10774630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766ff1f374d1b828cddc1a963b0d25939053004bf3631c81da9832d36b479215`  
		Last Modified: Thu, 01 Apr 2021 23:48:20 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efa16d3a484d7f57ee1c92fc25771e47ae6e751bbddb8528a2989e59d6be9d81`  
		Last Modified: Thu, 01 Apr 2021 23:48:23 GMT  
		Size: 15.7 MB (15654041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8a734bc60ab5138e705d32a97ab3328b74bae7851e77ac1ae05e79267e9c239`  
		Last Modified: Thu, 01 Apr 2021 23:48:19 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb46eab7f78d25735f58a2092aa2c2cdce1183fd7a690adde026d9d5477f6919`  
		Last Modified: Thu, 01 Apr 2021 23:48:19 GMT  
		Size: 16.9 KB (16930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8c446186f9c8178000c4cb6e8a5a6f30d618ffc990c5858fbd4de3529810b3e`  
		Last Modified: Thu, 01 Apr 2021 23:48:19 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd822c52132dfc786c54f3d4eedfa77b7c5a3b7fdaaba21e37d5f397630ed406`  
		Last Modified: Fri, 02 Apr 2021 05:41:50 GMT  
		Size: 3.1 MB (3070819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff8ae672391ee6def62d3f6a8cb2480575e876266f304bbdb70c01620fe4903`  
		Last Modified: Fri, 02 Apr 2021 05:41:47 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbaedc17515697da4e933c74f418ebfef6ba5b00cc227ac6f7e8c1630592984e`  
		Last Modified: Fri, 02 Apr 2021 05:41:50 GMT  
		Size: 553.0 KB (553004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e975107279c33167067708da36370e7d2b326c405d25e08c2423ee2a40066c00`  
		Last Modified: Fri, 02 Apr 2021 05:41:47 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b64c30adbedd7a8fd8250fa9b7630175916ac88a0328bc29a9082053cefefe44`  
		Last Modified: Fri, 02 Apr 2021 05:43:13 GMT  
		Size: 18.8 MB (18827104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:fpm-alpine` - linux; s390x

```console
$ docker pull drupal@sha256:6b5fbfc5b8e2768c8a9d9dbf0df36565841a2502c1aa8f70b92734ce2f232d78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.0 MB (50989239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d55c6299d60f2ed388091d981cb3b0f80220d534d68408905d1fc808df414ecf`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 31 Mar 2021 17:15:04 GMT
ADD file:1f37b92ea1f573c4810b1d056dc4880cf4035e143451d9b2b76fac1e3b462248 in / 
# Wed, 31 Mar 2021 17:15:04 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 01:20:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 01:20:35 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 01:20:36 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 01:20:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 01:20:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 01:24:10 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 01 Apr 2021 01:24:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 01:24:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 01:24:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 01:24:10 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Apr 2021 01:24:11 GMT
ENV PHP_VERSION=8.0.3
# Thu, 01 Apr 2021 01:24:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 01 Apr 2021 01:24:11 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 01 Apr 2021 01:24:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 01:24:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 01:27:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 01:27:22 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 01 Apr 2021 01:27:23 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 01:27:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 01:27:24 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 01:27:24 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 01 Apr 2021 01:27:25 GMT
STOPSIGNAL SIGQUIT
# Thu, 01 Apr 2021 01:27:25 GMT
EXPOSE 9000
# Thu, 01 Apr 2021 01:27:25 GMT
CMD ["php-fpm"]
# Thu, 01 Apr 2021 04:43:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 04:43:33 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 01 Apr 2021 19:00:06 GMT
COPY file:fcdd9873d1016333cd6a1e73b637568a047577950b59a36536176b39a60c66cf in /usr/local/bin/ 
# Thu, 01 Apr 2021 19:00:07 GMT
ENV DRUPAL_VERSION=9.1.5
# Thu, 01 Apr 2021 19:00:07 GMT
WORKDIR /opt/drupal
# Thu, 01 Apr 2021 19:00:37 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 01 Apr 2021 19:00:48 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:38ca5430c9af12b6b6dee7c10eb6b1eb0e4eb4f5f02a97890579c4b049d00233`  
		Last Modified: Wed, 31 Mar 2021 17:15:46 GMT  
		Size: 2.6 MB (2567453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f75ff5798a3be1bbf9691a3973afbe2cac00ea8c1f975b8b60d0b93b0b0e84`  
		Last Modified: Thu, 01 Apr 2021 02:25:58 GMT  
		Size: 1.4 MB (1382756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7ffde9ee48b9893e4b0d2bd8df2b125908e31b9101fe101724f1123a8d1ff04`  
		Last Modified: Thu, 01 Apr 2021 02:25:58 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f9afdc302e5e2c38c9828e1a1732a2b7d051d2a78bf81eace5124f0630ee38a`  
		Last Modified: Thu, 01 Apr 2021 02:25:57 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0320829ff1eb47cb438a2203ef84f408642d62184daaef6f03fa18c355e73aea`  
		Last Modified: Thu, 01 Apr 2021 02:26:25 GMT  
		Size: 10.8 MB (10774613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19020f4ba5721fb409b21496572df850ce62683fd80499aadda0f42a2af82cdf`  
		Last Modified: Thu, 01 Apr 2021 02:26:22 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:782d1854ea40b582798cf57bb47b57c3f2d8b307469341404972f082bbd33b01`  
		Last Modified: Thu, 01 Apr 2021 02:26:28 GMT  
		Size: 13.9 MB (13934605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d680063be70112cf8a7158f58b2a2c3256528724d9db37b654f2cc5f861266c`  
		Last Modified: Thu, 01 Apr 2021 02:26:22 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93970eeefd31e5d96a7c8e3c94c2ab57218f36f39e55508389cae80e308ce4eb`  
		Last Modified: Thu, 01 Apr 2021 02:26:22 GMT  
		Size: 16.9 KB (16876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8f524975abbb92888814aaa7693c7beefa627b68680091c3989eb8653410886`  
		Last Modified: Thu, 01 Apr 2021 02:26:22 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2773eef52a10db282875e3901f524d2f6bc397d66b20198d352176458c0c0505`  
		Last Modified: Thu, 01 Apr 2021 04:48:49 GMT  
		Size: 2.9 MB (2919608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4c0dc773f894550efa69e7fc2dd075f78c7c663639a1d6c7888d0eeb71a292`  
		Last Modified: Thu, 01 Apr 2021 04:48:49 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79b199ee56b5a758d9267ee769c402be0e4fbd332023fff3f67d713273080e5c`  
		Last Modified: Thu, 01 Apr 2021 19:17:48 GMT  
		Size: 553.0 KB (553005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2365375a4fd59290415b056ad039042ef1a1e2bb7c54357e0d8952ae880c8dd0`  
		Last Modified: Thu, 01 Apr 2021 19:17:48 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e74fee41f901d759782e305c09574ba17dcc830a6301dbdff17b51cb2ec529f`  
		Last Modified: Thu, 01 Apr 2021 19:17:53 GMT  
		Size: 18.8 MB (18826990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
