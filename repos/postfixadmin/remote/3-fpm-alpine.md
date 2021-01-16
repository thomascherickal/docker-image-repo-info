## `postfixadmin:3-fpm-alpine`

```console
$ docker pull postfixadmin@sha256:0efbaec842cbd544d9a7e09b5178aa9d6f65a0ea0d3a3a00972e17490a4c8cfd
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

### `postfixadmin:3-fpm-alpine` - linux; amd64

```console
$ docker pull postfixadmin@sha256:3dd83227c73a7f73c50613f993568ea58b503605cf5ca636890735d768975f9a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34856658 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d28bde05d235a6d7f9575aaceda3f126eb999141fe021c8b4ca171a8fb4ed187`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:41:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 08:41:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 08:41:55 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 08:41:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 08:41:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 08:48:59 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 08:49:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 08:49:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 08:49:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 09:04:03 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 17:44:01 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 17:44:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 17:44:02 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 17:44:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jan 2021 17:44:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:52:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jan 2021 17:52:29 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:52:30 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jan 2021 17:52:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jan 2021 17:52:31 GMT
WORKDIR /var/www/html
# Thu, 07 Jan 2021 17:52:32 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 07 Jan 2021 17:52:32 GMT
STOPSIGNAL SIGQUIT
# Thu, 07 Jan 2021 17:52:32 GMT
EXPOSE 9000
# Thu, 07 Jan 2021 17:52:32 GMT
CMD ["php-fpm"]
# Fri, 15 Jan 2021 19:22:39 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 15 Jan 2021 19:22:40 GMT
RUN apk add --no-cache 		bash 		su-exec
# Fri, 15 Jan 2021 19:23:09 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 15 Jan 2021 19:23:09 GMT
ARG POSTFIXADMIN_VERSION=3.3.3
# Fri, 15 Jan 2021 19:23:09 GMT
ARG POSTFIXADMIN_SHA512=363b91eb07f263a0f595e020725cacf9f9de058adaef3987efb3257d0e6fba526b075f8328e47763256278797ec946305d1e4c8ff5c55d77753f9ed72bfa4121
# Fri, 15 Jan 2021 19:23:09 GMT
ENV POSTFIXADMIN_VERSION=3.3.3
# Fri, 15 Jan 2021 19:23:09 GMT
ENV POSTFIXADMIN_SHA512=363b91eb07f263a0f595e020725cacf9f9de058adaef3987efb3257d0e6fba526b075f8328e47763256278797ec946305d1e4c8ff5c55d77753f9ed72bfa4121
# Fri, 15 Jan 2021 19:23:11 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 15 Jan 2021 19:23:11 GMT
COPY file:0fe00ebe424ff03d907bf923ba92aa5d9e121221f969ba3b91c842dd670d93c9 in /usr/local/bin/ 
# Fri, 15 Jan 2021 19:23:11 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 15 Jan 2021 19:23:12 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e2096094279456885c5847855bddf4d9ac3b5c4f7f0ff73ef92fa69821ff86`  
		Last Modified: Thu, 17 Dec 2020 11:05:30 GMT  
		Size: 1.3 MB (1340903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320f26ee9b1c7b4c2ce0b67550a066ea859fb8796c0ff8de576f7e1b330342da`  
		Last Modified: Thu, 17 Dec 2020 11:05:30 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4612e05a72cfb0fde0de7565baa2660900747122288141d8dba25482f4983fe0`  
		Last Modified: Thu, 17 Dec 2020 11:05:30 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e0e3aa22e445286becccbdab24843c31f01402438adddd0d08b06b35d3e2c2`  
		Last Modified: Thu, 07 Jan 2021 20:31:25 GMT  
		Size: 10.3 MB (10345668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1731c161c4e9fd95a50fcf21c329aa5cd8cc275443b8fba2f313cef1f9022ae3`  
		Last Modified: Thu, 07 Jan 2021 20:31:23 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1297ca4f980950e23e704be0c39c25d9235f63a72e35f285b9b2f81d3611be04`  
		Last Modified: Thu, 07 Jan 2021 20:31:27 GMT  
		Size: 14.3 MB (14259382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d1811e7312c7d0db9079bdcd6e276416fb25341bace7371208e526177bf32e6`  
		Last Modified: Thu, 07 Jan 2021 20:31:22 GMT  
		Size: 2.3 KB (2256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8afa185a2b089b95b0b646d8ef6045e836141019794ab2ed6c79467efd37af`  
		Last Modified: Thu, 07 Jan 2021 20:31:22 GMT  
		Size: 16.9 KB (16885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89fbeb3e30d210e1e463710889f040727c03d618d183853e73cbe0973002b606`  
		Last Modified: Thu, 07 Jan 2021 20:31:23 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b281964d7a1017303c4c63d1d853c7fe5f167300c52a0b5c614a5e67c32760af`  
		Last Modified: Fri, 15 Jan 2021 19:24:05 GMT  
		Size: 559.5 KB (559492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5640ff2d44cd8dc00288d3edb19ddf9f3ec2af6817a3b90687759913af282ee8`  
		Last Modified: Fri, 15 Jan 2021 19:24:05 GMT  
		Size: 3.7 MB (3670309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127f8e52b0691eae20943a2896df666a88f38724e0db493acd95d350cd59b14b`  
		Last Modified: Fri, 15 Jan 2021 19:24:05 GMT  
		Size: 1.9 MB (1850736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad3af34b33b3f6ab4e80b0839315f68e063d94061d0e59c1a64815a4ed00314`  
		Last Modified: Fri, 15 Jan 2021 19:24:05 GMT  
		Size: 1.6 KB (1565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; arm variant v6

```console
$ docker pull postfixadmin@sha256:52c80af8b002d9fe7edf714ed75c73cb9d82a96877112fa2fd319b187e8e378d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33725932 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e3740d0c2356a69d55321644d3ab9ed038b468bb7bb10c8bf151e0c7061402f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 15 Jan 2021 01:51:19 GMT
ADD file:f2665ccfd90cf53580dc87c3e57db7c223147c686554b1d6e3fc166cce818b3e in / 
# Fri, 15 Jan 2021 01:51:20 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 22:53:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 22:53:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 22:54:00 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 22:54:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 22:54:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 22:57:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 15 Jan 2021 22:57:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 22:57:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 22:57:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 23:04:53 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 15 Jan 2021 23:04:54 GMT
ENV PHP_VERSION=7.4.14
# Fri, 15 Jan 2021 23:04:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 15 Jan 2021 23:04:57 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 15 Jan 2021 23:05:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:05:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:08:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 15 Jan 2021 23:08:43 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:08:46 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 Jan 2021 23:08:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 Jan 2021 23:08:47 GMT
WORKDIR /var/www/html
# Fri, 15 Jan 2021 23:08:49 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 15 Jan 2021 23:08:50 GMT
STOPSIGNAL SIGQUIT
# Fri, 15 Jan 2021 23:08:51 GMT
EXPOSE 9000
# Fri, 15 Jan 2021 23:08:51 GMT
CMD ["php-fpm"]
# Sat, 16 Jan 2021 00:31:02 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Sat, 16 Jan 2021 00:31:08 GMT
RUN apk add --no-cache 		bash 		su-exec
# Sat, 16 Jan 2021 00:32:24 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Sat, 16 Jan 2021 00:32:26 GMT
ARG POSTFIXADMIN_VERSION=3.3.3
# Sat, 16 Jan 2021 00:32:28 GMT
ARG POSTFIXADMIN_SHA512=363b91eb07f263a0f595e020725cacf9f9de058adaef3987efb3257d0e6fba526b075f8328e47763256278797ec946305d1e4c8ff5c55d77753f9ed72bfa4121
# Sat, 16 Jan 2021 00:32:33 GMT
ENV POSTFIXADMIN_VERSION=3.3.3
# Sat, 16 Jan 2021 00:32:36 GMT
ENV POSTFIXADMIN_SHA512=363b91eb07f263a0f595e020725cacf9f9de058adaef3987efb3257d0e6fba526b075f8328e47763256278797ec946305d1e4c8ff5c55d77753f9ed72bfa4121
# Sat, 16 Jan 2021 00:32:43 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Sat, 16 Jan 2021 00:32:44 GMT
COPY file:0fe00ebe424ff03d907bf923ba92aa5d9e121221f969ba3b91c842dd670d93c9 in /usr/local/bin/ 
# Sat, 16 Jan 2021 00:32:45 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 16 Jan 2021 00:32:45 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b550170d5d44558603032e2371fa7a2fb3575b38b2c64ad8be4ab798bcad44d3`  
		Last Modified: Fri, 15 Jan 2021 01:52:01 GMT  
		Size: 2.6 MB (2621576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3110258b4da6fc6756faa0ee4ede2d02a24ff821ba8f1ba72a75739fc89161fa`  
		Last Modified: Fri, 15 Jan 2021 23:27:01 GMT  
		Size: 1.7 MB (1684838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef6d6cdd312890c0852fd22903c40d68137566e06f947a0c3461bba58aab6fb`  
		Last Modified: Fri, 15 Jan 2021 23:27:00 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61428ad89e8a3dd97317b0da99d3c4b4f36306fd1b554393af68eea521ad75c`  
		Last Modified: Fri, 15 Jan 2021 23:27:00 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501e96d58ae0f12c5a1a41afdbb32e1483b1b2c04ca3397b061dafb8cb17cfda`  
		Last Modified: Fri, 15 Jan 2021 23:28:56 GMT  
		Size: 10.3 MB (10346238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8133164fb29d3f035534996fcd855903daae10abf48150745921a635cb886488`  
		Last Modified: Fri, 15 Jan 2021 23:28:54 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fceb2932ca7e517d29e62262eb0b808e81373d1c0783c35acbdfeb76bd494293`  
		Last Modified: Fri, 15 Jan 2021 23:28:59 GMT  
		Size: 13.7 MB (13693430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5b6321994790c1c8e72aff5708c282bd05b5f75ed8fb4acd19e1734740bb61d`  
		Last Modified: Fri, 15 Jan 2021 23:28:54 GMT  
		Size: 2.3 KB (2260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97871dc00558a93fd6587169b027fd27db14328c2727beef20496ab4ba354931`  
		Last Modified: Fri, 15 Jan 2021 23:28:54 GMT  
		Size: 17.5 KB (17529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61ed8dfb28531e5e81f4e7d688bcb99cfb2ca9d7a23f08f5976289cb6c0e76e`  
		Last Modified: Fri, 15 Jan 2021 23:28:54 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66347354e59ddee558d5bf97f29cbb2da8618daed447d7c834fe7062d15d263d`  
		Last Modified: Sat, 16 Jan 2021 00:33:16 GMT  
		Size: 572.3 KB (572306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f453335044c22354101ea1d5ac028e61de15ee2f42bc89432218b30ede57d8`  
		Last Modified: Sat, 16 Jan 2021 00:33:17 GMT  
		Size: 2.9 MB (2924979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc7b76eca8cd3a3c19d123c8043f0552b37be735a45d5387598b8dadddb3638`  
		Last Modified: Sat, 16 Jan 2021 00:33:17 GMT  
		Size: 1.9 MB (1850749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3819652e55fe048b550f8f8c6cba02790ff5c75218c076f90f74a69c4a70f8d`  
		Last Modified: Sat, 16 Jan 2021 00:33:16 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; arm variant v7

```console
$ docker pull postfixadmin@sha256:ae55d580eb90eb8888f9293919a6a63788d8e07051cee29bc8b640b7d51f1cd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32556426 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a4c7b9bb80fbe1156ce6a3268d5348750705178954b900f918e5f225a42637cf`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 15 Jan 2021 01:58:27 GMT
ADD file:718d7c24a8d6ff0feb2843cf8c3ca4b7ef1fb523a45dea568404259a7b4e6f10 in / 
# Fri, 15 Jan 2021 01:58:29 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 23:04:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 23:04:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 23:04:07 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 23:04:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 23:04:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 23:08:08 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 15 Jan 2021 23:08:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:08:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:08:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 23:16:20 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 15 Jan 2021 23:16:21 GMT
ENV PHP_VERSION=7.4.14
# Fri, 15 Jan 2021 23:16:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 15 Jan 2021 23:16:23 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 15 Jan 2021 23:16:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:16:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:19:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 15 Jan 2021 23:20:01 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:20:05 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 Jan 2021 23:20:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 Jan 2021 23:20:07 GMT
WORKDIR /var/www/html
# Fri, 15 Jan 2021 23:20:09 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 15 Jan 2021 23:20:10 GMT
STOPSIGNAL SIGQUIT
# Fri, 15 Jan 2021 23:20:11 GMT
EXPOSE 9000
# Fri, 15 Jan 2021 23:20:11 GMT
CMD ["php-fpm"]
# Sat, 16 Jan 2021 00:52:58 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Sat, 16 Jan 2021 00:53:02 GMT
RUN apk add --no-cache 		bash 		su-exec
# Sat, 16 Jan 2021 00:53:59 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Sat, 16 Jan 2021 00:54:00 GMT
ARG POSTFIXADMIN_VERSION=3.3.3
# Sat, 16 Jan 2021 00:54:00 GMT
ARG POSTFIXADMIN_SHA512=363b91eb07f263a0f595e020725cacf9f9de058adaef3987efb3257d0e6fba526b075f8328e47763256278797ec946305d1e4c8ff5c55d77753f9ed72bfa4121
# Sat, 16 Jan 2021 00:54:01 GMT
ENV POSTFIXADMIN_VERSION=3.3.3
# Sat, 16 Jan 2021 00:54:02 GMT
ENV POSTFIXADMIN_SHA512=363b91eb07f263a0f595e020725cacf9f9de058adaef3987efb3257d0e6fba526b075f8328e47763256278797ec946305d1e4c8ff5c55d77753f9ed72bfa4121
# Sat, 16 Jan 2021 00:54:05 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Sat, 16 Jan 2021 00:54:06 GMT
COPY file:0fe00ebe424ff03d907bf923ba92aa5d9e121221f969ba3b91c842dd670d93c9 in /usr/local/bin/ 
# Sat, 16 Jan 2021 00:54:07 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 16 Jan 2021 00:54:08 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:0f34ce5da94097b8c334f6b2065a010aced9855c3532e4462e9bd1b0a4c4b3f6`  
		Last Modified: Fri, 15 Jan 2021 01:59:13 GMT  
		Size: 2.4 MB (2422744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cecec77a7b5b50913bcb9f7bfe0c5fdcebb948b947747285290197c13902be91`  
		Last Modified: Fri, 15 Jan 2021 23:42:36 GMT  
		Size: 1.6 MB (1555130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0496082b3c55009a50b47ce80bf27dd7451aaa7e13b5b4ccbe886a780c614dd1`  
		Last Modified: Fri, 15 Jan 2021 23:42:33 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af351861d88fff830659b71d51e45b8e623d31cb86c764fab107e6c39ca5a717`  
		Last Modified: Fri, 15 Jan 2021 23:42:33 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b641e2b9da12e18bef312739ada811a79b50ce5892b425292468662ef536b8b0`  
		Last Modified: Fri, 15 Jan 2021 23:44:59 GMT  
		Size: 10.3 MB (10346235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dc9fd32bbef60ac4128a4c440ce73f136bda82cb0e7fb09d6340e33c251770`  
		Last Modified: Fri, 15 Jan 2021 23:44:55 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80249d618c0703ada578087f1f9d0bfcb4cfcfee735c95aeed1766d38d1dd6ba`  
		Last Modified: Fri, 15 Jan 2021 23:44:59 GMT  
		Size: 12.8 MB (12818131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7eb73debe0a6e73c44261435b543e9bc9bde1195f6378d00dcfaafe8e855523`  
		Last Modified: Fri, 15 Jan 2021 23:44:55 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5e380bb404fc283f3acaa481ce72a2a7f0786b2d6e221780e342478766f120d`  
		Last Modified: Fri, 15 Jan 2021 23:44:55 GMT  
		Size: 17.5 KB (17523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e743154b5f13d538ad220f13d540905883afd455c3178388670294273549f3`  
		Last Modified: Fri, 15 Jan 2021 23:44:55 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7f9af51669a703596e0475e5383187a46c2ef0b5a4527a2fd1b638eb736069c`  
		Last Modified: Sat, 16 Jan 2021 00:54:36 GMT  
		Size: 521.3 KB (521277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46cf03daf220dcb3c594e6db4bd6cfd6904d9d9e8e120aabab7cd657e2fb426f`  
		Last Modified: Sat, 16 Jan 2021 00:54:37 GMT  
		Size: 3.0 MB (3010366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e523ac8375b8b953dc8d32dbf3044fa27a771d92747991f6e26080b921444b`  
		Last Modified: Sat, 16 Jan 2021 00:54:37 GMT  
		Size: 1.9 MB (1850737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:897f87f660f8cae79a962dd7b7e0dedd0990718446a0170c677ffe69d597511b`  
		Last Modified: Sat, 16 Jan 2021 00:54:36 GMT  
		Size: 1.6 KB (1563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull postfixadmin@sha256:6093e809a91c182d3cbda0db6af333cc7e733f236413e1f6c0d5bbc05fef04fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34597556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edc7ebc0d7d05e3acebd02b7dbedca7692c6b4d1bd4f657950bcd6a06c9b6bbd`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:46:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 05:46:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 05:46:55 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 05:46:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 05:47:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 05:51:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 05:51:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 05:51:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 05:51:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 06:01:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 18:10:16 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 18:10:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 18:10:19 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 18:10:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jan 2021 18:10:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 18:14:10 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jan 2021 18:14:13 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 07 Jan 2021 18:14:19 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jan 2021 18:14:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jan 2021 18:14:23 GMT
WORKDIR /var/www/html
# Thu, 07 Jan 2021 18:14:26 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 07 Jan 2021 18:14:27 GMT
STOPSIGNAL SIGQUIT
# Thu, 07 Jan 2021 18:14:28 GMT
EXPOSE 9000
# Thu, 07 Jan 2021 18:14:29 GMT
CMD ["php-fpm"]
# Fri, 15 Jan 2021 18:44:34 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 15 Jan 2021 18:44:37 GMT
RUN apk add --no-cache 		bash 		su-exec
# Fri, 15 Jan 2021 18:45:28 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 15 Jan 2021 18:45:29 GMT
ARG POSTFIXADMIN_VERSION=3.3.3
# Fri, 15 Jan 2021 18:45:30 GMT
ARG POSTFIXADMIN_SHA512=363b91eb07f263a0f595e020725cacf9f9de058adaef3987efb3257d0e6fba526b075f8328e47763256278797ec946305d1e4c8ff5c55d77753f9ed72bfa4121
# Fri, 15 Jan 2021 18:45:30 GMT
ENV POSTFIXADMIN_VERSION=3.3.3
# Fri, 15 Jan 2021 18:45:31 GMT
ENV POSTFIXADMIN_SHA512=363b91eb07f263a0f595e020725cacf9f9de058adaef3987efb3257d0e6fba526b075f8328e47763256278797ec946305d1e4c8ff5c55d77753f9ed72bfa4121
# Fri, 15 Jan 2021 18:45:34 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 15 Jan 2021 18:45:35 GMT
COPY file:0fe00ebe424ff03d907bf923ba92aa5d9e121221f969ba3b91c842dd670d93c9 in /usr/local/bin/ 
# Fri, 15 Jan 2021 18:45:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 15 Jan 2021 18:45:36 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349511631cc12dc049249fd94f9012c505ccb000f16147091cb84874846fb9b1`  
		Last Modified: Thu, 17 Dec 2020 07:10:16 GMT  
		Size: 1.3 MB (1342931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053bd098149c8419c2b9b5a2702c5d9c4e9de3b2131447e18aacde4047de2d88`  
		Last Modified: Thu, 17 Dec 2020 07:10:15 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00122640c7f935b33a14c9e88b946165e75935d6cd28f9b2d20d783d43c21423`  
		Last Modified: Thu, 17 Dec 2020 07:10:15 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b5acc908a258e5ea1e9e972d38e9c30289ffd2ee6928306144fe083c0d4f8e`  
		Last Modified: Thu, 07 Jan 2021 19:32:43 GMT  
		Size: 10.3 MB (10345707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e6f3407f8c8dfce02d9af40a7389c76895567a98e4c301cf32f6e99d77d4903`  
		Last Modified: Thu, 07 Jan 2021 19:32:38 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e56a5f41aef0511951736887d91745c3ce87340112017cdbf06a52c612f55a0`  
		Last Modified: Thu, 07 Jan 2021 19:32:44 GMT  
		Size: 14.1 MB (14069158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e612c8d029ee6da1fbe15c022a56168ac7d065910f59f06e6a7eca6295658a58`  
		Last Modified: Thu, 07 Jan 2021 19:32:38 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aae5e4982009ebe825a79c0b78bd6a71897136ff417de539835a0187623e8dfc`  
		Last Modified: Thu, 07 Jan 2021 19:32:38 GMT  
		Size: 16.9 KB (16897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df852066d9437f2097bba880b52a68a2e3e7e53d9d81b7ef1a8c71166f69613e`  
		Last Modified: Thu, 07 Jan 2021 19:32:38 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d61cd68ccd3ae7c32ee08924b7179da384f60204b1ca2a0f7f720034f522e42`  
		Last Modified: Fri, 15 Jan 2021 18:47:04 GMT  
		Size: 570.4 KB (570365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b85eabd783ca358854bc6ced5d080b63c6a9a9c9a7f41a89d5b235b23ccccba`  
		Last Modified: Fri, 15 Jan 2021 18:47:04 GMT  
		Size: 3.7 MB (3678406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b91034b9aaec1af434a956184dfab1aad530ffafb0d09b65b559e39a8af4bc`  
		Last Modified: Fri, 15 Jan 2021 18:47:04 GMT  
		Size: 1.9 MB (1850744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d24f5f5709e4b5aa502dbea62d07fee29c77291c7eb9eed291da04eb86a5b4f`  
		Last Modified: Fri, 15 Jan 2021 18:47:03 GMT  
		Size: 1.6 KB (1568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; 386

```console
$ docker pull postfixadmin@sha256:f9b50036352413b97d185c92574dfa5b77971876463fbdec2cee129742468c92
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35501957 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:401664179ec88ba6ede20710e33d5bdf02820747ea8ca38d0abea874fa9db7e3`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 03:34:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 03:34:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 03:34:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 03:34:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 03:34:07 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 03:40:09 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 03:40:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 03:40:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 03:40:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 03:52:35 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 18:21:27 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 18:21:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 18:21:28 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 18:21:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jan 2021 18:21:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 18:31:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jan 2021 18:31:36 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 07 Jan 2021 18:31:37 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jan 2021 18:31:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jan 2021 18:31:38 GMT
WORKDIR /var/www/html
# Thu, 07 Jan 2021 18:31:38 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 07 Jan 2021 18:31:39 GMT
STOPSIGNAL SIGQUIT
# Thu, 07 Jan 2021 18:31:39 GMT
EXPOSE 9000
# Thu, 07 Jan 2021 18:31:39 GMT
CMD ["php-fpm"]
# Fri, 15 Jan 2021 18:40:37 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 15 Jan 2021 18:40:38 GMT
RUN apk add --no-cache 		bash 		su-exec
# Fri, 15 Jan 2021 18:41:10 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 15 Jan 2021 18:41:10 GMT
ARG POSTFIXADMIN_VERSION=3.3.3
# Fri, 15 Jan 2021 18:41:10 GMT
ARG POSTFIXADMIN_SHA512=363b91eb07f263a0f595e020725cacf9f9de058adaef3987efb3257d0e6fba526b075f8328e47763256278797ec946305d1e4c8ff5c55d77753f9ed72bfa4121
# Fri, 15 Jan 2021 18:41:11 GMT
ENV POSTFIXADMIN_VERSION=3.3.3
# Fri, 15 Jan 2021 18:41:11 GMT
ENV POSTFIXADMIN_SHA512=363b91eb07f263a0f595e020725cacf9f9de058adaef3987efb3257d0e6fba526b075f8328e47763256278797ec946305d1e4c8ff5c55d77753f9ed72bfa4121
# Fri, 15 Jan 2021 18:41:13 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 15 Jan 2021 18:41:13 GMT
COPY file:0fe00ebe424ff03d907bf923ba92aa5d9e121221f969ba3b91c842dd670d93c9 in /usr/local/bin/ 
# Fri, 15 Jan 2021 18:41:13 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 15 Jan 2021 18:41:13 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94d120997ac65664d4944fb3d9d4551e8e118f43c788aa67591c2cb54010aed`  
		Last Modified: Thu, 17 Dec 2020 05:43:55 GMT  
		Size: 1.4 MB (1439814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657c96696eb3a101b3148ccc28a870e751ee94e39bb2f3cc1745bdec7655b033`  
		Last Modified: Thu, 17 Dec 2020 05:43:55 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25357089a74d7e4f4ee1bc77cd180c431537e393399785f113a7f2fe4ac7614`  
		Last Modified: Thu, 17 Dec 2020 05:43:52 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4a0403170d088ecd930d7283bba2b96eba4f8af70e2683bed18bbce107f3de5`  
		Last Modified: Thu, 07 Jan 2021 21:13:41 GMT  
		Size: 10.3 MB (10345646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a5a38b02f7cf978e61b430eb3e6593fe1c12aa329324d6059a56c049bde5d6b`  
		Last Modified: Thu, 07 Jan 2021 21:13:38 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c34fb4de243b08ba3f630842f80f7f1230f8e8b6614d2c7448965668cd2c4f4b`  
		Last Modified: Thu, 07 Jan 2021 21:13:41 GMT  
		Size: 14.6 MB (14642409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53ffae42ea54c9f236d04fa540bf1f1242011612aa274badb7aa2016756bfd91`  
		Last Modified: Thu, 07 Jan 2021 21:13:38 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6937b3bf2a4b961c8473fd7533035729145f5e34c4b073fba6e77ec0b0d65a7`  
		Last Modified: Thu, 07 Jan 2021 21:13:37 GMT  
		Size: 16.9 KB (16877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35a93bf8b149a000359c6da6ed421a6b74dad7314746494296e75782021a1b71`  
		Last Modified: Thu, 07 Jan 2021 21:13:41 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4159b6cbfdc6597dc2a66c247a1c97fa9c05b72917d5208d425986eb41780644`  
		Last Modified: Fri, 15 Jan 2021 18:42:07 GMT  
		Size: 600.4 KB (600387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088e5072fdfe73409f151f3c6849f0c3a7148dbe5b994ff2323c51f6b6910850`  
		Last Modified: Fri, 15 Jan 2021 18:42:08 GMT  
		Size: 3.8 MB (3797734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca996861b1aff4594eddf0e25406d91a0fef92cbb2cb849e5323837e2c7305ac`  
		Last Modified: Fri, 15 Jan 2021 18:42:09 GMT  
		Size: 1.9 MB (1850736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440fbfffe470fb8d65de76135a9735a638cda4bfdb55b5dde1a82deae15a5764`  
		Last Modified: Fri, 15 Jan 2021 18:42:07 GMT  
		Size: 1.6 KB (1566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; ppc64le

```console
$ docker pull postfixadmin@sha256:28aca0a562d675cd2ada8d4201ce6b5685e327c89c97dcc0ea5f64e3086e0e38
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.0 MB (35987968 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe95bb12d7025c8a30fec5778dec1d28de7c75ed0e9bb13e569c944b146df03f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:02:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 06:02:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 06:03:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 06:03:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 06:03:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 06:09:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 17 Dec 2020 06:09:41 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 06:09:45 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 06:09:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 06:21:39 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 18:04:06 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 18:04:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 18:04:20 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 18:04:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jan 2021 18:04:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 18:08:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jan 2021 18:08:50 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Thu, 07 Jan 2021 18:09:10 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jan 2021 18:09:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jan 2021 18:09:27 GMT
WORKDIR /var/www/html
# Thu, 07 Jan 2021 18:09:47 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 07 Jan 2021 18:09:53 GMT
STOPSIGNAL SIGQUIT
# Thu, 07 Jan 2021 18:10:01 GMT
EXPOSE 9000
# Thu, 07 Jan 2021 18:10:09 GMT
CMD ["php-fpm"]
# Fri, 15 Jan 2021 19:22:16 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 15 Jan 2021 19:22:30 GMT
RUN apk add --no-cache 		bash 		su-exec
# Fri, 15 Jan 2021 19:23:39 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 15 Jan 2021 19:23:44 GMT
ARG POSTFIXADMIN_VERSION=3.3.3
# Fri, 15 Jan 2021 19:23:48 GMT
ARG POSTFIXADMIN_SHA512=363b91eb07f263a0f595e020725cacf9f9de058adaef3987efb3257d0e6fba526b075f8328e47763256278797ec946305d1e4c8ff5c55d77753f9ed72bfa4121
# Fri, 15 Jan 2021 19:23:55 GMT
ENV POSTFIXADMIN_VERSION=3.3.3
# Fri, 15 Jan 2021 19:23:59 GMT
ENV POSTFIXADMIN_SHA512=363b91eb07f263a0f595e020725cacf9f9de058adaef3987efb3257d0e6fba526b075f8328e47763256278797ec946305d1e4c8ff5c55d77753f9ed72bfa4121
# Fri, 15 Jan 2021 19:24:14 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 15 Jan 2021 19:24:22 GMT
COPY file:0fe00ebe424ff03d907bf923ba92aa5d9e121221f969ba3b91c842dd670d93c9 in /usr/local/bin/ 
# Fri, 15 Jan 2021 19:24:25 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 15 Jan 2021 19:24:32 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4878c44618050313be4a5ac046d572683a6e0d371586c31a768e1768423df9a3`  
		Last Modified: Thu, 17 Dec 2020 08:04:10 GMT  
		Size: 1.4 MB (1383302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577c712c96426aadbf75437b4aae5841ed84ba25ee142ec3aaaf86802464d6f9`  
		Last Modified: Thu, 17 Dec 2020 08:04:08 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a10ca736025b1646c79fbd378c22773ccb82df4aadc2cb960dea6eacb8bbb16`  
		Last Modified: Thu, 17 Dec 2020 08:04:08 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:209b716f68e5de6d72b17c8f89fb302689dc70c27ec1e0fb95eb2a64bf2f6c26`  
		Last Modified: Thu, 07 Jan 2021 19:53:56 GMT  
		Size: 10.3 MB (10345699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795fe2cb0d85f09ac5fd362886605ffe47de33dca98304b0edbb05b43226b05e`  
		Last Modified: Thu, 07 Jan 2021 19:53:49 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a00e93768d44b4d819c0b84d8e36474ed1954df991b0781eca12f4c05c642fd`  
		Last Modified: Thu, 07 Jan 2021 19:53:53 GMT  
		Size: 15.2 MB (15242506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b52cc00460e457621f5626c2a2f1c7825c2a549aca5882443c242233b9ec96b`  
		Last Modified: Thu, 07 Jan 2021 19:53:49 GMT  
		Size: 2.3 KB (2256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e4c85da768e87e90315e39e7006fb0061013511d102dcedbf7a4c4ce8d09c5`  
		Last Modified: Thu, 07 Jan 2021 19:53:49 GMT  
		Size: 16.9 KB (16933 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d0426794e655a38e1690046ce95746e292c4b9d313859acd1ac7d0dd66a4608`  
		Last Modified: Thu, 07 Jan 2021 19:53:49 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a21a3e34db66a7b5c48697ee71c323c2146cb0927eedfdd950e53c38517f59`  
		Last Modified: Fri, 15 Jan 2021 19:26:15 GMT  
		Size: 625.0 KB (625008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf9e4bb66ef4f6dcac50cb317ddcf48d77373bfdb84d8c4c7296bf334982641d`  
		Last Modified: Fri, 15 Jan 2021 19:26:16 GMT  
		Size: 3.7 MB (3704244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1fc2043c0c0ece43da14c26ebc94bdf3e4ca30248dae85395f189e256be170`  
		Last Modified: Fri, 15 Jan 2021 19:26:16 GMT  
		Size: 1.9 MB (1850753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97c6cc3bfd1c509dd76d00d4b4599619a38b9f041734ce6fa7a1c8351f0d1ec7`  
		Last Modified: Fri, 15 Jan 2021 19:26:15 GMT  
		Size: 1.6 KB (1567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; s390x

```console
$ docker pull postfixadmin@sha256:380adbeb125cc34791ac4a7969db8e828b8c93edc177e8a501730800bae5faa1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34156115 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a93dac2b88a2d8788656ad76921d4a728eda0b1fc7ca735816a12627dedab8f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 15 Jan 2021 01:51:34 GMT
ADD file:3ba807ca8ed73ca14224dd26a883f2399031fa32430f035cc5ae97b5e6db0ca7 in / 
# Fri, 15 Jan 2021 01:51:35 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 22:57:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 22:57:12 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 22:57:13 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 22:57:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 22:57:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 23:02:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 15 Jan 2021 23:02:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:02:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:02:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 23:12:03 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 15 Jan 2021 23:12:04 GMT
ENV PHP_VERSION=7.4.14
# Fri, 15 Jan 2021 23:12:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 15 Jan 2021 23:12:05 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 15 Jan 2021 23:12:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:12:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:17:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 15 Jan 2021 23:17:10 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:17:11 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 Jan 2021 23:17:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 Jan 2021 23:17:12 GMT
WORKDIR /var/www/html
# Fri, 15 Jan 2021 23:17:13 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 15 Jan 2021 23:17:13 GMT
STOPSIGNAL SIGQUIT
# Fri, 15 Jan 2021 23:17:13 GMT
EXPOSE 9000
# Fri, 15 Jan 2021 23:17:13 GMT
CMD ["php-fpm"]
# Sat, 16 Jan 2021 00:50:49 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Sat, 16 Jan 2021 00:50:50 GMT
RUN apk add --no-cache 		bash 		su-exec
# Sat, 16 Jan 2021 00:51:26 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		imap-dev 		krb5-dev 		postgresql-dev 		sqlite-dev 	; 	docker-php-ext-configure 		imap --with-imap-ssl --with-kerberos 	; 	docker-php-ext-install -j "$(nproc)" 		imap 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Sat, 16 Jan 2021 00:51:26 GMT
ARG POSTFIXADMIN_VERSION=3.3.3
# Sat, 16 Jan 2021 00:51:27 GMT
ARG POSTFIXADMIN_SHA512=363b91eb07f263a0f595e020725cacf9f9de058adaef3987efb3257d0e6fba526b075f8328e47763256278797ec946305d1e4c8ff5c55d77753f9ed72bfa4121
# Sat, 16 Jan 2021 00:51:27 GMT
ENV POSTFIXADMIN_VERSION=3.3.3
# Sat, 16 Jan 2021 00:51:27 GMT
ENV POSTFIXADMIN_SHA512=363b91eb07f263a0f595e020725cacf9f9de058adaef3987efb3257d0e6fba526b075f8328e47763256278797ec946305d1e4c8ff5c55d77753f9ed72bfa4121
# Sat, 16 Jan 2021 00:51:29 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Sat, 16 Jan 2021 00:51:30 GMT
COPY file:0fe00ebe424ff03d907bf923ba92aa5d9e121221f969ba3b91c842dd670d93c9 in /usr/local/bin/ 
# Sat, 16 Jan 2021 00:51:30 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Sat, 16 Jan 2021 00:51:30 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3997176601fb5d5ac06922718668ede4acac00a5c0daef8a9099fd76ce93047f`  
		Last Modified: Fri, 15 Jan 2021 01:52:40 GMT  
		Size: 2.6 MB (2601720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497e79d9095f9ba4812f1150c33ad07d399f559fea8e3c4fe8553e02f2cf8b6a`  
		Last Modified: Fri, 15 Jan 2021 23:39:10 GMT  
		Size: 1.8 MB (1756352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99527660904ffc5aed1d27bb86166f189e04b5df76d7becf74efffb1836eaf5e`  
		Last Modified: Fri, 15 Jan 2021 23:39:10 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9b51111e1ef5a5156e505d6369bb2d4e21354a1203636fca6f26de34df9c15`  
		Last Modified: Fri, 15 Jan 2021 23:39:10 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d269e26eca744ab118d303ed1eac4fca6b7baa5e74aea3e5f37f74dfe29114`  
		Last Modified: Fri, 15 Jan 2021 23:45:52 GMT  
		Size: 10.3 MB (10346239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d8122b6ee9e9743feec1e0415d4126b817779545ecdee127a76ad836819965`  
		Last Modified: Fri, 15 Jan 2021 23:45:49 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b24745045083bc2b62ee123b2d4a91ac9e43bf73b286436cce7be1603699771`  
		Last Modified: Fri, 15 Jan 2021 23:45:51 GMT  
		Size: 14.1 MB (14073331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c385972279a75eb7924a6a415338c0d323906987cfd7c32cb8f26385e7dfe04`  
		Last Modified: Fri, 15 Jan 2021 23:45:49 GMT  
		Size: 2.3 KB (2257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54c5e0dfe3da28722eb099fc47db991ad2bf810d2435ec2f2e73abd85011df4e`  
		Last Modified: Fri, 15 Jan 2021 23:45:49 GMT  
		Size: 17.5 KB (17523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05aa2df3835a4d4c751ab86a6c670783a3d2238593f39fd844eb10e857928795`  
		Last Modified: Fri, 15 Jan 2021 23:45:49 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8eb7125c79601cea4846da751f3b1b2c0d34ed58bfa9a91e7ce12ca3827567`  
		Last Modified: Sat, 16 Jan 2021 00:52:10 GMT  
		Size: 617.3 KB (617321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d493f65bec39038f5b53408022bb6d539994bc488e18f5910201b6bc55e80781`  
		Last Modified: Sat, 16 Jan 2021 00:52:09 GMT  
		Size: 2.9 MB (2878608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7b495063782f6375494c315699d7b69eceece961b39e9130727ec390aecf0d`  
		Last Modified: Sat, 16 Jan 2021 00:52:10 GMT  
		Size: 1.9 MB (1850739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cec504156965c7e182cb45a7b16f5a1a8979d9a28b94a7cec2579c1a7f947289`  
		Last Modified: Sat, 16 Jan 2021 00:52:11 GMT  
		Size: 1.6 KB (1561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
