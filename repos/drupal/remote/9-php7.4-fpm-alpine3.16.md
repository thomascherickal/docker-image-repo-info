## `drupal:9-php7.4-fpm-alpine3.16`

```console
$ docker pull drupal@sha256:9b1a5569b603d934e4ab198a3d584a010a540b8cc309ac6e6d078b332770d7d4
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

### `drupal:9-php7.4-fpm-alpine3.16` - linux; amd64

```console
$ docker pull drupal@sha256:2f11991eac9a9c5a744775c372bbe3b0e831374a8a5db83d9ce15a75b2f31044
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.0 MB (51039248 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5fd48cae314156041dbf523b16d430e5995e5e57affc027936ec6d5b6363427`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:21:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 06 Oct 2022 23:21:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 06 Oct 2022 23:21:52 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 06 Oct 2022 23:21:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 06 Oct 2022 23:21:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 06 Oct 2022 23:21:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 06 Oct 2022 23:21:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 06 Oct 2022 23:21:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 07 Oct 2022 00:34:50 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 07 Oct 2022 00:34:51 GMT
ENV PHP_VERSION=7.4.32
# Fri, 07 Oct 2022 00:34:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Fri, 07 Oct 2022 00:34:51 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Fri, 07 Oct 2022 00:34:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 07 Oct 2022 00:34:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 07 Oct 2022 00:42:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 07 Oct 2022 00:42:12 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 07 Oct 2022 00:42:13 GMT
RUN docker-php-ext-enable sodium
# Fri, 07 Oct 2022 00:42:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 07 Oct 2022 00:42:13 GMT
WORKDIR /var/www/html
# Fri, 07 Oct 2022 00:42:13 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 07 Oct 2022 00:42:14 GMT
STOPSIGNAL SIGQUIT
# Fri, 07 Oct 2022 00:42:14 GMT
EXPOSE 9000
# Fri, 07 Oct 2022 00:42:14 GMT
CMD ["php-fpm"]
# Fri, 07 Oct 2022 07:00:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 07:00:57 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 17 Oct 2022 20:47:47 GMT
COPY file:885ab970f10508225fd61630bb5f5deca9a4c5f5efa71af5b20e1efa22fecb2c in /usr/local/bin/ 
# Mon, 17 Oct 2022 20:47:47 GMT
ENV DRUPAL_VERSION=9.4.8
# Mon, 17 Oct 2022 20:47:47 GMT
WORKDIR /opt/drupal
# Mon, 17 Oct 2022 20:48:00 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 17 Oct 2022 20:48:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e3d893f0c48a66489b58937fa04412ed69f5d5fac3caf0cfad1fbfcf1d76f1a`  
		Last Modified: Fri, 07 Oct 2022 01:00:52 GMT  
		Size: 1.7 MB (1721106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e145bee0134d72cb2154c552a09f6ad3aff2f689dbc21569a41a22fa106707f`  
		Last Modified: Fri, 07 Oct 2022 01:00:52 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b06443bf3c2fd550395a4f14db54c869b35981ee29ab7da6bdab3816b1f3c8b`  
		Last Modified: Fri, 07 Oct 2022 01:00:52 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b7efc692d42dead324b12ce34e0f64fccadcafa5452948705615cfdda9218d`  
		Last Modified: Fri, 07 Oct 2022 01:08:16 GMT  
		Size: 10.4 MB (10439218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af5daa387348b1c4cdfb105127b72ba31a7a7b3966181c67c1252fec4dde6ee0`  
		Last Modified: Fri, 07 Oct 2022 01:08:15 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666f57addfdedb581772e84e3790c24d37961e53c84547f3806a16e2476903fa`  
		Last Modified: Fri, 07 Oct 2022 01:08:57 GMT  
		Size: 11.5 MB (11456381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c165b7f9f1010e25d3213849d32743547aa30b71e448ad852933e891d546c1b7`  
		Last Modified: Fri, 07 Oct 2022 01:08:55 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7af4fb7ae1e5d539407b05307ac0b11a9f9b6b30399ff428f0881bc4fd440bad`  
		Last Modified: Fri, 07 Oct 2022 01:08:55 GMT  
		Size: 18.6 KB (18624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b2877e24a9a24fb112f128555c09d5788876c5469e9293194e8f9f38470184`  
		Last Modified: Fri, 07 Oct 2022 01:08:55 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdaaa121a148c83ccb4353fa527ca3f81bb0c9bf977b3676875ef6785debfd33`  
		Last Modified: Fri, 07 Oct 2022 07:27:12 GMT  
		Size: 2.0 MB (1991959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac671712461cb4df945266a5889d5579b3a74ec65ecc2509c7789bb34cd7637`  
		Last Modified: Fri, 07 Oct 2022 07:27:11 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b95264d92f7d899ab99867e5b28f7dfcb225749623ff86e882779b57e1ce4d8`  
		Last Modified: Mon, 17 Oct 2022 21:12:55 GMT  
		Size: 694.8 KB (694773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e2aab7f9c687e9f0797c0d5218055ad47c14f33461d9f77d55a9ae6ef5e1f6`  
		Last Modified: Mon, 17 Oct 2022 21:12:54 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34800e90cd72d1a3a37f1f9a65ee2668b0daf1ea1f4db4ddfc62c2b01e65b735`  
		Last Modified: Mon, 17 Oct 2022 21:13:00 GMT  
		Size: 21.9 MB (21897744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-fpm-alpine3.16` - linux; arm variant v6

```console
$ docker pull drupal@sha256:095b4cd0f7df1ab3bf5df68daf8468e5a52d3c4c07e2d421af1aefb2e5d23831
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.9 MB (49917168 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4b96a7868ff118c9a04af1c5eb7346308b457f9664f312acc827a28d8b16e11`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 10:52:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 07 Oct 2022 10:52:42 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 07 Oct 2022 10:52:43 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 07 Oct 2022 10:52:43 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 07 Oct 2022 10:52:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 07 Oct 2022 10:52:44 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 07 Oct 2022 10:52:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 07 Oct 2022 10:52:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 07 Oct 2022 14:25:09 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 07 Oct 2022 14:25:09 GMT
ENV PHP_VERSION=7.4.32
# Fri, 07 Oct 2022 14:25:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Fri, 07 Oct 2022 14:25:09 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Fri, 07 Oct 2022 14:25:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 07 Oct 2022 14:25:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 07 Oct 2022 14:50:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 07 Oct 2022 14:50:28 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 07 Oct 2022 14:50:29 GMT
RUN docker-php-ext-enable sodium
# Fri, 07 Oct 2022 14:50:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 07 Oct 2022 14:50:29 GMT
WORKDIR /var/www/html
# Fri, 07 Oct 2022 14:50:30 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 07 Oct 2022 14:50:30 GMT
STOPSIGNAL SIGQUIT
# Fri, 07 Oct 2022 14:50:30 GMT
EXPOSE 9000
# Fri, 07 Oct 2022 14:50:30 GMT
CMD ["php-fpm"]
# Sat, 08 Oct 2022 04:54:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 08 Oct 2022 04:54:10 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 17 Oct 2022 20:09:10 GMT
COPY file:885ab970f10508225fd61630bb5f5deca9a4c5f5efa71af5b20e1efa22fecb2c in /usr/local/bin/ 
# Mon, 17 Oct 2022 20:09:10 GMT
ENV DRUPAL_VERSION=9.4.8
# Mon, 17 Oct 2022 20:09:10 GMT
WORKDIR /opt/drupal
# Mon, 17 Oct 2022 20:09:24 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 17 Oct 2022 20:09:25 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d191c17da875daaa84306d059e38a7cd955acc38f3161b54eb8cf82490ecdc7d`  
		Last Modified: Fri, 07 Oct 2022 15:44:25 GMT  
		Size: 1.7 MB (1708053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48519d7ac42ec4f1527826be3e3fb6c8046a417fa4068666aa8ecda7dd491803`  
		Last Modified: Fri, 07 Oct 2022 15:44:24 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c07557f41d067618e790ecd8d83d6ee9875b6a13ffa1c8c237a5144429ee98e`  
		Last Modified: Fri, 07 Oct 2022 15:44:24 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0cd5e0d7ce485c8cefc0432e03f2189f2e18956be0107171f46cb9e93a9c7dc`  
		Last Modified: Fri, 07 Oct 2022 15:53:12 GMT  
		Size: 10.4 MB (10439217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:282b408e735c89477e0a7ce1da1d0011ee06e483b4bbbb1ebdefe26f114bf68e`  
		Last Modified: Fri, 07 Oct 2022 15:53:09 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:650df8c5168cebee658538d3c5e9fb7adca1068abed72681693098e2fab155a2`  
		Last Modified: Fri, 07 Oct 2022 15:54:09 GMT  
		Size: 10.7 MB (10723009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9dfc04ba6683dd5fcdf93fecdb9d47ed3c95c1889e34261677fdb277b7dcc95`  
		Last Modified: Fri, 07 Oct 2022 15:54:06 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6594e03d910696836b4d5abe5162027791b37e1da9f8b4c2259d14d4857ee122`  
		Last Modified: Fri, 07 Oct 2022 15:54:06 GMT  
		Size: 18.6 KB (18631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3bba64db06b6161e889111c9a87bfdb34366e41815681f6c4d4a1d8dc6e458`  
		Last Modified: Fri, 07 Oct 2022 15:54:06 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b9761f08c0ea4371f9f3025627302483c99c13fc5029dc04f64073199c5c88`  
		Last Modified: Sat, 08 Oct 2022 05:08:44 GMT  
		Size: 1.8 MB (1808416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb01789fb0f7b7c3e5980e609f187ca1bc00ae372aac2f12cbcf4348c765ec4c`  
		Last Modified: Sat, 08 Oct 2022 05:08:44 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f72dcda3a2f4f29d99e51f15432ee39327d060e182d6f5a1f523e1391ab1aef`  
		Last Modified: Mon, 17 Oct 2022 20:22:04 GMT  
		Size: 694.8 KB (694772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0f2564acd23e0da4a9289705cee275cb3715220776f36f83ea26560ea8de244`  
		Last Modified: Mon, 17 Oct 2022 20:22:03 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e134f181136075d7a35b9965c809683e48801e28aa943df82e1500db973c52a4`  
		Last Modified: Mon, 17 Oct 2022 20:22:19 GMT  
		Size: 21.9 MB (21897711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-fpm-alpine3.16` - linux; arm variant v7

```console
$ docker pull drupal@sha256:47293b347b33cdebc204831390c86099e1a284e9442507a1951e771aaf09ddcc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (49016458 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef104643d089514e590ad9a248fd59e46d6d1b8a4f8850f77da6737bbcecb0ca`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 14:13:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 10 Aug 2022 14:13:14 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 10 Aug 2022 14:13:15 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 10 Aug 2022 14:13:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 10 Aug 2022 14:13:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 10 Aug 2022 14:13:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 14:13:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 14:13:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 10 Aug 2022 17:55:24 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Sep 2022 16:20:20 GMT
ENV PHP_VERSION=7.4.32
# Thu, 29 Sep 2022 16:20:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Thu, 29 Sep 2022 16:20:20 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Thu, 29 Sep 2022 16:20:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Sep 2022 16:20:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Sep 2022 16:51:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Sep 2022 16:51:01 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 29 Sep 2022 16:51:02 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Sep 2022 16:51:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Sep 2022 16:51:02 GMT
WORKDIR /var/www/html
# Thu, 29 Sep 2022 16:51:03 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Sep 2022 16:51:03 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Sep 2022 16:51:03 GMT
EXPOSE 9000
# Thu, 29 Sep 2022 16:51:03 GMT
CMD ["php-fpm"]
# Sat, 08 Oct 2022 06:36:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 08 Oct 2022 06:36:56 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 17 Oct 2022 20:28:31 GMT
COPY file:885ab970f10508225fd61630bb5f5deca9a4c5f5efa71af5b20e1efa22fecb2c in /usr/local/bin/ 
# Mon, 17 Oct 2022 20:28:31 GMT
ENV DRUPAL_VERSION=9.4.8
# Mon, 17 Oct 2022 20:28:31 GMT
WORKDIR /opt/drupal
# Mon, 17 Oct 2022 20:28:49 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 17 Oct 2022 20:28:50 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533661cc695e850f2ce9a61f8d6bcabf20631bc4be493498e7c06a85445a834d`  
		Last Modified: Wed, 10 Aug 2022 19:17:39 GMT  
		Size: 1.6 MB (1575470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ea8309925b47b4d8ed5708b410d6856267d8d8dea3544802ae2a6d8e16e2a5`  
		Last Modified: Wed, 10 Aug 2022 19:17:38 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a23ce236c2c67c8bab1a6d9e5111a49299c4b7a07b9914b84c845eb1ff3c3ab`  
		Last Modified: Wed, 10 Aug 2022 19:17:38 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b82260a504b8353f33bdc9d71d1a2c6b246a7bab654c9c0f830652fd6483de`  
		Last Modified: Thu, 29 Sep 2022 18:10:09 GMT  
		Size: 10.4 MB (10439210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd8714581859c2a0e7acdc7500ffd8d03286fab296f95d8a3456deaa47c5fe68`  
		Last Modified: Thu, 29 Sep 2022 18:10:08 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a9b90356672a37ea2237ce6702dba8159fb63a9d2b404b585d0e5dadc170fdf`  
		Last Modified: Thu, 29 Sep 2022 18:10:59 GMT  
		Size: 10.3 MB (10306804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f144fd695c5a3a8569e9f2758e92039d647ec05498b40bc52fc2db3e64f1a7f`  
		Last Modified: Thu, 29 Sep 2022 18:10:57 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aedfb8328ff577d54e6a8976db624fb74c0bfb1c6aee91ddabfceab3e813cf65`  
		Last Modified: Thu, 29 Sep 2022 18:10:57 GMT  
		Size: 18.7 KB (18654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f00ec3db54254fcb259a2833078c3a9b4e9016b38b4f5fc4cc51dd7ef2437932`  
		Last Modified: Thu, 29 Sep 2022 18:10:57 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96fe9a54b0dda1cb730cf0c07e6c4377818c247a5bb89df49421eaf054ba25d7`  
		Last Modified: Sat, 08 Oct 2022 07:24:29 GMT  
		Size: 1.7 MB (1653418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3696108505606c097cc447c71eae29d2c88e4ce8db0ba7c3366d56813d5dc4c4`  
		Last Modified: Sat, 08 Oct 2022 07:24:28 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366bf8ba6a85ab0250b15717f7c483196107acf878867682f3808b41133d3c01`  
		Last Modified: Mon, 17 Oct 2022 21:12:36 GMT  
		Size: 694.8 KB (694773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a416ab6d38f0d6052aac6151f6b06996c96174f734b3280f514bb00ab8a012ad`  
		Last Modified: Mon, 17 Oct 2022 21:12:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f6516ac2fee2c960382acd1371563641e7ddb08cad4eb8139d845baeac9344`  
		Last Modified: Mon, 17 Oct 2022 21:12:51 GMT  
		Size: 21.9 MB (21897669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-fpm-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:dd8c0769c2c73ea11badbfac21ee31246f993e43df57ad27ed77098918861739
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50711510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f3f0f75f7141994d0990b626a09bf3752f28f233542f598b04db374a7e9fdb0`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Tue, 25 Oct 2022 16:24:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 25 Oct 2022 16:24:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 25 Oct 2022 16:24:55 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 25 Oct 2022 16:24:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 25 Oct 2022 16:24:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 25 Oct 2022 16:24:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 25 Oct 2022 16:24:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 25 Oct 2022 16:24:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 25 Oct 2022 19:16:55 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 25 Oct 2022 19:16:55 GMT
ENV PHP_VERSION=7.4.32
# Tue, 25 Oct 2022 19:16:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Tue, 25 Oct 2022 19:16:55 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Tue, 25 Oct 2022 19:17:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 25 Oct 2022 19:17:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 25 Oct 2022 19:22:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 25 Oct 2022 19:22:23 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 25 Oct 2022 19:22:24 GMT
RUN docker-php-ext-enable sodium
# Tue, 25 Oct 2022 19:22:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 25 Oct 2022 19:22:24 GMT
WORKDIR /var/www/html
# Tue, 25 Oct 2022 19:22:24 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 25 Oct 2022 19:22:25 GMT
STOPSIGNAL SIGQUIT
# Tue, 25 Oct 2022 19:22:25 GMT
EXPOSE 9000
# Tue, 25 Oct 2022 19:22:25 GMT
CMD ["php-fpm"]
# Wed, 26 Oct 2022 12:23:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 26 Oct 2022 12:23:16 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 26 Oct 2022 12:23:16 GMT
COPY file:885ab970f10508225fd61630bb5f5deca9a4c5f5efa71af5b20e1efa22fecb2c in /usr/local/bin/ 
# Wed, 26 Oct 2022 12:23:16 GMT
ENV DRUPAL_VERSION=9.4.8
# Wed, 26 Oct 2022 12:23:16 GMT
WORKDIR /opt/drupal
# Wed, 26 Oct 2022 12:23:26 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 26 Oct 2022 12:23:27 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19c3c1a63608ee746cfd0fb1d310f407f855ea0809df0a8d336fd6e4501ceae2`  
		Last Modified: Tue, 25 Oct 2022 19:41:26 GMT  
		Size: 1.7 MB (1715562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78ebdb03735b66ed04ec81a33c9949c64b7ed3437ce31650fea31e9fc0acc293`  
		Last Modified: Tue, 25 Oct 2022 19:41:26 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:661297bd570d111eb52d0966fa7e261bea3a4eda3f9fea437202fc7fd169dee7`  
		Last Modified: Tue, 25 Oct 2022 19:41:26 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:664868964080c3c7ee3868f6fd862ae9dac393f3c15d3b511d813445f5cb7619`  
		Last Modified: Tue, 25 Oct 2022 20:01:01 GMT  
		Size: 10.4 MB (10439215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ffb7a98299cdeea38dba628512187ed7b815e35488d00836e2f27852d54afb`  
		Last Modified: Tue, 25 Oct 2022 20:01:00 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18dfa75e0306e62dfdd489f6cc09977fd7e43caf0e809015964d9687d01fe75a`  
		Last Modified: Tue, 25 Oct 2022 20:01:40 GMT  
		Size: 11.3 MB (11284539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:666852b83a2af8f8fa12dd9cb41dc12efca0ea69665511fa355bb3822b24a358`  
		Last Modified: Tue, 25 Oct 2022 20:01:38 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50ae3dc1fb5f0ad09f274c1122a3979adb05d43e9b8ebff1691d8d8cd52bb486`  
		Last Modified: Tue, 25 Oct 2022 20:01:38 GMT  
		Size: 18.6 KB (18643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f8f2d896239d47e85d282760926f21786b452da85e6b01fd988c2a5bce69c1`  
		Last Modified: Tue, 25 Oct 2022 20:01:38 GMT  
		Size: 8.4 KB (8440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba0a38d29334e990a567379d98bd14959be66f73030b17bc2b6310198b01c80`  
		Last Modified: Wed, 26 Oct 2022 12:50:33 GMT  
		Size: 1.9 MB (1940134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ec756963434fbd0f7485312a57dbeb404a15758d5b21efab6c5b2fd94531cc8`  
		Last Modified: Wed, 26 Oct 2022 12:50:32 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc4355067dd8dd3d9fee6d1d6296db4cc9ab0c7d95db1a415363387f8d609a8`  
		Last Modified: Wed, 26 Oct 2022 12:50:32 GMT  
		Size: 694.8 KB (694770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c410e07bfb072b3e1a00c7163ce5d963df532bbe4301ca7a05649dbf45b9b84f`  
		Last Modified: Wed, 26 Oct 2022 12:50:32 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053c7e4cd5bd5fdd4fbe177c25aaf8a8853a2b3a083cb18311c6b60ffb383abc`  
		Last Modified: Wed, 26 Oct 2022 12:50:36 GMT  
		Size: 21.9 MB (21897599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-fpm-alpine3.16` - linux; 386

```console
$ docker pull drupal@sha256:feb31ce85f798dccf93f144cacdbbf0a909f7024f6c6e14f37d69a61305e563f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51542859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:652b13c36d140345b7c59b5ccc355dc0f48bee7e1aaa383254957cfb2a382449`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:01:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 06 Oct 2022 21:01:28 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 06 Oct 2022 21:01:29 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 06 Oct 2022 21:01:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 06 Oct 2022 21:01:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 06 Oct 2022 21:01:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 06 Oct 2022 21:01:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 06 Oct 2022 21:01:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 06 Oct 2022 22:15:24 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 06 Oct 2022 22:15:25 GMT
ENV PHP_VERSION=7.4.32
# Thu, 06 Oct 2022 22:15:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Thu, 06 Oct 2022 22:15:27 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Thu, 06 Oct 2022 22:15:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Oct 2022 22:15:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 06 Oct 2022 22:22:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 06 Oct 2022 22:22:54 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 06 Oct 2022 22:22:54 GMT
RUN docker-php-ext-enable sodium
# Thu, 06 Oct 2022 22:22:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 06 Oct 2022 22:22:56 GMT
WORKDIR /var/www/html
# Thu, 06 Oct 2022 22:22:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 06 Oct 2022 22:22:58 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:22:59 GMT
EXPOSE 9000
# Thu, 06 Oct 2022 22:23:00 GMT
CMD ["php-fpm"]
# Fri, 07 Oct 2022 03:04:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 03:04:35 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 17 Oct 2022 20:05:59 GMT
COPY file:885ab970f10508225fd61630bb5f5deca9a4c5f5efa71af5b20e1efa22fecb2c in /usr/local/bin/ 
# Mon, 17 Oct 2022 20:05:59 GMT
ENV DRUPAL_VERSION=9.4.8
# Mon, 17 Oct 2022 20:06:00 GMT
WORKDIR /opt/drupal
# Mon, 17 Oct 2022 20:06:15 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 17 Oct 2022 20:06:16 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8429c35581dc2b06177afb14a55afbd6b92a75a15232d3596d5ef954c2b1fcdf`  
		Last Modified: Thu, 06 Oct 2022 22:46:39 GMT  
		Size: 1.8 MB (1820480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c702fb4048195b35060feca6dfae579d104b48448b0d0ddf019c60b1745fd0c`  
		Last Modified: Thu, 06 Oct 2022 22:46:42 GMT  
		Size: 1.2 KB (1235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac06596e4ff3720f72e504820e969f1ef3dcf30c54166b940d1022d7f9fdd61`  
		Last Modified: Thu, 06 Oct 2022 22:46:39 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5458c9da6e79c236eddfb18bbdb6f1359c52e1b6da799d6382051004297fb27`  
		Last Modified: Thu, 06 Oct 2022 22:55:37 GMT  
		Size: 10.4 MB (10438969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153dbefe8df979a402078b4061e23e311c95428f1a5a4559f494ff176b4098b5`  
		Last Modified: Thu, 06 Oct 2022 22:55:36 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:748ba659140e5e25d1cdc6da71c74e7471438f99583b03441dce6b2e50e902fa`  
		Last Modified: Thu, 06 Oct 2022 22:56:25 GMT  
		Size: 11.8 MB (11765154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c277a0508d62f8a0db2b2f9c6f09b699d848ca7ae18a638b378d22770a966b25`  
		Last Modified: Thu, 06 Oct 2022 22:56:23 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b371d2dbaa147a2563f8edfe1bcc2c4091dc8502c6c83aa28f1bb58fd20e2b8`  
		Last Modified: Thu, 06 Oct 2022 22:56:23 GMT  
		Size: 18.5 KB (18518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e94df3598c10a99b07d7b9a665a5dedc5854e07f20fed44076c7761d187244d`  
		Last Modified: Thu, 06 Oct 2022 22:56:23 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c5fa7365d555d9504f1047f207ff4e868ffbc6040b6edbabdcb489da8699b8`  
		Last Modified: Fri, 07 Oct 2022 03:42:07 GMT  
		Size: 2.1 MB (2085594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0eee8814a4bc72573f8cfdb5985b08fdf94f72eca95b9e0f1ac3d1120980aff`  
		Last Modified: Fri, 07 Oct 2022 03:42:06 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb93628815f7fd9cad0eee13418636661a9d55dc4f854b37a4160e1722b1b757`  
		Last Modified: Mon, 17 Oct 2022 20:42:38 GMT  
		Size: 694.8 KB (694774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d06cfa3ee711e8981da889d32f64aa4e2deec68943f05ba5c7d9d1e991e1f11`  
		Last Modified: Mon, 17 Oct 2022 20:42:37 GMT  
		Size: 114.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2612814252f3a59ded87ed81ae153ba68188b4e0af8b94a8c7352fac7cc0fc21`  
		Last Modified: Mon, 17 Oct 2022 20:42:42 GMT  
		Size: 21.9 MB (21898964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-fpm-alpine3.16` - linux; ppc64le

```console
$ docker pull drupal@sha256:a5e7d3ce3b4fe8d82f99283efd2910aa0f8c59bb9f923e70411fd985da08dbef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (51954148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:27f36fe5607001740e0fbba7ea92938c3bdf672c18a3f6a8fe3b243db95d7714`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:59:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 06 Oct 2022 23:59:49 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 06 Oct 2022 23:59:50 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 06 Oct 2022 23:59:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 06 Oct 2022 23:59:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 06 Oct 2022 23:59:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 06 Oct 2022 23:59:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 06 Oct 2022 23:59:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 07 Oct 2022 01:34:56 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 07 Oct 2022 01:34:56 GMT
ENV PHP_VERSION=7.4.32
# Fri, 07 Oct 2022 01:34:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Fri, 07 Oct 2022 01:34:57 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Fri, 07 Oct 2022 01:35:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 07 Oct 2022 01:35:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 07 Oct 2022 01:44:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 07 Oct 2022 01:44:51 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 07 Oct 2022 01:44:53 GMT
RUN docker-php-ext-enable sodium
# Fri, 07 Oct 2022 01:44:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 07 Oct 2022 01:44:54 GMT
WORKDIR /var/www/html
# Fri, 07 Oct 2022 01:44:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 07 Oct 2022 01:44:56 GMT
STOPSIGNAL SIGQUIT
# Fri, 07 Oct 2022 01:44:56 GMT
EXPOSE 9000
# Fri, 07 Oct 2022 01:44:57 GMT
CMD ["php-fpm"]
# Fri, 07 Oct 2022 08:38:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 08:39:00 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 17 Oct 2022 20:43:44 GMT
COPY file:885ab970f10508225fd61630bb5f5deca9a4c5f5efa71af5b20e1efa22fecb2c in /usr/local/bin/ 
# Mon, 17 Oct 2022 20:43:45 GMT
ENV DRUPAL_VERSION=9.4.8
# Mon, 17 Oct 2022 20:43:45 GMT
WORKDIR /opt/drupal
# Mon, 17 Oct 2022 20:44:09 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 17 Oct 2022 20:44:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca3a3b32081770d8d84a7e4ab84cdd4d01b5a6350d96ebd161d4e0612d2e4a9`  
		Last Modified: Fri, 07 Oct 2022 02:13:07 GMT  
		Size: 1.8 MB (1772297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2175d7fbb352f035d82bd9705fe1ed1816644aadaefa77a474166470fd00e42b`  
		Last Modified: Fri, 07 Oct 2022 02:13:06 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5ddaf49f63dc65bb9290753c44394973fdc7edbd724b1fbe4b8a1c440356cdb`  
		Last Modified: Fri, 07 Oct 2022 02:13:06 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902409380edaa04602248d9c49d41571378d3196cd8040bf8b27c21e81b29f31`  
		Last Modified: Fri, 07 Oct 2022 02:22:37 GMT  
		Size: 10.4 MB (10439222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd07f10b3863003712c8d2dd5ca481cb2dfbfa47a99118bb064b9dc110918a02`  
		Last Modified: Fri, 07 Oct 2022 02:22:36 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4534151d08c09decc2d3855974916f7c6c3f7655027c63e94466dc155a32874`  
		Last Modified: Fri, 07 Oct 2022 02:23:34 GMT  
		Size: 12.2 MB (12218160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3753da4da74febf8788b8a76d49a3a96a87f400afbf47b6f504a8235e5e8c12b`  
		Last Modified: Fri, 07 Oct 2022 02:23:31 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:015e138157a7ded140b725117cc3eca053e10d946744d49cb14e2b5144ce74c8`  
		Last Modified: Fri, 07 Oct 2022 02:23:31 GMT  
		Size: 18.6 KB (18623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0dc66123967f9bbc1000db8a8e2579862b594957d0a86fe3c12642f86571566`  
		Last Modified: Fri, 07 Oct 2022 02:23:31 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:929ae7ae061880f5690c35ffc11b3ba222f3fcdd5f46a3c30023dd164306de2c`  
		Last Modified: Fri, 07 Oct 2022 09:15:55 GMT  
		Size: 2.1 MB (2096587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff515d85734989036f414d96c56becb552f7d31fb9f9e0b072cff8623e7e5539`  
		Last Modified: Fri, 07 Oct 2022 09:15:54 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd266e728e78d32c15c90ed1310cfbc68f19a76522f31c6177cf234934eab914`  
		Last Modified: Mon, 17 Oct 2022 21:20:28 GMT  
		Size: 694.8 KB (694773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3793150f998e53b05463ce1ffdf9baea82a504fc2db87ffdb2fcc6d494c19c0`  
		Last Modified: Mon, 17 Oct 2022 21:20:27 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3eeccf2090789ff50f3951362eef33a9ea1fb3ef1d66fc318ac294e0022f3e`  
		Last Modified: Mon, 17 Oct 2022 21:20:49 GMT  
		Size: 21.9 MB (21897776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-fpm-alpine3.16` - linux; s390x

```console
$ docker pull drupal@sha256:9f927757510685c1266c9d2c7d25abb9050f091a541014406b2f509adf0af03e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.5 MB (50451286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3599cd6f91c977a730ab440e8fa1357a11e7b143415e18100e29e1e89ab35b80`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 01:27:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 07 Oct 2022 01:27:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 07 Oct 2022 01:27:51 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 07 Oct 2022 01:27:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 07 Oct 2022 01:27:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 07 Oct 2022 01:27:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 07 Oct 2022 01:27:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 07 Oct 2022 01:27:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 07 Oct 2022 02:54:04 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 07 Oct 2022 02:54:05 GMT
ENV PHP_VERSION=7.4.32
# Fri, 07 Oct 2022 02:54:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Fri, 07 Oct 2022 02:54:05 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Fri, 07 Oct 2022 02:54:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 07 Oct 2022 02:54:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 07 Oct 2022 03:02:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 07 Oct 2022 03:02:51 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 07 Oct 2022 03:02:52 GMT
RUN docker-php-ext-enable sodium
# Fri, 07 Oct 2022 03:02:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 07 Oct 2022 03:02:53 GMT
WORKDIR /var/www/html
# Fri, 07 Oct 2022 03:02:54 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 07 Oct 2022 03:02:54 GMT
STOPSIGNAL SIGQUIT
# Fri, 07 Oct 2022 03:02:54 GMT
EXPOSE 9000
# Fri, 07 Oct 2022 03:02:55 GMT
CMD ["php-fpm"]
# Fri, 07 Oct 2022 11:07:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 11:07:38 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Mon, 17 Oct 2022 20:07:37 GMT
COPY file:885ab970f10508225fd61630bb5f5deca9a4c5f5efa71af5b20e1efa22fecb2c in /usr/local/bin/ 
# Mon, 17 Oct 2022 20:07:37 GMT
ENV DRUPAL_VERSION=9.4.8
# Mon, 17 Oct 2022 20:07:37 GMT
WORKDIR /opt/drupal
# Mon, 17 Oct 2022 20:07:51 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Mon, 17 Oct 2022 20:07:56 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793dde3b687f0aaad5df5bdf75b8def5a75f3e23c18eed049b7f33b63d1d9d4f`  
		Last Modified: Fri, 07 Oct 2022 03:27:12 GMT  
		Size: 1.8 MB (1776077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69b020cae1039f28b7553cbfface89b8dbc71291be52523b4d9a21212a9ec8b`  
		Last Modified: Fri, 07 Oct 2022 03:27:12 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6defbdf58b88d9209932f344cee98a6544b064956c7921f9a570c497be009815`  
		Last Modified: Fri, 07 Oct 2022 03:27:12 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a705c096bde9a5125265b6913e6498ff0b0f43aa15c0f8e6b80038c0c9ce043c`  
		Last Modified: Fri, 07 Oct 2022 03:33:24 GMT  
		Size: 10.4 MB (10439230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7263598c7e158b90114d04503d2d31bb73cebaef116b499e13fb52f65f2f8788`  
		Last Modified: Fri, 07 Oct 2022 03:33:24 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378170a9c47a0b36c6ef66b3979a547022397966b2da6a0156d97635f1e0e218`  
		Last Modified: Fri, 07 Oct 2022 03:33:55 GMT  
		Size: 11.1 MB (11050739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63087733a13abe85e645f9772cfbeed1ae27a35c80fbe3419264560626231c9a`  
		Last Modified: Fri, 07 Oct 2022 03:33:54 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d3f1afdba9c7eacc878e494b08c43b5b85ea16dd94b2a1c960f5647f10fbb33`  
		Last Modified: Fri, 07 Oct 2022 03:33:54 GMT  
		Size: 18.6 KB (18639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8afab6ebd1ea2de6d6238e51849822a25f6acca7dff1979efb56f05618bbfa39`  
		Last Modified: Fri, 07 Oct 2022 03:33:54 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c602f90be5cac87f8236f256ced518fadcc2909c1d0c20bc3d530c6d811f1943`  
		Last Modified: Fri, 07 Oct 2022 11:37:57 GMT  
		Size: 2.0 MB (1970165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef9ce78c028ac339e25998a81147185ac7c2bc5443eb29f5cdd8a62a1020506`  
		Last Modified: Fri, 07 Oct 2022 11:37:56 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560a303070d9d207b209fd54b3fc5994d38365e87df00c91f95b7cd0e00c35e3`  
		Last Modified: Mon, 17 Oct 2022 20:31:23 GMT  
		Size: 694.8 KB (694773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1752101514b0932c7288d860dd57b268b87a97e7e405afda2a4cb4e2ec8c80f`  
		Last Modified: Mon, 17 Oct 2022 20:31:23 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca4177e9915d70029a4264a90a47de90c8756fa8e305d44cef2a6b01f6f1e3a`  
		Last Modified: Mon, 17 Oct 2022 20:31:27 GMT  
		Size: 21.9 MB (21897677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
