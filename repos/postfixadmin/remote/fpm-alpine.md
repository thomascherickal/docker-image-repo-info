## `postfixadmin:fpm-alpine`

```console
$ docker pull postfixadmin@sha256:763cbd111a1e289ccdd341c984d4c06b6abdd6e07109123af455e5133b5e2c1f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `postfixadmin:fpm-alpine` - linux; amd64

```console
$ docker pull postfixadmin@sha256:4612f4a4cf083e806581bd269af1b1888d5d8283a24eeeed800a3ac8631a750e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36194985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b2ac559031780f91d9797c0a5c2d3d5c71dd120899b24115c7db4d7980d6dd8`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 01:18:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 01:18:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 01:18:35 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 01:18:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 01:18:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 01:27:38 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 01:27:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 01:27:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 01:27:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Tue, 24 Mar 2020 01:56:11 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 24 Mar 2020 01:56:12 GMT
ENV PHP_VERSION=7.3.16
# Tue, 24 Mar 2020 01:56:12 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.16.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.16.tar.xz.asc/from/this/mirror
# Tue, 24 Mar 2020 01:56:12 GMT
ENV PHP_SHA256=91aaee3dbdc71b69b4f3292f9d99211172a2fa926c3f3bbdb0e85dab03dd2bcb PHP_MD5=
# Tue, 24 Mar 2020 01:56:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 24 Mar 2020 01:56:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 24 Mar 2020 02:03:23 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 24 Mar 2020 02:03:24 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Tue, 24 Mar 2020 02:03:27 GMT
RUN docker-php-ext-enable sodium
# Tue, 24 Mar 2020 02:03:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 24 Mar 2020 02:03:28 GMT
WORKDIR /var/www/html
# Tue, 24 Mar 2020 02:03:29 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 24 Mar 2020 02:03:29 GMT
STOPSIGNAL SIGQUIT
# Tue, 24 Mar 2020 02:03:30 GMT
EXPOSE 9000
# Tue, 24 Mar 2020 02:03:30 GMT
CMD ["php-fpm"]
# Tue, 24 Mar 2020 04:54:15 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Tue, 24 Mar 2020 04:54:16 GMT
RUN apk add --no-cache 		bash 		coreutils
# Tue, 24 Mar 2020 04:54:42 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		sqlite-dev 		postgresql-dev 	; 	docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Tue, 24 Mar 2020 04:54:42 GMT
ARG POSTFIXADMIN_VERSION=3.2.3
# Tue, 24 Mar 2020 04:54:42 GMT
ARG POSTFIXADMIN_SHA512=d44addb9a3ca830caf55b603363054df561d659957f21cab7523465ebf02ca18abe7fcf298fe718d957d0b7bf5613e2dde69c78c26e0f7f6f595d79b28fe08ab
# Tue, 24 Mar 2020 04:54:42 GMT
ENV POSTFIXADMIN_VERSION=3.2.3
# Tue, 24 Mar 2020 04:54:43 GMT
ENV POSTFIXADMIN_SHA512=d44addb9a3ca830caf55b603363054df561d659957f21cab7523465ebf02ca18abe7fcf298fe718d957d0b7bf5613e2dde69c78c26e0f7f6f595d79b28fe08ab
# Tue, 24 Mar 2020 04:54:44 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Tue, 24 Mar 2020 04:54:44 GMT
COPY file:83be1dbd46cfa4c9ff6241f21a00fcd952c07b15bab1c6cf82fac6bfbae210c8 in /usr/local/bin/ 
# Tue, 24 Mar 2020 04:54:44 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 24 Mar 2020 04:54:45 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61c449d5d9102f11bc559aba323f82389b7be6118dea453e8273a7f8cc971ea`  
		Last Modified: Tue, 24 Mar 2020 02:42:25 GMT  
		Size: 1.4 MB (1354647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fde16e1397a31e46a1030c8f769012ebe10f171fc564c77a692053c845975ff`  
		Last Modified: Tue, 24 Mar 2020 02:42:24 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1096698ab2a54e6370c1f2b9c6bb71ae2bb54e306f246aa436b77e1351ff1cf`  
		Last Modified: Tue, 24 Mar 2020 02:42:25 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e09ee4033d1f636e39d6cd200fa0451906b5417d71fcf17e1dcb97eb8b745e5`  
		Last Modified: Tue, 24 Mar 2020 02:43:49 GMT  
		Size: 12.1 MB (12133350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32670cfc718884cbe40e9158ede48957de177808b6889cf3e0dd3a02e53698cd`  
		Last Modified: Tue, 24 Mar 2020 02:43:46 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3bfbcc96d33915afdf2cc66767bbf705b8c047b08f99347bdd3e943d28fb69a`  
		Last Modified: Tue, 24 Mar 2020 02:43:50 GMT  
		Size: 14.5 MB (14465522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:095f83f78721704875575f13144e7b1683c69713e0c00762962a63d0292f3d8d`  
		Last Modified: Tue, 24 Mar 2020 02:43:46 GMT  
		Size: 2.2 KB (2215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6234ddc68641c475c5f736d39fb36a1c925fc59d755593474f87b3846e5c21b`  
		Last Modified: Tue, 24 Mar 2020 02:43:46 GMT  
		Size: 16.9 KB (16910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f7af26f613dae4046542ee2180cfb8b343d2a3dd00d807b276001131c624877`  
		Last Modified: Tue, 24 Mar 2020 02:43:46 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261a6b75114d86e989cb6d45818aeddc3b9f7f954b17c576f9740ddb5de44899`  
		Last Modified: Tue, 24 Mar 2020 04:54:59 GMT  
		Size: 1.1 MB (1098550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:965bd7cb2e83a4449d4068ff0313585ee344f08c1db1140df6b3f065f7573dd5`  
		Last Modified: Tue, 24 Mar 2020 04:55:00 GMT  
		Size: 3.0 MB (2975119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b69bc32df34deb3a2e59c3a44530ba83720c52d7172b0598a162dc3bbb22be`  
		Last Modified: Tue, 24 Mar 2020 04:54:59 GMT  
		Size: 1.3 MB (1333779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3310d918f2e15c92dd0c47dc2b8b98bda73004b6caf85c45521a577707380b52`  
		Last Modified: Tue, 24 Mar 2020 04:54:59 GMT  
		Size: 1.3 KB (1277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; arm variant v6

```console
$ docker pull postfixadmin@sha256:6e84109dcc8bda598c193b7576d34fcb836725baaa81479dd5a99912947fe9f2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34826268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aed312e1f0ea0881a881d2617dc600cbb68e3d13c1f05465f80b6b1aac303cd2`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 02:16:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 02:16:45 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 02:16:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 02:16:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 02:16:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 02:21:00 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 02:21:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 02:21:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 02:21:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Tue, 24 Mar 2020 02:33:54 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 16 Apr 2020 21:24:08 GMT
ENV PHP_VERSION=7.3.17
# Thu, 16 Apr 2020 21:24:09 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.17.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.17.tar.xz.asc/from/this/mirror
# Thu, 16 Apr 2020 21:24:11 GMT
ENV PHP_SHA256=6a30304c27f7e7a94538f5ffec599f600ee93aedbbecad8aa4f8bec539b10ad8 PHP_MD5=
# Thu, 16 Apr 2020 21:24:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Apr 2020 21:24:24 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Apr 2020 21:28:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 16 Apr 2020 21:28:45 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 16 Apr 2020 21:28:47 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Apr 2020 21:28:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Apr 2020 21:28:48 GMT
WORKDIR /var/www/html
# Thu, 16 Apr 2020 21:28:50 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 16 Apr 2020 21:28:51 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Apr 2020 21:28:51 GMT
EXPOSE 9000
# Thu, 16 Apr 2020 21:28:52 GMT
CMD ["php-fpm"]
# Thu, 16 Apr 2020 22:51:35 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 16 Apr 2020 22:51:40 GMT
RUN apk add --no-cache 		bash 		coreutils
# Thu, 16 Apr 2020 22:52:39 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		sqlite-dev 		postgresql-dev 	; 	docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 16 Apr 2020 22:52:40 GMT
ARG POSTFIXADMIN_VERSION=3.2.3
# Thu, 16 Apr 2020 22:52:41 GMT
ARG POSTFIXADMIN_SHA512=d44addb9a3ca830caf55b603363054df561d659957f21cab7523465ebf02ca18abe7fcf298fe718d957d0b7bf5613e2dde69c78c26e0f7f6f595d79b28fe08ab
# Thu, 16 Apr 2020 22:52:41 GMT
ENV POSTFIXADMIN_VERSION=3.2.3
# Thu, 16 Apr 2020 22:52:43 GMT
ENV POSTFIXADMIN_SHA512=d44addb9a3ca830caf55b603363054df561d659957f21cab7523465ebf02ca18abe7fcf298fe718d957d0b7bf5613e2dde69c78c26e0f7f6f595d79b28fe08ab
# Thu, 16 Apr 2020 22:52:46 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 16 Apr 2020 22:52:47 GMT
COPY file:83be1dbd46cfa4c9ff6241f21a00fcd952c07b15bab1c6cf82fac6bfbae210c8 in /usr/local/bin/ 
# Thu, 16 Apr 2020 22:52:48 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 16 Apr 2020 22:52:49 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ea08e138832a1357c5a2058da55929de016d0715372ec90df8716d8f08e8aa`  
		Last Modified: Tue, 24 Mar 2020 02:56:26 GMT  
		Size: 1.3 MB (1321096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6155177d2f4f58391e952733581935ca259371ca891a8e72311ff15a4b0caaf9`  
		Last Modified: Tue, 24 Mar 2020 02:56:26 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64588fb2e6842997faa53e9e5d4ec63be60ac226be4ae2eb5a97bff62263b14e`  
		Last Modified: Tue, 24 Mar 2020 02:56:25 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7080eed68284b7455cf60bd385ebd6768963f76c1165c8c162e5d341db1acc6e`  
		Last Modified: Thu, 16 Apr 2020 21:49:47 GMT  
		Size: 12.1 MB (12135777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04539e418f4743ae9133bb0ab4e889badf0eb6fe2768b93d4df2bcfcd52207c6`  
		Last Modified: Thu, 16 Apr 2020 21:49:43 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8cb31d73cb33cee8400bd7166a1a2d415822b2ec78b35e5f7d72b3828269706`  
		Last Modified: Thu, 16 Apr 2020 21:49:49 GMT  
		Size: 13.4 MB (13428120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98e074fa81faa0c34ac7ac0ab1613941f65be512d0ee4e1000d4183a4fa3dd2b`  
		Last Modified: Thu, 16 Apr 2020 21:49:43 GMT  
		Size: 2.2 KB (2215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6db4db65ac1fad5127236b4d218fbe65af66f86180fd5265c1b1f927ca0ff23`  
		Last Modified: Thu, 16 Apr 2020 21:49:43 GMT  
		Size: 17.1 KB (17064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37caa7c5bb1c66852c507be1e58c44d46e9c874d105c70568209454ba7067c2d`  
		Last Modified: Thu, 16 Apr 2020 21:49:44 GMT  
		Size: 8.4 KB (8417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b80a8141bc501575464bc5a23cedef4d8ec0d2c59713ac1a3de8adc51258e7a`  
		Last Modified: Thu, 16 Apr 2020 22:53:10 GMT  
		Size: 1.1 MB (1108889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eea40effe34c801c99311a87d81064aec593e538e84913c41dd3e121b1691e14`  
		Last Modified: Thu, 16 Apr 2020 22:53:11 GMT  
		Size: 2.8 MB (2849014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27ddb4ae39663bc3603c24c46cbbed6da803f1530ddd4ad4204bc6c41f89567`  
		Last Modified: Thu, 16 Apr 2020 22:53:11 GMT  
		Size: 1.3 MB (1333795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:861827fafc260cb26542290e30fac49ed950e54065c6101735921a0f21c5c2a6`  
		Last Modified: Thu, 16 Apr 2020 22:53:11 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; arm variant v7

```console
$ docker pull postfixadmin@sha256:c467fe4e6dbcab7ad778953e596effd7a9e5565411664d846c4c79af31882b15
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33448290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ba34351f392398f6e5a066b85d5079bc2da23a2e34c0bd67cb132011125ef7ba`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 01:36:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 01:36:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 01:36:39 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 01:36:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 01:36:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 01:39:39 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 01:39:40 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 01:39:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 01:39:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Tue, 24 Mar 2020 01:49:08 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 24 Mar 2020 01:49:09 GMT
ENV PHP_VERSION=7.3.16
# Tue, 24 Mar 2020 01:49:09 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.16.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.16.tar.xz.asc/from/this/mirror
# Tue, 24 Mar 2020 01:49:10 GMT
ENV PHP_SHA256=91aaee3dbdc71b69b4f3292f9d99211172a2fa926c3f3bbdb0e85dab03dd2bcb PHP_MD5=
# Tue, 24 Mar 2020 01:49:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 24 Mar 2020 01:49:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 24 Mar 2020 01:51:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 24 Mar 2020 01:51:48 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Tue, 24 Mar 2020 01:51:50 GMT
RUN docker-php-ext-enable sodium
# Tue, 24 Mar 2020 01:51:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 24 Mar 2020 01:51:51 GMT
WORKDIR /var/www/html
# Tue, 24 Mar 2020 01:51:54 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 24 Mar 2020 01:51:54 GMT
STOPSIGNAL SIGQUIT
# Tue, 24 Mar 2020 01:51:55 GMT
EXPOSE 9000
# Tue, 24 Mar 2020 01:51:56 GMT
CMD ["php-fpm"]
# Tue, 24 Mar 2020 03:35:08 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Tue, 24 Mar 2020 03:35:12 GMT
RUN apk add --no-cache 		bash 		coreutils
# Tue, 24 Mar 2020 03:36:14 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		sqlite-dev 		postgresql-dev 	; 	docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Tue, 24 Mar 2020 03:36:16 GMT
ARG POSTFIXADMIN_VERSION=3.2.3
# Tue, 24 Mar 2020 03:36:17 GMT
ARG POSTFIXADMIN_SHA512=d44addb9a3ca830caf55b603363054df561d659957f21cab7523465ebf02ca18abe7fcf298fe718d957d0b7bf5613e2dde69c78c26e0f7f6f595d79b28fe08ab
# Tue, 24 Mar 2020 03:36:18 GMT
ENV POSTFIXADMIN_VERSION=3.2.3
# Tue, 24 Mar 2020 03:36:19 GMT
ENV POSTFIXADMIN_SHA512=d44addb9a3ca830caf55b603363054df561d659957f21cab7523465ebf02ca18abe7fcf298fe718d957d0b7bf5613e2dde69c78c26e0f7f6f595d79b28fe08ab
# Tue, 24 Mar 2020 03:36:25 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Tue, 24 Mar 2020 03:36:27 GMT
COPY file:83be1dbd46cfa4c9ff6241f21a00fcd952c07b15bab1c6cf82fac6bfbae210c8 in /usr/local/bin/ 
# Tue, 24 Mar 2020 03:36:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 24 Mar 2020 03:36:29 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221e0c8c991c3fdd8db1ec76c1a911aa0f946325ec2cf15d22a25693accc6edc`  
		Last Modified: Tue, 24 Mar 2020 02:07:16 GMT  
		Size: 1.2 MB (1227325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeaee6722c9e078934e8f34fe0dc55d3f3c28d742e92ce6b3e86775beaeeb44`  
		Last Modified: Tue, 24 Mar 2020 02:07:16 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84528978bcc1c0fe1d795bbe412f0a4123fa9119c11c98cd9b1ab8c5db8203f0`  
		Last Modified: Tue, 24 Mar 2020 02:07:16 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eda6e0d34e828ce8e8dd9efb0c2272f1addf00e813d5faa0e250ac1e56b726a`  
		Last Modified: Tue, 24 Mar 2020 02:08:51 GMT  
		Size: 12.1 MB (12133369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:581fd0df565dfdf9fa030d939cc5438a85b6a1aadd9cfb8e17f0cffd8d78a000`  
		Last Modified: Tue, 24 Mar 2020 02:08:47 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f838a6efa2443ba97bb2214f15dc321f29394c259618e664c272cd1e3e8738`  
		Last Modified: Tue, 24 Mar 2020 02:08:51 GMT  
		Size: 12.6 MB (12563182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87befac5eace204a0f989da42597e3ed787680fa956a946afec52808fe9d55a6`  
		Last Modified: Tue, 24 Mar 2020 02:08:48 GMT  
		Size: 2.2 KB (2213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24bc33b4319ab2bdff433bcfc1ebce2a3464819a641eee06e19dd6e50c2dec5`  
		Last Modified: Tue, 24 Mar 2020 02:08:48 GMT  
		Size: 16.9 KB (16865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dcb66b93ceaaf184b0f0be65fcb63eb8ab5f305046ef5216110e140c4b53d6a`  
		Last Modified: Tue, 24 Mar 2020 02:08:48 GMT  
		Size: 8.4 KB (8411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cab767f08bf71f76817ac33efb4e0a1219e550679e654ee7b9ff8544c20f515`  
		Last Modified: Tue, 24 Mar 2020 03:37:20 GMT  
		Size: 1.0 MB (1007409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6220607217804baa59e5e6bb72d4057c21ed07f5fbf524cfe227d611a7713425`  
		Last Modified: Tue, 24 Mar 2020 03:37:21 GMT  
		Size: 2.7 MB (2731929 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feb2f1fcd77c918239cb475539cc9857eea023780f9b6b3c8c280a0012de9ae1`  
		Last Modified: Tue, 24 Mar 2020 03:37:21 GMT  
		Size: 1.3 MB (1333793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5de9cb11a23082270025b6ef3fc04bbc32394fc22c578740728bbf990dc5108f`  
		Last Modified: Tue, 24 Mar 2020 03:37:20 GMT  
		Size: 1.3 KB (1279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull postfixadmin@sha256:ec98f473623b1df74a9b33f4215867c9a1b7c86f74dba405171d6d25fb8b5a12
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35876923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17181c1f62fc2dd5bfe663c51ee147785d6b51729e8025d7ec7bcf4550f5c7b9`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:27:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 00:27:19 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 00:27:21 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 00:27:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 00:27:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 00:31:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 00:31:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 00:31:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 00:31:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Tue, 24 Mar 2020 00:43:23 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 24 Mar 2020 00:43:23 GMT
ENV PHP_VERSION=7.3.16
# Tue, 24 Mar 2020 00:43:25 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.16.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.16.tar.xz.asc/from/this/mirror
# Tue, 24 Mar 2020 00:43:26 GMT
ENV PHP_SHA256=91aaee3dbdc71b69b4f3292f9d99211172a2fa926c3f3bbdb0e85dab03dd2bcb PHP_MD5=
# Tue, 24 Mar 2020 00:43:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 24 Mar 2020 00:43:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 24 Mar 2020 00:46:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 24 Mar 2020 00:46:28 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Tue, 24 Mar 2020 00:46:31 GMT
RUN docker-php-ext-enable sodium
# Tue, 24 Mar 2020 00:46:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 24 Mar 2020 00:46:32 GMT
WORKDIR /var/www/html
# Tue, 24 Mar 2020 00:46:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 24 Mar 2020 00:46:35 GMT
STOPSIGNAL SIGQUIT
# Tue, 24 Mar 2020 00:46:36 GMT
EXPOSE 9000
# Tue, 24 Mar 2020 00:46:36 GMT
CMD ["php-fpm"]
# Tue, 24 Mar 2020 07:11:58 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Tue, 24 Mar 2020 07:12:00 GMT
RUN apk add --no-cache 		bash 		coreutils
# Tue, 24 Mar 2020 07:12:45 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		sqlite-dev 		postgresql-dev 	; 	docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Tue, 24 Mar 2020 07:12:46 GMT
ARG POSTFIXADMIN_VERSION=3.2.3
# Tue, 24 Mar 2020 07:12:46 GMT
ARG POSTFIXADMIN_SHA512=d44addb9a3ca830caf55b603363054df561d659957f21cab7523465ebf02ca18abe7fcf298fe718d957d0b7bf5613e2dde69c78c26e0f7f6f595d79b28fe08ab
# Tue, 24 Mar 2020 07:12:47 GMT
ENV POSTFIXADMIN_VERSION=3.2.3
# Tue, 24 Mar 2020 07:12:48 GMT
ENV POSTFIXADMIN_SHA512=d44addb9a3ca830caf55b603363054df561d659957f21cab7523465ebf02ca18abe7fcf298fe718d957d0b7bf5613e2dde69c78c26e0f7f6f595d79b28fe08ab
# Tue, 24 Mar 2020 07:12:50 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Tue, 24 Mar 2020 07:12:51 GMT
COPY file:83be1dbd46cfa4c9ff6241f21a00fcd952c07b15bab1c6cf82fac6bfbae210c8 in /usr/local/bin/ 
# Tue, 24 Mar 2020 07:12:51 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 24 Mar 2020 07:12:52 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee501176ea6c9d16dc12649d7c62f4b6466cc96eaf80bfcea3aa261a052ec099`  
		Last Modified: Tue, 24 Mar 2020 01:03:05 GMT  
		Size: 1.4 MB (1359430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876007701d95df62eb874f76916e4d139709812e5e0be471c4107729808d6af`  
		Last Modified: Tue, 24 Mar 2020 01:03:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ed02bd016dcfb57e62d938f46a81237af426353ef7df647b64c3b3a93276a7`  
		Last Modified: Tue, 24 Mar 2020 01:03:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2cc8840affcbe1779c1af710215aa419bd5623de8e3ce5a27f7812e5bd6f5b`  
		Last Modified: Tue, 24 Mar 2020 01:04:37 GMT  
		Size: 12.1 MB (12133363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc407b68bcf3dd2fd76e069843663d462611cfadc74467b1535df447a95b0e55`  
		Last Modified: Tue, 24 Mar 2020 01:04:33 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ab01b4a37f1f8a9b9f356d82f8ee3ee9205b0acce0a23e213e4838eb580060c`  
		Last Modified: Tue, 24 Mar 2020 01:04:39 GMT  
		Size: 14.2 MB (14200626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1063d773aa59567942be63285eb6f4b4ab0b9559ba0ecd953c8cfa77e91f2e30`  
		Last Modified: Tue, 24 Mar 2020 01:04:33 GMT  
		Size: 2.2 KB (2219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e89b212938840b5a387f36fa9338b4ef45391c796a35993ef22d2016112377e`  
		Last Modified: Tue, 24 Mar 2020 01:04:33 GMT  
		Size: 16.9 KB (16892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a4f70c5290d7f704641b7581a0b95a9d6959c50247ad72bc3c91f7d686b5394`  
		Last Modified: Tue, 24 Mar 2020 01:04:34 GMT  
		Size: 8.4 KB (8410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d69ba91077983d945300ad63fe7ca943138b5b24439ad961d7d004958ee920`  
		Last Modified: Tue, 24 Mar 2020 07:13:25 GMT  
		Size: 1.1 MB (1122354 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b120dc9321cdb164237ab4635885f375eb957f17631d4e0c5868f8bbdaa2c3f`  
		Last Modified: Tue, 24 Mar 2020 07:13:25 GMT  
		Size: 3.0 MB (2973402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b387e5ee01da44d509de92d550f4df55c333b25ba089ce673376df2bb14b3b46`  
		Last Modified: Tue, 24 Mar 2020 07:13:25 GMT  
		Size: 1.3 MB (1333793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f8cb8982d1be3f33fe483245ad3284b8c27d45550e9b925d4328d0471b97954`  
		Last Modified: Tue, 24 Mar 2020 07:13:25 GMT  
		Size: 1.3 KB (1273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; 386

```console
$ docker pull postfixadmin@sha256:602f8c4ae49bbf1255ba1fe3064477a87d86ab8b258854dcb223448d69ea48fd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.9 MB (36856485 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cb0164f272209bc6099b7149f7db8ca21b9b17fca4d33c407f71661447a8d73`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:38:28 GMT
ADD file:99c8234abafd4fa915c0b826eb0e3be0e6aaa7c1e33cb1214ef71a99e9c02e06 in / 
# Mon, 23 Mar 2020 21:38:28 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 02:43:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 02:43:35 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 02:43:36 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 02:43:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 02:43:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 02:51:22 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 02:51:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 02:51:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 02:51:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Tue, 24 Mar 2020 03:17:11 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 16 Apr 2020 23:28:24 GMT
ENV PHP_VERSION=7.3.17
# Thu, 16 Apr 2020 23:28:25 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.17.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.17.tar.xz.asc/from/this/mirror
# Thu, 16 Apr 2020 23:28:25 GMT
ENV PHP_SHA256=6a30304c27f7e7a94538f5ffec599f600ee93aedbbecad8aa4f8bec539b10ad8 PHP_MD5=
# Thu, 16 Apr 2020 23:28:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Apr 2020 23:28:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Apr 2020 23:37:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 16 Apr 2020 23:37:26 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 16 Apr 2020 23:37:28 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Apr 2020 23:37:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Apr 2020 23:37:29 GMT
WORKDIR /var/www/html
# Thu, 16 Apr 2020 23:37:30 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 16 Apr 2020 23:37:30 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Apr 2020 23:37:31 GMT
EXPOSE 9000
# Thu, 16 Apr 2020 23:37:31 GMT
CMD ["php-fpm"]
# Fri, 17 Apr 2020 01:48:42 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 17 Apr 2020 01:48:45 GMT
RUN apk add --no-cache 		bash 		coreutils
# Fri, 17 Apr 2020 01:49:40 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		sqlite-dev 		postgresql-dev 	; 	docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 17 Apr 2020 01:49:41 GMT
ARG POSTFIXADMIN_VERSION=3.2.3
# Fri, 17 Apr 2020 01:49:41 GMT
ARG POSTFIXADMIN_SHA512=d44addb9a3ca830caf55b603363054df561d659957f21cab7523465ebf02ca18abe7fcf298fe718d957d0b7bf5613e2dde69c78c26e0f7f6f595d79b28fe08ab
# Fri, 17 Apr 2020 01:49:42 GMT
ENV POSTFIXADMIN_VERSION=3.2.3
# Fri, 17 Apr 2020 01:49:42 GMT
ENV POSTFIXADMIN_SHA512=d44addb9a3ca830caf55b603363054df561d659957f21cab7523465ebf02ca18abe7fcf298fe718d957d0b7bf5613e2dde69c78c26e0f7f6f595d79b28fe08ab
# Fri, 17 Apr 2020 01:49:45 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 17 Apr 2020 01:49:45 GMT
COPY file:83be1dbd46cfa4c9ff6241f21a00fcd952c07b15bab1c6cf82fac6bfbae210c8 in /usr/local/bin/ 
# Fri, 17 Apr 2020 01:49:45 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 17 Apr 2020 01:49:46 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:43f6a4398e1c9e860dfb5c93d7049ab9eedf814513bd6d07e06077c560303c7a`  
		Last Modified: Mon, 23 Mar 2020 21:38:48 GMT  
		Size: 2.8 MB (2806122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8addccc9b68d6aad59a5f93e0ca1813c5d09a0c7943108d860d8c29f6bebdb5`  
		Last Modified: Tue, 24 Mar 2020 04:03:48 GMT  
		Size: 1.5 MB (1452601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb273244de1495dfb0044080245a9fa0c6f3d8a2ab5f30610237d9a76e66cd4`  
		Last Modified: Tue, 24 Mar 2020 04:03:47 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d6dffa3f09145ac45428f87b062a4603137dadcaa84454812f81f70b71ea07`  
		Last Modified: Tue, 24 Mar 2020 04:03:47 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed9722924b705c741520c91b9f3be18edcc473ac47bfc9a164e1e14fa74b7b1f`  
		Last Modified: Fri, 17 Apr 2020 00:16:46 GMT  
		Size: 12.1 MB (12135764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ad1893a363545a9820327dc36be7b895b2fc2a9b0b791716519bba7782299c`  
		Last Modified: Fri, 17 Apr 2020 00:16:44 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fac5475cb4370c99b569755439998e484833e1a017e015a6ca206bbc71914d6`  
		Last Modified: Fri, 17 Apr 2020 00:16:49 GMT  
		Size: 14.8 MB (14842633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8b7194ddb54d549f091f93818eba5ba5154d80bafe250a180657630e051a765`  
		Last Modified: Fri, 17 Apr 2020 00:16:43 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76c9e3c3d645ef428b09c405777cac765323931a0caef24ddc4e9643eccae648`  
		Last Modified: Fri, 17 Apr 2020 00:16:43 GMT  
		Size: 17.1 KB (17060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9905f6e1e864ecbb65d5c717cc99e72e771972b8f6a68ae70043cdcd21ad5d73`  
		Last Modified: Fri, 17 Apr 2020 00:16:44 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325b0b6d800f641d0228eda17b34f55225369827ccdace1506df7bdb4b2023d7`  
		Last Modified: Fri, 17 Apr 2020 01:50:34 GMT  
		Size: 1.2 MB (1187457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2acf41117a7abb22b2f2002cb9bc445778a795815626843fe5f050aa7a92380`  
		Last Modified: Fri, 17 Apr 2020 01:50:34 GMT  
		Size: 3.1 MB (3067208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db9260f808e5f2d7f971d128d28c24dab0a8e8f6ed3e997fdde439c2dd168eb`  
		Last Modified: Fri, 17 Apr 2020 01:50:34 GMT  
		Size: 1.3 MB (1333783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:130561c65c511f51df1f414d2a07f3ea30ca5ff8363fdbacfa1da99d3cd55cf1`  
		Last Modified: Fri, 17 Apr 2020 01:50:32 GMT  
		Size: 1.3 KB (1276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:fpm-alpine` - linux; ppc64le

```console
$ docker pull postfixadmin@sha256:1fa77c3d19f76d81961fe0f42fb0b24e16026cfe0af2c50d4a76e36faa21c279
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37388908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c22f8e8107844f2f01ed02a42af7f2276cb2600edc3d84b2b8f212b30bf56127`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:21:29 GMT
ADD file:4b35131542b9682214e1c2c72fe3cea215a10e2f775e87befecd80fe2228d5a0 in / 
# Mon, 23 Mar 2020 21:21:32 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:27:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 00:27:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 00:27:38 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 00:27:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 00:27:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 00:32:28 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 00:32:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 00:32:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 00:32:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Tue, 24 Mar 2020 00:47:49 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 24 Mar 2020 00:47:51 GMT
ENV PHP_VERSION=7.3.16
# Tue, 24 Mar 2020 00:47:54 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.16.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.16.tar.xz.asc/from/this/mirror
# Tue, 24 Mar 2020 00:47:57 GMT
ENV PHP_SHA256=91aaee3dbdc71b69b4f3292f9d99211172a2fa926c3f3bbdb0e85dab03dd2bcb PHP_MD5=
# Tue, 24 Mar 2020 00:48:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 24 Mar 2020 00:48:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 24 Mar 2020 00:52:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Tue, 24 Mar 2020 00:52:17 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Tue, 24 Mar 2020 00:52:28 GMT
RUN docker-php-ext-enable sodium
# Tue, 24 Mar 2020 00:52:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 24 Mar 2020 00:52:36 GMT
WORKDIR /var/www/html
# Tue, 24 Mar 2020 00:52:47 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 24 Mar 2020 00:52:50 GMT
STOPSIGNAL SIGQUIT
# Tue, 24 Mar 2020 00:52:56 GMT
EXPOSE 9000
# Tue, 24 Mar 2020 00:53:01 GMT
CMD ["php-fpm"]
# Tue, 24 Mar 2020 04:21:41 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Tue, 24 Mar 2020 04:21:48 GMT
RUN apk add --no-cache 		bash 		coreutils
# Tue, 24 Mar 2020 04:22:29 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		sqlite-dev 		postgresql-dev 	; 	docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Tue, 24 Mar 2020 04:22:31 GMT
ARG POSTFIXADMIN_VERSION=3.2.3
# Tue, 24 Mar 2020 04:22:34 GMT
ARG POSTFIXADMIN_SHA512=d44addb9a3ca830caf55b603363054df561d659957f21cab7523465ebf02ca18abe7fcf298fe718d957d0b7bf5613e2dde69c78c26e0f7f6f595d79b28fe08ab
# Tue, 24 Mar 2020 04:22:37 GMT
ENV POSTFIXADMIN_VERSION=3.2.3
# Tue, 24 Mar 2020 04:22:39 GMT
ENV POSTFIXADMIN_SHA512=d44addb9a3ca830caf55b603363054df561d659957f21cab7523465ebf02ca18abe7fcf298fe718d957d0b7bf5613e2dde69c78c26e0f7f6f595d79b28fe08ab
# Tue, 24 Mar 2020 04:22:47 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Tue, 24 Mar 2020 04:22:50 GMT
COPY file:83be1dbd46cfa4c9ff6241f21a00fcd952c07b15bab1c6cf82fac6bfbae210c8 in /usr/local/bin/ 
# Tue, 24 Mar 2020 04:22:53 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Tue, 24 Mar 2020 04:22:55 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:bc1c99f4ba60de0d3ca52dc6855483e24c91884e33df71f502bbff6eb909d9b9`  
		Last Modified: Mon, 23 Mar 2020 21:22:12 GMT  
		Size: 2.8 MB (2820052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681c4a6dbdeb5b4877c85db3edbb08e40a877342795a3e7ba7f543a65586c417`  
		Last Modified: Tue, 24 Mar 2020 01:16:24 GMT  
		Size: 1.4 MB (1397873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e23455f025d83291061d4165e722b934e986f58c2b3d71b62a0918166d19db`  
		Last Modified: Tue, 24 Mar 2020 01:16:23 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c3447d90e80a01a72c494bf3563b1379704fcf4fb8b5b207596bbeeac49fc3`  
		Last Modified: Tue, 24 Mar 2020 01:16:22 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc254a86c9277744e5d5921909889f235e10113bc35de89f269763623419a2c7`  
		Last Modified: Tue, 24 Mar 2020 01:18:50 GMT  
		Size: 12.1 MB (12133377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98942a1122c3eeb1e146b0d5e1292cc308a99df4a2bbef470291b4073d86bc9`  
		Last Modified: Tue, 24 Mar 2020 01:18:46 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f171cdde581ebda3a09092fee88c92865e75df5fe91fa15059f313c520f1c4f6`  
		Last Modified: Tue, 24 Mar 2020 01:18:50 GMT  
		Size: 15.5 MB (15483479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7f27b32f8500e4ec3ba7bf8a7b9d962ead0df603de44068135df4d959a0aac`  
		Last Modified: Tue, 24 Mar 2020 01:18:46 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adaf87e529908aa18bf53d65009afdea973db887e28144ce1221ec5aa70bf7be`  
		Last Modified: Tue, 24 Mar 2020 01:18:45 GMT  
		Size: 16.9 KB (16876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2a188be6bc76b4405243d376fc5a21e7065e1988fcafcf0d77d061666431726`  
		Last Modified: Tue, 24 Mar 2020 01:18:45 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45526e1aba5c811849d9f7b4c5631a3de1205b3388d0a9a2ea55777bee40b49`  
		Last Modified: Tue, 24 Mar 2020 04:23:28 GMT  
		Size: 1.2 MB (1179773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e87334f40499f31d62cfda959d3affcd39188ca3df5e6f7e153d62e66715a42`  
		Last Modified: Tue, 24 Mar 2020 04:23:28 GMT  
		Size: 3.0 MB (3009762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a504915ddd8ad87e6fbe045a814d76931564dcd310e02a1ce75d4cfd72be859a`  
		Last Modified: Tue, 24 Mar 2020 04:23:28 GMT  
		Size: 1.3 MB (1333790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95777df91f814fb412693bd08b491d21544904a6dacfc0ee23177f4a7aee4810`  
		Last Modified: Tue, 24 Mar 2020 04:23:27 GMT  
		Size: 1.3 KB (1275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
