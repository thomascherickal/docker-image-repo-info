## `php:7-cli-alpine3.11`

```console
$ docker pull php@sha256:cca3223dd47fb67aed2823a56bdae000a3b16f9416919c61465b94d921792633
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `php:7-cli-alpine3.11` - linux; amd64

```console
$ docker pull php@sha256:9eba9931dab5b5747c9dccdb755357c26be37cb366c0720231ec7ee283424b37
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.7 MB (30656461 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46270e428dbb548c7b9b312f90e24a6c97d1f1de19205eabeea8098d08592cae`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 24 Dec 2019 19:20:12 GMT
ADD file:36fdc8cb08228a87093fb227736f4ce1d4d6c15366326dea541fbbd863976ee5 in / 
# Tue, 24 Dec 2019 19:20:12 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 21:47:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 26 Dec 2019 21:47:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 26 Dec 2019 21:47:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 26 Dec 2019 21:47:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 26 Dec 2019 21:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 26 Dec 2019 21:47:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 26 Dec 2019 21:47:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 26 Dec 2019 21:47:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 26 Dec 2019 21:47:55 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 26 Dec 2019 21:47:55 GMT
ENV PHP_VERSION=7.4.1
# Thu, 26 Dec 2019 21:47:55 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.1.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.1.tar.xz.asc/from/this/mirror
# Thu, 26 Dec 2019 21:47:55 GMT
ENV PHP_SHA256=561bb866bdd509094be00f4ece7c3543ec971c4d878645ee81437e291cffc762 PHP_MD5=
# Thu, 26 Dec 2019 21:47:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 26 Dec 2019 21:47:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 26 Dec 2019 21:55:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 26 Dec 2019 21:55:56 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Thu, 26 Dec 2019 21:55:58 GMT
RUN docker-php-ext-enable sodium
# Thu, 26 Dec 2019 21:55:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 26 Dec 2019 21:55:58 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:e6b0cf9c0882fb079c9d35361d12ff4691f916b6d825061247d1bd0b26d7cf3f`  
		Last Modified: Tue, 24 Dec 2019 19:20:40 GMT  
		Size: 2.8 MB (2801778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c7a574e8632727fe466d1871c39e4fea951243dc9f0a56bdc55cb8720f4aac6`  
		Last Modified: Thu, 26 Dec 2019 23:05:01 GMT  
		Size: 1.4 MB (1354713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a6c65f587e94ae6bd946a70d456e75c7543d38cb03271622a815f3b5398ec74`  
		Last Modified: Thu, 26 Dec 2019 23:05:00 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba33e4b639bb4e1187590b34ea007a27393fbda41d6f3ad10d04c9a0bd1cde4a`  
		Last Modified: Thu, 26 Dec 2019 23:05:00 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94182f10949f8b172016cbddea1d7b4417514c40d0fd664a0895d3b0f93fcbe`  
		Last Modified: Thu, 26 Dec 2019 23:05:00 GMT  
		Size: 10.3 MB (10264403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06b2b4baeabcdc2692442b4f6a6512b1f6b20697c8ec9b984503705cc81039a`  
		Last Modified: Thu, 26 Dec 2019 23:04:59 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6abb9ac3b49074e4561b65dbf3c4beaab0b50ef72743a04656dd6e664bcdecc`  
		Last Modified: Thu, 26 Dec 2019 23:05:03 GMT  
		Size: 16.2 MB (16158246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8028c0b7a7e712cf77e535c0d109ae5bce6ae34cefcd8ebf46b640214b5c91`  
		Last Modified: Thu, 26 Dec 2019 23:04:59 GMT  
		Size: 2.2 KB (2217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1cc7bad024a2e7896c445c24345d1b9226c1c7ed0adbc57145db4d8ce9aea2f`  
		Last Modified: Thu, 26 Dec 2019 23:04:59 GMT  
		Size: 73.2 KB (73165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-alpine3.11` - linux; arm variant v6

```console
$ docker pull php@sha256:b877057eca41c87d45e887b0730ceeef5e80311c6d8ef46049f4b8a35fab16f1
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.2 MB (29237318 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fcf1e6fc15f7400de85a1ea3971cd7efec6687196e95a21b531367d436d19ac2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 24 Dec 2019 18:49:41 GMT
ADD file:c4f944e24d0f2e758363506e8b98b3b53973ec18dd4dd23da3f09520ef22c65c in / 
# Tue, 24 Dec 2019 18:49:42 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 22:20:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 26 Dec 2019 22:20:16 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 26 Dec 2019 22:20:18 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 26 Dec 2019 22:20:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 26 Dec 2019 22:20:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 26 Dec 2019 22:20:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 26 Dec 2019 22:20:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 26 Dec 2019 22:20:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 26 Dec 2019 22:20:24 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 26 Dec 2019 22:20:25 GMT
ENV PHP_VERSION=7.4.1
# Thu, 26 Dec 2019 22:20:26 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.1.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.1.tar.xz.asc/from/this/mirror
# Thu, 26 Dec 2019 22:20:27 GMT
ENV PHP_SHA256=561bb866bdd509094be00f4ece7c3543ec971c4d878645ee81437e291cffc762 PHP_MD5=
# Thu, 26 Dec 2019 22:20:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 26 Dec 2019 22:20:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 26 Dec 2019 22:24:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 26 Dec 2019 22:24:26 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Thu, 26 Dec 2019 22:24:30 GMT
RUN docker-php-ext-enable sodium
# Thu, 26 Dec 2019 22:24:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 26 Dec 2019 22:24:35 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:546eec1e02ac5f4494868d8b22e8ced00773a2fba8e25b3edd30002889874299`  
		Last Modified: Tue, 24 Dec 2019 18:50:07 GMT  
		Size: 2.6 MB (2612021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f2222aeb0ea56ad08de7753e2ed3f6c40f7093cda7436e94583ce0f0922072`  
		Last Modified: Thu, 26 Dec 2019 23:02:36 GMT  
		Size: 1.3 MB (1321130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f893e696ec7590309f1a77539ce734af052f1aa42c48aaf6f478453dcd7eafa`  
		Last Modified: Thu, 26 Dec 2019 23:02:35 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ad230ebfba33233fbafdd19ca2939dfd20dffdc83636c23f9285017935fca9`  
		Last Modified: Thu, 26 Dec 2019 23:02:35 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44905e88daf12c640968d3d790a02e11babe5d4f4730e6fcd3eae081f8df2f62`  
		Last Modified: Thu, 26 Dec 2019 23:02:34 GMT  
		Size: 10.3 MB (10264410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e91ff6ebef94b35989b1200b9d2564b71aa5e20f03fbc2c75bf57786cdca79`  
		Last Modified: Thu, 26 Dec 2019 23:02:34 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e6b1bfceee6e3798ac6b36213aede482172b522e4c9d17635d9418419bd0672`  
		Last Modified: Thu, 26 Dec 2019 23:02:39 GMT  
		Size: 15.0 MB (14962846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb6b063069fde53011cbbab0f1fc6cb9f8b02fb20f6f0e986394d971347f38c0`  
		Last Modified: Thu, 26 Dec 2019 23:02:34 GMT  
		Size: 2.2 KB (2214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f29f685cf530bfbe1b0003111bed088314ef583a2585bb11a10d7463dfc5dd8`  
		Last Modified: Thu, 26 Dec 2019 23:02:34 GMT  
		Size: 72.7 KB (72680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-alpine3.11` - linux; arm variant v7

```console
$ docker pull php@sha256:caf3f215ae94652f32fd4609aad78ec5ccaf161694fb0d7c687f653a5d6c9ae9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28020667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7fb7264ab8c6c091c1dddbf2ec8bbccb6979c34faed0ab01a933349a397c2bc`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 24 Dec 2019 18:59:09 GMT
ADD file:caf7ca25875eddd2bfa2d1e56663bb52d278a85f6ee1314f9ccf01dc4da8070a in / 
# Tue, 24 Dec 2019 18:59:10 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 21:28:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 26 Dec 2019 21:28:59 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 26 Dec 2019 21:29:01 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 26 Dec 2019 21:29:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 26 Dec 2019 21:29:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 26 Dec 2019 21:29:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 26 Dec 2019 21:29:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 26 Dec 2019 21:29:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 26 Dec 2019 21:29:05 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 26 Dec 2019 21:29:05 GMT
ENV PHP_VERSION=7.4.1
# Thu, 26 Dec 2019 21:29:06 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.1.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.1.tar.xz.asc/from/this/mirror
# Thu, 26 Dec 2019 21:29:06 GMT
ENV PHP_SHA256=561bb866bdd509094be00f4ece7c3543ec971c4d878645ee81437e291cffc762 PHP_MD5=
# Thu, 26 Dec 2019 21:29:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 26 Dec 2019 21:29:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 26 Dec 2019 21:31:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 26 Dec 2019 21:31:34 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Thu, 26 Dec 2019 21:31:36 GMT
RUN docker-php-ext-enable sodium
# Thu, 26 Dec 2019 21:31:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 26 Dec 2019 21:31:38 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:3922e475e500b2739b5e74787fc80622853325822f71f8bd3de7e5b09654d60f`  
		Last Modified: Tue, 24 Dec 2019 18:59:33 GMT  
		Size: 2.4 MB (2416691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d850653ef66a74bc2f65e933df679895db53bc6e01d23076dbc532056eec8a7`  
		Last Modified: Thu, 26 Dec 2019 22:01:17 GMT  
		Size: 1.2 MB (1227347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed0b2f0bcd9c23ef1f79be9d752fea5f714457c75308002cf597d596e8b1c1a`  
		Last Modified: Thu, 26 Dec 2019 22:01:17 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d77de73a7de2b81d6828d80578fc934edf55e039effcf2bb8555e6a0b5864080`  
		Last Modified: Thu, 26 Dec 2019 22:01:17 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc1b35828f88798cdf411520e8541662fa44c3e21d0b46b668e5ad1ce38f24`  
		Last Modified: Thu, 26 Dec 2019 22:01:17 GMT  
		Size: 10.3 MB (10264419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1ac53e078b99a6ba0cf4e8600a0ba5aa6bd3b579e0f86d78a3b18bd692976a`  
		Last Modified: Thu, 26 Dec 2019 22:01:16 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a349634f832daa7e54f052c5c5fce54336c7089c5997981c3be8552baf32c10c`  
		Last Modified: Thu, 26 Dec 2019 22:01:21 GMT  
		Size: 14.0 MB (14035302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef07c3ed8c6baead6c71677fb97b0bef1c3762881b234e8ed7aa21c0470854ed`  
		Last Modified: Thu, 26 Dec 2019 22:01:16 GMT  
		Size: 2.2 KB (2216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01eab0467fa0094e7e35ef8de9b09468e7ae8b53efc431442a1a9af5a5be310a`  
		Last Modified: Thu, 26 Dec 2019 22:01:16 GMT  
		Size: 72.7 KB (72675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull php@sha256:cf27182d3fc5b0909f933147257a5a4b89da6365e4259bbdf53e9e9bf6aafde4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.8 MB (28786464 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3271813d8f3a723d6fda8b6d29d061f7355d0cbc917df062e8caa6d2eca08936`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:29:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 18 Jan 2020 02:29:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 18 Jan 2020 02:29:16 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 02:29:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 18 Jan 2020 02:29:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 18 Jan 2020 02:29:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 02:29:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 02:29:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 18 Jan 2020 02:29:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 18 Jan 2020 02:29:30 GMT
ENV PHP_VERSION=7.4.1
# Sat, 18 Jan 2020 02:29:32 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.1.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.1.tar.xz.asc/from/this/mirror
# Sat, 18 Jan 2020 02:29:34 GMT
ENV PHP_SHA256=561bb866bdd509094be00f4ece7c3543ec971c4d878645ee81437e291cffc762 PHP_MD5=
# Sat, 18 Jan 2020 02:29:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 18 Jan 2020 02:29:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:35:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 18 Jan 2020 02:35:21 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:35:35 GMT
RUN docker-php-ext-enable sodium
# Sat, 18 Jan 2020 02:35:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 18 Jan 2020 02:35:38 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34df684e328567a0a35db6301bcecffeb8c2ab6a69340a96db5d3e73a9fde3da`  
		Last Modified: Sat, 18 Jan 2020 03:18:17 GMT  
		Size: 1.4 MB (1359426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbaaf99effdf014f4ce62ee67d7cf9f23205c645f22d554e6e925ef12ffcd70`  
		Last Modified: Sat, 18 Jan 2020 03:18:17 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99838bf36837f5d2206ac07b2f399dca053921c575c4e9ea8fce917f1672383a`  
		Last Modified: Sat, 18 Jan 2020 03:18:17 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5e42cfbdbf343910de141f9b7c69235cd16a413b76f2f0a0ba726374d66949`  
		Last Modified: Sat, 18 Jan 2020 03:18:16 GMT  
		Size: 10.3 MB (10264387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9857761503690c3280431885b7c9740d21342b55a1fe8c477763a730e23b8f15`  
		Last Modified: Sat, 18 Jan 2020 03:18:15 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269c1fe103f2898bc57979904174326812ec9f159fc861b81742084a34d29ad8`  
		Last Modified: Sat, 18 Jan 2020 03:18:20 GMT  
		Size: 14.4 MB (14362670 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdedbc5f789532e7b2cc6ad2daafc9b3643f5babd446e2578f46a123f710d930`  
		Last Modified: Sat, 18 Jan 2020 03:18:15 GMT  
		Size: 2.2 KB (2211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a13a2daca864aa72e7aa9c0cb15c554a5940fde39f05d0fb30cc7d7df10c28a1`  
		Last Modified: Sat, 18 Jan 2020 03:18:15 GMT  
		Size: 72.7 KB (72674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-alpine3.11` - linux; 386

```console
$ docker pull php@sha256:66d121d7c182bf8f38fd1448f67a7ff29483aeb1ccc637eff9097c2de2d7feb3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31171065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c90ff87670266486dd2a4ad82975edd728618cd0898c35f123cf1a5a1add5b2`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 24 Dec 2019 19:38:57 GMT
ADD file:d0127a9692e8445993a88163cb741dbb23fa25436dd65289e76b08484264b397 in / 
# Tue, 24 Dec 2019 19:38:57 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 22:36:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 26 Dec 2019 22:36:13 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 26 Dec 2019 22:36:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 26 Dec 2019 22:36:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 26 Dec 2019 22:36:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 26 Dec 2019 22:36:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 26 Dec 2019 22:36:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 26 Dec 2019 22:36:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 26 Dec 2019 22:36:17 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 26 Dec 2019 22:36:18 GMT
ENV PHP_VERSION=7.4.1
# Thu, 26 Dec 2019 22:36:18 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.1.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.1.tar.xz.asc/from/this/mirror
# Thu, 26 Dec 2019 22:36:18 GMT
ENV PHP_SHA256=561bb866bdd509094be00f4ece7c3543ec971c4d878645ee81437e291cffc762 PHP_MD5=
# Thu, 26 Dec 2019 22:36:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 26 Dec 2019 22:36:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 26 Dec 2019 22:45:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 26 Dec 2019 22:45:50 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Thu, 26 Dec 2019 22:45:51 GMT
RUN docker-php-ext-enable sodium
# Thu, 26 Dec 2019 22:45:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 26 Dec 2019 22:45:52 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:57bbc6f150623b3e4f01930af4ab2efa6ed5df02319341a08b1ce0bbd7e4afdf`  
		Last Modified: Tue, 24 Dec 2019 19:39:19 GMT  
		Size: 2.8 MB (2805146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db25e971d6f24055202f90f96d257a719817ad73623eaf02d98fb13c2dbe9a1b`  
		Last Modified: Fri, 27 Dec 2019 00:00:12 GMT  
		Size: 1.5 MB (1452611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ecdadbdbb91bc66f820e5b3077004286155b3e618cc444f493d7e73b400333`  
		Last Modified: Fri, 27 Dec 2019 00:00:12 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8331211b40f9489961b63904af5f93f96465efa4f5202ee08600fd1fe3caec6c`  
		Last Modified: Fri, 27 Dec 2019 00:00:11 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1feab22a6dc5f30ac5d6a419e21b0ad02df0633e9376cda5af697a214a1677e`  
		Last Modified: Fri, 27 Dec 2019 00:00:12 GMT  
		Size: 10.3 MB (10264412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f291e0ec174ac10d076b738bdd8d7b5a352fd362d9659a6cb4b7c5cf7e219323`  
		Last Modified: Fri, 27 Dec 2019 00:00:10 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeee04bc33533cf870952c9aab9489299215c7b4a6077fc85ded1a38354bfa34`  
		Last Modified: Fri, 27 Dec 2019 00:00:17 GMT  
		Size: 16.6 MB (16572401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4baee82eaeb4bb25b75b28052d7aec12a58e5f0b9cc3abdccdea6d742bda1e`  
		Last Modified: Fri, 27 Dec 2019 00:00:10 GMT  
		Size: 2.2 KB (2215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f01721c87d29cd0ad25164e2a64d81439e2201e730353ea8a64a5324af5aaaa6`  
		Last Modified: Fri, 27 Dec 2019 00:00:10 GMT  
		Size: 72.3 KB (72336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-alpine3.11` - linux; ppc64le

```console
$ docker pull php@sha256:66a9829bc1cfc3b083a3464971e1c898859eec3e0fff4ba5dfddafe18e387c28
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.6 MB (31629287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e9d00f83fa0d97dcf6ae12bd156621dc8434baa6f588bde628cb01e5f8a98227`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 24 Dec 2019 19:28:37 GMT
ADD file:4d85451a651e236d899cd849617594eb6babf24079f9b2269134ad06d89bdecc in / 
# Tue, 24 Dec 2019 19:28:38 GMT
CMD ["/bin/sh"]
# Thu, 26 Dec 2019 22:21:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 26 Dec 2019 22:21:09 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 26 Dec 2019 22:21:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 26 Dec 2019 22:21:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 26 Dec 2019 22:21:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 26 Dec 2019 22:21:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 26 Dec 2019 22:21:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 26 Dec 2019 22:21:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Thu, 26 Dec 2019 22:21:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 26 Dec 2019 22:21:31 GMT
ENV PHP_VERSION=7.4.1
# Thu, 26 Dec 2019 22:21:32 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.1.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.1.tar.xz.asc/from/this/mirror
# Thu, 26 Dec 2019 22:21:34 GMT
ENV PHP_SHA256=561bb866bdd509094be00f4ece7c3543ec971c4d878645ee81437e291cffc762 PHP_MD5=
# Thu, 26 Dec 2019 22:21:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 26 Dec 2019 22:21:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 26 Dec 2019 22:26:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 26 Dec 2019 22:26:57 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Thu, 26 Dec 2019 22:27:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 26 Dec 2019 22:27:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 26 Dec 2019 22:27:22 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:a5dee701e1e87430161d8fce67e77ee5e132bdbafe165c52490a36df654c7660`  
		Last Modified: Tue, 24 Dec 2019 19:29:09 GMT  
		Size: 2.8 MB (2816482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5787caafdab36524ef14f193793a44b3b5f54da82c98e8152770c2868fd93b11`  
		Last Modified: Thu, 26 Dec 2019 23:13:04 GMT  
		Size: 1.4 MB (1397977 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691639ddfd73c88dfeda1734ababccfaed311f9d747bf07d41c6e7fed2880baf`  
		Last Modified: Thu, 26 Dec 2019 23:13:03 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa2a706347c576336f1e0145755e4fa707710b3f42dc7d18903fcee51bb72842`  
		Last Modified: Thu, 26 Dec 2019 23:13:02 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c9367473ae473e3b4307b84581a68ce338708fd02c58387ea03ebbf3b336c4`  
		Last Modified: Thu, 26 Dec 2019 23:13:00 GMT  
		Size: 10.3 MB (10264430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bce400ab5b594b3c37b04d8ff93ef76324ad103b89b864086646553aa374ae3a`  
		Last Modified: Thu, 26 Dec 2019 23:12:59 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df72cd13deac5a2de7a62833b97945cc48eb13a954c074f0c2ef27d321ad172`  
		Last Modified: Thu, 26 Dec 2019 23:13:09 GMT  
		Size: 17.1 MB (17073151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a993ff611f4ce5c9ad8c688b7d218dfaf24788380583d0b8ff19758b953565b`  
		Last Modified: Thu, 26 Dec 2019 23:12:59 GMT  
		Size: 2.2 KB (2216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6b2a23101f41428ee2ad1948c90b3eaf9cda596853a790ebdb59a2e5f3a4353`  
		Last Modified: Thu, 26 Dec 2019 23:12:59 GMT  
		Size: 73.0 KB (73011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
