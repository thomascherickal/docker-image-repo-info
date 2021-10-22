## `postfixadmin:fpm-alpine`

```console
$ docker pull postfixadmin@sha256:cff3bc9d5d4bd243a26745defa182d1f222533a9586ae2a5bf1d32b1879c6b89
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

### `postfixadmin:fpm-alpine` - linux; amd64

```console
$ docker pull postfixadmin@sha256:ca69fe4371376e120a90ef4a272b7e484c0fb1f8e25f63400dfd8ef694401787
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.3 MB (35261746 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1753da47b74174cf8a1fff4487edc7f0e25df9a1005c26c54e209033f3bed08f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 21:00:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 27 Aug 2021 21:00:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 27 Aug 2021 21:00:52 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 27 Aug 2021 21:00:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 27 Aug 2021 21:00:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 27 Aug 2021 21:00:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 21:00:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 21:00:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 27 Aug 2021 21:42:08 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 24 Sep 2021 00:41:47 GMT
ENV PHP_VERSION=7.4.24
# Fri, 24 Sep 2021 00:41:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Fri, 24 Sep 2021 00:41:47 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Fri, 24 Sep 2021 00:42:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 24 Sep 2021 00:42:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Oct 2021 00:02:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 15 Oct 2021 00:02:19 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 15 Oct 2021 00:02:21 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 Oct 2021 00:02:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 Oct 2021 00:02:21 GMT
WORKDIR /var/www/html
# Fri, 15 Oct 2021 00:02:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 15 Oct 2021 00:02:22 GMT
STOPSIGNAL SIGQUIT
# Fri, 15 Oct 2021 00:02:23 GMT
EXPOSE 9000
# Fri, 15 Oct 2021 00:02:23 GMT
CMD ["php-fpm"]
# Thu, 21 Oct 2021 20:00:04 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 21 Oct 2021 20:00:06 GMT
RUN apk add --no-cache 		bash 		su-exec
# Thu, 21 Oct 2021 20:00:34 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 21 Oct 2021 20:00:34 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Thu, 21 Oct 2021 20:00:35 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 21 Oct 2021 20:00:35 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Thu, 21 Oct 2021 20:00:35 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 21 Oct 2021 20:00:36 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 21 Oct 2021 20:00:37 GMT
COPY file:dd64bcdfb88c8d8226922cdb27ef4f39484186ee00149b5e857b343561566a74 in /usr/local/bin/ 
# Thu, 21 Oct 2021 20:00:37 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 21 Oct 2021 20:00:37 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:153eea49496a46a69cf5f48803e9014824a6be1d3e04f9ee47cd3f395aba6d76`  
		Last Modified: Fri, 27 Aug 2021 22:41:22 GMT  
		Size: 1.7 MB (1707843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11efd0df1fcb3f56e825ef3449f199b261f44e0130a10cb77fcf78339cb88173`  
		Last Modified: Fri, 27 Aug 2021 22:41:22 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3f3214c344df86e90fe2ae24d643d9dbc5dcfd6f229f4ee58f7c60c6f0cc895`  
		Last Modified: Fri, 27 Aug 2021 22:41:22 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11801e573c1ee31d53c6decdf5375edd55e8decaffec447068657a3233118e31`  
		Last Modified: Fri, 24 Sep 2021 01:42:42 GMT  
		Size: 10.4 MB (10392314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831aca17040b231f3b58011e30b649d9f23aa0c6951694b2c36d798f92c5c6fc`  
		Last Modified: Fri, 24 Sep 2021 01:42:40 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caf190cc16814e15d6004b9b48494f81506ec7c62b0a4b1a523553edf6f6dad4`  
		Last Modified: Fri, 15 Oct 2021 02:38:04 GMT  
		Size: 14.6 MB (14603306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5c98fdc2ee2dbc34288553c31192ac19650f48de7dd3950fcee603e17ca2b3`  
		Last Modified: Fri, 15 Oct 2021 02:38:01 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022cb9b83caff15b341182ded42e25c68807659b9a8416fb470107ba38b4e982`  
		Last Modified: Fri, 15 Oct 2021 02:38:00 GMT  
		Size: 17.8 KB (17836 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244ad0d274e9449bf7f844462c4ea262ccce9bf67c77e7d66c422887648fe407`  
		Last Modified: Fri, 15 Oct 2021 02:38:00 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea17547203b625da283a35a0acb8bf618215505f7cd7bc05f8ab92e22c74fc58`  
		Last Modified: Thu, 21 Oct 2021 20:01:59 GMT  
		Size: 467.6 KB (467622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ac61d2ee987ae4093bdec0a97aff758b91da449d3043fb5cc6b150d43b0eed`  
		Last Modified: Thu, 21 Oct 2021 20:01:58 GMT  
		Size: 3.4 MB (3379086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3b58784c6d485e0756133af7a7a9227eb65359c1c76476f33f60dc185510277`  
		Last Modified: Thu, 21 Oct 2021 20:01:59 GMT  
		Size: 1.9 MB (1864929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d074111ce47c6d6809e5a0ccb421d2b00635139306bf6dd62c9433ac2a51aa0`  
		Last Modified: Thu, 21 Oct 2021 20:01:58 GMT  
		Size: 1.6 KB (1593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; arm variant v6

```console
$ docker pull postfixadmin@sha256:cd164e266be385f9679ceb197e709ed0d8d8476fdf2a93a9b32ae53ac71967e7
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33702653 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8be6380276c710e97d1257ade8b8f59465d85529fea5967a546eb28f9db25020`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 27 Aug 2021 17:49:29 GMT
ADD file:1c1c4520d49cb6e8f795f3b953d1ed3c3c77868b98b53a455169c254fcec5acd in / 
# Fri, 27 Aug 2021 17:49:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 20:48:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 27 Aug 2021 20:48:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 27 Aug 2021 20:48:06 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 27 Aug 2021 20:48:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 27 Aug 2021 20:48:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 27 Aug 2021 20:48:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 20:48:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 20:48:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 27 Aug 2021 21:09:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Sep 2021 21:20:01 GMT
ENV PHP_VERSION=7.4.24
# Thu, 23 Sep 2021 21:20:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Thu, 23 Sep 2021 21:20:02 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Thu, 23 Sep 2021 21:20:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 23 Sep 2021 21:20:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 Oct 2021 20:51:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 14 Oct 2021 20:51:24 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 14 Oct 2021 20:51:26 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 Oct 2021 20:51:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 Oct 2021 20:51:27 GMT
WORKDIR /var/www/html
# Thu, 14 Oct 2021 20:51:29 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 14 Oct 2021 20:51:29 GMT
STOPSIGNAL SIGQUIT
# Thu, 14 Oct 2021 20:51:30 GMT
EXPOSE 9000
# Thu, 14 Oct 2021 20:51:30 GMT
CMD ["php-fpm"]
# Fri, 15 Oct 2021 00:38:35 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 15 Oct 2021 00:38:38 GMT
RUN apk add --no-cache 		bash 		su-exec
# Fri, 15 Oct 2021 00:40:04 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 15 Oct 2021 00:40:04 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Fri, 15 Oct 2021 00:40:05 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 15 Oct 2021 00:40:05 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Fri, 15 Oct 2021 00:40:05 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 15 Oct 2021 00:40:09 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 15 Oct 2021 00:40:09 GMT
COPY file:dd64bcdfb88c8d8226922cdb27ef4f39484186ee00149b5e857b343561566a74 in /usr/local/bin/ 
# Fri, 15 Oct 2021 00:40:10 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 15 Oct 2021 00:40:10 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:2e78c0f86ba9a1fed30df20cb48c9cc73e9626399f12749d36b892ff99c0ecf5`  
		Last Modified: Fri, 27 Aug 2021 17:50:55 GMT  
		Size: 2.6 MB (2627447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05720bf4927bb754d842782fff2d045d42b804759e30b8312cbf75272e200af`  
		Last Modified: Fri, 27 Aug 2021 21:55:19 GMT  
		Size: 1.7 MB (1696736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c9951b98a5bb83a868efe164832e7d1a35e9a078a82219f95634454a864a332`  
		Last Modified: Fri, 27 Aug 2021 21:55:18 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a6baa29c72aee654b7205fcfbde95333a6e9a5dfadc1a99d94e64c957f543ac`  
		Last Modified: Fri, 27 Aug 2021 21:55:18 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f93eacfb7dfae0e34322570ccf553900fa76e5ee2544d7db5bed09aa3cc3bf24`  
		Last Modified: Thu, 23 Sep 2021 22:34:24 GMT  
		Size: 10.4 MB (10392323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d380197e3ca66e5873002b5b8217c9aa20c03d4d6db1be92b40a472f9049691d`  
		Last Modified: Thu, 23 Sep 2021 22:34:22 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:321e940eb4f8b29480966819e792fe9c3683c27dde46c00857aa3b448f3483a6`  
		Last Modified: Thu, 14 Oct 2021 21:59:25 GMT  
		Size: 13.6 MB (13592181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5beec81e89829a17b04186cf481d1de8e86bbfabb856419c2a8a17a7bddd663a`  
		Last Modified: Thu, 14 Oct 2021 21:59:16 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6347cacbb30bcbbb3295a52add6d31143de0a6e3049aa4de35f7d871664eefa2`  
		Last Modified: Thu, 14 Oct 2021 21:59:16 GMT  
		Size: 17.9 KB (17850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2064bb0d65e56081b257b258547cebd4d56b8904892ebdd4e9af9a485830b7cc`  
		Last Modified: Thu, 14 Oct 2021 21:59:17 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:923ff3853a062549be639cc3a9dfa0d376901d31e05a87c0580866a6e3b9f5d0`  
		Last Modified: Fri, 15 Oct 2021 00:40:43 GMT  
		Size: 456.1 KB (456066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784044955aa2aa93e381a679defc713a31309f0bdc539754e49cb3146f7e893c`  
		Last Modified: Fri, 15 Oct 2021 00:40:44 GMT  
		Size: 3.0 MB (3040748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:449dcf4c2d77c5e3f21f6626127c5440054c16782a02fbb495d399d52df4f0fb`  
		Last Modified: Fri, 15 Oct 2021 00:40:44 GMT  
		Size: 1.9 MB (1864934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926596174007555bb806be51e36320597ee76f516cfb47d8db934d61098b2c12`  
		Last Modified: Fri, 15 Oct 2021 00:40:43 GMT  
		Size: 1.6 KB (1592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; arm variant v7

```console
$ docker pull postfixadmin@sha256:c9623c876accff66754daf9209361d80ddda32282442a718af00ac4f1a9ffdbb
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32583029 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c91651d7edf74a55b73a8a5b92f0a8b9a4108e59e363c7b766539dfc5eb35e56`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 27 Aug 2021 17:57:31 GMT
ADD file:a7da7992ccea54d3295231027614f138aa45c4d4a25ea6ec9bf7b316b9f67d95 in / 
# Fri, 27 Aug 2021 17:57:32 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 22:38:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 27 Aug 2021 22:38:57 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 27 Aug 2021 22:38:59 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 27 Aug 2021 22:38:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 27 Aug 2021 22:39:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 27 Aug 2021 22:39:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 22:39:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 22:39:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 27 Aug 2021 23:03:36 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Sep 2021 23:47:09 GMT
ENV PHP_VERSION=7.4.24
# Thu, 23 Sep 2021 23:47:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Thu, 23 Sep 2021 23:47:10 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Thu, 23 Sep 2021 23:47:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 23 Sep 2021 23:47:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 Oct 2021 21:59:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 14 Oct 2021 21:59:53 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 14 Oct 2021 21:59:55 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 Oct 2021 21:59:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 Oct 2021 21:59:57 GMT
WORKDIR /var/www/html
# Thu, 14 Oct 2021 21:59:59 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 14 Oct 2021 21:59:59 GMT
STOPSIGNAL SIGQUIT
# Thu, 14 Oct 2021 22:00:00 GMT
EXPOSE 9000
# Thu, 14 Oct 2021 22:00:00 GMT
CMD ["php-fpm"]
# Fri, 22 Oct 2021 02:02:13 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 22 Oct 2021 02:02:15 GMT
RUN apk add --no-cache 		bash 		su-exec
# Fri, 22 Oct 2021 02:03:36 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 22 Oct 2021 02:03:36 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Fri, 22 Oct 2021 02:03:37 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 22 Oct 2021 02:03:37 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Fri, 22 Oct 2021 02:03:38 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 22 Oct 2021 02:03:41 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 22 Oct 2021 02:03:42 GMT
COPY file:dd64bcdfb88c8d8226922cdb27ef4f39484186ee00149b5e857b343561566a74 in /usr/local/bin/ 
# Fri, 22 Oct 2021 02:03:42 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 22 Oct 2021 02:03:43 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a14774a5a62e0f454febaec7cb603e18a6a8e25ef9da4a4da85b155bdd5e5a7a`  
		Last Modified: Fri, 27 Aug 2021 17:59:00 GMT  
		Size: 2.4 MB (2430419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d1ef9481330a95ddf334887e1f8fce317a5ac59b648f285f67a4985d219de7`  
		Last Modified: Fri, 27 Aug 2021 23:55:36 GMT  
		Size: 1.6 MB (1564608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05b9b552be19301d7e17adf942310cefe01c3c4c7bfd107dfa0db3768b973a3`  
		Last Modified: Fri, 27 Aug 2021 23:55:35 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1716cacc7a16c9894f45061a30c476d428c6142feadd35c9c6d4f7f6fd3f510`  
		Last Modified: Fri, 27 Aug 2021 23:55:36 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75a6f082933109ca62a31c80caa66addab02d19528c6458b3260404f3561e98c`  
		Last Modified: Fri, 24 Sep 2021 02:03:21 GMT  
		Size: 10.4 MB (10392312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c160d1ff3fe45502a7764c4172cc1b53d7156b70c4f55e8b5c1ea55bd5e0102`  
		Last Modified: Fri, 24 Sep 2021 02:03:19 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc9835f527d0089327cd05da81beda11413467e0bb8c1a5b1399d2781ef5e0f`  
		Last Modified: Fri, 15 Oct 2021 00:54:40 GMT  
		Size: 12.7 MB (12712806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336c461a7feb6b4d6b842edf7e603d0e8c82162004e81c09b170e8e122edfe9e`  
		Last Modified: Fri, 15 Oct 2021 00:54:32 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80a25676bb6e73707eda140dd1b3464e205efa3ca7b5615f1ded3327f15b7a8`  
		Last Modified: Fri, 15 Oct 2021 00:54:32 GMT  
		Size: 17.8 KB (17837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36a7243bdfb7492edbf068c3e77636768bdae623b2780378d813f0473d0f7fa`  
		Last Modified: Fri, 15 Oct 2021 00:54:31 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81dd3d7579fc21a847758ce9640b348036c3a4cfc857f28b014000da7481882b`  
		Last Modified: Fri, 22 Oct 2021 02:06:16 GMT  
		Size: 416.5 KB (416481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa26c68284bbf9a611ae6803be1b06007486f4d80ff151651f1df867668bb0b`  
		Last Modified: Fri, 22 Oct 2021 02:06:17 GMT  
		Size: 3.2 MB (3169272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c9c471ea36dd82361bb212112b0100ab029f11270564f66b32796132cafaba`  
		Last Modified: Fri, 22 Oct 2021 02:06:18 GMT  
		Size: 1.9 MB (1864928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:218f7eacbbdec57a0307f3a33da0fbb527fa3c64726da0d34f026347de4fe9a4`  
		Last Modified: Fri, 22 Oct 2021 02:06:16 GMT  
		Size: 1.6 KB (1594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull postfixadmin@sha256:b69385633666ac05d67d0a0a9b1df76bf33c498b0cd058ad0eaaf7868c7a8211
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34688887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98a53f22ff1cd275f160a547343980a543480b6fbbd130256147157fa4afdace`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 27 Aug 2021 17:39:33 GMT
ADD file:dc8af9c7bfe9f9541e1db38dea01c4201609f3075b31e108f2073ffed8c5e4b9 in / 
# Fri, 27 Aug 2021 17:39:33 GMT
CMD ["/bin/sh"]
# Thu, 14 Oct 2021 20:36:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 14 Oct 2021 20:36:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 14 Oct 2021 20:36:51 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 14 Oct 2021 20:36:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 14 Oct 2021 20:36:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 14 Oct 2021 20:36:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 20:36:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 14 Oct 2021 20:36:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 14 Oct 2021 21:57:38 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 14 Oct 2021 21:57:39 GMT
ENV PHP_VERSION=7.4.24
# Thu, 14 Oct 2021 21:57:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Thu, 14 Oct 2021 21:57:41 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Thu, 14 Oct 2021 21:57:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 14 Oct 2021 21:57:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 Oct 2021 22:04:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 14 Oct 2021 22:04:46 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 14 Oct 2021 22:04:47 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 Oct 2021 22:04:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 Oct 2021 22:04:48 GMT
WORKDIR /var/www/html
# Thu, 14 Oct 2021 22:04:49 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 14 Oct 2021 22:04:50 GMT
STOPSIGNAL SIGQUIT
# Thu, 14 Oct 2021 22:04:51 GMT
EXPOSE 9000
# Thu, 14 Oct 2021 22:04:52 GMT
CMD ["php-fpm"]
# Thu, 21 Oct 2021 19:38:19 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 21 Oct 2021 19:38:21 GMT
RUN apk add --no-cache 		bash 		su-exec
# Thu, 21 Oct 2021 19:38:55 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 21 Oct 2021 19:38:56 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Thu, 21 Oct 2021 19:38:57 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 21 Oct 2021 19:38:58 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Thu, 21 Oct 2021 19:38:59 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Thu, 21 Oct 2021 19:39:01 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 21 Oct 2021 19:39:03 GMT
COPY file:dd64bcdfb88c8d8226922cdb27ef4f39484186ee00149b5e857b343561566a74 in /usr/local/bin/ 
# Thu, 21 Oct 2021 19:39:03 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 21 Oct 2021 19:39:04 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:552d1f2373af9bfe12033568ebbfb0ccbb0de11279f9a415a29207e264d7f4d9`  
		Last Modified: Fri, 27 Aug 2021 17:40:18 GMT  
		Size: 2.7 MB (2711827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f327d3d40ef42fee7962b876cfb120bd90ebf3bfbb01a662273165a80f532bc5`  
		Last Modified: Thu, 14 Oct 2021 23:10:23 GMT  
		Size: 1.7 MB (1711094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3586b69bdc11c600d1a1fa08218deb50a3359adfd5fe05c1401367547802557`  
		Last Modified: Thu, 14 Oct 2021 23:10:23 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226a5565cd990bb48f75a1947472074866fbc1221fc87002d4528f444557b48f`  
		Last Modified: Thu, 14 Oct 2021 23:10:23 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9bb6b5b5aab3d8651588526ac7764a08da41482115dcb6997110856520e481`  
		Last Modified: Thu, 14 Oct 2021 23:22:08 GMT  
		Size: 10.4 MB (10392104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab14c724dd071a2ebacd55a7edeed9e759593a79764a841af96747e86663c12`  
		Last Modified: Thu, 14 Oct 2021 23:22:07 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b8605805992fcbd45fdcdeb78aad828e9b24768492a6be88edec10661f8cdf9`  
		Last Modified: Thu, 14 Oct 2021 23:22:53 GMT  
		Size: 14.1 MB (14139873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:facd4415e63be6e1f911d5d0e67c2a6bff5b9e96e31887c61289c0d5b1284e62`  
		Last Modified: Thu, 14 Oct 2021 23:22:51 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3028893f7c248330e174978b85060e0b8fb57c3654830ccd2d6958a015b1bc`  
		Last Modified: Thu, 14 Oct 2021 23:22:51 GMT  
		Size: 17.7 KB (17723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df7308c705c8084466a8c7734df491e7ae7c1e847b3109c20949d381b62ceea`  
		Last Modified: Thu, 14 Oct 2021 23:22:51 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a3d51c94a069fc227b6dc60cb8677078c86b9e75e93194eb8d3720a009ed1d`  
		Last Modified: Thu, 21 Oct 2021 19:40:38 GMT  
		Size: 475.6 KB (475570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11bafdf8a8301e8bfb02c1d6411fe7786e6bae9269dc3c755fdf0a355a1796c4`  
		Last Modified: Thu, 21 Oct 2021 19:40:38 GMT  
		Size: 3.4 MB (3361591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3afe5439d10f42feb38490941ce110be9321f66b25d013e57c489cb4871c9dc4`  
		Last Modified: Thu, 21 Oct 2021 19:40:38 GMT  
		Size: 1.9 MB (1864813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39362b0b19b4b44e7233e27ca9026c0dfa821e9d956f06dd88a866b999283eb5`  
		Last Modified: Thu, 21 Oct 2021 19:40:37 GMT  
		Size: 1.6 KB (1595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; 386

```console
$ docker pull postfixadmin@sha256:76f676e66e48624882bb67929e85532af6fe473aa3ff3cf44f42d7b6b4432b44
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35855229 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:639b6509dc2d7c510f70464e09e99f852376c9a394552b3de58c7f6fb58b1dbf`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 27 Aug 2021 17:38:29 GMT
ADD file:42a7bc5a08b546b47049dd0f89ae4e7a8c86342f87000f39ade3ff52916a6c2e in / 
# Fri, 27 Aug 2021 17:38:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:59:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 27 Aug 2021 19:59:48 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 27 Aug 2021 19:59:49 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 27 Aug 2021 19:59:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 27 Aug 2021 19:59:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 27 Aug 2021 19:59:50 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 19:59:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 19:59:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 27 Aug 2021 20:38:42 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 24 Sep 2021 01:36:51 GMT
ENV PHP_VERSION=7.4.24
# Fri, 24 Sep 2021 01:36:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Fri, 24 Sep 2021 01:36:52 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Fri, 24 Sep 2021 01:37:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 24 Sep 2021 01:37:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Oct 2021 00:40:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 15 Oct 2021 00:40:37 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 15 Oct 2021 00:40:39 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 Oct 2021 00:40:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 Oct 2021 00:40:39 GMT
WORKDIR /var/www/html
# Fri, 15 Oct 2021 00:40:41 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 15 Oct 2021 00:40:41 GMT
STOPSIGNAL SIGQUIT
# Fri, 15 Oct 2021 00:40:41 GMT
EXPOSE 9000
# Fri, 15 Oct 2021 00:40:42 GMT
CMD ["php-fpm"]
# Fri, 15 Oct 2021 07:31:48 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 15 Oct 2021 07:31:49 GMT
RUN apk add --no-cache 		bash 		su-exec
# Fri, 15 Oct 2021 07:32:22 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 15 Oct 2021 07:32:22 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Fri, 15 Oct 2021 07:32:22 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 15 Oct 2021 07:32:22 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Fri, 15 Oct 2021 07:32:23 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 15 Oct 2021 07:32:24 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 15 Oct 2021 07:32:25 GMT
COPY file:dd64bcdfb88c8d8226922cdb27ef4f39484186ee00149b5e857b343561566a74 in /usr/local/bin/ 
# Fri, 15 Oct 2021 07:32:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 15 Oct 2021 07:32:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b11ae9fc5d8a106cfed3a6f6c75e5b5b5797c566fac4411622b4055df6541286`  
		Last Modified: Fri, 27 Aug 2021 17:39:18 GMT  
		Size: 2.8 MB (2822857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fa6b193871895593dd2e9300b768212b024272930161ab8524f40a5735edd63`  
		Last Modified: Fri, 27 Aug 2021 21:44:10 GMT  
		Size: 1.8 MB (1805371 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f324621ef2d45fa9d97583b1efc3fb241066b4dbf696e2dd38327a90d1e6813`  
		Last Modified: Fri, 27 Aug 2021 21:44:09 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d22e796392b3e282fea08fa6cb0da352053587b646a938425cb7c4171bf25a2`  
		Last Modified: Fri, 27 Aug 2021 21:44:09 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f678a6ab9284de86b1f53a53843b3b5ce6a0f7b7c1d1940c225655eb1719660`  
		Last Modified: Fri, 24 Sep 2021 02:36:10 GMT  
		Size: 10.4 MB (10392305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16f41f2f488250503ed8ae2aaa80d2aa859abb85073c9d32d7a7fb7d3533fe0f`  
		Last Modified: Fri, 24 Sep 2021 02:36:09 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14b702481d6779e2b200a21b90d9b494080bfb446edb30d439547e4d90128d8`  
		Last Modified: Fri, 15 Oct 2021 03:20:06 GMT  
		Size: 15.0 MB (15011404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb228f4b314a6359c5685ec2c333d7b1a881c660bdc3cb0acd1a8d84c5ce4ccd`  
		Last Modified: Fri, 15 Oct 2021 03:20:02 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e19a897a3509ae8337d965899d092d8c5e094c15ffe02826ca094ed90159e298`  
		Last Modified: Fri, 15 Oct 2021 03:20:02 GMT  
		Size: 17.8 KB (17834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940799ba862f57450d0d81bfd282ef38ccac6628868d0500c2bc34998242616f`  
		Last Modified: Fri, 15 Oct 2021 03:20:02 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b22259e39dfd90e35e96eae55cdb65f8267ab28a97d848060be9c7e03f8274a3`  
		Last Modified: Fri, 15 Oct 2021 07:34:09 GMT  
		Size: 503.7 KB (503651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b2fb0c3765edbeba209cb26830e5be651272a850e614bb91f042811bac48bb`  
		Last Modified: Fri, 15 Oct 2021 07:34:10 GMT  
		Size: 3.4 MB (3422506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70db997bfda6900537e900faf7740fe52ba472735ce424440c2c39a5b6146246`  
		Last Modified: Fri, 15 Oct 2021 07:34:10 GMT  
		Size: 1.9 MB (1864932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bca0729573ed3d296bb3997fda8feb32725b02213fade3e3e5b1f9504f476f3`  
		Last Modified: Fri, 15 Oct 2021 07:34:09 GMT  
		Size: 1.6 KB (1594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; ppc64le

```console
$ docker pull postfixadmin@sha256:c3be5d3140a50eb4b7767f94b8cc69fb133ae2c34436b985ae51cf2762cc23e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.4 MB (36412583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d257c99298a932eda75f522a6b7ac390907fe97c6f09e3d7c9c4afad61e40981`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 27 Aug 2021 19:39:54 GMT
ADD file:d213c56ffc24a5051e8060fd0fec1a0520367c10d88ab16321c36336b6c66098 in / 
# Fri, 27 Aug 2021 19:39:59 GMT
CMD ["/bin/sh"]
# Sat, 28 Aug 2021 00:22:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 28 Aug 2021 00:22:14 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 28 Aug 2021 00:22:24 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 28 Aug 2021 00:22:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 28 Aug 2021 00:22:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 28 Aug 2021 00:22:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Aug 2021 00:22:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 28 Aug 2021 00:22:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 28 Aug 2021 00:51:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 24 Sep 2021 01:47:56 GMT
ENV PHP_VERSION=7.4.24
# Fri, 24 Sep 2021 01:48:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Fri, 24 Sep 2021 01:48:10 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Fri, 24 Sep 2021 01:48:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 24 Sep 2021 01:48:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 Oct 2021 22:42:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 14 Oct 2021 22:42:26 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 14 Oct 2021 22:42:37 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 Oct 2021 22:42:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 Oct 2021 22:42:40 GMT
WORKDIR /var/www/html
# Thu, 14 Oct 2021 22:42:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 14 Oct 2021 22:42:50 GMT
STOPSIGNAL SIGQUIT
# Thu, 14 Oct 2021 22:42:52 GMT
EXPOSE 9000
# Thu, 14 Oct 2021 22:42:55 GMT
CMD ["php-fpm"]
# Fri, 22 Oct 2021 01:53:59 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 22 Oct 2021 01:54:19 GMT
RUN apk add --no-cache 		bash 		su-exec
# Fri, 22 Oct 2021 01:55:22 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 22 Oct 2021 01:55:25 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Fri, 22 Oct 2021 01:55:28 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 22 Oct 2021 01:55:30 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Fri, 22 Oct 2021 01:55:31 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 22 Oct 2021 01:55:43 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 22 Oct 2021 01:55:46 GMT
COPY file:dd64bcdfb88c8d8226922cdb27ef4f39484186ee00149b5e857b343561566a74 in /usr/local/bin/ 
# Fri, 22 Oct 2021 01:55:53 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 22 Oct 2021 01:55:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:63da8ca98f7b4b94381aed56862a60aecf355d9428b9aeb7c61d5bd017100c18`  
		Last Modified: Fri, 27 Aug 2021 19:41:06 GMT  
		Size: 2.8 MB (2812284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:317a4af98e0d6a07fca505c073eaef771202280f717e9eec5693da72e342352b`  
		Last Modified: Sat, 28 Aug 2021 01:41:31 GMT  
		Size: 1.8 MB (1753694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f45086a93088805a1f9f81303c856d62fa5a43ec294f558743c42e803fa376`  
		Last Modified: Sat, 28 Aug 2021 01:41:31 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0bbbefa425da2cee0e640dda470f0cb14892652fd6f89c03319eff15fdf1720`  
		Last Modified: Sat, 28 Aug 2021 01:41:31 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be9f2846f59e25b5d91083285c18a048a5568e5af228e1b3b3d285289bee06d0`  
		Last Modified: Fri, 24 Sep 2021 05:14:41 GMT  
		Size: 10.4 MB (10392306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08c0dfeb627997b6c7a86fb3b812740311973d42643db4951c59a6ec6648a66a`  
		Last Modified: Fri, 24 Sep 2021 05:14:38 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5770cb230e93d91939f8d5871643b9e7245d027b8b0484b4565dd28fae11937`  
		Last Modified: Fri, 15 Oct 2021 00:58:05 GMT  
		Size: 15.7 MB (15650540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7932c38884da5d26cd562b2f9898a33a8f75fd55cd8cb86b8324507b336b1a8`  
		Last Modified: Fri, 15 Oct 2021 00:57:57 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aac4eb56604f284931497aa935ad516b2cc0c916eabfd55cbc28c2f10860418`  
		Last Modified: Fri, 15 Oct 2021 00:57:57 GMT  
		Size: 17.8 KB (17840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb3b1e13a85467726add53f18dfb24816017a31da9366b6bc90e9e3d31db890`  
		Last Modified: Fri, 15 Oct 2021 00:57:57 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273a3ea21353c04be173ab7c7afaa24c923111cf25aa74ce57a5fb2b6bf1c91d`  
		Last Modified: Fri, 22 Oct 2021 01:57:38 GMT  
		Size: 532.8 KB (532811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0472aeca5365fe5b922b9356b00995f6dfe70cf2b5cb6667738c67da75c3436c`  
		Last Modified: Fri, 22 Oct 2021 01:57:38 GMT  
		Size: 3.4 MB (3373808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88aa4ab12ffcf05a1304a4496d82f913d0afe8f375bd3f830590d858fe45fffe`  
		Last Modified: Fri, 22 Oct 2021 01:57:38 GMT  
		Size: 1.9 MB (1864929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6efafdc5ed42e55a8d6d598a314b96b0e0f6bbb2d5ca4d2734eaee647c84441f`  
		Last Modified: Fri, 22 Oct 2021 01:57:38 GMT  
		Size: 1.6 KB (1596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; s390x

```console
$ docker pull postfixadmin@sha256:704cdb43ba9c45dae8766e8dcba50cea424b0ef0f7ada7a7966496b36288edde
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34115908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cbd15b9fb1ec02cdad4d4900f16ecd774a77ec71bf68e5f8aca5ffc9ec0dee2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 27 Aug 2021 17:41:29 GMT
ADD file:9b40ee281e8797067fb2ae207c406084cb81593090338a8b7cb09ade52168daa in / 
# Fri, 27 Aug 2021 17:41:30 GMT
CMD ["/bin/sh"]
# Fri, 27 Aug 2021 19:39:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 27 Aug 2021 19:39:17 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 27 Aug 2021 19:39:19 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 27 Aug 2021 19:39:20 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 27 Aug 2021 19:39:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 27 Aug 2021 19:39:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 19:39:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 27 Aug 2021 19:39:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 27 Aug 2021 20:05:34 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Sep 2021 20:56:47 GMT
ENV PHP_VERSION=7.4.24
# Thu, 23 Sep 2021 20:56:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.24.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.24.tar.xz.asc
# Thu, 23 Sep 2021 20:56:48 GMT
ENV PHP_SHA256=ff7658ee2f6d8af05b48c21146af5f502e121def4e76e862df5ec9fa06e98734
# Thu, 23 Sep 2021 20:56:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 23 Sep 2021 20:56:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 Oct 2021 21:10:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 14 Oct 2021 21:10:05 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 14 Oct 2021 21:10:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 Oct 2021 21:10:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 Oct 2021 21:10:08 GMT
WORKDIR /var/www/html
# Thu, 14 Oct 2021 21:10:09 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 14 Oct 2021 21:10:10 GMT
STOPSIGNAL SIGQUIT
# Thu, 14 Oct 2021 21:10:10 GMT
EXPOSE 9000
# Thu, 14 Oct 2021 21:10:11 GMT
CMD ["php-fpm"]
# Fri, 15 Oct 2021 00:03:02 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 15 Oct 2021 00:03:03 GMT
RUN apk add --no-cache 		bash 		su-exec
# Fri, 15 Oct 2021 00:03:25 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 15 Oct 2021 00:03:26 GMT
ARG POSTFIXADMIN_VERSION=3.3.10
# Fri, 15 Oct 2021 00:03:26 GMT
ARG POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 15 Oct 2021 00:03:26 GMT
ENV POSTFIXADMIN_VERSION=3.3.10
# Fri, 15 Oct 2021 00:03:26 GMT
ENV POSTFIXADMIN_SHA512=e00fc9ea343a928976d191adfa01020ee0c6ddbe80a39e01ca2ee414a18247958f033970f378fe4a9974636172a5e094e57117ee9ac7b930c592f433097a7aca
# Fri, 15 Oct 2021 00:03:27 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 15 Oct 2021 00:03:28 GMT
COPY file:dd64bcdfb88c8d8226922cdb27ef4f39484186ee00149b5e857b343561566a74 in /usr/local/bin/ 
# Fri, 15 Oct 2021 00:03:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 15 Oct 2021 00:03:28 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:da14cb6b6dc946dbb2d84386bcaca84e2d46f650767cd11bdb3331ec9d623988`  
		Last Modified: Fri, 27 Aug 2021 17:42:25 GMT  
		Size: 2.6 MB (2603464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ad9a79bad26bb06d3574174d09fe708da08d7c89009c1af214a9c824e97007`  
		Last Modified: Fri, 27 Aug 2021 20:52:39 GMT  
		Size: 1.8 MB (1768214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b673ca8861cb9f3ee8bc162276486c2037e038a90f72a7d1604e8df25f6c10d7`  
		Last Modified: Fri, 27 Aug 2021 20:52:39 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b1a84628a9effaa859862a214dd288520209fad79d46dc04e5559d3853ceea`  
		Last Modified: Fri, 27 Aug 2021 20:52:39 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46720fc5ed123402fe764370ef6f0feb2ed2918a5ccaee352cfc0d7d750b145`  
		Last Modified: Thu, 23 Sep 2021 22:08:04 GMT  
		Size: 10.4 MB (10392315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e88097d4dd618489dd16e3fba70151cdacab276fb4b9437d791bfb07cac054b`  
		Last Modified: Thu, 23 Sep 2021 22:08:03 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955eb3be735e94d74345a59ada608a0859bc840cfd0de8df2aea58f5362954f7`  
		Last Modified: Thu, 14 Oct 2021 22:17:35 GMT  
		Size: 14.0 MB (13975570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24c698ff633191cee7f5b884f73a9c63fe92068b40fc6e3a661aaa534d6e64d`  
		Last Modified: Thu, 14 Oct 2021 22:17:33 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5265633bb1db5d7eca99a7c2193bb8e4f4f26f2577157872bfed8ecaa974d35a`  
		Last Modified: Thu, 14 Oct 2021 22:17:33 GMT  
		Size: 17.9 KB (17857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415b2d4d560310481b50af67206ca3d906a3461dece236931ecf822793801216`  
		Last Modified: Thu, 14 Oct 2021 22:17:33 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2491afa2c0f9e24d34dcde9689bbdebdcdd2204b62c4ddc14d469e238123b38`  
		Last Modified: Fri, 15 Oct 2021 00:04:41 GMT  
		Size: 484.7 KB (484744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d48424d4cbc8619d81add2ea95272b5e0836ae77a40575fdc8fecde76df0f0b`  
		Last Modified: Fri, 15 Oct 2021 00:04:41 GMT  
		Size: 3.0 MB (2994453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb13eecc941ee3d1d10145af40f9c532c7134ec8666dec89cbee34f6aa836b60`  
		Last Modified: Fri, 15 Oct 2021 00:04:41 GMT  
		Size: 1.9 MB (1864928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1725ed1bc69f6a2990106e839c48ed03f053bc6ff3d51c7308ab7d7d03bb5dce`  
		Last Modified: Fri, 15 Oct 2021 00:04:41 GMT  
		Size: 1.6 KB (1592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
