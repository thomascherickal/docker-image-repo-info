## `php:8-cli-alpine3.17`

```console
$ docker pull php@sha256:a4148ca7a6199eaad67484122148597c6721d0974a3dc41d574afd9e6eb9ee54
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

### `php:8-cli-alpine3.17` - linux; amd64

```console
$ docker pull php@sha256:45cf2e0149e14957b614321f1c9c50a90986f3dc523f3a9a83a2bf9a904a0dd9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34358816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b674211ab0cc78f1a829af38354c5cc9d4a80c31e56293d19448b29844ffb524`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 10:17:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 10:17:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 10:17:24 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 10:17:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 11 Feb 2023 10:17:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 11 Feb 2023 10:17:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 10:17:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 10:17:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 11 Feb 2023 10:17:25 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 16 Mar 2023 21:46:18 GMT
ENV PHP_VERSION=8.2.4
# Thu, 16 Mar 2023 21:46:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Thu, 16 Mar 2023 21:46:18 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Thu, 16 Mar 2023 21:46:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Mar 2023 21:46:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Mar 2023 21:50:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Mar 2023 21:50:00 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 16 Mar 2023 21:50:01 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Mar 2023 21:50:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Mar 2023 21:50:01 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80fdb865a69a85ee910e603ec69d253469dd9367105df81057c89ef565ab971`  
		Last Modified: Sat, 11 Feb 2023 11:20:06 GMT  
		Size: 1.9 MB (1869555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4dbeadc75c19cda75784e259745d42dd938cf860218f8fec2103bf0852be3c7`  
		Last Modified: Sat, 11 Feb 2023 11:20:06 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257b31b3391b9ce8882eab2c50f2cb64279987f785eeba45218d0b14aa3d74cb`  
		Last Modified: Sat, 11 Feb 2023 11:20:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b819c7c781e43403811c73f00c7d3fbcc9e8476dc7da90a4f8539522c02f94`  
		Last Modified: Thu, 16 Mar 2023 23:07:41 GMT  
		Size: 12.0 MB (12012472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da2f9afa1ef0a2f2910745b04b4659c7f2926f6b9d66111cd9a983483d167ec`  
		Last Modified: Thu, 16 Mar 2023 23:07:40 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac800a07cfde1a58321169064cba466148efbc6cb0c3564221db63b9b1a0a864`  
		Last Modified: Thu, 16 Mar 2023 23:07:43 GMT  
		Size: 17.1 MB (17078869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb98ea6960fc8dd5f4dac680951e172a63c78ab2035725aa2db5279b4335571`  
		Last Modified: Thu, 16 Mar 2023 23:07:40 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2de4d1cc9a594316e50639665ba018f201b4eff00cd9ce8e30fe33d9ec624c0`  
		Last Modified: Thu, 16 Mar 2023 23:07:40 GMT  
		Size: 19.0 KB (18997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-cli-alpine3.17` - linux; arm variant v6

```console
$ docker pull php@sha256:3d702980f137b95a189331a90e3d15dd01cc0880c96fdbadef62161b7637411e
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32323034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b5fd04e121dde9199ee402cc7d77d15d1c85a8a28cf1c7edbf16f29f2cf4085`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 21:07:07 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 13 Mar 2023 21:07:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 13 Mar 2023 21:07:09 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 13 Mar 2023 21:07:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 13 Mar 2023 21:07:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 13 Mar 2023 21:07:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 13 Mar 2023 21:07:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 13 Mar 2023 21:07:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 13 Mar 2023 21:07:10 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 16 Mar 2023 21:40:31 GMT
ENV PHP_VERSION=8.2.4
# Thu, 16 Mar 2023 21:40:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Thu, 16 Mar 2023 21:40:32 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Thu, 16 Mar 2023 21:40:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Mar 2023 21:40:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Mar 2023 21:43:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Mar 2023 21:43:38 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 16 Mar 2023 21:43:39 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Mar 2023 21:43:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Mar 2023 21:43:39 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b525ba211658332771b8d1e1e6274a63819ca62cce4ae60af48bd6ea6de2e81e`  
		Last Modified: Mon, 13 Mar 2023 22:29:45 GMT  
		Size: 1.9 MB (1865508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da8f3139761283dde8c51dccb6f9887eedcebb955cb74f916390ef170c7f432c`  
		Last Modified: Mon, 13 Mar 2023 22:29:45 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d473bc0ad5e16dc9e7a8b062b4d46e1bc4c325a792b684246fdf4710b85a59`  
		Last Modified: Mon, 13 Mar 2023 22:29:45 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8835cc1969b1afc8d85c69c79cc58c60641558c8a14d7a08f24a6f84be987f`  
		Last Modified: Thu, 16 Mar 2023 22:19:01 GMT  
		Size: 12.0 MB (12012453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d547bb7c96df742a5ffdca56ffd0542397848b4516fa46434d3299b2480a482`  
		Last Modified: Thu, 16 Mar 2023 22:18:59 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7080ec385d9906c0f8d3d6cae5c5a4f91f0ac591e35e3dff58e2214df16c814c`  
		Last Modified: Thu, 16 Mar 2023 22:19:03 GMT  
		Size: 15.3 MB (15310983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2dad1ec9c6551ec4da9b19c5f1330ca1161279df5eae79a65bf9c447a9f333`  
		Last Modified: Thu, 16 Mar 2023 22:18:59 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7069152e8ad1b1972adbb5f367e899e141f7965df86ee19165fc0b063a69390`  
		Last Modified: Thu, 16 Mar 2023 22:18:59 GMT  
		Size: 18.7 KB (18730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-cli-alpine3.17` - linux; arm variant v7

```console
$ docker pull php@sha256:4011407fa0c539a9c519193bac79eb9854cd9af068393f4071c0c4b3731144a0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (30966689 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5fc03c690efbe13a84103253e24ea58c5a4a265184fcf1e201b7ef77e5b538a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 21:36:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 01 Mar 2023 21:36:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 01 Mar 2023 21:36:52 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Mar 2023 21:36:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Mar 2023 21:36:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Mar 2023 21:36:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 21:36:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 21:36:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Mar 2023 21:36:53 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 16 Mar 2023 23:08:25 GMT
ENV PHP_VERSION=8.2.4
# Thu, 16 Mar 2023 23:08:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Thu, 16 Mar 2023 23:08:26 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Thu, 16 Mar 2023 23:08:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Mar 2023 23:08:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Mar 2023 23:11:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Mar 2023 23:11:20 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 16 Mar 2023 23:11:21 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Mar 2023 23:11:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Mar 2023 23:11:21 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9169ee53f4934f506408e6416f765930339b501b32c7cc932909cc1f0c22190`  
		Last Modified: Wed, 01 Mar 2023 23:08:09 GMT  
		Size: 1.7 MB (1715927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c652394f365d675be459982d3ff25a0cd449736b35738b11ada9fbcd26323603`  
		Last Modified: Wed, 01 Mar 2023 23:08:08 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8004a620a679d75c3c87ee59d53822c6d18bd9cb75d9bb8e515e1aa829e823e`  
		Last Modified: Wed, 01 Mar 2023 23:08:09 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585318d04b0768eac27489a51e819a57e9d298b39b385773e8bfc52e60e29466`  
		Last Modified: Fri, 17 Mar 2023 00:13:10 GMT  
		Size: 12.0 MB (12012451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7dbaa575aac70098c5c2a23aec2646c1d0261a80b073a421b1d86a316e060eb`  
		Last Modified: Fri, 17 Mar 2023 00:13:09 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027bd3231bfc57567aa59894a815b74c720c802320f4f7221a62a954e917a338`  
		Last Modified: Fri, 17 Mar 2023 00:13:12 GMT  
		Size: 14.3 MB (14346599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146216f2f904d6aa9bb82e1c8ddba3ed4add7c18a48daf516f6df9c4ca3256f7`  
		Last Modified: Fri, 17 Mar 2023 00:13:09 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990d9d5da49e8ff94014b342b4c02f145d0a8959b14ef283ee1799efa85848ba`  
		Last Modified: Fri, 17 Mar 2023 00:13:09 GMT  
		Size: 18.7 KB (18742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-cli-alpine3.17` - linux; arm64 variant v8

```console
$ docker pull php@sha256:89224668a5a1fd2bc4cd5b0a4a5406d099e022a7033cfbc611aef7af6653c5c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34143590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34e447fd73d72c4bd80510b459a3961a4adac095f11a6ec9d78db3ce7594fa8e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 02:02:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 02:02:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 02:02:56 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 02:02:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 11 Feb 2023 02:02:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 11 Feb 2023 02:02:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 02:02:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 02:02:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 11 Feb 2023 02:02:57 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 16 Mar 2023 21:58:35 GMT
ENV PHP_VERSION=8.2.4
# Thu, 16 Mar 2023 21:58:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Thu, 16 Mar 2023 21:58:35 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Thu, 16 Mar 2023 21:58:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Mar 2023 21:58:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Mar 2023 22:02:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Mar 2023 22:02:16 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 16 Mar 2023 22:02:17 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Mar 2023 22:02:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Mar 2023 22:02:18 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65da1d1bbae15a06f79c4d79d885439cb51d02c27c69741770a1ace04a962454`  
		Last Modified: Sat, 11 Feb 2023 03:02:23 GMT  
		Size: 1.9 MB (1862646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53689469854ea07050d653c2567c0a362a36bf42c1db6ad7ca78f0ce04d4a862`  
		Last Modified: Sat, 11 Feb 2023 03:02:22 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c363c99e0af7af0ce7cc0c3b401461324b37d279159235d225fb19c056c4c1`  
		Last Modified: Sat, 11 Feb 2023 03:02:22 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0288061eba67898564b8e4024dac619fc8bcf935df961b67ce7d23add82110ff`  
		Last Modified: Thu, 16 Mar 2023 23:17:41 GMT  
		Size: 12.0 MB (12012452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18ad46cc84736bba0e2e38b27cbefd11136f5338d49c741e3c3789c1a5c527d`  
		Last Modified: Thu, 16 Mar 2023 23:17:40 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d392b8f42f31fd16073cf82da18cae7cdc2691a9fc229c22fec670a3beba247b`  
		Last Modified: Thu, 16 Mar 2023 23:17:42 GMT  
		Size: 17.0 MB (16983274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:857b532d1f657eea334a4317d80cd0ed696ff6de19333e3fb84ccf4c32925468`  
		Last Modified: Thu, 16 Mar 2023 23:17:40 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53763a5bf727cee337102ea5b39d35bd95fcf9e3624f05ee59b657d1d33c68e`  
		Last Modified: Thu, 16 Mar 2023 23:17:40 GMT  
		Size: 18.8 KB (18783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-cli-alpine3.17` - linux; 386

```console
$ docker pull php@sha256:70dad1cb3e56cb783aacbfa797177710abf3d2a19622baf86d0b8e0e8872daab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34626273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c803be2d13fad71b85573c5c4dc1966dd1e858ca0434a8d1e142fdcc8b79db23`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 15:08:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 01 Mar 2023 15:08:13 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 01 Mar 2023 15:08:14 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Mar 2023 15:08:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Mar 2023 15:08:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Mar 2023 15:08:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 15:08:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 15:08:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Mar 2023 15:08:15 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 16 Mar 2023 22:24:06 GMT
ENV PHP_VERSION=8.2.4
# Thu, 16 Mar 2023 22:24:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Thu, 16 Mar 2023 22:24:06 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Thu, 16 Mar 2023 22:24:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Mar 2023 22:24:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Mar 2023 22:30:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Mar 2023 22:30:24 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 16 Mar 2023 22:30:25 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Mar 2023 22:30:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Mar 2023 22:30:25 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5394292b2b83b2b876e0f3301349b0299305f8034ed3fa062d20c20268efbd52`  
		Last Modified: Wed, 01 Mar 2023 18:23:52 GMT  
		Size: 2.0 MB (1991827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e923c580cf6f27c534dc0869dfae4f7e9e424c149940e20be2ffef7aa344c424`  
		Last Modified: Wed, 01 Mar 2023 18:23:51 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c6096004f76a359d1c0d104682a61452036bae13908723157c118939b617b6`  
		Last Modified: Wed, 01 Mar 2023 18:23:51 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ded1c7a129a9af2111df13579707410ee5c3cb762262264c4d63522545fc981d`  
		Last Modified: Fri, 17 Mar 2023 00:41:25 GMT  
		Size: 12.0 MB (12012460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6282b32a6a31cc75e05f9314b6ad115b6f7674b6784c17fe6cc73eef79626072`  
		Last Modified: Fri, 17 Mar 2023 00:41:24 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98701c0d5f607ef64daeeefb812134655fcf2e3ed07e2ade95ea06f68b23514d`  
		Last Modified: Fri, 17 Mar 2023 00:41:28 GMT  
		Size: 17.2 MB (17186226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc98bd698fa280c5b05f7237d440476ba44bea9fbc690bc8e692d0657a670432`  
		Last Modified: Fri, 17 Mar 2023 00:41:24 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85c5df9e8d6d9a1af385107a5b93a88af8c8412913a928448308dd3366ff1a72`  
		Last Modified: Fri, 17 Mar 2023 00:41:24 GMT  
		Size: 18.9 KB (18935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-cli-alpine3.17` - linux; ppc64le

```console
$ docker pull php@sha256:7128f62fd8f78f30febe24b94bf3f4afb9cc6f71834fe4bc33c3ffa684ef542c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35245290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd0839ad64b235e161c185a15495ec7c1fbac2b4b08774b5c8d84877c7f3463e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 23:08:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 10 Feb 2023 23:08:28 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 10 Feb 2023 23:08:29 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 10 Feb 2023 23:08:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 10 Feb 2023 23:08:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 10 Feb 2023 23:08:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 10 Feb 2023 23:08:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 10 Feb 2023 23:08:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 10 Feb 2023 23:08:33 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 16 Mar 2023 21:19:04 GMT
ENV PHP_VERSION=8.2.4
# Thu, 16 Mar 2023 21:19:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Thu, 16 Mar 2023 21:19:06 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Thu, 16 Mar 2023 21:19:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Mar 2023 21:19:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Mar 2023 21:23:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Mar 2023 21:23:49 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 16 Mar 2023 21:23:51 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Mar 2023 21:23:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Mar 2023 21:23:55 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bfa1898e4103c3c306fd301195ab70581ac39be1be2ad84260c45520aaa5d05`  
		Last Modified: Sat, 11 Feb 2023 00:28:07 GMT  
		Size: 1.9 MB (1946683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fded8faaf0ac23f23c9b92d38d3e833d89b91908a65685dd807fc5ed5718e57`  
		Last Modified: Sat, 11 Feb 2023 00:28:07 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8afe3cb27338f4dc17809e93d8c3ba65ea9bbe27288f937f4e25fb03bc6010`  
		Last Modified: Sat, 11 Feb 2023 00:28:06 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d18933fe75c9cadca119aae89252044f675c22a371fc0c92825cf994ae8e68`  
		Last Modified: Thu, 16 Mar 2023 22:50:34 GMT  
		Size: 12.0 MB (12012456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:699ea80da01efb93c4e706235cd8ee37689177fd52ace25720c00a550f8e5607`  
		Last Modified: Thu, 16 Mar 2023 22:50:33 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5424f0499a7e1f9441006a719599606e343d70f763003d6180cda02d4ed76a12`  
		Last Modified: Thu, 16 Mar 2023 22:50:38 GMT  
		Size: 17.9 MB (17872142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dc84856a4793aef0f605e1afe85b1c0b55d258a4d04842a007a7d501e36a0fb`  
		Last Modified: Thu, 16 Mar 2023 22:50:33 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b9c05b3617a96d2a20ce72936b85ee8936572b762410fcaa25b6fc613ddbcd`  
		Last Modified: Thu, 16 Mar 2023 22:50:33 GMT  
		Size: 18.8 KB (18786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:8-cli-alpine3.17` - linux; s390x

```console
$ docker pull php@sha256:f0b10fe1d757a1e66e777f7651fd088728cb51e7904587fb355af3ad6783d834
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33078033 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1ea280311a22392f7523a4e58ee45e688b2d8639028bff2f72491b49fd92328d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:40:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 03:40:21 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 03:40:22 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 03:40:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 11 Feb 2023 03:40:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 11 Feb 2023 03:40:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 03:40:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 03:40:23 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 11 Feb 2023 03:40:23 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 16 Mar 2023 23:20:53 GMT
ENV PHP_VERSION=8.2.4
# Thu, 16 Mar 2023 23:20:53 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Thu, 16 Mar 2023 23:20:53 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Thu, 16 Mar 2023 23:20:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 16 Mar 2023 23:20:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Mar 2023 23:23:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Mar 2023 23:23:42 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 16 Mar 2023 23:23:43 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Mar 2023 23:23:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Mar 2023 23:23:43 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3e08f96f9a305daacf9ee42f9847666c785231f5db9684aae1648426463f923`  
		Last Modified: Sat, 11 Feb 2023 04:35:13 GMT  
		Size: 1.9 MB (1917113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2b2b7eda29298bc923307ecd06eca2607d89341d31329cad08c2ddd6d3dda03`  
		Last Modified: Sat, 11 Feb 2023 04:35:13 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87dc1497b9a6351ab931f19c686d45bea176daa8f6da7db62dce416a091a4944`  
		Last Modified: Sat, 11 Feb 2023 04:35:14 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3169a184f100830ad590780b537538990268f68449768dfb81b3f2611957571`  
		Last Modified: Fri, 17 Mar 2023 00:12:55 GMT  
		Size: 12.0 MB (12012467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:204dc179b3902b536f78384f1b400bfb7f2c7a3afd041f635c026a2423dfae2e`  
		Last Modified: Fri, 17 Mar 2023 00:12:54 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0890949dad93f3e25242cf4c3690fce168ed9b3c0e06806559bdf4c6a338c246`  
		Last Modified: Fri, 17 Mar 2023 00:12:57 GMT  
		Size: 16.0 MB (15950067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3bde6c4ef275aa9ae6a8168cd6e18d4ca2d08ba0e5232d0ea3647b61f4b5be8`  
		Last Modified: Fri, 17 Mar 2023 00:12:54 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a223ee500b65eeb2e536bba722407e5b7c4c849bd85560fa0ae42802af5758`  
		Last Modified: Fri, 17 Mar 2023 00:12:54 GMT  
		Size: 18.8 KB (18794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
