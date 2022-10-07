## `drupal:9-php7.4-fpm-alpine3.15`

```console
$ docker pull drupal@sha256:c25928d96e67e71f3858089e668777919f753b9f85f72655f435f02a9c9394a5
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

### `drupal:9-php7.4-fpm-alpine3.15` - linux; amd64

```console
$ docker pull drupal@sha256:5fc9a4488c5f73afd006f0353d9139c85515182fb5ee501054905f3c59b6be2e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51505455 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d7c43f40fb6caa162c5ee95293444e358c15180ef05c1e28ac4481749b783aa`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 21:32:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 09 Aug 2022 21:32:57 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 09 Aug 2022 21:32:57 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 09 Aug 2022 21:32:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Aug 2022 21:32:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Aug 2022 21:32:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 21:32:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 21:32:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Aug 2022 22:45:35 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Sep 2022 14:53:45 GMT
ENV PHP_VERSION=7.4.32
# Thu, 29 Sep 2022 14:53:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Thu, 29 Sep 2022 14:53:45 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Thu, 29 Sep 2022 14:53:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Sep 2022 14:53:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Sep 2022 15:00:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Sep 2022 15:00:41 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 29 Sep 2022 15:00:42 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Sep 2022 15:00:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Sep 2022 15:00:43 GMT
WORKDIR /var/www/html
# Thu, 29 Sep 2022 15:00:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Sep 2022 15:00:43 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Sep 2022 15:00:43 GMT
EXPOSE 9000
# Thu, 29 Sep 2022 15:00:43 GMT
CMD ["php-fpm"]
# Thu, 29 Sep 2022 16:01:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 29 Sep 2022 16:01:37 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 29 Sep 2022 16:01:37 GMT
COPY file:31957edf88ab81c875036fac642510adba17e7f664ade12ad4cc270b8b01a7d0 in /usr/local/bin/ 
# Thu, 29 Sep 2022 20:01:59 GMT
ENV DRUPAL_VERSION=9.4.7
# Thu, 29 Sep 2022 20:01:59 GMT
WORKDIR /opt/drupal
# Thu, 29 Sep 2022 20:02:13 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 29 Sep 2022 20:02:14 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797cd885d77976aede5fcea7a54982e7ce7ae729f160ec02fcb520966fb9f082`  
		Last Modified: Tue, 09 Aug 2022 23:01:36 GMT  
		Size: 1.7 MB (1714235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28678576693ffd0509bd7c77d71c271fa2905fd08d7ffa84bc961d26857bb1e0`  
		Last Modified: Tue, 09 Aug 2022 23:01:35 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:410b9a6b1c40098ac9b2d8c619933060123f1451a0a4774d2fc8f96061da3907`  
		Last Modified: Tue, 09 Aug 2022 23:01:35 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4237e82d2055b7f43c88a53739eceaca89a20f0751d9a73714fa6249fb20798e`  
		Last Modified: Thu, 29 Sep 2022 15:17:03 GMT  
		Size: 10.4 MB (10439246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24518bca5a39956d9e458a5b559b187d214b38db20e6ece3bb838992f8ca7498`  
		Last Modified: Thu, 29 Sep 2022 15:17:02 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da4d33c8b0ea04cd515283a9176ab788f28826cac7edf9b42d6327c6c19cd59`  
		Last Modified: Thu, 29 Sep 2022 15:17:27 GMT  
		Size: 11.7 MB (11681167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa73227ba2aa5ce2366a68b3e3ca8a38312717efe12d5bd026efb0f11db0649`  
		Last Modified: Thu, 29 Sep 2022 15:17:25 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8e22fb5b64bc5af8e2261ba21a881261cede4534ecc6ca8159b622e9efb1df`  
		Last Modified: Thu, 29 Sep 2022 15:17:26 GMT  
		Size: 18.7 KB (18720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3a46b2203833482235741c526c486b0c0504cdd5dfd3843275703a49f2d4a9b`  
		Last Modified: Thu, 29 Sep 2022 15:17:25 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1784115d0d91a3c5918c730ee7f196b37ec4e06fec797bbfa6d6b6f7335f173`  
		Last Modified: Thu, 29 Sep 2022 16:13:42 GMT  
		Size: 2.2 MB (2241738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb036f5d23e45d2c5143ae537f8d5502ed4b5aa62906ec80e8301abd526a7b0`  
		Last Modified: Thu, 29 Sep 2022 16:13:41 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f0cd9c74de4526195116b798b319aea774033b9e43300640da23a4717552b2d`  
		Last Modified: Thu, 29 Sep 2022 16:13:41 GMT  
		Size: 692.6 KB (692570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:623931bcac11ebd0bca4a0ce610cdd78fba7c30146f65e90bc44a8a7b5ae9f8d`  
		Last Modified: Thu, 29 Sep 2022 20:27:25 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b02dc1ff5f51ef52c23e0b31eb3c161c3f00dfcb45a402a78ef3f8eef5a52e7`  
		Last Modified: Thu, 29 Sep 2022 20:27:30 GMT  
		Size: 21.9 MB (21880877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-fpm-alpine3.15` - linux; arm variant v6

```console
$ docker pull drupal@sha256:4f324f26c8b6fdc5172cdd0ed0f7095b2cb548398748c32c50a2669180d16891
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.3 MB (50345441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92808086e6ab72247abc09bf11cb0264728a7ef809989fcc6a5cdd47f9372b54`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:29 GMT
ADD file:89cb25f97e17bed5c56311280efe5cfa78422d8ffbe36232195d13f94d67417e in / 
# Tue, 09 Aug 2022 17:49:29 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 11:58:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 10 Aug 2022 11:58:59 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 10 Aug 2022 11:58:59 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 10 Aug 2022 11:59:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 10 Aug 2022 11:59:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 10 Aug 2022 11:59:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 11:59:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 11:59:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 10 Aug 2022 15:41:45 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Sep 2022 15:42:06 GMT
ENV PHP_VERSION=7.4.32
# Thu, 29 Sep 2022 15:42:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Thu, 29 Sep 2022 15:42:06 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Thu, 29 Sep 2022 15:42:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Sep 2022 15:42:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Sep 2022 16:09:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Sep 2022 16:09:38 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 29 Sep 2022 16:09:39 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Sep 2022 16:09:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Sep 2022 16:09:40 GMT
WORKDIR /var/www/html
# Thu, 29 Sep 2022 16:09:41 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Sep 2022 16:09:41 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Sep 2022 16:09:41 GMT
EXPOSE 9000
# Thu, 29 Sep 2022 16:09:41 GMT
CMD ["php-fpm"]
# Thu, 29 Sep 2022 17:42:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 29 Sep 2022 17:42:46 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 29 Sep 2022 17:42:46 GMT
COPY file:31957edf88ab81c875036fac642510adba17e7f664ade12ad4cc270b8b01a7d0 in /usr/local/bin/ 
# Thu, 29 Sep 2022 21:20:39 GMT
ENV DRUPAL_VERSION=9.4.7
# Thu, 29 Sep 2022 21:20:40 GMT
WORKDIR /opt/drupal
# Thu, 29 Sep 2022 21:21:05 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 29 Sep 2022 21:21:06 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:293b708aa6fb80967f27727d5c9c53ac9ba9cac376bed2ad02c17a5cca317b35`  
		Last Modified: Tue, 09 Aug 2022 17:50:52 GMT  
		Size: 2.6 MB (2631127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ea44f56e79ac635f0bc28f2e8ccb48e4329bf3a70a28dfc32a00235f7e87ce1`  
		Last Modified: Wed, 10 Aug 2022 16:22:21 GMT  
		Size: 1.7 MB (1703745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cb213a3741596d1489bfa19c597649b09ffbaff3be454947cb8487499987d2b`  
		Last Modified: Wed, 10 Aug 2022 16:22:20 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31a34313d0e689879aa079a162c614af2f26b6f6841bbf431f17c1afe6fcf1a1`  
		Last Modified: Wed, 10 Aug 2022 16:22:20 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6729fae70bcf4a1cbe7cb223b4b126c98abffd95789e2a0c760d2ba0afa72954`  
		Last Modified: Thu, 29 Sep 2022 16:39:16 GMT  
		Size: 10.4 MB (10439240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a602c0bc0195b17f201cb851b814ca128d4d53246310512b8914e58f1d2abf65`  
		Last Modified: Thu, 29 Sep 2022 16:39:13 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04ffe2e463041bb29e697963cf29ca6d1348465d290164b9922cb1d301497ba1`  
		Last Modified: Thu, 29 Sep 2022 16:39:52 GMT  
		Size: 11.0 MB (10950854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a65fba64b26a3f2ff3301972306723d6d788d5df317c20a0dd282d32d477bb39`  
		Last Modified: Thu, 29 Sep 2022 16:39:48 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78b6381c6fb0520389c015ef4d0e922003e624a39d44d12a819dad7baf8a1181`  
		Last Modified: Thu, 29 Sep 2022 16:39:48 GMT  
		Size: 18.7 KB (18719 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50da439a70502a073bd04c27dd76dda8e6a4f9c545205c6831e8a920202e8cc3`  
		Last Modified: Thu, 29 Sep 2022 16:39:48 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f77a776b8e1f3d33060bac8c5a81f3f7bec138340c3a3b896e3c331342bda1`  
		Last Modified: Thu, 29 Sep 2022 17:52:00 GMT  
		Size: 2.0 MB (2014428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3188aa7fe0e817ff73a29462e95ada3910cbba86939f4be04328f634a1ad7d37`  
		Last Modified: Thu, 29 Sep 2022 17:51:59 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10b0169e9c8dd55bccb8591bf3ed6c3f6b6392bb14c987879b0b3c4fdbffccfb`  
		Last Modified: Thu, 29 Sep 2022 17:52:00 GMT  
		Size: 692.6 KB (692577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:013cdd077e6a7bc63e0adf2c1da00420ad4d302bfb3fd96a847aa3d3cfab639e`  
		Last Modified: Thu, 29 Sep 2022 21:35:37 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e688ef9e35ca0057ee63868bb09c8fa1674304e00b2af1bb4eeb1cef6deaeb9f`  
		Last Modified: Thu, 29 Sep 2022 21:35:52 GMT  
		Size: 21.9 MB (21881358 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-fpm-alpine3.15` - linux; arm variant v7

```console
$ docker pull drupal@sha256:7597436b95294e0e60fe298ba737f6506200bc52330efa50515ed65c83db3937
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49191116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:15b90ffc605d170291b166d532a0843a91ab5991c84752578b484ab16f70760f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:52 GMT
ADD file:0bd18306f21937a9572e68c768f05f4a9d8341b40c2379a7bfcb857c77734a14 in / 
# Tue, 09 Aug 2022 16:57:52 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 14:53:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 10 Aug 2022 14:53:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 10 Aug 2022 14:53:58 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 10 Aug 2022 14:53:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 10 Aug 2022 14:53:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 10 Aug 2022 14:53:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 14:53:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 14:53:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 10 Aug 2022 18:31:43 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Sep 2022 17:05:07 GMT
ENV PHP_VERSION=7.4.32
# Thu, 29 Sep 2022 17:05:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Thu, 29 Sep 2022 17:05:07 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Thu, 29 Sep 2022 17:05:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Sep 2022 17:05:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Sep 2022 17:32:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Sep 2022 17:32:35 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 29 Sep 2022 17:32:36 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Sep 2022 17:32:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Sep 2022 17:32:37 GMT
WORKDIR /var/www/html
# Thu, 29 Sep 2022 17:32:37 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Sep 2022 17:32:37 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Sep 2022 17:32:37 GMT
EXPOSE 9000
# Thu, 29 Sep 2022 17:32:38 GMT
CMD ["php-fpm"]
# Thu, 29 Sep 2022 22:04:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 29 Sep 2022 22:04:47 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 29 Sep 2022 22:04:47 GMT
COPY file:31957edf88ab81c875036fac642510adba17e7f664ade12ad4cc270b8b01a7d0 in /usr/local/bin/ 
# Thu, 29 Sep 2022 22:04:47 GMT
ENV DRUPAL_VERSION=9.4.7
# Thu, 29 Sep 2022 22:04:47 GMT
WORKDIR /opt/drupal
# Thu, 29 Sep 2022 22:05:06 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 29 Sep 2022 22:05:07 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:59775c20a906b1a49edcdc41a700a795998979d6ecf8f8d9cd7cbdf45e686d81`  
		Last Modified: Tue, 09 Aug 2022 16:59:12 GMT  
		Size: 2.4 MB (2435092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ba4d92c56600d1a8cf7dc9a595c294dcaa6b54c4f5374b60a252ae2f17b991c`  
		Last Modified: Wed, 10 Aug 2022 19:19:05 GMT  
		Size: 1.6 MB (1571628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5da42e613e53f10981d38e44870af4f3fff20605befbc0957b2ba5bc1f59265`  
		Last Modified: Wed, 10 Aug 2022 19:19:04 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea190ec38af2c760f3563e46d384fc23a661c273e994595f6fd329e5e6e7585b`  
		Last Modified: Wed, 10 Aug 2022 19:19:04 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87017832fda8d1f72a7f2e42f0d957cd92d26e4d1109de96f27520841409d29d`  
		Last Modified: Thu, 29 Sep 2022 18:11:56 GMT  
		Size: 10.4 MB (10439248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ff929691c05d4c5b3ae28a8c1fa0b4e87b0b992e0d63c3307c0af97189ccbc`  
		Last Modified: Thu, 29 Sep 2022 18:11:55 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5fc7f67b944bbc7c797abd0a1d5cd1c4884ad36b441a571f7c293dbe9ad0f2`  
		Last Modified: Thu, 29 Sep 2022 18:12:25 GMT  
		Size: 10.3 MB (10283704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b28f9029b7de894e6ccd491a843b9260c418394ebdaec4723c0a0f64dbefe447`  
		Last Modified: Thu, 29 Sep 2022 18:12:23 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d08e513b0c7a7b07f3923b165cd9a79d2e13a3ef40e13a66d1beba77a7ee60`  
		Last Modified: Thu, 29 Sep 2022 18:12:23 GMT  
		Size: 18.7 KB (18702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d45aefd4a3bebfa0721baf84e7b99361aaeccde9070a2de887dab98879e943e`  
		Last Modified: Thu, 29 Sep 2022 18:12:23 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36357d0cd676db95d684005f68ca6df66dfdcfcf3e59f2effb4b3667a514a1b`  
		Last Modified: Thu, 29 Sep 2022 22:52:30 GMT  
		Size: 1.9 MB (1855189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494195a35dd51ba996ea3e99412f87461ebbd6b859b510b662b717bce146eedd`  
		Last Modified: Thu, 29 Sep 2022 22:52:29 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a24e5313bbba2effdffa2076c2650df7aba99d6eb0084f4729d29bbb508eef8`  
		Last Modified: Thu, 29 Sep 2022 22:52:29 GMT  
		Size: 692.6 KB (692585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71a9f0a4b49085f6a1a255960c2273749a8a18f081ea971f2bc1eaae220b4e7e`  
		Last Modified: Thu, 29 Sep 2022 22:52:29 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6865d2411416b583c9170c2f25d70b79d4eaa5de6923dc1d530ef72b4fe1da70`  
		Last Modified: Thu, 29 Sep 2022 22:52:48 GMT  
		Size: 21.9 MB (21881575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-fpm-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:a875c5c20e863c8830e54e97f22768baf257b714e7dd39b6076335c8fbbc7fda
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.2 MB (51192124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:43d90bae0b92656e3634f5f02e5ea1866b70a2a1a27c1198a618839773e6ab33`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:22:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 10 Aug 2022 00:22:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 10 Aug 2022 00:22:28 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 10 Aug 2022 00:22:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 10 Aug 2022 00:22:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 10 Aug 2022 00:22:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 00:22:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 00:22:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 10 Aug 2022 01:54:17 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Sep 2022 15:19:28 GMT
ENV PHP_VERSION=7.4.32
# Thu, 29 Sep 2022 15:19:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Thu, 29 Sep 2022 15:19:30 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Thu, 29 Sep 2022 15:19:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Sep 2022 15:19:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Sep 2022 15:26:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Sep 2022 15:26:53 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 29 Sep 2022 15:26:54 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Sep 2022 15:26:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Sep 2022 15:26:55 GMT
WORKDIR /var/www/html
# Thu, 29 Sep 2022 15:26:56 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Sep 2022 15:26:57 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Sep 2022 15:26:58 GMT
EXPOSE 9000
# Thu, 29 Sep 2022 15:26:59 GMT
CMD ["php-fpm"]
# Thu, 29 Sep 2022 16:43:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 29 Sep 2022 16:43:08 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 29 Sep 2022 16:43:10 GMT
COPY file:31957edf88ab81c875036fac642510adba17e7f664ade12ad4cc270b8b01a7d0 in /usr/local/bin/ 
# Thu, 29 Sep 2022 20:41:05 GMT
ENV DRUPAL_VERSION=9.4.7
# Thu, 29 Sep 2022 20:41:06 GMT
WORKDIR /opt/drupal
# Thu, 29 Sep 2022 20:41:21 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 29 Sep 2022 20:41:22 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7a58d677a68ad3c648f0ba099ffbcb42c48ada3198266e10d1484b6693dbc2`  
		Last Modified: Wed, 10 Aug 2022 02:15:46 GMT  
		Size: 1.7 MB (1714756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100c816700973fc580272b58f48f95cb3600c7998953bcead7fba47d2b00a7b4`  
		Last Modified: Wed, 10 Aug 2022 02:15:45 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94771bf70d5316c0aeae680711bbba99dd5e5ff33b07f4d75b9ee80683b41eef`  
		Last Modified: Wed, 10 Aug 2022 02:15:45 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc046f3dc13be324efd6850b78cccd4a73e09b5feb4ebd08e33d6bcf090daff5`  
		Last Modified: Thu, 29 Sep 2022 15:50:36 GMT  
		Size: 10.4 MB (10439004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0590127bc80585dbaf9d740caf4300eeb6f9047ae57398e49d7a57de83bb58f`  
		Last Modified: Thu, 29 Sep 2022 15:50:35 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d7677dfc2d65a8c0984aa73348c85392bf44147122a36f649758bc195a2295a`  
		Last Modified: Thu, 29 Sep 2022 15:51:04 GMT  
		Size: 11.5 MB (11513814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ce03fd8eb31352aca29e0353da12b63df93b813245ca746952e5ee1af424dbd`  
		Last Modified: Thu, 29 Sep 2022 15:51:01 GMT  
		Size: 2.4 KB (2445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6212521ab255eee4bc5074f9bdd4147fa7b5297f0d527adfaaa79a1b7683128`  
		Last Modified: Thu, 29 Sep 2022 15:51:01 GMT  
		Size: 18.6 KB (18618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16e6dd3a7da59626d20c51a6056df34ceca0e8888eeda83055c9519bd70bd2d5`  
		Last Modified: Thu, 29 Sep 2022 15:51:01 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635ccda5d9e730631843ab00198285f84bfc975c6ce99dbbfcadbb357ad0cd5c`  
		Last Modified: Thu, 29 Sep 2022 17:04:35 GMT  
		Size: 2.2 MB (2198265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bb6fb97cf96c1e7c0e3f5b533957c989b8c8cce4d6416f827283084b26459f`  
		Last Modified: Thu, 29 Sep 2022 17:04:35 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29492272b92bd8fd54d5121defd2db842fce6e6aa038c18f2d15dd8ec7480ef2`  
		Last Modified: Thu, 29 Sep 2022 17:04:35 GMT  
		Size: 692.6 KB (692571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13b00d9967ccd05f1d0cf28380f0fdb4700fa686306407199a59e9391a132038`  
		Last Modified: Thu, 29 Sep 2022 21:18:16 GMT  
		Size: 115.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d32a69114ca3d53299c2c34bd1dac246b3e6d1708df6542513a27a5289f0e75`  
		Last Modified: Thu, 29 Sep 2022 21:18:22 GMT  
		Size: 21.9 MB (21883374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-fpm-alpine3.15` - linux; 386

```console
$ docker pull drupal@sha256:890a9267e63433de734b343093d9cf7f5f3b5bb274e4bf141e988e6ba50fbf1f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51729191 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20a8a87ea844c05edc42e712bd080740c93bd0ba20f9f80534eac40d5bec66a5`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:47 GMT
ADD file:d51bb92de86c49ee5486066d12194be78c8b9a8452c44577e2dfeef1945a0138 in / 
# Tue, 09 Aug 2022 17:38:47 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 21:14:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 06 Oct 2022 21:14:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 06 Oct 2022 21:14:21 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 06 Oct 2022 21:14:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 06 Oct 2022 21:14:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 06 Oct 2022 21:14:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 06 Oct 2022 21:14:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 06 Oct 2022 21:14:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 06 Oct 2022 22:27:04 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 06 Oct 2022 22:27:04 GMT
ENV PHP_VERSION=7.4.32
# Thu, 06 Oct 2022 22:27:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Thu, 06 Oct 2022 22:27:06 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Thu, 06 Oct 2022 22:27:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Oct 2022 22:27:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 06 Oct 2022 22:33:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 06 Oct 2022 22:33:36 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 06 Oct 2022 22:33:36 GMT
RUN docker-php-ext-enable sodium
# Thu, 06 Oct 2022 22:33:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 06 Oct 2022 22:33:38 GMT
WORKDIR /var/www/html
# Thu, 06 Oct 2022 22:33:39 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 06 Oct 2022 22:33:40 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Oct 2022 22:33:41 GMT
EXPOSE 9000
# Thu, 06 Oct 2022 22:33:42 GMT
CMD ["php-fpm"]
# Fri, 07 Oct 2022 03:05:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 03:05:38 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 07 Oct 2022 03:05:40 GMT
COPY file:31957edf88ab81c875036fac642510adba17e7f664ade12ad4cc270b8b01a7d0 in /usr/local/bin/ 
# Fri, 07 Oct 2022 03:05:40 GMT
ENV DRUPAL_VERSION=9.4.7
# Fri, 07 Oct 2022 03:05:41 GMT
WORKDIR /opt/drupal
# Fri, 07 Oct 2022 03:05:55 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 07 Oct 2022 03:05:57 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:f8c6eeaa55b0f135b7fddb3d7745a98ca4d8f06d2898611234b9ef99e1183073`  
		Last Modified: Tue, 09 Aug 2022 17:39:50 GMT  
		Size: 2.8 MB (2828516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2bc5695a671be5ab49e8ef9515c45bac9868ef6942e7eba7847b6da07ad66a3`  
		Last Modified: Thu, 06 Oct 2022 22:47:55 GMT  
		Size: 1.8 MB (1814937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac1cf10e2861b18fd0893eede83d16bb09da2377a48f51f2548edc988b8671c1`  
		Last Modified: Thu, 06 Oct 2022 22:47:54 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a46660760b73ac2d1b70f96a2768c2d134fe41fb72e20f52e83e1c4836ecaac`  
		Last Modified: Thu, 06 Oct 2022 22:47:54 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df34328ec22962d68feed975286fb39f28cc78e543cef8c558925f7261f7ec03`  
		Last Modified: Thu, 06 Oct 2022 22:57:17 GMT  
		Size: 10.4 MB (10439010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10515348077b35132e1b4e597551850a4fe20ca9d610bdb46192f7556531d2e5`  
		Last Modified: Thu, 06 Oct 2022 22:57:16 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e9baa50a693dbf9cef3c072770ed219f7755e6cb41d8880531a1481e47b588`  
		Last Modified: Thu, 06 Oct 2022 22:57:45 GMT  
		Size: 11.7 MB (11730055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ac083072940a2eeca35e924f425acf9aae56a9cbf53d48966c9555642d33f5`  
		Last Modified: Thu, 06 Oct 2022 22:57:43 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04f6e8d4fa007e4ed76393c583c1fbbf4f049439a10fcb8879f3e615ca9db446`  
		Last Modified: Thu, 06 Oct 2022 22:57:44 GMT  
		Size: 18.6 KB (18579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cf9012970afcf638237035a84b445ff0c6ddd4e5b793d447526108243858259`  
		Last Modified: Thu, 06 Oct 2022 22:57:43 GMT  
		Size: 8.4 KB (8438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff3f53122152518cc7fb0068d432ef37105868a7046a969791b5e359b774bfc`  
		Last Modified: Fri, 07 Oct 2022 03:42:47 GMT  
		Size: 2.3 MB (2309164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56b695997e72aa88aa12a84f8a448c9fcd82a397c6a21940058b40a022d7fc1a`  
		Last Modified: Fri, 07 Oct 2022 03:42:46 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4e1a10947a3b2a34fc14c2692a3f5c2c3a63d05d6952ec905481415122bd6f`  
		Last Modified: Fri, 07 Oct 2022 03:42:46 GMT  
		Size: 692.6 KB (692574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:593da363950eb20357fd73b580aff43c30d05f71497b0a5192991a2c519263b8`  
		Last Modified: Fri, 07 Oct 2022 03:42:46 GMT  
		Size: 113.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18468d1b69912c6605358d32f57617876cbc6ff331df1e25fac5a981101ad8af`  
		Last Modified: Fri, 07 Oct 2022 03:42:51 GMT  
		Size: 21.9 MB (21883080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-fpm-alpine3.15` - linux; ppc64le

```console
$ docker pull drupal@sha256:5503524793b38162eeb7492d09a517a89584bce2db3a96a526972e62f331e72c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52479518 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9dfda59dd2876a3efe5ff55b79ee314ac689938c1306f0c775004198d7a9de5f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:54:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 09 Aug 2022 19:54:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 09 Aug 2022 19:54:35 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 09 Aug 2022 19:54:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Aug 2022 19:54:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Aug 2022 19:54:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 19:54:37 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 19:54:37 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Aug 2022 21:32:36 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Sep 2022 14:50:35 GMT
ENV PHP_VERSION=7.4.32
# Thu, 29 Sep 2022 14:50:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Thu, 29 Sep 2022 14:50:35 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Thu, 29 Sep 2022 14:50:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Sep 2022 14:50:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Sep 2022 15:00:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Sep 2022 15:00:23 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 29 Sep 2022 15:00:25 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Sep 2022 15:00:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Sep 2022 15:00:26 GMT
WORKDIR /var/www/html
# Thu, 29 Sep 2022 15:00:27 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Sep 2022 15:00:27 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Sep 2022 15:00:28 GMT
EXPOSE 9000
# Thu, 29 Sep 2022 15:00:28 GMT
CMD ["php-fpm"]
# Thu, 29 Sep 2022 15:56:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 29 Sep 2022 15:56:48 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 29 Sep 2022 15:56:48 GMT
COPY file:31957edf88ab81c875036fac642510adba17e7f664ade12ad4cc270b8b01a7d0 in /usr/local/bin/ 
# Thu, 29 Sep 2022 20:15:43 GMT
ENV DRUPAL_VERSION=9.4.7
# Thu, 29 Sep 2022 20:15:43 GMT
WORKDIR /opt/drupal
# Thu, 29 Sep 2022 20:16:08 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 29 Sep 2022 20:16:13 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51d49a1268b677011b409f2df6d403755672a64b2476335bda8590d5132b1a1`  
		Last Modified: Tue, 09 Aug 2022 21:57:49 GMT  
		Size: 1.8 MB (1762163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:168ee424c0d63cd625d432ed1b59a6f2b5849627e702196a992e40a95b2e0b67`  
		Last Modified: Tue, 09 Aug 2022 21:57:48 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860bf2a5e9500032fb3e4ace19c4dbe49e838df439fe8172edac8164e82c15a3`  
		Last Modified: Tue, 09 Aug 2022 21:57:48 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90e76e253cbbedc674814ff718ba6a1fdae1b6e2e6912d0d4cbfb4ae280a64a4`  
		Last Modified: Thu, 29 Sep 2022 15:24:02 GMT  
		Size: 10.4 MB (10439251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a874dcfb38f0f1304944a742ede072cb21ef0448b0dc519054656757bfb1d350`  
		Last Modified: Thu, 29 Sep 2022 15:24:00 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e27404a026805f8cb03f14c5ee15b64da03026e3cb907dce235fa42fcf249af`  
		Last Modified: Thu, 29 Sep 2022 15:24:36 GMT  
		Size: 12.4 MB (12413092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ccdd18ba2141c2f0543ef4ff211e599a9889a530487500b8d892dabe6d075a`  
		Last Modified: Thu, 29 Sep 2022 15:24:32 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8788c7d7dd9d318af7b8f638a41b012c9474d2fa205a981de0bcf18e7d5f742`  
		Last Modified: Thu, 29 Sep 2022 15:24:32 GMT  
		Size: 18.7 KB (18720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55906d0344a8c377f709538b21e45463b4dab56cae153fa3f8097c7deb79cda1`  
		Last Modified: Thu, 29 Sep 2022 15:24:32 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f01d4ab61ec72e5702f6a93430286542d62e5c4843776433f02a8d46859b3cc`  
		Last Modified: Thu, 29 Sep 2022 16:15:51 GMT  
		Size: 2.4 MB (2445950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:330cd118d7f3e12ce704f9e2987667b1f743364f5f19cbd5b7e28f450c76c9d3`  
		Last Modified: Thu, 29 Sep 2022 16:15:50 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:072063d7bf09012532650264ef980e2af5c046a0ca5fbcca25c8d5d434bf3364`  
		Last Modified: Thu, 29 Sep 2022 16:15:50 GMT  
		Size: 692.6 KB (692584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acd24b019bbb687f09a3c42322e82e7e51784f48f3fd050fe28e20a18a77b072`  
		Last Modified: Thu, 29 Sep 2022 20:51:37 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c87bd5187e1f6bd2c9e8c81d6b79bc43c22daedbcc21a3734caee92dfab2942`  
		Last Modified: Thu, 29 Sep 2022 20:51:59 GMT  
		Size: 21.9 MB (21881375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:9-php7.4-fpm-alpine3.15` - linux; s390x

```console
$ docker pull drupal@sha256:59cac5019ea69a2b4bdd9411be751faf1f8ba8fc233a8fa3a3bf00f8ca9df54e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.0 MB (50957001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e10d263fe02546e75a73f1f02849111a34c921f2139b8fc8d4811ad71c64cbb2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 23:32:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 09 Aug 2022 23:32:29 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 09 Aug 2022 23:32:31 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 09 Aug 2022 23:32:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Aug 2022 23:32:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Aug 2022 23:32:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 23:32:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 23:32:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 10 Aug 2022 00:52:26 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Sep 2022 15:05:00 GMT
ENV PHP_VERSION=7.4.32
# Thu, 29 Sep 2022 15:05:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Thu, 29 Sep 2022 15:05:00 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Thu, 29 Sep 2022 15:05:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 29 Sep 2022 15:05:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 29 Sep 2022 15:10:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 29 Sep 2022 15:10:45 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 29 Sep 2022 15:10:46 GMT
RUN docker-php-ext-enable sodium
# Thu, 29 Sep 2022 15:10:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 29 Sep 2022 15:10:46 GMT
WORKDIR /var/www/html
# Thu, 29 Sep 2022 15:10:47 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 29 Sep 2022 15:10:47 GMT
STOPSIGNAL SIGQUIT
# Thu, 29 Sep 2022 15:10:47 GMT
EXPOSE 9000
# Thu, 29 Sep 2022 15:10:47 GMT
CMD ["php-fpm"]
# Thu, 29 Sep 2022 16:12:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 29 Sep 2022 16:12:10 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 29 Sep 2022 16:12:10 GMT
COPY file:31957edf88ab81c875036fac642510adba17e7f664ade12ad4cc270b8b01a7d0 in /usr/local/bin/ 
# Thu, 29 Sep 2022 19:51:15 GMT
ENV DRUPAL_VERSION=9.4.7
# Thu, 29 Sep 2022 19:51:15 GMT
WORKDIR /opt/drupal
# Thu, 29 Sep 2022 19:51:28 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 29 Sep 2022 19:51:31 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23435d6f332bdec76345d9b8c7b25366dab57121713621f34ea44a6a19bbb3eb`  
		Last Modified: Wed, 10 Aug 2022 01:22:14 GMT  
		Size: 1.8 MB (1774832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e46eecb980e2a5d45c58328c006bb9455521558389033fd9733e22901035459`  
		Last Modified: Wed, 10 Aug 2022 01:22:14 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fefa7d36d57256207376324466e3201608351511c4675fa18f32bbebeaa1600`  
		Last Modified: Wed, 10 Aug 2022 01:22:02 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59fc4dfc89a9730fb43ea0b244ffca12459bd908ce0df7d007ab46d7316fc10a`  
		Last Modified: Thu, 29 Sep 2022 15:29:23 GMT  
		Size: 10.4 MB (10439255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2cf6a5f91109574915be1ac3689374918f091bfe12fd534ac3bdb192505befe3`  
		Last Modified: Thu, 29 Sep 2022 15:29:23 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bae24f304ba635cf015b059ce52a41a98b05066b8cbcc96fade282bd712cd26d`  
		Last Modified: Thu, 29 Sep 2022 15:29:42 GMT  
		Size: 11.3 MB (11284501 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab0269fafb1269f8616648e6017a04756e20250d094117de91e3e1d06d27ba86`  
		Last Modified: Thu, 29 Sep 2022 15:29:40 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c195336eba0361c027d66b342e042d47cd277328a2152c4c4f572fa56d0b2991`  
		Last Modified: Thu, 29 Sep 2022 15:29:40 GMT  
		Size: 18.7 KB (18740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b8b9a3243b8f7523435d339f58deefa92e8ea48c02a97e28987a24ebb5e5e4`  
		Last Modified: Thu, 29 Sep 2022 15:29:40 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0165cb132f5c311c2025717e486193e8f6d39e6b4b8fd4ca79751e74603f96f0`  
		Last Modified: Thu, 29 Sep 2022 16:28:13 GMT  
		Size: 2.2 MB (2246195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88749f8e267fccff665bf8a9194f05691bb140687d58e18f7bcf80a5d69b3787`  
		Last Modified: Thu, 29 Sep 2022 16:28:13 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a43d7694c6e84382145246cfde13bd10ed1a9c5d03193a6481b7b19744e59b9`  
		Last Modified: Thu, 29 Sep 2022 16:28:13 GMT  
		Size: 692.6 KB (692580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6635345b450cc945fca1c9803c28d95ad75ea5226abac89f9de9c2a7e0b355c8`  
		Last Modified: Thu, 29 Sep 2022 20:13:18 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ca04f35c67ca25cf6aa7a106fefddde5bf8dac0f067837d6bfc18a49472e35`  
		Last Modified: Thu, 29 Sep 2022 20:13:22 GMT  
		Size: 21.9 MB (21881418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
