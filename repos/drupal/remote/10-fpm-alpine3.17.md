## `drupal:10-fpm-alpine3.17`

```console
$ docker pull drupal@sha256:161d1e01ab401a1b65c0fcdb6fc3fed69d7bc94aa1cabfc030cb7572f6ae177d
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

### `drupal:10-fpm-alpine3.17` - linux; amd64

```console
$ docker pull drupal@sha256:a996ee1138f255b5b2ae7b8b4f51402e150013d1c35db6a3f99f50d77d29fe55
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51557360 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e388fd3f88b437e1ebb8b9b988f28d98a4ed97228f4cb214514d0a26a650725a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:59:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 09 Aug 2023 04:59:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 09 Aug 2023 04:59:56 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 09 Aug 2023 04:59:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 09 Aug 2023 04:59:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 09 Aug 2023 04:59:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 09 Aug 2023 04:59:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 09 Aug 2023 04:59:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 09 Aug 2023 05:22:23 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 09 Aug 2023 05:44:35 GMT
ENV PHP_VERSION=8.2.8
# Wed, 09 Aug 2023 05:44:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Wed, 09 Aug 2023 05:44:35 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Wed, 09 Aug 2023 05:44:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 09 Aug 2023 05:44:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 09 Aug 2023 05:51:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 09 Aug 2023 05:51:59 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 09 Aug 2023 05:52:00 GMT
RUN docker-php-ext-enable sodium
# Wed, 09 Aug 2023 05:52:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 09 Aug 2023 05:52:00 GMT
WORKDIR /var/www/html
# Wed, 09 Aug 2023 05:52:00 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 09 Aug 2023 05:52:00 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 05:52:00 GMT
EXPOSE 9000
# Wed, 09 Aug 2023 05:52:01 GMT
CMD ["php-fpm"]
# Wed, 09 Aug 2023 10:40:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 09 Aug 2023 10:40:32 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 09 Aug 2023 10:40:32 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Wed, 09 Aug 2023 10:40:32 GMT
ENV DRUPAL_VERSION=10.1.2
# Wed, 09 Aug 2023 10:40:32 GMT
WORKDIR /opt/drupal
# Wed, 09 Aug 2023 10:40:41 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 09 Aug 2023 10:40:42 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35d73d8a432227f5347f0b50ab4abfa5fbb04413370e36eee386841829655bf`  
		Last Modified: Wed, 09 Aug 2023 07:10:06 GMT  
		Size: 1.9 MB (1894005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a251dfb292c22a24c55dd5b924de2a148f72e5a98cd4b8e8cdba940ba0e3b45`  
		Last Modified: Wed, 09 Aug 2023 07:10:06 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d959040f204ac17e6c5337ab8b1b0ef9f58c2621bb783598e4fc6cf6aa7e8c54`  
		Last Modified: Wed, 09 Aug 2023 07:10:05 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:586dafb284bca2204cf7514e8f2b0b1525382c5fbdc4fff6ffd05797adbb84f7`  
		Last Modified: Wed, 09 Aug 2023 07:14:33 GMT  
		Size: 12.1 MB (12055548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5949c85dfbeb4697a805c4c1ee5816c1d3d305f3ef6faa520979532b042d298e`  
		Last Modified: Wed, 09 Aug 2023 07:14:32 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7477b3c3df71a02386ed179091493fc6f181dc37deab78a35265e266e499703b`  
		Last Modified: Wed, 09 Aug 2023 07:14:58 GMT  
		Size: 12.8 MB (12783033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:454eb424ddef3050befb294ea20c17e5e16eb82eb1361cacc08d1b094f295cf4`  
		Last Modified: Wed, 09 Aug 2023 07:14:56 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fea4fe16619e309362ee0abe9fb83838d17738710801554c44a5a104fc2c0f4`  
		Last Modified: Wed, 09 Aug 2023 07:14:56 GMT  
		Size: 19.0 KB (18977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f5f68fb799f9085849cca24ea07865b9540761fc612a75765b5b395014553d`  
		Last Modified: Wed, 09 Aug 2023 07:14:56 GMT  
		Size: 9.2 KB (9181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2cafcfdfcdb026d7c32eea33c91d7241360f55495c993fb06287eadc267766c`  
		Last Modified: Wed, 09 Aug 2023 10:56:36 GMT  
		Size: 2.2 MB (2208051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6093aa3f4c27ad193a682c6e26064420086533a90472ac19a748ead03593fde1`  
		Last Modified: Wed, 09 Aug 2023 10:56:36 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8954c457dc8f0275e4bdc350b58e3f96e17ad28248829dab784f646def5eafef`  
		Last Modified: Wed, 09 Aug 2023 10:56:36 GMT  
		Size: 698.2 KB (698238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:995df127f2012ac4538d609a8c99e15ecdd4e5720a92c82e17dd241c25394155`  
		Last Modified: Wed, 09 Aug 2023 10:56:36 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e83d6b3cdc3811c6c0606309c8e5c77f7444300718cc00892c9ac9c2b54f9bbc`  
		Last Modified: Wed, 09 Aug 2023 10:56:40 GMT  
		Size: 18.5 MB (18506787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:10-fpm-alpine3.17` - linux; arm variant v6

```console
$ docker pull drupal@sha256:e41463ad49617ce2e67942d264157dc2cc22b20bda5c2911be5ae6c7e9249cb0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49554783 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9348bd9261116f22b11e23ecf4370367f8c124aa0f7c72892b70bcb8a769fbdc`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:49:17 GMT
ADD file:cb3f59b0f701cb6ef552e7f8ada1707cf82747c95b69759924061ff9ac6dbe72 in / 
# Mon, 07 Aug 2023 19:49:18 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:15:05 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 09 Aug 2023 00:15:06 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 09 Aug 2023 00:15:07 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 09 Aug 2023 00:15:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 09 Aug 2023 00:15:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 09 Aug 2023 00:15:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 09 Aug 2023 00:15:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 09 Aug 2023 00:15:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 09 Aug 2023 00:33:24 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 17 Aug 2023 22:59:57 GMT
ENV PHP_VERSION=8.2.9
# Thu, 17 Aug 2023 22:59:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.9.tar.xz.asc
# Thu, 17 Aug 2023 22:59:57 GMT
ENV PHP_SHA256=1e6cb77f997613864ab3127fbfc6a8c7fdaa89a95e8ed6167617b913b4de4765
# Thu, 17 Aug 2023 23:00:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Aug 2023 23:00:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Aug 2023 23:06:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Aug 2023 23:06:21 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 17 Aug 2023 23:06:23 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Aug 2023 23:06:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Aug 2023 23:06:23 GMT
WORKDIR /var/www/html
# Thu, 17 Aug 2023 23:06:24 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 17 Aug 2023 23:06:24 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Aug 2023 23:06:24 GMT
EXPOSE 9000
# Thu, 17 Aug 2023 23:06:24 GMT
CMD ["php-fpm"]
# Thu, 17 Aug 2023 23:36:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 17 Aug 2023 23:36:01 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 17 Aug 2023 23:36:01 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Thu, 17 Aug 2023 23:36:01 GMT
ENV DRUPAL_VERSION=10.1.2
# Thu, 17 Aug 2023 23:36:01 GMT
WORKDIR /opt/drupal
# Thu, 17 Aug 2023 23:36:16 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Thu, 17 Aug 2023 23:36:20 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:342323bc858ed9706f7953ab06cbf6785b678c55ef2317577af748533d11165b`  
		Last Modified: Mon, 07 Aug 2023 19:49:53 GMT  
		Size: 3.1 MB (3112450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e56d818f54805e003ab7e46f53ba337d9f4339dd6916a1f94c60461593def908`  
		Last Modified: Wed, 09 Aug 2023 01:36:29 GMT  
		Size: 1.9 MB (1882223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f0dea045ab38115be3f8e3c75c91d8f5238cd0a82e175a912b363243b361303`  
		Last Modified: Wed, 09 Aug 2023 01:36:28 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e38f7c637accb9c42bb3e74b63120c3f3d3a8534a9816754e87a1af32bb4734`  
		Last Modified: Wed, 09 Aug 2023 01:36:28 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c8bd8ecd4bc7db476938c5a8de24f1e4f6444996d254c03e7a852775c6af5a5`  
		Last Modified: Thu, 17 Aug 2023 23:13:03 GMT  
		Size: 12.1 MB (12056154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9f3f02d5b9dbfed09e1a39584fc188a297e04a2fddc077418d4061ee7d34cb`  
		Last Modified: Thu, 17 Aug 2023 23:13:02 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295e7724765a73cbeb6a554e210238418e84295be1e44cc91a5e508f85d1c1bd`  
		Last Modified: Thu, 17 Aug 2023 23:13:31 GMT  
		Size: 11.6 MB (11586301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83eda402e45849cedb26f3912d67c30fdebcb540468b742a66d437bc2e3d901c`  
		Last Modified: Thu, 17 Aug 2023 23:13:29 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee12a96ad05eeec9f3842c5efa08960d6481245fa8ec92883ca798a62a666d45`  
		Last Modified: Thu, 17 Aug 2023 23:13:29 GMT  
		Size: 18.8 KB (18756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fce11409a2c3b4f1203528c4e92dc779686a5690754fe930e51baf3cfaf1aa4`  
		Last Modified: Thu, 17 Aug 2023 23:13:29 GMT  
		Size: 9.2 KB (9182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0771c01675433ad4359ee9ae5ef5e92f7db6f6512968aa3e0c419128ad071109`  
		Last Modified: Thu, 17 Aug 2023 23:39:59 GMT  
		Size: 1.7 MB (1679286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c004c6cb0c3d076dfb1c2cf51bc33322b9abca283439c90b6740ec1a83001c7`  
		Last Modified: Thu, 17 Aug 2023 23:39:59 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66cc4b911a9819555b9696f6feddd239209f0b25637d9716ddc32bec36aaf3a6`  
		Last Modified: Thu, 17 Aug 2023 23:39:59 GMT  
		Size: 698.2 KB (698236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c450ef9d0ce54d3c3dd14a43c9631889ba4ea60495435dcb9c24bcaa1a8525`  
		Last Modified: Thu, 17 Aug 2023 23:39:59 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3edbe11505ec79bb6688d5cebd94fbddc0fe367c8033ec6732c5627bcc40f9ef`  
		Last Modified: Thu, 17 Aug 2023 23:40:05 GMT  
		Size: 18.5 MB (18507261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:10-fpm-alpine3.17` - linux; arm variant v7

```console
$ docker pull drupal@sha256:168b6bfd2a2f6ec81fb1411da09a3655c71222222f5e24bac32f1916c9e0ec3b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.3 MB (48333137 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4065c05e41469806ab56e4f2e42ce2c29d5af18c2e611b8df4abb83035e9ac5`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:57:29 GMT
ADD file:7f36c30ba2b714d09a8650dba1545abdf892443dadbe9113b9a166b84ba7ac3f in / 
# Mon, 07 Aug 2023 19:57:29 GMT
CMD ["/bin/sh"]
# Mon, 07 Aug 2023 23:52:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 07 Aug 2023 23:52:57 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 07 Aug 2023 23:52:58 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 07 Aug 2023 23:52:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 07 Aug 2023 23:52:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Mon, 07 Aug 2023 23:52:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 07 Aug 2023 23:52:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 07 Aug 2023 23:52:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 08 Aug 2023 00:08:40 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Tue, 08 Aug 2023 00:24:25 GMT
ENV PHP_VERSION=8.2.8
# Tue, 08 Aug 2023 00:24:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Tue, 08 Aug 2023 00:24:25 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Tue, 08 Aug 2023 00:24:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 08 Aug 2023 00:24:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 08 Aug 2023 00:29:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 08 Aug 2023 00:29:27 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 08 Aug 2023 00:29:28 GMT
RUN docker-php-ext-enable sodium
# Tue, 08 Aug 2023 00:29:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 08 Aug 2023 00:29:28 GMT
WORKDIR /var/www/html
# Tue, 08 Aug 2023 00:29:29 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Tue, 08 Aug 2023 00:29:29 GMT
STOPSIGNAL SIGQUIT
# Tue, 08 Aug 2023 00:29:29 GMT
EXPOSE 9000
# Tue, 08 Aug 2023 00:29:29 GMT
CMD ["php-fpm"]
# Tue, 08 Aug 2023 06:07:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Tue, 08 Aug 2023 06:07:52 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 08 Aug 2023 06:07:52 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Tue, 08 Aug 2023 06:07:52 GMT
ENV DRUPAL_VERSION=10.1.2
# Tue, 08 Aug 2023 06:07:52 GMT
WORKDIR /opt/drupal
# Tue, 08 Aug 2023 06:08:03 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Tue, 08 Aug 2023 06:08:04 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b82e4fd40279a40aa2eecd301fabb2dca254727cc09daa8d0caf69ac28c44af1`  
		Last Modified: Mon, 07 Aug 2023 19:58:08 GMT  
		Size: 2.9 MB (2869425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c88c9d990b3479f32cd8fe3f2938fedbf5d5dd45ae8d3c6327b23b28cd338e6`  
		Last Modified: Tue, 08 Aug 2023 01:09:06 GMT  
		Size: 1.7 MB (1732838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:234b29e1bf87b402db95683770ec3279b8750893193812fd5aaf093824deee0f`  
		Last Modified: Tue, 08 Aug 2023 01:09:06 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281e9b6223cc3ea016463be76acc6919f4fbf7995e01395867e3002ec07b7489`  
		Last Modified: Tue, 08 Aug 2023 01:09:06 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a330f314340abf5172895b430b0de8c268684de5aa94884e8c64b11fcb92a3b6`  
		Last Modified: Tue, 08 Aug 2023 01:13:37 GMT  
		Size: 12.1 MB (12055538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23952ff385fea740584a2305167ba14b580551540f56343946db7287b6bffe7`  
		Last Modified: Tue, 08 Aug 2023 01:13:36 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfc98009dbda0e26950a21668a78e112ec49133b4817aafc3484e2cb31871d14`  
		Last Modified: Tue, 08 Aug 2023 01:14:04 GMT  
		Size: 10.9 MB (10890553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77b3a254e791f8ac972fc7dc73bce9763d8118386ad86fbcae3b996403811aa`  
		Last Modified: Tue, 08 Aug 2023 01:14:02 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bcfdd38bc639b6475d664d5dd62aa098feaee5475a18b57f424e63095b28f65`  
		Last Modified: Tue, 08 Aug 2023 01:14:02 GMT  
		Size: 18.8 KB (18772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88afb7b1f15589e67e215aac658e2ddd1c363e6b1e57db7b0a6a15f38d36f214`  
		Last Modified: Tue, 08 Aug 2023 01:14:02 GMT  
		Size: 9.2 KB (9175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:833e149f8e53555cd4a79f587cda6d5bb315177512ad00e858ee98a975c2a4c9`  
		Last Modified: Tue, 08 Aug 2023 06:17:47 GMT  
		Size: 1.5 MB (1546676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4277fb2f2fc1aae3f5d3b9ed9b599a9b59d997d496d8f9ab2c5a6bb29661f47`  
		Last Modified: Tue, 08 Aug 2023 06:17:46 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc763853923e90007f8c6317b80117e1d2f14fbbaca7d1a8ee38f24c490d008`  
		Last Modified: Tue, 08 Aug 2023 06:17:46 GMT  
		Size: 698.2 KB (698240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:632a2c5851f10044bc103f018b48b60717a95181d5d8154fcd372272e4c68282`  
		Last Modified: Tue, 08 Aug 2023 06:17:46 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f47df2ea82a69ea550992b12a93ccff4d08c46fa1486b74ebdb8b65c00fd9b85`  
		Last Modified: Tue, 08 Aug 2023 06:17:51 GMT  
		Size: 18.5 MB (18506989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:10-fpm-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:fb5e072ff0fe6566e65875a2ee7ff1eb6ee2de4ead90d8c2f63de835b34f2ac0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51661889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c49b3ee24e6a1e8852eeb33345d98fe72a3a910c105f8ce164aff07b89a0e3b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:39:22 GMT
ADD file:9e054a25c83111adc857a7f988336ee40eea5e1794ed30a80d465e8d472342e2 in / 
# Mon, 07 Aug 2023 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 05:18:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 09 Aug 2023 05:18:47 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 09 Aug 2023 05:18:47 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 09 Aug 2023 05:18:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 09 Aug 2023 05:18:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 09 Aug 2023 05:18:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 09 Aug 2023 05:18:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 09 Aug 2023 05:18:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 09 Aug 2023 05:41:46 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 17 Aug 2023 23:17:17 GMT
ENV PHP_VERSION=8.2.9
# Thu, 17 Aug 2023 23:17:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.9.tar.xz.asc
# Thu, 17 Aug 2023 23:17:17 GMT
ENV PHP_SHA256=1e6cb77f997613864ab3127fbfc6a8c7fdaa89a95e8ed6167617b913b4de4765
# Thu, 17 Aug 2023 23:17:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Aug 2023 23:17:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Aug 2023 23:24:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Aug 2023 23:24:21 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 17 Aug 2023 23:24:22 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Aug 2023 23:24:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Aug 2023 23:24:22 GMT
WORKDIR /var/www/html
# Thu, 17 Aug 2023 23:24:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 17 Aug 2023 23:24:22 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Aug 2023 23:24:22 GMT
EXPOSE 9000
# Thu, 17 Aug 2023 23:24:23 GMT
CMD ["php-fpm"]
# Fri, 18 Aug 2023 00:46:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 18 Aug 2023 00:46:32 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 18 Aug 2023 00:46:32 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Fri, 18 Aug 2023 00:46:32 GMT
ENV DRUPAL_VERSION=10.1.2
# Fri, 18 Aug 2023 00:46:32 GMT
WORKDIR /opt/drupal
# Fri, 18 Aug 2023 00:46:42 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 18 Aug 2023 00:46:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:4060ece20d7ac783f52cbe28a35fd5b06f90f7b4d773bae0d956024e85ff35b6`  
		Last Modified: Mon, 07 Aug 2023 19:39:59 GMT  
		Size: 3.3 MB (3258290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97fc3822d6a537a85e38c638aaebb66cb4635f05b4a09c9bec8c6a40c6b3cf1c`  
		Last Modified: Wed, 09 Aug 2023 07:19:21 GMT  
		Size: 1.9 MB (1891587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa9d729b26ba8dd3b5ba7d57ad74a6891e452dc5e81ffd903fe5a862d5b92ef`  
		Last Modified: Wed, 09 Aug 2023 07:19:21 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c555f4ccaaa11d1f905038598b6dd4197005c1835f69b88927dbdb2bf39489f6`  
		Last Modified: Wed, 09 Aug 2023 07:19:21 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321e5d748fe357533535f73ba9a9c8d5fbee18cfed12234da7704be9af8ffa83`  
		Last Modified: Thu, 17 Aug 2023 23:35:55 GMT  
		Size: 12.1 MB (12056160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:670509fe7976e9b860509bcb39d153cfc6f95ce4848b642ce4b0e9126607707a`  
		Last Modified: Thu, 17 Aug 2023 23:35:54 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3679419fe428b0d05ff8423c85d9302f2fd05c90ae55da5ab59caf8325cd2d`  
		Last Modified: Thu, 17 Aug 2023 23:36:19 GMT  
		Size: 12.8 MB (12772496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66d622a7d0540cd06971240f08a68c83854cc6b3dbeaf92d120eb09673eabab3`  
		Last Modified: Thu, 17 Aug 2023 23:36:17 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a07ea555564ee5984628a9aaaa18de6e047fa8d96573497cc5bba82267c190`  
		Last Modified: Thu, 17 Aug 2023 23:36:17 GMT  
		Size: 18.8 KB (18774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe7f6f6e43e3da5ed228fd2048347951ecf006f09c9d7322c70523a85f6c5405`  
		Last Modified: Thu, 17 Aug 2023 23:36:17 GMT  
		Size: 9.2 KB (9179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e3198ebe9958e07506b77fc3c220fada27d0e02d4f2a0138c19b7082cb720e`  
		Last Modified: Fri, 18 Aug 2023 00:56:48 GMT  
		Size: 2.4 MB (2444850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6af794e9d37b6927951e6d7eb6e115af096f42fd41d59b2e0bc47cc9118be39`  
		Last Modified: Fri, 18 Aug 2023 00:56:47 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d530625178d3a2b2979285d55d91a463ffbfc24a4e6ffe5170cc107e0bf81bc`  
		Last Modified: Fri, 18 Aug 2023 00:56:47 GMT  
		Size: 698.2 KB (698237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e2d232deb55d1fb50307f3cb010c37cbcb7962c8e48000e0a52272e61d0fcfd`  
		Last Modified: Fri, 18 Aug 2023 00:56:47 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55b6875edab8b24db4fff7bf6ce05c088108eb975c609130312d6f089d70ec7c`  
		Last Modified: Fri, 18 Aug 2023 00:56:51 GMT  
		Size: 18.5 MB (18507383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:10-fpm-alpine3.17` - linux; 386

```console
$ docker pull drupal@sha256:c715e6a6167398bb23bdf4804c9a40140be1b1ea06a9778ffa98934fb865c10a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52085992 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44f1b3f65abe8338684b04b62d267dbafce83d34062febb5d0c5383a56fd4659`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:30 GMT
ADD file:437e2411fa3e4795a759f54507f41caa000169f0c32600ec49b4397313cd0884 in / 
# Mon, 07 Aug 2023 19:38:30 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 23:32:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 08 Aug 2023 23:32:19 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 08 Aug 2023 23:32:19 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 08 Aug 2023 23:32:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 08 Aug 2023 23:32:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 08 Aug 2023 23:32:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 08 Aug 2023 23:32:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 08 Aug 2023 23:32:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 09 Aug 2023 00:10:34 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 17 Aug 2023 23:42:40 GMT
ENV PHP_VERSION=8.2.9
# Thu, 17 Aug 2023 23:42:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.9.tar.xz.asc
# Thu, 17 Aug 2023 23:42:40 GMT
ENV PHP_SHA256=1e6cb77f997613864ab3127fbfc6a8c7fdaa89a95e8ed6167617b913b4de4765
# Thu, 17 Aug 2023 23:42:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Aug 2023 23:42:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Aug 2023 23:55:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Aug 2023 23:55:05 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 17 Aug 2023 23:55:06 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Aug 2023 23:55:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Aug 2023 23:55:06 GMT
WORKDIR /var/www/html
# Thu, 17 Aug 2023 23:55:07 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 17 Aug 2023 23:55:07 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Aug 2023 23:55:07 GMT
EXPOSE 9000
# Thu, 17 Aug 2023 23:55:07 GMT
CMD ["php-fpm"]
# Fri, 18 Aug 2023 00:56:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 18 Aug 2023 00:56:28 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 18 Aug 2023 00:56:28 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Fri, 18 Aug 2023 00:56:28 GMT
ENV DRUPAL_VERSION=10.1.2
# Fri, 18 Aug 2023 00:56:29 GMT
WORKDIR /opt/drupal
# Fri, 18 Aug 2023 00:56:42 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 18 Aug 2023 00:56:43 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:ddc7d64c528fabaad61cc880e91abba829973f743d753415145211971f9ee10d`  
		Last Modified: Mon, 07 Aug 2023 19:39:10 GMT  
		Size: 3.4 MB (3413779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02eabb7e56821471af526d4bf90d6f12a963e25c14699f506b9d0df77d3b9b07`  
		Last Modified: Wed, 09 Aug 2023 03:12:04 GMT  
		Size: 2.0 MB (2013298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d9b5233e9bd34988ce65c686bd5c4dccb957a4f4374c6b3d875b69c62618c2`  
		Last Modified: Wed, 09 Aug 2023 03:12:03 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec45cbb48e240567a01027034d0105d2cf21191c96a25b6448299d1e2e7db0dc`  
		Last Modified: Wed, 09 Aug 2023 03:12:03 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587fc6ff82f334b2b0554421d180c357e5f81324c47ed02b9ce3187db84ca0f9`  
		Last Modified: Fri, 18 Aug 2023 00:10:01 GMT  
		Size: 12.1 MB (12056150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce60246535cd64cfebed2debc0f0b2cd373251c71275ff6ad98354e2fcf148d2`  
		Last Modified: Fri, 18 Aug 2023 00:10:00 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8520cf82e239125108926d8975659c36bea7a77057b205c6c07e66a5335e9426`  
		Last Modified: Fri, 18 Aug 2023 00:10:30 GMT  
		Size: 13.1 MB (13076733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0c576fa28af1172f52aeb3c51efdf2cc6c707be95875ad01b7bcac23f68805`  
		Last Modified: Fri, 18 Aug 2023 00:10:26 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e788a4ebb64b32076c0ec423ab6c838116071fb8bcfaeb80d198d8bc9c32cb6`  
		Last Modified: Fri, 18 Aug 2023 00:10:26 GMT  
		Size: 19.0 KB (18969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:396ecf5dc8a96c019b767941809357f4322b9bbbc96bdef5e4bd5d6d77c66195`  
		Last Modified: Fri, 18 Aug 2023 00:10:26 GMT  
		Size: 9.2 KB (9179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cff9c9bd554681f3b91cd1b84fcb4af5eea9de140a41d4a7d060042305648e1`  
		Last Modified: Fri, 18 Aug 2023 01:08:33 GMT  
		Size: 2.3 MB (2287620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd47937e5ac51b30d6140fd6e51d7ea81944169852d27d2f19643f466705e6b5`  
		Last Modified: Fri, 18 Aug 2023 01:08:33 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365aed42d8798ffabe43f7897172e5d60d3fe27ba4556a4353d728180cb5ee2a`  
		Last Modified: Fri, 18 Aug 2023 01:08:33 GMT  
		Size: 698.2 KB (698232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fa88efe82292dee94f4fd7cb0c17d95d7477e756509982f2e0946b4d40db5b7`  
		Last Modified: Fri, 18 Aug 2023 01:08:33 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f11fb0c4a3de4881cf9ad9561dc305dac3b9ba997e74604f01cbe3125f6bf9c`  
		Last Modified: Fri, 18 Aug 2023 01:08:40 GMT  
		Size: 18.5 MB (18507102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:10-fpm-alpine3.17` - linux; ppc64le

```console
$ docker pull drupal@sha256:a6a7b07a86d7f9f1b5ae7a654b28006a858822e0f236eee171f774ec66fb46f7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.8 MB (51796350 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85fd6d9a350235c5f3a9e20d24cb48721a25497d42a27613c1d18ff4e04fea04`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 20:16:35 GMT
ADD file:52f28bcdd6e1c6f85b2b5d66ace37ed6cef0da8ce5c58e246549427361b64c1d in / 
# Mon, 07 Aug 2023 20:16:36 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 00:36:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 09 Aug 2023 00:36:32 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 09 Aug 2023 00:36:34 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 09 Aug 2023 00:36:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 09 Aug 2023 00:36:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 09 Aug 2023 00:36:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 09 Aug 2023 00:36:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 09 Aug 2023 00:36:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 09 Aug 2023 01:04:01 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Wed, 09 Aug 2023 01:31:07 GMT
ENV PHP_VERSION=8.2.8
# Wed, 09 Aug 2023 01:31:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.8.tar.xz.asc
# Wed, 09 Aug 2023 01:31:08 GMT
ENV PHP_SHA256=cfe1055fbcd486de7d3312da6146949aae577365808790af6018205567609801
# Wed, 09 Aug 2023 01:31:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 09 Aug 2023 01:31:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 09 Aug 2023 01:39:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 09 Aug 2023 01:39:37 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 09 Aug 2023 01:39:40 GMT
RUN docker-php-ext-enable sodium
# Wed, 09 Aug 2023 01:39:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 09 Aug 2023 01:39:41 GMT
WORKDIR /var/www/html
# Wed, 09 Aug 2023 01:39:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 09 Aug 2023 01:39:43 GMT
STOPSIGNAL SIGQUIT
# Wed, 09 Aug 2023 01:39:44 GMT
EXPOSE 9000
# Wed, 09 Aug 2023 01:39:46 GMT
CMD ["php-fpm"]
# Wed, 09 Aug 2023 11:12:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Wed, 09 Aug 2023 11:12:07 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 09 Aug 2023 11:12:07 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Wed, 09 Aug 2023 11:12:07 GMT
ENV DRUPAL_VERSION=10.1.2
# Wed, 09 Aug 2023 11:12:08 GMT
WORKDIR /opt/drupal
# Wed, 09 Aug 2023 11:12:37 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Wed, 09 Aug 2023 11:12:41 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:1e00d0a2a797866697ccca7b6307a9182e2852583b2b3be3928d196e4cb8ba3d`  
		Last Modified: Mon, 07 Aug 2023 20:17:39 GMT  
		Size: 3.4 MB (3391349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0430d9da42b848cdfe58f7019d881723ad193550e8e075a6e0423c0035af9290`  
		Last Modified: Wed, 09 Aug 2023 03:08:51 GMT  
		Size: 2.0 MB (1978452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eaae3eec60cd402fe32ab9b22419762950ea77d3c0f36c444376cb29ae9866d`  
		Last Modified: Wed, 09 Aug 2023 03:08:50 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b596614f85ae3d5aa46a5adf6df698a239bb7f94bf3a12a898a2f34d1b01948`  
		Last Modified: Wed, 09 Aug 2023 03:08:50 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0ea2e0f9734e7d468e8a686f6702eb5a888a4ec9543de1d688e493acb1b0196`  
		Last Modified: Wed, 09 Aug 2023 03:15:28 GMT  
		Size: 12.1 MB (12055537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a5f8e3e2e543486080c2657c485597a68bb3e3d38adb3f49e42cc09fd14aea`  
		Last Modified: Wed, 09 Aug 2023 03:15:27 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b416fdc9506acd23e1264844bf6243e289156be000efbe28433634acd9f8017`  
		Last Modified: Wed, 09 Aug 2023 03:16:10 GMT  
		Size: 13.2 MB (13200456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e9f9611947004bb1a7f75b6177a420e51238d328900ac4cb23aa1d6231e93b`  
		Last Modified: Wed, 09 Aug 2023 03:16:06 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b0b2b2c2f375ea23e25670daa4c046db6a6f984af86fff25e0e4b5dd25ad09b`  
		Last Modified: Wed, 09 Aug 2023 03:16:06 GMT  
		Size: 18.8 KB (18778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9128430ee895e4066b571796fc6f92476d691143294dc67de0a4f9d93079fa58`  
		Last Modified: Wed, 09 Aug 2023 03:16:06 GMT  
		Size: 9.2 KB (9180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ccac98071802e8f311be4594dea556f9c97444d6afdcb7c323d3bfb5162ac6`  
		Last Modified: Wed, 09 Aug 2023 11:36:23 GMT  
		Size: 1.9 MB (1932138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d1e5ab71959eeeffbe7f543ed2b4f568db33886be7c0f3125028130e65fe17`  
		Last Modified: Wed, 09 Aug 2023 11:36:22 GMT  
		Size: 313.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:087e61c5fb784d4c84a3638f292ef01096b3e32a7d633f19a913fe3d330680f8`  
		Last Modified: Wed, 09 Aug 2023 11:36:23 GMT  
		Size: 698.2 KB (698235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c2dea88718e70f93ac06218d11f9db434301fb691dff95de08930c2528bb091`  
		Last Modified: Wed, 09 Aug 2023 11:36:22 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e026cdc06bc5f490435f6f1cbc6a65bea262805830605357ae9cb5b5998576b3`  
		Last Modified: Wed, 09 Aug 2023 11:36:31 GMT  
		Size: 18.5 MB (18507289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:10-fpm-alpine3.17` - linux; s390x

```console
$ docker pull drupal@sha256:4d818553550cf629552f833057ff97f9564f60d1391d4462d6f38a254211de22
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50128705 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1865024bf9485ab07f43d0842878d13a2546a238c11bd4cc451a1f7c8067b988`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 07 Aug 2023 19:42:01 GMT
ADD file:2e221805acb91c51e7afa6b926252ab2260cdf2e166f3d917a98384f3a157622 in / 
# Mon, 07 Aug 2023 19:42:02 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 04:48:15 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 09 Aug 2023 04:48:17 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 09 Aug 2023 04:48:17 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 09 Aug 2023 04:48:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 09 Aug 2023 04:48:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Wed, 09 Aug 2023 04:48:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 09 Aug 2023 04:48:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 09 Aug 2023 04:48:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 09 Aug 2023 05:07:07 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 17 Aug 2023 23:15:50 GMT
ENV PHP_VERSION=8.2.9
# Thu, 17 Aug 2023 23:15:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.9.tar.xz.asc
# Thu, 17 Aug 2023 23:15:51 GMT
ENV PHP_SHA256=1e6cb77f997613864ab3127fbfc6a8c7fdaa89a95e8ed6167617b913b4de4765
# Thu, 17 Aug 2023 23:15:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Aug 2023 23:15:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Aug 2023 23:21:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Aug 2023 23:21:40 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 17 Aug 2023 23:21:41 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Aug 2023 23:21:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Aug 2023 23:21:41 GMT
WORKDIR /var/www/html
# Thu, 17 Aug 2023 23:21:41 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 17 Aug 2023 23:21:41 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Aug 2023 23:21:42 GMT
EXPOSE 9000
# Thu, 17 Aug 2023 23:21:42 GMT
CMD ["php-fpm"]
# Fri, 18 Aug 2023 00:49:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 18 Aug 2023 00:49:41 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 18 Aug 2023 00:49:41 GMT
COPY file:57a209d1c54d80b9471ec2393baac168e72338a189d9d79c9b885adb816fa7a3 in /usr/local/bin/ 
# Fri, 18 Aug 2023 00:49:41 GMT
ENV DRUPAL_VERSION=10.1.2
# Fri, 18 Aug 2023 00:49:41 GMT
WORKDIR /opt/drupal
# Fri, 18 Aug 2023 00:49:54 GMT
RUN set -eux; 	export COMPOSER_HOME="$(mktemp -d)"; 	composer create-project --no-interaction "drupal/recommended-project:$DRUPAL_VERSION" ./; 	chown -R www-data:www-data web/sites web/modules web/themes; 	rmdir /var/www/html; 	ln -sf /opt/drupal/web /var/www/html; 	rm -rf "$COMPOSER_HOME"
# Fri, 18 Aug 2023 00:50:01 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/opt/drupal/vendor/bin
```

-	Layers:
	-	`sha256:b69f31b9e61dae76a66eb3f9dd10f9f86d10116c6339347c47739dcf850af4d3`  
		Last Modified: Mon, 07 Aug 2023 19:42:48 GMT  
		Size: 3.2 MB (3175974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ddd9810e38ade4edb33de878142288e25baf77eda87b2a3363e97a58d4e7060`  
		Last Modified: Wed, 09 Aug 2023 06:27:47 GMT  
		Size: 1.9 MB (1947170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e098e94dfa574a06fbd59f9eaf19ed33840ae1cd9fcf8126f68887ce4b150c`  
		Last Modified: Wed, 09 Aug 2023 06:27:46 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad968e05b291295ac69fa36a11daaa02c3c7f6dbc64035ebe1a887b06fda8abf`  
		Last Modified: Wed, 09 Aug 2023 06:27:46 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c0086add9f5c5d92fd6848982c3aa2044400ba3053144f49e54770cfe778eb4`  
		Last Modified: Thu, 17 Aug 2023 23:33:38 GMT  
		Size: 12.1 MB (12056172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ef08676325e17d04f8d16335d5f6ab707f2cf31e0131767a9c20a20e21a4ba`  
		Last Modified: Thu, 17 Aug 2023 23:33:37 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8d11b19c923838e0c3c439a57b7af1454f2ba869e07eaf86a52e9e4bc7cbe7`  
		Last Modified: Thu, 17 Aug 2023 23:33:54 GMT  
		Size: 11.9 MB (11899322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f069b6d8365c440ebaa6ed454221bea8cb4dedd28ffd989ae7ff274dfdb3f21`  
		Last Modified: Thu, 17 Aug 2023 23:33:52 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3521a4f2bb176fa03996bf9b8d45724350acfa640b289c285180b5766ca1637`  
		Last Modified: Thu, 17 Aug 2023 23:33:52 GMT  
		Size: 18.8 KB (18800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6dfc47ee1c56973bef33f7f954c291d82fb7cd23ed287cee3f60469e03093c`  
		Last Modified: Thu, 17 Aug 2023 23:33:52 GMT  
		Size: 9.2 KB (9183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001f21aeb77a6745515318c5e8841aec2cda10e43134cdde9c9a9c423e2b9c6a`  
		Last Modified: Fri, 18 Aug 2023 01:03:26 GMT  
		Size: 1.8 MB (1811851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:713f77fb55dffcb5c507753834ccce088ad6da770aa05740051187b8149d1952`  
		Last Modified: Fri, 18 Aug 2023 01:03:26 GMT  
		Size: 312.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e3bd30610609cbbe9a4b4de091cc328c15eb22fe83ba02b0732bb5aafb83234`  
		Last Modified: Fri, 18 Aug 2023 01:03:26 GMT  
		Size: 698.2 KB (698238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1b9104cfe20e6bd8ba5c803b66046fbd88717f22ef5800f9f3ccbc89964fa2e`  
		Last Modified: Fri, 18 Aug 2023 01:03:26 GMT  
		Size: 149.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3eb33f44cd07c014a2442b15c83ebe8c497e2b98bc1d9ad3cf0d9858f0efc75`  
		Last Modified: Fri, 18 Aug 2023 01:03:30 GMT  
		Size: 18.5 MB (18507056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
