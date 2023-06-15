## `drupal:9-fpm-alpine3.17`

```console
$ docker pull drupal@sha256:894aa6ef33585f536d1b40d165734ce4061f31036057e764d7195a5ab12a3a2b
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

### `drupal:9-fpm-alpine3.17` - linux; amd64

```console
$ docker pull drupal@sha256:3460645cd9a4419207c7ac5f1cc512ab734510b9322ac910a33bbd2a9a7fd164
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.4 MB (55373072 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e177f5bc9b9cff3a860eb975dfde9b6cdb421dff8805fa069cfc141afa951bef`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:42:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Jun 2023 00:42:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Jun 2023 00:42:37 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Jun 2023 00:42:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Jun 2023 00:42:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 15 Jun 2023 00:42:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 00:42:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 00:42:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Jun 2023 01:28:25 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 15 Jun 2023 01:28:25 GMT
ENV PHP_VERSION=8.1.20
# Thu, 15 Jun 2023 01:28:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.20.tar.xz.asc
# Thu, 15 Jun 2023 01:28:25 GMT
ENV PHP_SHA256=4c9973f599e93ed5e8ce2b45ce1d41bb8fb54ce642824fd23e56b52fd75029a6
# Thu, 15 Jun 2023 01:28:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Jun 2023 01:28:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Jun 2023 01:35:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Jun 2023 01:35:58 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 15 Jun 2023 01:35:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Jun 2023 01:35:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Jun 2023 01:35:59 GMT
WORKDIR /var/www/html
# Thu, 15 Jun 2023 01:35:59 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 15 Jun 2023 01:35:59 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 01:35:59 GMT
EXPOSE 9000
# Thu, 15 Jun 2023 01:36:00 GMT
CMD ["php-fpm"]
# Thu, 15 Jun 2023 07:31:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 15 Jun 2023 07:31:35 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 15 Jun 2023 07:31:35 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Thu, 15 Jun 2023 07:32:26 GMT
ENV DRUPAL_VERSION=9.5.9
# Thu, 15 Jun 2023 07:32:26 GMT
WORKDIR /opt/drupal
# Thu, 15 Jun 2023 07:32:38 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 15 Jun 2023 07:32:39 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2d0e53cae4fa9e99bf4244568126b8df6d69fe6ee06580fe987d0ac9bc1c51`  
		Last Modified: Thu, 15 Jun 2023 02:07:56 GMT  
		Size: 1.9 MB (1891710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0018871e86ff704c651cf77f534a17074a5da1002810199a8bcd197e0f2b7e3`  
		Last Modified: Thu, 15 Jun 2023 02:07:56 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:399c2bf9de3aced3bdb63485e296ec23ab7f52a54441ccb6d70b52fd4dd30e02`  
		Last Modified: Thu, 15 Jun 2023 02:07:55 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9fc4bfe09c6fd4dee445dc995366a7b4bd22c23320cfdce91ee022867e8fec`  
		Last Modified: Thu, 15 Jun 2023 02:12:16 GMT  
		Size: 11.8 MB (11813669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c28c4abbb1d9f850dada7b15969d8b5c5597e8eaa495bc9076e97644035239`  
		Last Modified: Thu, 15 Jun 2023 02:12:15 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d486286d2f60890dd6230313bcb80e54a2c704167cf76693fa76db40490c948`  
		Last Modified: Thu, 15 Jun 2023 02:12:37 GMT  
		Size: 12.5 MB (12493242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6260e964a29f3f82409318d08b2cfed4b16586b303c32c84e77d74d388a67c9`  
		Last Modified: Thu, 15 Jun 2023 02:12:35 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb1f6e3b8976ed42ea70a993e3effe71da387b916b90c143bff4d022e1588bc`  
		Last Modified: Thu, 15 Jun 2023 02:12:35 GMT  
		Size: 19.0 KB (18967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c996aae3a719d3e7f45bc5455d46911887deda6960bca44ce44b9a1310245ff`  
		Last Modified: Thu, 15 Jun 2023 02:12:35 GMT  
		Size: 8.9 KB (8879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38518b1024431939a143381c59248016c500d308fe00e49ba76f66ad96c4495c`  
		Last Modified: Thu, 15 Jun 2023 07:39:55 GMT  
		Size: 2.2 MB (2205899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb8a7652826ee251b9b418b479c34ca1f78a58dfa4ff4bfc6c889fab557996e`  
		Last Modified: Thu, 15 Jun 2023 07:39:54 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48bff9c980218b2cdbc5c7d170e7095a1077d2f10d654437fb35ad67474e8755`  
		Last Modified: Thu, 15 Jun 2023 07:39:54 GMT  
		Size: 698.2 KB (698237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:066c9e7ea49a2898a5e97d92a94a3723c29e5978b74f6e5603ee88bf66b81ea8`  
		Last Modified: Thu, 15 Jun 2023 07:41:01 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b39d9b300abca210e3dd24db51726518eaff2aa6f016c3333e2cfd397331cb`  
		Last Modified: Thu, 15 Jun 2023 07:41:06 GMT  
		Size: 22.9 MB (22862822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-alpine3.17` - linux; arm variant v6

```console
$ docker pull drupal@sha256:aeaac9851b7ee4f2639e9361acb0541d3543bafc5fd085a4cc27353c24e2eb84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.4 MB (53359635 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcc287c1811d5d5fc80b6b1ea05e58d31fab34590fcfb92ac33f78418f31eeba`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 18:49:25 GMT
ADD file:07e668ef139dce7f076143a30b89ff57885c8539d8b5764ac1bd5277d9936702 in / 
# Wed, 14 Jun 2023 18:49:25 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:12:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Jun 2023 00:12:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Jun 2023 00:12:22 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Jun 2023 00:12:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Jun 2023 00:12:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 15 Jun 2023 00:12:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 00:12:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 00:12:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Jun 2023 00:48:06 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 15 Jun 2023 00:48:07 GMT
ENV PHP_VERSION=8.1.20
# Thu, 15 Jun 2023 00:48:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.20.tar.xz.asc
# Thu, 15 Jun 2023 00:48:07 GMT
ENV PHP_SHA256=4c9973f599e93ed5e8ce2b45ce1d41bb8fb54ce642824fd23e56b52fd75029a6
# Thu, 15 Jun 2023 00:48:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Jun 2023 00:48:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Jun 2023 00:54:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Jun 2023 00:54:27 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 15 Jun 2023 00:54:29 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Jun 2023 00:54:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Jun 2023 00:54:29 GMT
WORKDIR /var/www/html
# Thu, 15 Jun 2023 00:54:30 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 15 Jun 2023 00:54:31 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 00:54:31 GMT
EXPOSE 9000
# Thu, 15 Jun 2023 00:54:31 GMT
CMD ["php-fpm"]
# Thu, 15 Jun 2023 07:38:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 15 Jun 2023 07:38:45 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 15 Jun 2023 07:38:45 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Thu, 15 Jun 2023 07:39:19 GMT
ENV DRUPAL_VERSION=9.5.9
# Thu, 15 Jun 2023 07:39:19 GMT
WORKDIR /opt/drupal
# Thu, 15 Jun 2023 07:39:31 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 15 Jun 2023 07:39:32 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:33ec62e98ceea71d24212ee03e239c2d5538dbe7c98f41c42e8b2693fedf58fb`  
		Last Modified: Wed, 14 Jun 2023 18:50:00 GMT  
		Size: 3.1 MB (3110916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaf22d1d692138b9e57071d39851f829f232b8f3852af079a2961453ba31c5c`  
		Last Modified: Thu, 15 Jun 2023 01:18:03 GMT  
		Size: 1.9 MB (1878933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0857b1d531af3d47422625dae6d0da81a3c69a1d8124d4756481afd3f4b05485`  
		Last Modified: Thu, 15 Jun 2023 01:18:03 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1ee0b1458dcd2b82cfe16e510b5edfb32836b137345c314aedd96c772c9e2fd`  
		Last Modified: Thu, 15 Jun 2023 01:18:03 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742fdce25f8d432c2f800ef7e0b74a27f05ecf687d0403be1f4ce3809e668d7f`  
		Last Modified: Thu, 15 Jun 2023 01:22:07 GMT  
		Size: 11.8 MB (11813662 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98d117ece08e662b3bb93d64ed3a05fe82eea3b2e4b259bd1c1feb6935a6fef`  
		Last Modified: Thu, 15 Jun 2023 01:22:06 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6906880b90803f4018d54fc1b673c149920e0c32fc587b18f88f1c05d338fcbb`  
		Last Modified: Thu, 15 Jun 2023 01:22:25 GMT  
		Size: 11.3 MB (11294929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b99192a60c0a9c9a86ba5b940bd8836fa049550edaf564a959226700903e2a`  
		Last Modified: Thu, 15 Jun 2023 01:22:22 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e3a685990382d5ead00e09d7507093674e50e1e25365c29a66c78bb82ad07f4`  
		Last Modified: Thu, 15 Jun 2023 01:22:23 GMT  
		Size: 18.7 KB (18746 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5074edde843163a627826334bf5c44b52d7c5d0b2423985ddb5a989a0e141c9`  
		Last Modified: Thu, 15 Jun 2023 01:22:23 GMT  
		Size: 8.9 KB (8879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c16c82463c712d6153fa5f27cbcf6a17ae19207e83e03db5a1abf566e0695a2`  
		Last Modified: Thu, 15 Jun 2023 07:43:40 GMT  
		Size: 1.7 MB (1667761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fe2e256f23939e1cccfeddeb781e8c69bb10da0984f8ff85be660c9ea8f2617`  
		Last Modified: Thu, 15 Jun 2023 07:43:40 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd4fb705371d91e9a5be1a8a96fd784af3c8a8e9feee5315f657cc613b1c1f5`  
		Last Modified: Thu, 15 Jun 2023 07:43:40 GMT  
		Size: 698.2 KB (698237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c66f2f6e7befec0c9b8418ec078f92cec0a5c0f495443a3695c9edc5a8c9be7`  
		Last Modified: Thu, 15 Jun 2023 07:44:37 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77f7851a4c23d2fd01fc29c778bee234ab57b33f62ce6c47a51d3e37fcc48d3b`  
		Last Modified: Thu, 15 Jun 2023 07:44:45 GMT  
		Size: 22.9 MB (22862642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-alpine3.17` - linux; arm variant v7

```console
$ docker pull drupal@sha256:6da878fca4c862b10abadc451a1d0d0130d1266881f6552fe7e616bff0f0a7b8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.2 MB (52160124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ba6171d52853fe68232e26dfebef819cd33d82066fef43a9d6ca722bdff98d6`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 22:36:20 GMT
ADD file:5e92075a8d9a5898d661caf9c2be8a83fb25742251b4ebdc0c3d448a6dc58e4a in / 
# Wed, 14 Jun 2023 22:36:20 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 05:49:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Jun 2023 05:49:24 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Jun 2023 05:49:24 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Jun 2023 05:49:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Jun 2023 05:49:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 15 Jun 2023 05:49:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 05:49:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 05:49:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Jun 2023 06:21:02 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 15 Jun 2023 06:21:02 GMT
ENV PHP_VERSION=8.1.20
# Thu, 15 Jun 2023 06:21:03 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.20.tar.xz.asc
# Thu, 15 Jun 2023 06:21:03 GMT
ENV PHP_SHA256=4c9973f599e93ed5e8ce2b45ce1d41bb8fb54ce642824fd23e56b52fd75029a6
# Thu, 15 Jun 2023 06:21:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Jun 2023 06:21:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:26:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Jun 2023 06:26:56 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 15 Jun 2023 06:26:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Jun 2023 06:26:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Jun 2023 06:26:58 GMT
WORKDIR /var/www/html
# Thu, 15 Jun 2023 06:26:58 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 15 Jun 2023 06:26:58 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 06:26:58 GMT
EXPOSE 9000
# Thu, 15 Jun 2023 06:26:58 GMT
CMD ["php-fpm"]
# Thu, 15 Jun 2023 10:05:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 15 Jun 2023 10:05:33 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 15 Jun 2023 10:05:33 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Thu, 15 Jun 2023 10:06:17 GMT
ENV DRUPAL_VERSION=9.5.9
# Thu, 15 Jun 2023 10:06:17 GMT
WORKDIR /opt/drupal
# Thu, 15 Jun 2023 10:06:35 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 15 Jun 2023 10:06:36 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:f929d112168394cf1fbe294a86fbe5173dd92df4daac8cb09437b17dfc5df802`  
		Last Modified: Wed, 14 Jun 2023 22:37:01 GMT  
		Size: 2.9 MB (2868554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843b9be152d4cd0c3de22f6fb9284ad2c5dafc56e0cd77fa68b1c24f55df924b`  
		Last Modified: Thu, 15 Jun 2023 06:53:14 GMT  
		Size: 1.7 MB (1729849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a35d433c619ac5af5e64c3c595b3bc873ad3f2197d7a53638876588561e7543a`  
		Last Modified: Thu, 15 Jun 2023 06:53:14 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82cf8ee65ec812346ccaa3b847e8487521cbb1284308eb32599ac968d20d449f`  
		Last Modified: Thu, 15 Jun 2023 06:53:14 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7aa687af2124f5b7ba0c4fd47e9d98cda8f991e7521beb9449b28f979f56527`  
		Last Modified: Thu, 15 Jun 2023 06:57:23 GMT  
		Size: 11.8 MB (11813648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed1837abde731eb439bcbc3a7d7127b211f6e9063e91223de7f29361671315f`  
		Last Modified: Thu, 15 Jun 2023 06:57:22 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c172a1c6c55a64eff24aa064523f859fff81677cb89161459cf355505d38e130`  
		Last Modified: Thu, 15 Jun 2023 06:57:38 GMT  
		Size: 10.6 MB (10617485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a6ac56227a23cd628a31c83f8556cf356514021a396a23f48d36b5d13ae31cb`  
		Last Modified: Thu, 15 Jun 2023 06:57:36 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7f397177c7cb930752eba51767603e47e0b81e59a4391eb923b222a7ae0869`  
		Last Modified: Thu, 15 Jun 2023 06:57:36 GMT  
		Size: 18.8 KB (18759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9920f410d00d6b3e0ab19b86ceb5f0c75451c1678e49214476e1e70328203546`  
		Last Modified: Thu, 15 Jun 2023 06:57:36 GMT  
		Size: 8.9 KB (8880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5a2059f50f91eb7a13012deb30faec40e500cb4b9ac3ef3476ed485b56a4df5`  
		Last Modified: Thu, 15 Jun 2023 10:13:13 GMT  
		Size: 1.5 MB (1536906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65081cb07d5aae6dbdea3838930a14c9cfa166d603ccf390c0c3126a7aae519d`  
		Last Modified: Thu, 15 Jun 2023 10:13:12 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d236283f0a66578966a74d479535b28abdf3d1dd4e41f531514381b4fb3aa0cc`  
		Last Modified: Thu, 15 Jun 2023 10:13:13 GMT  
		Size: 698.2 KB (698238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b1ed2371315ffa3ad6c88b8e7cde92d61e276a1413874db61f29ff390cd510`  
		Last Modified: Thu, 15 Jun 2023 10:14:21 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9a5cb5fde1b36c1eca3d46b25d92624a6249130cd09947e0ef5b81060e5fa8`  
		Last Modified: Thu, 15 Jun 2023 10:14:28 GMT  
		Size: 22.9 MB (22862877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:eaa1de3a2af9f77383f93d1766587d07b21255a782aab051366111d6c5bd0c3d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.5 MB (55476954 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a2abe742c877f4f21eb15737202d8c860287fb20838efccb0e552d30d3a7c509`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 20:49:04 GMT
ADD file:6f6c919dc1fe5a56c2664a26a702d77203039cdd4c91e39da57063ea5d3f3094 in / 
# Wed, 14 Jun 2023 20:49:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 03:17:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Jun 2023 03:17:47 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Jun 2023 03:17:47 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Jun 2023 03:17:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Jun 2023 03:17:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 15 Jun 2023 03:17:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 03:17:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 03:17:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Jun 2023 04:04:26 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 15 Jun 2023 04:04:26 GMT
ENV PHP_VERSION=8.1.20
# Thu, 15 Jun 2023 04:04:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.20.tar.xz.asc
# Thu, 15 Jun 2023 04:04:26 GMT
ENV PHP_SHA256=4c9973f599e93ed5e8ce2b45ce1d41bb8fb54ce642824fd23e56b52fd75029a6
# Thu, 15 Jun 2023 04:04:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Jun 2023 04:04:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Jun 2023 04:11:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Jun 2023 04:11:57 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 15 Jun 2023 04:11:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Jun 2023 04:11:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Jun 2023 04:11:58 GMT
WORKDIR /var/www/html
# Thu, 15 Jun 2023 04:11:58 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 15 Jun 2023 04:11:58 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 04:11:58 GMT
EXPOSE 9000
# Thu, 15 Jun 2023 04:11:58 GMT
CMD ["php-fpm"]
# Thu, 15 Jun 2023 08:12:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 15 Jun 2023 08:12:34 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 15 Jun 2023 08:12:34 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Thu, 15 Jun 2023 08:13:08 GMT
ENV DRUPAL_VERSION=9.5.9
# Thu, 15 Jun 2023 08:13:08 GMT
WORKDIR /opt/drupal
# Thu, 15 Jun 2023 08:13:17 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 15 Jun 2023 08:13:18 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:edb6bdbacee93be93e930669f43e2e922c8594676aa342a70e2221361fd1914d`  
		Last Modified: Wed, 14 Jun 2023 20:49:35 GMT  
		Size: 3.3 MB (3261139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6675870db3e226ae39aec542092b3563b0352c3123a698108eeb8b98d51c47e`  
		Last Modified: Thu, 15 Jun 2023 04:40:00 GMT  
		Size: 1.9 MB (1890568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786e1ff66e74a63d03dac9ca2ad422f0d24773d8a7fbafb18f4a5c5f376516d0`  
		Last Modified: Thu, 15 Jun 2023 04:40:00 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3fbb55376f1fbddb9b8d7aff626e903b3d86a702ae59267b0dbc350e6d8f066`  
		Last Modified: Thu, 15 Jun 2023 04:40:00 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3772329fbfeeeb7d795c3077501e93f2f86017dd62470fa09686508c6a408cac`  
		Last Modified: Thu, 15 Jun 2023 04:43:55 GMT  
		Size: 11.8 MB (11813669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5944a81ee31ede01e59aebbd1d8dbc0befebca08aeeb9769fb8895dd26749439`  
		Last Modified: Thu, 15 Jun 2023 04:43:53 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88c8b89e8ca180e90b63a51217e80af2fb2fb216ca8af3e30fe036116631447e`  
		Last Modified: Thu, 15 Jun 2023 04:44:08 GMT  
		Size: 12.5 MB (12475887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cce9d06c20fc9e91e904b2a06fc42e8ea80da7c61cf22ece483ca559279ec820`  
		Last Modified: Thu, 15 Jun 2023 04:44:07 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09f7a0268d00293ae989beb63c816e53c7e26d847f6f624365b7ab43782f8621`  
		Last Modified: Thu, 15 Jun 2023 04:44:07 GMT  
		Size: 18.8 KB (18764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39589febf6ef10fc63f1335092d01d9a636a7a0b0ee17eb3931ede42af69eaea`  
		Last Modified: Thu, 15 Jun 2023 04:44:07 GMT  
		Size: 8.9 KB (8878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24438eda803e396b5874ab7cb612448d0e16e3fd13d4027e098638a2569eb79f`  
		Last Modified: Thu, 15 Jun 2023 08:19:12 GMT  
		Size: 2.4 MB (2442196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3da242e04101a01b2f280b076e08c6d9cedb7bf060964f63d9ca508a10af05e`  
		Last Modified: Thu, 15 Jun 2023 08:19:11 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f1cc82a4bbd4af984cf221c1356fd129da23971c4734f732b2f999aa90b1b1`  
		Last Modified: Thu, 15 Jun 2023 08:19:11 GMT  
		Size: 698.2 KB (698238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:632195315e46ee93ad2a4915dca5708b52a2ab7a779a6dda769297f6b94c3115`  
		Last Modified: Thu, 15 Jun 2023 08:20:14 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62c9fac6a5f8012440546ee6c0830835006749506072bb19758b25879bdb95b7`  
		Last Modified: Thu, 15 Jun 2023 08:20:18 GMT  
		Size: 22.9 MB (22862682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-alpine3.17` - linux; 386

```console
$ docker pull drupal@sha256:56dae4281c3d108bfc9ecfac119ea6b1d591295d7b8896fe8934259af794cf17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55889768 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8c4049e4749aabfee324bab260138c5ca9aa003bd92a1f86307854cb515b55e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Jun 2023 22:33:26 GMT
ADD file:39180f040ebe17a01f8b9502d7b463edade8158d87fa99e47ac0b1f369e11a65 in / 
# Wed, 14 Jun 2023 22:33:26 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 06:45:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Jun 2023 06:45:40 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Jun 2023 06:45:40 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Jun 2023 06:45:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Jun 2023 06:45:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 15 Jun 2023 06:45:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 06:45:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Jun 2023 06:45:41 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Jun 2023 08:02:52 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 15 Jun 2023 08:02:52 GMT
ENV PHP_VERSION=8.1.20
# Thu, 15 Jun 2023 08:02:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.20.tar.xz.asc
# Thu, 15 Jun 2023 08:02:52 GMT
ENV PHP_SHA256=4c9973f599e93ed5e8ce2b45ce1d41bb8fb54ce642824fd23e56b52fd75029a6
# Thu, 15 Jun 2023 08:03:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Jun 2023 08:03:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Jun 2023 08:15:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Jun 2023 08:15:20 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 15 Jun 2023 08:15:21 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Jun 2023 08:15:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Jun 2023 08:15:22 GMT
WORKDIR /var/www/html
# Thu, 15 Jun 2023 08:15:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 15 Jun 2023 08:15:22 GMT
STOPSIGNAL SIGQUIT
# Thu, 15 Jun 2023 08:15:22 GMT
EXPOSE 9000
# Thu, 15 Jun 2023 08:15:22 GMT
CMD ["php-fpm"]
# Thu, 15 Jun 2023 10:37:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 15 Jun 2023 10:37:29 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 15 Jun 2023 10:37:29 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Thu, 15 Jun 2023 10:38:12 GMT
ENV DRUPAL_VERSION=9.5.9
# Thu, 15 Jun 2023 10:38:12 GMT
WORKDIR /opt/drupal
# Thu, 15 Jun 2023 10:38:25 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 15 Jun 2023 10:38:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:187bd96dd637d3adfc7a9b61a1e7465181bbfe90dbf7a2830dfba97e4e3243a4`  
		Last Modified: Wed, 14 Jun 2023 22:34:01 GMT  
		Size: 3.4 MB (3412675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0ab42f445a14d312224d50de9656823d067b8b77d7ffbced92b4d89721b9c82`  
		Last Modified: Thu, 15 Jun 2023 09:11:01 GMT  
		Size: 2.0 MB (2009153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ef70e62fe8d901e2eab796d14bc28729e1a9dcb13a00f1d79c87c7b3c196385`  
		Last Modified: Thu, 15 Jun 2023 09:11:01 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02943f9427c9dcc994074154103fdd6add9e01d288f8f7f95f208c5d37df613c`  
		Last Modified: Thu, 15 Jun 2023 09:11:01 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e857636499c147300e6e146426a43b5bfd9bb09cc461cc1160989cbfe3da703`  
		Last Modified: Thu, 15 Jun 2023 09:15:40 GMT  
		Size: 11.8 MB (11813665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b155a608106d608cd10db39711eb5a49efee0f4a3e5be72533bceb1b41c01e`  
		Last Modified: Thu, 15 Jun 2023 09:15:38 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d28b77f532f91d304d683eb73c45f613cb6621d2e893ea6a027db72be1591b1`  
		Last Modified: Thu, 15 Jun 2023 09:15:58 GMT  
		Size: 12.8 MB (12776767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeceabb1bb142e6b19e1208225602523547427c2a95abd8d0ec148142966b4ee`  
		Last Modified: Thu, 15 Jun 2023 09:15:55 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7286ff57f2c332080f11b1945514408d64f7986a3bcf80b6d581a2fc7c48272`  
		Last Modified: Thu, 15 Jun 2023 09:15:55 GMT  
		Size: 19.0 KB (18957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32968ebb9389b5c8fadf0b1fbde3e62a7348558fff22e0754292b360f95660c3`  
		Last Modified: Thu, 15 Jun 2023 09:15:55 GMT  
		Size: 8.9 KB (8878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5662e47928c9f295fb220460c09959e5d669431ebacd6174db47c4ecf4f9c09`  
		Last Modified: Thu, 15 Jun 2023 10:45:48 GMT  
		Size: 2.3 MB (2283736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8636c00435a812ba97149685fc9c95ae43147da8f8af146317babc4674ebf48b`  
		Last Modified: Thu, 15 Jun 2023 10:45:47 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33254293468267ace84ae0bceb2f6f21d2e8b223df7a3d4b11b541cc603e7766`  
		Last Modified: Thu, 15 Jun 2023 10:45:48 GMT  
		Size: 698.2 KB (698239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa46bfeabea6ad7a0bb28b451b7fc0a5ec6dc94c1ddd547567524972c5063e9f`  
		Last Modified: Thu, 15 Jun 2023 10:47:06 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa179e05c5dc27d3b19e5432e7faaad754120aca22148d35cac882aee2a33a36`  
		Last Modified: Thu, 15 Jun 2023 10:47:14 GMT  
		Size: 22.9 MB (22862762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-alpine3.17` - linux; ppc64le

```console
$ docker pull drupal@sha256:e3e45cc37b96c2aa0fb87391aafc56fe010fa7b7f9e99a035680bbcb24850c65
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58354809 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc369ae6b2ddd698a6e7fd7f67fc8d4eacf2900deefa2fd433db9a4ecacdfc9a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 29 Mar 2023 18:16:27 GMT
ADD file:e95c1f256ba4bda85c5cbc0d8e84e6f329aa17c9dd2715b2da043e2139049124 in / 
# Wed, 29 Mar 2023 18:16:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:36:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 29 Mar 2023 22:36:32 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 29 Mar 2023 22:36:33 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 29 Mar 2023 22:36:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 29 Mar 2023 22:36:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 29 Mar 2023 22:36:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 29 Mar 2023 22:36:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 29 Mar 2023 22:36:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 29 Mar 2023 23:07:42 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 09 Jun 2023 01:16:58 GMT
ENV PHP_VERSION=8.1.20
# Fri, 09 Jun 2023 01:16:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.20.tar.xz.asc
# Fri, 09 Jun 2023 01:16:58 GMT
ENV PHP_SHA256=4c9973f599e93ed5e8ce2b45ce1d41bb8fb54ce642824fd23e56b52fd75029a6
# Fri, 09 Jun 2023 01:17:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 09 Jun 2023 01:17:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 09 Jun 2023 01:24:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 09 Jun 2023 01:24:58 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 09 Jun 2023 01:25:00 GMT
RUN docker-php-ext-enable sodium
# Fri, 09 Jun 2023 01:25:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 09 Jun 2023 01:25:00 GMT
WORKDIR /var/www/html
# Fri, 09 Jun 2023 01:25:01 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 09 Jun 2023 01:25:01 GMT
STOPSIGNAL SIGQUIT
# Fri, 09 Jun 2023 01:25:01 GMT
EXPOSE 9000
# Fri, 09 Jun 2023 01:25:02 GMT
CMD ["php-fpm"]
# Fri, 09 Jun 2023 03:04:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 09 Jun 2023 03:04:16 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 12 Jun 2023 19:37:43 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Mon, 12 Jun 2023 19:40:17 GMT
ENV DRUPAL_VERSION=9.5.9
# Mon, 12 Jun 2023 19:40:18 GMT
WORKDIR /opt/drupal
# Mon, 12 Jun 2023 19:40:42 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 12 Jun 2023 19:40:47 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:1b7d25764eb3d3c55d73f5dfb9e3e9d75f3f39132e1b16142319de2a062dd673`  
		Last Modified: Wed, 29 Mar 2023 18:17:14 GMT  
		Size: 3.4 MB (3390935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdac02b375fa12e4f7e544161fe642829107cb793b902ce9767a6fd39b686cc4`  
		Last Modified: Wed, 29 Mar 2023 23:54:26 GMT  
		Size: 2.0 MB (1957752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:678a0f24012397aebcdbcea1e47fc787669721aa4dcc86d8a479a3dfaaf65bc5`  
		Last Modified: Wed, 29 Mar 2023 23:54:25 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:120694ccc44924cba22112225821e706b18ee4ef54190ecb4f21d5a8b6262ec4`  
		Last Modified: Wed, 29 Mar 2023 23:54:25 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c125b61903038afeadf6d982a9f3927546ede32121d8dfdaa3f36dbbf5b45a24`  
		Last Modified: Fri, 09 Jun 2023 02:32:17 GMT  
		Size: 11.8 MB (11813655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce8b7d35fe79733e0274d651bd833a16d4bfbae8a4ec222dd854601a5bf4881e`  
		Last Modified: Fri, 09 Jun 2023 02:32:16 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b5cc7d26e5bb19d87c1954259d16e3f46fee892d6b581b951e56190c7ce9478`  
		Last Modified: Fri, 09 Jun 2023 02:32:43 GMT  
		Size: 15.7 MB (15674784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c4a6bb5cfc6902a6ff15ba2b8a34a79d31ee9136130399a2742c8b30f5e638c`  
		Last Modified: Fri, 09 Jun 2023 02:32:38 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a0e5d0f6a894dcd3140170f82dbd0818eed4c31184317659ff9aa93d3752e2`  
		Last Modified: Fri, 09 Jun 2023 02:32:38 GMT  
		Size: 18.9 KB (18889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f963751773b2fe9ad4103da9f26059d6c8e3e0175834b8e27d191342b2d20ffe`  
		Last Modified: Fri, 09 Jun 2023 02:32:38 GMT  
		Size: 8.9 KB (8880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcefb02ec1283f9054901f1996523730141ac651a1003aaeb71d011dfbb5e7df`  
		Last Modified: Fri, 09 Jun 2023 03:25:17 GMT  
		Size: 1.9 MB (1923498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17e4826b458f2f74bfce0c3b42715de720d7afe5be9a53e30d41679211bbd248`  
		Last Modified: Fri, 09 Jun 2023 03:25:16 GMT  
		Size: 314.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49c7a793208f26cdc57ddc16d5ef0a226d58595a58dc2204644fbb5a050ea1e9`  
		Last Modified: Mon, 12 Jun 2023 19:56:11 GMT  
		Size: 698.2 KB (698241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:299aedbb134a6049ba6750bdab00dd6378b5228d6c4b610b86cb3a824d5cd3a3`  
		Last Modified: Mon, 12 Jun 2023 20:00:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b8556793dc73c7e1ba80cb989c5799dda25a87b0e5d219bb1f01b9241c9853`  
		Last Modified: Mon, 12 Jun 2023 20:00:47 GMT  
		Size: 22.9 MB (22863234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-fpm-alpine3.17` - linux; s390x

```console
$ docker pull drupal@sha256:910be3263c7bb0c7cb3786bd97a99daf0be154d27923b96f2109bf476817192f
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.6 MB (56553851 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:77bb83b67fdc307d866a66b8fba9ae2d45c7b595e3e23847d875a30ed6c4cf07`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 29 Mar 2023 17:41:57 GMT
ADD file:675ad8acf4b076e34aeeba26dd482be7640df5912b1ec5e3183b7eb69c01e83e in / 
# Wed, 29 Mar 2023 17:41:57 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:02:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 29 Mar 2023 19:03:01 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 29 Mar 2023 19:03:01 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 29 Mar 2023 19:03:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 29 Mar 2023 19:03:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 29 Mar 2023 19:03:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 29 Mar 2023 19:03:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 29 Mar 2023 19:03:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 29 Mar 2023 19:23:01 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 09 Jun 2023 00:55:39 GMT
ENV PHP_VERSION=8.1.20
# Fri, 09 Jun 2023 00:55:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.20.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.20.tar.xz.asc
# Fri, 09 Jun 2023 00:55:39 GMT
ENV PHP_SHA256=4c9973f599e93ed5e8ce2b45ce1d41bb8fb54ce642824fd23e56b52fd75029a6
# Fri, 09 Jun 2023 00:55:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 09 Jun 2023 00:55:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 09 Jun 2023 01:01:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 09 Jun 2023 01:01:04 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 09 Jun 2023 01:01:05 GMT
RUN docker-php-ext-enable sodium
# Fri, 09 Jun 2023 01:01:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 09 Jun 2023 01:01:05 GMT
WORKDIR /var/www/html
# Fri, 09 Jun 2023 01:01:06 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 09 Jun 2023 01:01:06 GMT
STOPSIGNAL SIGQUIT
# Fri, 09 Jun 2023 01:01:06 GMT
EXPOSE 9000
# Fri, 09 Jun 2023 01:01:06 GMT
CMD ["php-fpm"]
# Fri, 09 Jun 2023 02:05:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 09 Jun 2023 02:05:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 12 Jun 2023 20:00:49 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Mon, 12 Jun 2023 20:02:11 GMT
ENV DRUPAL_VERSION=9.5.9
# Mon, 12 Jun 2023 20:02:11 GMT
WORKDIR /opt/drupal
# Mon, 12 Jun 2023 20:02:22 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 12 Jun 2023 20:02:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:a76f78d8854217635d8049ec8501edb806f961e72989cfff8503982e6ff2579d`  
		Last Modified: Wed, 29 Mar 2023 17:42:31 GMT  
		Size: 3.2 MB (3175187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6521aff379460e3b23538794f9f58987d8c205d856adb8b1906678f475549d`  
		Last Modified: Wed, 29 Mar 2023 19:53:09 GMT  
		Size: 1.9 MB (1926778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09ccc0e3e0585970bf7f018f1b481c5bda3c11ade58ae10a67fac7eb146920ec`  
		Last Modified: Wed, 29 Mar 2023 19:53:09 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffa02384e22bdeff50d42395895a9ce2b39494195bc42784c30061aa4ea5384`  
		Last Modified: Wed, 29 Mar 2023 19:53:09 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3402ace89152441ac7d199f7d3cee24a56ade6b9641e7297fe5c3f4682a6ab`  
		Last Modified: Fri, 09 Jun 2023 01:39:41 GMT  
		Size: 11.8 MB (11813657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ae5448bad198f00d9d8b1ddb45e958fd3dd8fc74d1030d2dd5b0ee18c10618`  
		Last Modified: Fri, 09 Jun 2023 01:39:40 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfab716aac91c3a4754aef0092dc326bbf772dce6ee2c2749afad1f20b39d99b`  
		Last Modified: Fri, 09 Jun 2023 01:39:53 GMT  
		Size: 14.2 MB (14242110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2caf1cb2284e2279dea5071b1c5e753c1167c7764c11ab5c261d9e1e0501c015`  
		Last Modified: Fri, 09 Jun 2023 01:39:51 GMT  
		Size: 2.4 KB (2445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2717a47340667abb71735e4882881ebdf56cfdb3452400cfa2339ee6eace2ea1`  
		Last Modified: Fri, 09 Jun 2023 01:39:51 GMT  
		Size: 18.9 KB (18895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56de5280ccea55333ff2628a4fe13eaf5bd8e132003dd6e48b7885045f35b1c`  
		Last Modified: Fri, 09 Jun 2023 01:39:52 GMT  
		Size: 8.9 KB (8876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5dce2c105ab08c5a5cb1ad8aa86bb8b16c9e32cb670c21ab3d9df79198d422a`  
		Last Modified: Fri, 09 Jun 2023 02:16:56 GMT  
		Size: 1.8 MB (1802569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf3b43da45248eda8dabbc4e4631404e606cc496f94366e48e579496da2b766d`  
		Last Modified: Fri, 09 Jun 2023 02:16:56 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545811056b0a6706d88ff11f7835ebd37259306c34e71e0b9c9b43cc8bbfd2b7`  
		Last Modified: Mon, 12 Jun 2023 20:10:51 GMT  
		Size: 698.2 KB (698241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3eee282528dd1a310f929247b1fc92d05b1f6ec2b0303f1f1606aa09acd781b`  
		Last Modified: Mon, 12 Jun 2023 20:12:11 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f98902f25f853a70e5f2d1da4fcd64fdaa409572b14c2319ce10d256aa9dc90`  
		Last Modified: Mon, 12 Jun 2023 20:12:15 GMT  
		Size: 22.9 MB (22862603 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
