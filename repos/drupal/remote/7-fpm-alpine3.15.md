## `drupal:7-fpm-alpine3.15`

```console
$ docker pull drupal@sha256:c1607d3a2eb0e33b2e7db0ce75c6251f73aab718550437071f37604c68a2966d
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

### `drupal:7-fpm-alpine3.15` - linux; amd64

```console
$ docker pull drupal@sha256:71d4b606d3c76e5fe72e172f8d04b71db808c4fbb93e230d3e6b4d48d5f9375e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32086860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1f400ab1f935adb9c8983279509822e9bbbffc0c761b8bbf44444788ed9ff835`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Thu, 06 Oct 2022 23:34:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 06 Oct 2022 23:34:31 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 06 Oct 2022 23:34:31 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 06 Oct 2022 23:34:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 06 Oct 2022 23:34:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 06 Oct 2022 23:34:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 06 Oct 2022 23:34:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 06 Oct 2022 23:34:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 07 Oct 2022 00:46:00 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 07 Oct 2022 00:46:00 GMT
ENV PHP_VERSION=7.4.32
# Fri, 07 Oct 2022 00:46:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Fri, 07 Oct 2022 00:46:00 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Fri, 07 Oct 2022 00:46:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 07 Oct 2022 00:46:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 07 Oct 2022 00:52:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 07 Oct 2022 00:52:53 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 07 Oct 2022 00:52:54 GMT
RUN docker-php-ext-enable sodium
# Fri, 07 Oct 2022 00:52:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 07 Oct 2022 00:52:55 GMT
WORKDIR /var/www/html
# Fri, 07 Oct 2022 00:52:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 07 Oct 2022 00:52:55 GMT
STOPSIGNAL SIGQUIT
# Fri, 07 Oct 2022 00:52:55 GMT
EXPOSE 9000
# Fri, 07 Oct 2022 00:52:55 GMT
CMD ["php-fpm"]
# Fri, 07 Oct 2022 07:01:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 07:01:54 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 07 Oct 2022 07:07:54 GMT
ENV DRUPAL_VERSION=7.92
# Fri, 07 Oct 2022 07:07:54 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Fri, 07 Oct 2022 07:07:56 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:442a61c63ceec3c20b6f19e35cb326055977dd34ecd556ce0b1f259b4deb2811`  
		Last Modified: Fri, 07 Oct 2022 01:01:58 GMT  
		Size: 1.7 MB (1714315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40ecb9ad4887ee043c35bdc43fbcbe19410538db2a2dfcc338b7a19d667f6b0d`  
		Last Modified: Fri, 07 Oct 2022 01:01:58 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa18066724a6bc8d6344f4910a873654708fdaaedc58dadef81ecfa31625752`  
		Last Modified: Fri, 07 Oct 2022 01:01:57 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de38ae237c7c3fb398d4deb7ccfb174ef31da1d952263fc49c20f071e29c3228`  
		Last Modified: Fri, 07 Oct 2022 01:09:41 GMT  
		Size: 10.4 MB (10439235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71d937b9c6951f4354a3829a2971f33f2f4b1a76b7318d5ea78affd9847278d3`  
		Last Modified: Fri, 07 Oct 2022 01:09:40 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c45552b77aeb389faa6767d71672c0bfb3196d765bf56f94dcf3e58965150f5`  
		Last Modified: Fri, 07 Oct 2022 01:10:06 GMT  
		Size: 11.4 MB (11439068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9554b96399e257e83e3d34d83063c1f3b21be9eaf6117d9a72812712230e9e6a`  
		Last Modified: Fri, 07 Oct 2022 01:10:04 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadb8d597ee9c6cf070e4392abab1aa691317edc04d7f1d8746a1acb38cfcee6`  
		Last Modified: Fri, 07 Oct 2022 01:10:04 GMT  
		Size: 18.7 KB (18678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2810ce1ee32e6241cb8078f55b90b2d41037d1dac0e144e6cbc7441d3919f8`  
		Last Modified: Fri, 07 Oct 2022 01:10:04 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0090348d4c880a0400c2f3420177198db58790ebf708111c617ff35eb198c63`  
		Last Modified: Fri, 07 Oct 2022 07:27:45 GMT  
		Size: 2.2 MB (2241722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8310b62c682274d4f3295a3e9aefc51c16f86fa16e8619a97e2b4a4663b49bee`  
		Last Modified: Fri, 07 Oct 2022 07:27:44 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72fafdf7eb13ba4a7a06cb25aabfc94b9fec8611bb3c21b72c01eac90b107a5`  
		Last Modified: Fri, 07 Oct 2022 07:36:21 GMT  
		Size: 3.4 MB (3397089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-fpm-alpine3.15` - linux; arm variant v6

```console
$ docker pull drupal@sha256:00e350b5563107e8016b77d10aaa643e90050c08f0ac737b12f8312c447c112d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31168438 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2081462ffe5d24862610b5cefcc885594a94288d37d8bef5b65107c9ee1b90da`
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
# Thu, 29 Sep 2022 17:45:52 GMT
ENV DRUPAL_VERSION=7.92
# Thu, 29 Sep 2022 17:45:53 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Thu, 29 Sep 2022 17:45:54 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
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
	-	`sha256:9e665dc3c076171fe60cefc4f04c798f09899cef5a87e3d09aab0097e92fb423`  
		Last Modified: Thu, 29 Sep 2022 17:54:22 GMT  
		Size: 3.4 MB (3397081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-fpm-alpine3.15` - linux; arm variant v7

```console
$ docker pull drupal@sha256:19fb77e614c3d3d3d29e7dfc445c93feec997b688f374d963f282eeab8f2e077
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.0 MB (30013886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4edde6cdf3c4fa722954801bc33e98ecd83be22ef03ed92bb13183a7814b6864`
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
# Thu, 29 Sep 2022 22:17:06 GMT
ENV DRUPAL_VERSION=7.92
# Thu, 29 Sep 2022 22:17:06 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Thu, 29 Sep 2022 22:17:07 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
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
	-	`sha256:4e9a7596edbc799133f94e2f5607cf5e36dfc9cfad2281b52df30d98d8430977`  
		Last Modified: Thu, 29 Sep 2022 23:10:12 GMT  
		Size: 3.4 MB (3397079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-fpm-alpine3.15` - linux; arm64 variant v8

```console
$ docker pull drupal@sha256:acca446a28411167cf9b8ef70bffa7d29b08e68e4899ba24558c369eae95be66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31764128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92ab86866eb8918ee080c9406cab1d041d6db3324af465aca5c4a1e9cfc9d426`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:51 GMT
ADD file:4b51a9d40f20d2beb29d0759b161d2b9403493453beb509de4e86a5d98513f16 in / 
# Tue, 09 Aug 2022 17:39:51 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 02:03:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 07 Oct 2022 02:03:49 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 07 Oct 2022 02:03:50 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 07 Oct 2022 02:03:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 07 Oct 2022 02:03:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 07 Oct 2022 02:03:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 07 Oct 2022 02:03:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 07 Oct 2022 02:03:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 07 Oct 2022 03:34:14 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 07 Oct 2022 03:34:14 GMT
ENV PHP_VERSION=7.4.32
# Fri, 07 Oct 2022 03:34:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Fri, 07 Oct 2022 03:34:16 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Fri, 07 Oct 2022 03:34:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 07 Oct 2022 03:34:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 07 Oct 2022 03:41:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 07 Oct 2022 03:41:24 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 07 Oct 2022 03:41:25 GMT
RUN docker-php-ext-enable sodium
# Fri, 07 Oct 2022 03:41:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 07 Oct 2022 03:41:27 GMT
WORKDIR /var/www/html
# Fri, 07 Oct 2022 03:41:28 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 07 Oct 2022 03:41:29 GMT
STOPSIGNAL SIGQUIT
# Fri, 07 Oct 2022 03:41:30 GMT
EXPOSE 9000
# Fri, 07 Oct 2022 03:41:31 GMT
CMD ["php-fpm"]
# Fri, 07 Oct 2022 09:11:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 09:12:00 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 07 Oct 2022 09:22:13 GMT
ENV DRUPAL_VERSION=7.92
# Fri, 07 Oct 2022 09:22:14 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Fri, 07 Oct 2022 09:22:16 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:47517142f6ba87eca6b7bdca1e0df160b74671c81e4b9605dad38c1862a43be3`  
		Last Modified: Tue, 09 Aug 2022 17:40:55 GMT  
		Size: 2.7 MB (2718439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ef4160b59db95388d7d1f40edd7ea55620908d359e7f9a50b8f0b9e5af3518d`  
		Last Modified: Fri, 07 Oct 2022 03:55:04 GMT  
		Size: 1.7 MB (1714903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:889dbf78a331b35c50db2692b30ee48ce3f969825e2e94195a452d0ffd1d7d31`  
		Last Modified: Fri, 07 Oct 2022 03:55:03 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4828cd345bac85039fea07a4bb41833d839b35e754ff2d0a81f5addbfb65b6c2`  
		Last Modified: Fri, 07 Oct 2022 03:55:03 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f585b703e583d3c2f3fc1872eb2bff8b2ff47cb36c8518e8359085466cf3f83b`  
		Last Modified: Fri, 07 Oct 2022 04:04:22 GMT  
		Size: 10.4 MB (10439000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75d3333032a566c7075464eb2f2011b166d0c7ba73eebdc0df9d5956ac568f8f`  
		Last Modified: Fri, 07 Oct 2022 04:04:21 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:516d6fcf2a8d9ccd65a737610ca198117b20172bb461c473559b46c5f3118533`  
		Last Modified: Fri, 07 Oct 2022 04:04:50 GMT  
		Size: 11.3 MB (11265052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3efbaa92960fbc940628e1c0f03a1a571b730ce9fe6fd3f43c0c406d6d500afa`  
		Last Modified: Fri, 07 Oct 2022 04:04:48 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4787d27eb4564058d58424e296b042bd02d8845b27518c9283f680eee83f01c0`  
		Last Modified: Fri, 07 Oct 2022 04:04:48 GMT  
		Size: 18.6 KB (18569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfd013db2ac0440905d6233053f8b32a959de417acd963e716cb2cb935eec954`  
		Last Modified: Fri, 07 Oct 2022 04:04:48 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe381f196955a6cc9572812e3b35b79dedb9c32d1f00059f28c5ac5ba42c2ce7`  
		Last Modified: Fri, 07 Oct 2022 09:48:54 GMT  
		Size: 2.2 MB (2198204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6819a5c71362a2e726f1f7b57e25bd0d618422ba5799314b6da917c9cd7312`  
		Last Modified: Fri, 07 Oct 2022 09:48:54 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d663f4db9cae662edabe580026efd9ed4a443b6ef2513c07180877f64183fe0`  
		Last Modified: Fri, 07 Oct 2022 09:58:28 GMT  
		Size: 3.4 MB (3396797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-fpm-alpine3.15` - linux; 386

```console
$ docker pull drupal@sha256:f95f46df3c03d0ad0e9fca7f5c5a0e5c6d10062b956b8ded72ce26e99d357f70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32550221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f872fe8f91e57ae22374f6047545655b04e547c54fcdc29a43fca826c792c8b4`
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
# Fri, 07 Oct 2022 03:14:23 GMT
ENV DRUPAL_VERSION=7.92
# Fri, 07 Oct 2022 03:14:24 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Fri, 07 Oct 2022 03:14:26 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
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
	-	`sha256:d5c554a1b18ee40562071c0db39893b24d06ff21dcb038bb0f74f6a026f47a14`  
		Last Modified: Fri, 07 Oct 2022 03:52:45 GMT  
		Size: 3.4 MB (3396797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-fpm-alpine3.15` - linux; ppc64le

```console
$ docker pull drupal@sha256:0cf21ae70fabcd21762f6c5f4f6438249680d9dc2f5b0bf2186be723623336f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33041791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d129c78d70b3941edaff06bbff39c582b46373a14a9d0cead8940d70bf95fba7`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:20 GMT
ADD file:be31abb0aba89ed5ff9200736a1c46091abc3845d0e332efd5e5c874ef2c99d1 in / 
# Tue, 09 Aug 2022 17:17:21 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 00:16:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 07 Oct 2022 00:16:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 07 Oct 2022 00:16:09 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 07 Oct 2022 00:16:10 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 07 Oct 2022 00:16:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 07 Oct 2022 00:16:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 07 Oct 2022 00:16:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 07 Oct 2022 00:16:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 07 Oct 2022 01:50:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 07 Oct 2022 01:50:02 GMT
ENV PHP_VERSION=7.4.32
# Fri, 07 Oct 2022 01:50:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Fri, 07 Oct 2022 01:50:02 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Fri, 07 Oct 2022 01:50:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 07 Oct 2022 01:50:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 07 Oct 2022 01:59:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 07 Oct 2022 01:59:38 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 07 Oct 2022 01:59:40 GMT
RUN docker-php-ext-enable sodium
# Fri, 07 Oct 2022 01:59:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 07 Oct 2022 01:59:40 GMT
WORKDIR /var/www/html
# Fri, 07 Oct 2022 01:59:41 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 07 Oct 2022 01:59:42 GMT
STOPSIGNAL SIGQUIT
# Fri, 07 Oct 2022 01:59:42 GMT
EXPOSE 9000
# Fri, 07 Oct 2022 01:59:42 GMT
CMD ["php-fpm"]
# Fri, 07 Oct 2022 08:40:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 08:40:44 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 07 Oct 2022 08:49:26 GMT
ENV DRUPAL_VERSION=7.92
# Fri, 07 Oct 2022 08:49:27 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Fri, 07 Oct 2022 08:49:29 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:deb7065b3304c3a9834f31b8a53e8d6089060e9c6522668abd22f1f4d9f52ca7`  
		Last Modified: Tue, 09 Aug 2022 17:18:45 GMT  
		Size: 2.8 MB (2812989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a95c73f7a3c32a8bc59a8cfd4ba6b491407a1ab76333dff422ca76f9b298f4f`  
		Last Modified: Fri, 07 Oct 2022 02:14:32 GMT  
		Size: 1.8 MB (1762301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8742d5d79b941a6dbaebe4c0c07389415e5fc9874cf767d1a09a4e847c89ad55`  
		Last Modified: Fri, 07 Oct 2022 02:14:32 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1140a353543e91674064708467958bbfae46120db8560786aeafd2cae15c784c`  
		Last Modified: Fri, 07 Oct 2022 02:14:32 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8197cafbe5b71e13ffdfc352ce9f2e48d46c70b06535e3630f955786c20986cc`  
		Last Modified: Fri, 07 Oct 2022 02:24:31 GMT  
		Size: 10.4 MB (10439254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824b570812b5114708df8a89328caff822e1d8174421e103eb63521ac95d3c51`  
		Last Modified: Fri, 07 Oct 2022 02:24:30 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65abe89b9080bcf580718933be29dd715221e5cc657388374a90f434d5b859b4`  
		Last Modified: Fri, 07 Oct 2022 02:25:05 GMT  
		Size: 12.2 MB (12152365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c3526d45361b67cf1b95781287a52e6339d3e022daa27a631c29ae1e7138e70`  
		Last Modified: Fri, 07 Oct 2022 02:25:01 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e96ec668c6d06be3319926ec1b29defd38ff1d045b8be90aeab9abd9b997a89`  
		Last Modified: Fri, 07 Oct 2022 02:25:01 GMT  
		Size: 18.7 KB (18673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d5d1b8862fd5905585be1c02efa3e3e8a0cc0e95817c5f56e4070eaceaa496`  
		Last Modified: Fri, 07 Oct 2022 02:25:01 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5301a78c2bbea7f536920fd364a3154577abcec2eef4cf232fc817c0cfbd9f`  
		Last Modified: Fri, 07 Oct 2022 09:16:54 GMT  
		Size: 2.4 MB (2445886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e785a846d7d43d4309560f192b16f968f7101b51b1017e71b566450f597c54f5`  
		Last Modified: Fri, 07 Oct 2022 09:16:53 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65891f5634516e655a5da52ad6f5e2c18010e5646aa48bab527e692f32716bf9`  
		Last Modified: Fri, 07 Oct 2022 09:29:03 GMT  
		Size: 3.4 MB (3397074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `drupal:7-fpm-alpine3.15` - linux; s390x

```console
$ docker pull drupal@sha256:25abd1ddaf867b4d3d9702169101b69c4f9b242d776aeff9b3b82e54c71e3c4c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.5 MB (31518475 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:439d4092c75e31c83c885ece3f41cfe496710031cb6f70fe162403414e943422`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:54 GMT
ADD file:7489fa84133e97e4f40b13dd5159989b3594c9627d9147bfc4e33134944cc368 in / 
# Tue, 09 Aug 2022 17:41:54 GMT
CMD ["/bin/sh"]
# Fri, 07 Oct 2022 01:41:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 07 Oct 2022 01:41:14 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 07 Oct 2022 01:41:15 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 07 Oct 2022 01:41:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 07 Oct 2022 01:41:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 07 Oct 2022 01:41:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 07 Oct 2022 01:41:18 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 07 Oct 2022 01:41:18 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 07 Oct 2022 03:07:12 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 07 Oct 2022 03:07:12 GMT
ENV PHP_VERSION=7.4.32
# Fri, 07 Oct 2022 03:07:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.32.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.32.tar.xz.asc
# Fri, 07 Oct 2022 03:07:12 GMT
ENV PHP_SHA256=323332c991e8ef30b1d219cb10f5e30f11b5f319ce4c6642a5470d75ade7864a
# Fri, 07 Oct 2022 03:07:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 07 Oct 2022 03:07:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 07 Oct 2022 03:13:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 07 Oct 2022 03:13:32 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 07 Oct 2022 03:13:33 GMT
RUN docker-php-ext-enable sodium
# Fri, 07 Oct 2022 03:13:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 07 Oct 2022 03:13:34 GMT
WORKDIR /var/www/html
# Fri, 07 Oct 2022 03:13:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 07 Oct 2022 03:13:35 GMT
STOPSIGNAL SIGQUIT
# Fri, 07 Oct 2022 03:13:35 GMT
EXPOSE 9000
# Fri, 07 Oct 2022 03:13:35 GMT
CMD ["php-fpm"]
# Fri, 07 Oct 2022 11:09:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		coreutils 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 		postgresql-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg=/usr/include 		--with-webp 	; 		docker-php-ext-install -j "$(nproc)" 		gd 		opcache 		pdo_mysql 		pdo_pgsql 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .drupal-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 07 Oct 2022 11:09:49 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 07 Oct 2022 11:22:00 GMT
ENV DRUPAL_VERSION=7.92
# Fri, 07 Oct 2022 11:22:00 GMT
ENV DRUPAL_MD5=7f95bd4a6693ed5215aba4038c23c933
# Fri, 07 Oct 2022 11:22:02 GMT
RUN set -eux; 	curl -fSL "https://ftp.drupal.org/files/projects/drupal-${DRUPAL_VERSION}.tar.gz" -o drupal.tar.gz; 	echo "${DRUPAL_MD5} *drupal.tar.gz" | md5sum -c -; 	tar -xz --strip-components=1 -f drupal.tar.gz; 	rm drupal.tar.gz; 	chown -R www-data:www-data sites modules themes
```

-	Layers:
	-	`sha256:cdf710f5b7ee39c5124c50c753228dc9b8b1c1c0a1a38f1413487548565445c3`  
		Last Modified: Tue, 09 Aug 2022 17:42:56 GMT  
		Size: 2.6 MB (2606087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4016245521e8cb672f9b3d3192e643407660e1415a632bc4b0c2a90e3623d58`  
		Last Modified: Fri, 07 Oct 2022 03:28:01 GMT  
		Size: 1.8 MB (1774941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a74f4aa98ca85719e45f5094ba35ecb50114c5487399b322bca2000d6b216608`  
		Last Modified: Fri, 07 Oct 2022 03:28:01 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8d3c1f2848261ceb82465b2fca705caae3fdfdfaf9e7d96134d73bfeb6855f3`  
		Last Modified: Fri, 07 Oct 2022 03:28:01 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90f9c0dfa2306cc7989e5ad11590368f4fd4f77421bb4be8fccde47ba5af84c1`  
		Last Modified: Fri, 07 Oct 2022 03:34:28 GMT  
		Size: 10.4 MB (10439251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a40cdf3842d76b9f0c63cbbb7517cc326e21856aed1b24277f1bfc39972f40f`  
		Last Modified: Fri, 07 Oct 2022 03:34:27 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:143bb1c460ac463eed0b40509c255950a603b9e23c6f6641688d56552a20f46b`  
		Last Modified: Fri, 07 Oct 2022 03:34:48 GMT  
		Size: 11.0 MB (11023004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8331bfdbbb683f7a6838911017c4b964207a17c90ff6fe4c52ca178add9229`  
		Last Modified: Fri, 07 Oct 2022 03:34:46 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64df2759a413c09fe6b6893f00279614ab38778054f12896c8156805539e2c05`  
		Last Modified: Fri, 07 Oct 2022 03:34:46 GMT  
		Size: 18.7 KB (18695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eb0c3b7e084355ebc7e51d4c25369846dd6eb02f07ec025968e54441949b843`  
		Last Modified: Fri, 07 Oct 2022 03:34:46 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0007affec2adc723450d975626e1a83214df5b691a8f6ead8a3b4dfd17784d`  
		Last Modified: Fri, 07 Oct 2022 11:38:20 GMT  
		Size: 2.2 MB (2246177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc5cc3332028558e51f23059717e3d7fa1c663834bd26fab20d3c0adc23bed2`  
		Last Modified: Fri, 07 Oct 2022 11:38:20 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37103660f7dd7d88b77e6dcffc5a6d01850469451c7d6a5d734285db6d6d14e5`  
		Last Modified: Fri, 07 Oct 2022 11:43:19 GMT  
		Size: 3.4 MB (3397078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
