## `php:8-cli-alpine`

```console
$ docker pull php@sha256:b2d756925367bd8a5d6e0edc243134ed474844b6226379897fa70fea16b74133
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

### `php:8-cli-alpine` - linux; amd64

```console
$ docker pull php@sha256:39cb3ae8490239966326be40ca3f426c5d6eef2225c15250ab314b309175c2bf
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.4 MB (30426610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbd87967d02bf62e7d31dc3c4008144b1b4a8bfcb7089626f640fe0cc61c6873`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:48:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 07:48:45 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 07:48:47 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 07:48:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 07:48:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 07:48:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 07:48:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 07:48:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 08:32:27 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 19 Nov 2021 22:21:33 GMT
ENV PHP_VERSION=8.0.13
# Fri, 19 Nov 2021 22:21:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.13.tar.xz.asc
# Fri, 19 Nov 2021 22:21:33 GMT
ENV PHP_SHA256=cd976805ec2e9198417651027dfe16854ba2c2c388151ab9d4d268513d52ed52
# Fri, 19 Nov 2021 22:21:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 19 Nov 2021 22:21:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 19 Nov 2021 22:31:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 19 Nov 2021 22:31:06 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 19 Nov 2021 22:31:08 GMT
RUN docker-php-ext-enable sodium
# Fri, 19 Nov 2021 22:31:08 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 19 Nov 2021 22:31:08 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67f99012ff9aa7245baebc28963e44f53cc1832fcfaec246f78b5e7e861fbe6`  
		Last Modified: Sat, 13 Nov 2021 10:43:29 GMT  
		Size: 1.7 MB (1712224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db81da314e0b3e7be6d4c80bd6a2cdc1d7f66d6fffc8334a527f6b6e20fca340`  
		Last Modified: Sat, 13 Nov 2021 10:43:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5646ac679ebe77089fb6446f9911a66ae64db7d5b774d356b04c1c911ca0a081`  
		Last Modified: Sat, 13 Nov 2021 10:43:29 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b270ced5f88e06e3e565fd261ac8c3f51d68aa189019e89adcded81e6a53933`  
		Last Modified: Fri, 19 Nov 2021 23:12:55 GMT  
		Size: 10.9 MB (10874426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53da6390bea4346b325a012b56da6db4cda9e195ba573c1d39bf7a598e538d1c`  
		Last Modified: Fri, 19 Nov 2021 23:12:52 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af80a1407c3fe3f4f81811c5669faa8b11e0462bfdcddd5067bd0089bc3858e8`  
		Last Modified: Fri, 19 Nov 2021 23:12:56 GMT  
		Size: 15.0 MB (14994457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35f41405294baf6aa345cb3ca3f70f464edecf39bf342397aee5e309f2972587`  
		Last Modified: Fri, 19 Nov 2021 23:12:52 GMT  
		Size: 2.3 KB (2302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d675ff9726ea7b911aa14e65be26df717fd62fa11636b84b876c67980add97c`  
		Last Modified: Fri, 19 Nov 2021 23:12:52 GMT  
		Size: 18.2 KB (18196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-cli-alpine` - linux; arm variant v6

```console
$ docker pull php@sha256:7bab7cbc380d12de2e0cebfe8e2d7cf4c178c44f2c247dd060ae9e4d02ba188a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28871842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7101661b1f5e791ad3d3fcb828ae58fcf1b36da8a359eb2b4cd53bb0c54b24a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 01:00:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 01:00:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 01:00:57 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 01:00:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 01:00:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 01:01:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 01:01:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 01:01:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 01:21:11 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 19 Nov 2021 20:50:54 GMT
ENV PHP_VERSION=8.0.13
# Fri, 19 Nov 2021 20:50:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.13.tar.xz.asc
# Fri, 19 Nov 2021 20:50:55 GMT
ENV PHP_SHA256=cd976805ec2e9198417651027dfe16854ba2c2c388151ab9d4d268513d52ed52
# Fri, 19 Nov 2021 20:51:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 19 Nov 2021 20:51:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 19 Nov 2021 20:55:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 19 Nov 2021 20:55:58 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 19 Nov 2021 20:56:00 GMT
RUN docker-php-ext-enable sodium
# Fri, 19 Nov 2021 20:56:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 19 Nov 2021 20:56:01 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fb65eff99d3570be8bbee58e3796b49e0e6fbc64d6c2b55e01eaf1b07709af`  
		Last Modified: Sat, 13 Nov 2021 02:49:22 GMT  
		Size: 1.7 MB (1702248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe18ffa25cea29b8a20ba6c41b7485fd89e792d6d333919ea738dcff33555f`  
		Last Modified: Sat, 13 Nov 2021 02:49:21 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215c6f1ae3409a42a8b2531ec3f19b4dddc77724624fdc7fe72175b53fa03ad0`  
		Last Modified: Sat, 13 Nov 2021 02:49:21 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc1707b16dd4de1a68e7bfd4f5f2159f8c845b0188a346399f3de67509c9c6b`  
		Last Modified: Fri, 19 Nov 2021 21:22:39 GMT  
		Size: 10.9 MB (10874434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d1beade5491239ceb273a717cd3aa5cc502e753a6a406212cc6571bcac5271e`  
		Last Modified: Fri, 19 Nov 2021 21:22:36 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee9ccb93e4c984a3a6d81a5de5abe1601e1433ca9fe7979cf52bbedec016e9`  
		Last Modified: Fri, 19 Nov 2021 21:22:46 GMT  
		Size: 13.6 MB (13637238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00c115009c6662e9af1da77099122aa021746df99a9e5fd181c28ef1e5e231b6`  
		Last Modified: Fri, 19 Nov 2021 21:22:36 GMT  
		Size: 2.3 KB (2302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a699f41c1267f3c02741d3f56ee3abe91d0083b4b3ec1937db95b4e55506471f`  
		Last Modified: Fri, 19 Nov 2021 21:22:36 GMT  
		Size: 18.2 KB (18205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-cli-alpine` - linux; arm variant v7

```console
$ docker pull php@sha256:40b7eaf172f5eedb6469f5378fda7a5029b13c6126754736cccd14db9b2ad4cc
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.7 MB (27688093 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00052d92a4bb4dd650207894cfab317aabda9498d37fb18ecd739716c09e9420`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 02:20:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 02:20:29 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 02:20:30 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 02:20:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 02:20:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 02:20:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 02:20:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 02:20:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 02:42:32 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 19 Nov 2021 21:45:48 GMT
ENV PHP_VERSION=8.0.13
# Fri, 19 Nov 2021 21:45:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.13.tar.xz.asc
# Fri, 19 Nov 2021 21:45:49 GMT
ENV PHP_SHA256=cd976805ec2e9198417651027dfe16854ba2c2c388151ab9d4d268513d52ed52
# Fri, 19 Nov 2021 21:45:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 19 Nov 2021 21:45:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 19 Nov 2021 21:50:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 19 Nov 2021 21:50:06 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 19 Nov 2021 21:50:09 GMT
RUN docker-php-ext-enable sodium
# Fri, 19 Nov 2021 21:50:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 19 Nov 2021 21:50:10 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d591a38553bed13e4644c2ee36cc92a36f4f866265bcec258baef16176c11b`  
		Last Modified: Sat, 13 Nov 2021 04:21:17 GMT  
		Size: 1.6 MB (1571523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a132a38f5266edd87272c20d2129b4448b3dfb530a70424219ddd45fd1d2eb73`  
		Last Modified: Sat, 13 Nov 2021 04:21:16 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a99b8f25382a7fadffc08ae9ebf09b2a2be48a858daf03148035e46335c089a`  
		Last Modified: Sat, 13 Nov 2021 04:21:16 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fecad34cb37f0d9ce4c9e0326c587fd5b6952efc3f61951a67adaa9b199224f2`  
		Last Modified: Fri, 19 Nov 2021 22:36:31 GMT  
		Size: 10.9 MB (10874417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d74b53286e3e8f0333fc76fe414b995a4f1b9ead316ba3221614439faf82b4a`  
		Last Modified: Fri, 19 Nov 2021 22:36:28 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1be57144c925a11b5c99027824815a5593f89fd7d4e497351d022c01f10dba65`  
		Last Modified: Fri, 19 Nov 2021 22:36:37 GMT  
		Size: 12.8 MB (12781010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53eed337540d625c6d79bce484517d7188d0c0321a1dbc63e73bd6180e27b30a`  
		Last Modified: Fri, 19 Nov 2021 22:36:28 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f985ecd361fcf02ebbc80b951427100a280f14b6f747bc54b83c0ba8de8eb29`  
		Last Modified: Fri, 19 Nov 2021 22:36:28 GMT  
		Size: 18.2 KB (18196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-cli-alpine` - linux; arm64 variant v8

```console
$ docker pull php@sha256:b18ecee25ba51729de2f40e9ce450c0746b84dd20c642d650f01a4277058ebc3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.8 MB (29754156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9c7e1e928f539a92e9564a49e10b769763f66fb8fd57376cfb1bac625319d28`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:30:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 12 Nov 2021 19:30:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 12 Nov 2021 19:30:35 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 12 Nov 2021 19:30:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Nov 2021 19:30:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Nov 2021 19:30:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:30:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:30:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Nov 2021 20:02:23 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 19 Nov 2021 22:12:03 GMT
ENV PHP_VERSION=8.0.13
# Fri, 19 Nov 2021 22:12:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.13.tar.xz.asc
# Fri, 19 Nov 2021 22:12:05 GMT
ENV PHP_SHA256=cd976805ec2e9198417651027dfe16854ba2c2c388151ab9d4d268513d52ed52
# Fri, 19 Nov 2021 22:12:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 19 Nov 2021 22:12:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 19 Nov 2021 22:16:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 19 Nov 2021 22:16:48 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 19 Nov 2021 22:16:49 GMT
RUN docker-php-ext-enable sodium
# Fri, 19 Nov 2021 22:16:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 19 Nov 2021 22:16:51 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9716534ffbe55fb7b1cdc9c51401565113fe78d473379c595bf42e6d05fd5e6e`  
		Last Modified: Fri, 12 Nov 2021 21:25:50 GMT  
		Size: 1.7 MB (1711801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d47cbc9449ef4aab290c562e2d538c1152c89268a02bb026807264d1c3d6da`  
		Last Modified: Fri, 12 Nov 2021 21:25:49 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a654447725655854a94c8af1e17c61ba95c1eb179a627aa323bfd70bfbae408`  
		Last Modified: Fri, 12 Nov 2021 21:25:50 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:985b099de5b0991722ec2230a0fc92a6c7a0e309c24aa898752011b813aced32`  
		Last Modified: Fri, 19 Nov 2021 22:46:00 GMT  
		Size: 10.9 MB (10874198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f249285c5a1fd69a9d2a9c8b889a4abc4ca5e3209510661868c46b55a1b70a`  
		Last Modified: Fri, 19 Nov 2021 22:45:58 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1df7dd0438c398faf47d740777722e3403aab89f1e22cf63a9772473775f57b`  
		Last Modified: Fri, 19 Nov 2021 22:46:01 GMT  
		Size: 14.4 MB (14428087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c988abf682d7fdb919e46673194830178f4a53e13cdc14824973356cb9c919d1`  
		Last Modified: Fri, 19 Nov 2021 22:45:59 GMT  
		Size: 2.3 KB (2299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e64b7d3148de62ed89fbd68cd4a52147a3b988841838039c9433977e665ea7f`  
		Last Modified: Fri, 19 Nov 2021 22:45:58 GMT  
		Size: 18.1 KB (18121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-cli-alpine` - linux; 386

```console
$ docker pull php@sha256:6368c32f91e21c242f9525911080176ebfc187419b59d74516e90faed8622481
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30862271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d6141292cf240edcd49c9017fc0dbac5b944e5337f847af538797152114a141`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 00:47:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 00:47:24 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 00:47:26 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 00:47:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 00:47:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 00:47:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 00:47:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 00:47:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 01:29:07 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 19 Nov 2021 22:54:05 GMT
ENV PHP_VERSION=8.0.13
# Fri, 19 Nov 2021 22:54:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.13.tar.xz.asc
# Fri, 19 Nov 2021 22:54:06 GMT
ENV PHP_SHA256=cd976805ec2e9198417651027dfe16854ba2c2c388151ab9d4d268513d52ed52
# Fri, 19 Nov 2021 22:54:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 19 Nov 2021 22:54:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 19 Nov 2021 23:03:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 19 Nov 2021 23:03:41 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 19 Nov 2021 23:03:42 GMT
RUN docker-php-ext-enable sodium
# Fri, 19 Nov 2021 23:03:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 19 Nov 2021 23:03:43 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c05111b719bf0e9c81182879ace55b68244fff3ccaacc6813f9ce740b1adf4d`  
		Last Modified: Sat, 13 Nov 2021 04:00:31 GMT  
		Size: 1.8 MB (1812696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f12e62d2679739a2acadab070b1c7d0f433a8a46d449147d00fa5c4aa0a8753`  
		Last Modified: Sat, 13 Nov 2021 04:00:30 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3e1535943b040497915113f37b46a4ba0dc10f27aabcdb6dbf9d0b594ca8be`  
		Last Modified: Sat, 13 Nov 2021 04:00:30 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9286dcecc672d991827dada60a5e14a9e24ba476fee604b196cd2966b0a75c50`  
		Last Modified: Fri, 19 Nov 2021 23:44:16 GMT  
		Size: 10.9 MB (10874411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b81d38852aae66728f75f5b64f2ec5e75a565bd8947a1c231fa5e518e171d4ba`  
		Last Modified: Fri, 19 Nov 2021 23:44:14 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c8f1095ab6c6472889a7300702ab935b56832dfe21c32b134ad2f28eedd971`  
		Last Modified: Fri, 19 Nov 2021 23:44:19 GMT  
		Size: 15.3 MB (15321706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a6b4ddefea2c35d0be646d7b059cb67400729e16307e5b895756b252a17596`  
		Last Modified: Fri, 19 Nov 2021 23:44:14 GMT  
		Size: 2.3 KB (2296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a902e56a7ed531664e8a1f020ebd4bf5b4aa046f7536b545038f54c0f2436323`  
		Last Modified: Fri, 19 Nov 2021 23:44:15 GMT  
		Size: 18.2 KB (18190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-cli-alpine` - linux; ppc64le

```console
$ docker pull php@sha256:1cce9921e4459ae0c9a0639e603ff15b5ad0d259b630860fbd175da15c04f8ff
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31201810 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:352aa8aab006e8339f5dad9761c3cadbd31b57c04e53a2d9f07725e7ddee5db8`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:56:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 11:56:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 11:56:13 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 11:56:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 11:56:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 11:56:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 11:56:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 11:56:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 12:24:47 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 19 Nov 2021 22:08:34 GMT
ENV PHP_VERSION=8.0.13
# Fri, 19 Nov 2021 22:08:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.13.tar.xz.asc
# Fri, 19 Nov 2021 22:08:37 GMT
ENV PHP_SHA256=cd976805ec2e9198417651027dfe16854ba2c2c388151ab9d4d268513d52ed52
# Fri, 19 Nov 2021 22:08:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 19 Nov 2021 22:08:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 19 Nov 2021 22:14:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 19 Nov 2021 22:14:19 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 19 Nov 2021 22:14:27 GMT
RUN docker-php-ext-enable sodium
# Fri, 19 Nov 2021 22:14:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 19 Nov 2021 22:14:35 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf526002982778a0157923a6219fbadd645d22999e9251af0db89be07d002272`  
		Last Modified: Sat, 13 Nov 2021 14:08:23 GMT  
		Size: 1.8 MB (1759206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b47bb623f5bce1748b7a2c4e16b2726478248c03150000de676a1020aaeada`  
		Last Modified: Sat, 13 Nov 2021 14:08:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f035bbd1b7db7792a68686cccf93b48bd273f6f89375962d7fae46bab690f7ac`  
		Last Modified: Sat, 13 Nov 2021 14:08:23 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf09458e189ad07da9c76a19edc1b703076aec618cc0a40d567a0fe920b4c2df`  
		Last Modified: Fri, 19 Nov 2021 22:49:17 GMT  
		Size: 10.9 MB (10874418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2fb7bbc1d5b1d9bcf5c850c66985ad9413f3281584de85a9a5c0b64cb3a8b40`  
		Last Modified: Fri, 19 Nov 2021 22:49:16 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ff7a9aac2e4766eb31b1ff1d68e75008c10a0496973ca462556ec2081b5c7e`  
		Last Modified: Fri, 19 Nov 2021 22:49:20 GMT  
		Size: 15.7 MB (15728197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cd4511e9631ee0951d4a804439a213f9f15fa38d7e4411f1fd5f2542c3e67ea`  
		Last Modified: Fri, 19 Nov 2021 22:49:16 GMT  
		Size: 2.3 KB (2300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1871fbb270b9920038b0d2496579fec491fd49e34e93244f6269a95eb0b9d157`  
		Last Modified: Fri, 19 Nov 2021 22:49:16 GMT  
		Size: 18.2 KB (18196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-cli-alpine` - linux; s390x

```console
$ docker pull php@sha256:258803bd79d3a2bfbbec2f7e27a908062694def05d71b675e566e678fee63818
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.3 MB (29307786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41af723822cc4947353c1fdb6fa225e55a4e32fe19e23f18d4a88d24409bb873`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:35 GMT
ADD file:7e0cf02b3f015b1a0f867c03b2902b85f2140be1cee7af63c23f367a487e4577 in / 
# Fri, 12 Nov 2021 16:41:36 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:58:14 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 12 Nov 2021 19:58:15 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 12 Nov 2021 19:58:15 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 12 Nov 2021 19:58:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Nov 2021 19:58:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Nov 2021 19:58:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:58:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:58:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Nov 2021 20:11:25 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 19 Nov 2021 22:04:21 GMT
ENV PHP_VERSION=8.0.13
# Fri, 19 Nov 2021 22:04:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.13.tar.xz.asc
# Fri, 19 Nov 2021 22:04:21 GMT
ENV PHP_SHA256=cd976805ec2e9198417651027dfe16854ba2c2c388151ab9d4d268513d52ed52
# Fri, 19 Nov 2021 22:04:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 19 Nov 2021 22:04:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 19 Nov 2021 22:07:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 19 Nov 2021 22:07:15 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 19 Nov 2021 22:07:16 GMT
RUN docker-php-ext-enable sodium
# Fri, 19 Nov 2021 22:07:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 19 Nov 2021 22:07:16 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:817a13b0e05928f7491adbf1d2cf261ec35079112247bd03469bbe31156aca7c`  
		Last Modified: Fri, 12 Nov 2021 16:42:44 GMT  
		Size: 2.6 MB (2609278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c6db577f243875f52f246d8a7fdab675a850569d52d6bba314f58258225c1f`  
		Last Modified: Fri, 12 Nov 2021 21:10:48 GMT  
		Size: 1.8 MB (1774038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a472bfa2a1552842a7406f914151af808b4f2a9e245ddbfe7cbc332697f96b12`  
		Last Modified: Fri, 12 Nov 2021 21:10:47 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd3cea1835285017465c0df7a510c36971229f7066ec32d2ac436c4f9ac6ebd3`  
		Last Modified: Fri, 12 Nov 2021 21:10:48 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d565847491d8ba8774b757c3986240adc0c02cc0ebaa2cf3f35d8e5a7b6250`  
		Last Modified: Fri, 19 Nov 2021 22:31:43 GMT  
		Size: 10.9 MB (10874420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc82c537d5b0d6ff89cba901f006fce2ae757bc01d23d1d8b76be4ed5093d2a9`  
		Last Modified: Fri, 19 Nov 2021 22:31:43 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5fee1c8856ea40b6f3d64df4d1a6a9e10bd4f9159209ddc2526b6474923f93b`  
		Last Modified: Fri, 19 Nov 2021 22:31:45 GMT  
		Size: 14.0 MB (14027513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06f3a04be76cf14dfc61e69d072d87f6a739a4132d899250b6903afc92ce2191`  
		Last Modified: Fri, 19 Nov 2021 22:31:43 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e6051ed2167f4a30233213efbbf322435435c98afc85c327ab971d26832dafc`  
		Last Modified: Fri, 19 Nov 2021 22:31:43 GMT  
		Size: 18.2 KB (18211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
