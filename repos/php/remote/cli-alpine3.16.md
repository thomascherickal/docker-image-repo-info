## `php:cli-alpine3.16`

```console
$ docker pull php@sha256:5df0c539c5327521b8f508d48d50995767287ec9cf0622464d884f6a23d61d10
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

### `php:cli-alpine3.16` - linux; amd64

```console
$ docker pull php@sha256:353dc00f4c6f1563da79e6b8c06677bf22481671b86f318c3e7f5d2d4782390b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.4 MB (34369481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:231352980b055a4de4f84a52173a10ce6cf4761225da1ced8636a1cd74f929fa`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 19:48:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 19:48:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 19:48:09 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 19:48:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 19:48:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 19:48:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:48:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:48:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 19:48:10 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 22:45:29 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 22:45:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 22:45:29 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 22:45:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jul 2022 22:45:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:49:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 22:49:44 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:49:45 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 22:49:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 22:49:45 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde5ea1cb188409ac6276c7e55f3a6f6b0dfe9e3bd72711881e32183f03e8d99`  
		Last Modified: Wed, 25 May 2022 20:28:12 GMT  
		Size: 1.7 MB (1704858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3935ba60366aecf1bc3d1f0c663cb07711d490232ffa0ddde876eb4ebc40e469`  
		Last Modified: Wed, 25 May 2022 20:28:11 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4712e34f1d293d5afd1871939afc2d84d672bf03d6c4ef9c9558c720f40e5195`  
		Last Modified: Wed, 25 May 2022 20:28:11 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46ad320e620faa53b6f7e93de84a52b0754904e78e692376182cd0e923da8694`  
		Last Modified: Fri, 08 Jul 2022 00:15:26 GMT  
		Size: 11.7 MB (11742260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217a7e6d2acfa7109b199a77ef214693deec263c1b1e8dbf35c54ee04498c585`  
		Last Modified: Fri, 08 Jul 2022 00:15:25 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b3d966c79cde487a5d5355a658b4d2d6cea70d1b41a20817c3983b641bd219`  
		Last Modified: Fri, 08 Jul 2022 00:15:28 GMT  
		Size: 18.1 MB (18100353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4465162bf62f20786ada672d433a1ef16ec485e1b779ce47d2b2e9cb68e30127`  
		Last Modified: Fri, 08 Jul 2022 00:15:25 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d82d980f5987b02303fb58fbb3875f8d6fc985b4a6b33202ba5fc6a7b91101`  
		Last Modified: Fri, 08 Jul 2022 00:15:26 GMT  
		Size: 18.6 KB (18647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:cli-alpine3.16` - linux; arm variant v6

```console
$ docker pull php@sha256:a09533aedabe2bb219aec883120b8028931b589dc083bdecec7f3ab95cf34828
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32476274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e939463e8e863df83abfb3f7da70fb8dd5c250da8508699e16148dc9d278c6b4`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 21:50:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 21:50:07 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 21:50:08 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 21:50:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 21:50:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 21:50:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 21:50:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 21:50:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 21:50:12 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 21:24:18 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 21:24:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 21:24:19 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 21:24:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jul 2022 21:24:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 21:29:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 21:29:58 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 21:30:00 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 21:30:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 21:30:01 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e7eae6d0293087d982d321125f6f132894675f6acb732427528058758d6ae3`  
		Last Modified: Wed, 25 May 2022 22:46:23 GMT  
		Size: 1.7 MB (1693282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad96c7e3fdd13c53c906a10fab89b0dc599bf1746acd163f9648f8f9ec949de`  
		Last Modified: Wed, 25 May 2022 22:46:21 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1acccbd45290b92307c479937198ace1c187e0fd49d5e1ea72c1f5d7d5e1705`  
		Last Modified: Wed, 25 May 2022 22:46:21 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fa00277edf5af3bcea93a4e3e4aacf25d2b1f5c8c59a3493210c18e151ae238`  
		Last Modified: Thu, 07 Jul 2022 22:45:35 GMT  
		Size: 11.7 MB (11742258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f810c126b632d8fed8b53948cabb27aaa89fcdb205656dd28d53119f2ab4c55`  
		Last Modified: Thu, 07 Jul 2022 22:45:32 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b505ec5f5b1098dcc87e22bb2bb29029fd51ef682db493ee4950d787bccc0d9`  
		Last Modified: Thu, 07 Jul 2022 22:45:44 GMT  
		Size: 16.4 MB (16411674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:812f11c68d7e40de1457f7c9b290c5a6975ef4d0d2838357777b50274ce8a850`  
		Last Modified: Thu, 07 Jul 2022 22:45:32 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65dda250b6ec2906f8597e7c40cbc488180717fc6125aabfe58ea2fd2aada069`  
		Last Modified: Thu, 07 Jul 2022 22:45:32 GMT  
		Size: 18.5 KB (18451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:cli-alpine3.16` - linux; arm variant v7

```console
$ docker pull php@sha256:c9c25e74fcde909c9ee42188bf7a16f274b1b7fdbabd3d784a84281c390ae40e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.1 MB (31118891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a3ed6c16b7f58285027b3954ffe5c4f0e21b92211db1160af88dd650a63d89e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 19:01:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 19:01:25 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 19:01:27 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 19:01:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 19:01:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 19:01:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:01:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:01:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 19:01:31 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 22:57:41 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 22:57:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 22:57:42 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 22:57:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jul 2022 22:57:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 23:02:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 23:02:28 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 23:02:30 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 23:02:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 23:02:31 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68c4c667bd6865eca9aa9f496ecc527223b3162b260cad2e40c45ad49edc479`  
		Last Modified: Wed, 25 May 2022 20:09:19 GMT  
		Size: 1.6 MB (1560829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6bb9188dd796f59353a38be6412d00920f7c1da1effa359dc5c9a5724c0fb0`  
		Last Modified: Wed, 25 May 2022 20:09:18 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbde557014a2ec2c7a2e22a836cdf6978cf4aaea9b738859980a1d98c9b1282`  
		Last Modified: Wed, 25 May 2022 20:09:18 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:874b17b70d3dcdc229bea0fa13e8a9c46a393c0b2a1a8adbc1ac9ca1dcd1c4a5`  
		Last Modified: Fri, 08 Jul 2022 01:14:24 GMT  
		Size: 11.7 MB (11742246 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2ad42a8a59d26981614895494bc1ced0f5bdb5c6ea6b9e9b672e0d3a93027b`  
		Last Modified: Fri, 08 Jul 2022 01:14:21 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6de7d33e53cc54e0938256dc0e24a8d156d05af19410cff0cd0feff18f6790ea`  
		Last Modified: Fri, 08 Jul 2022 01:14:31 GMT  
		Size: 15.4 MB (15381265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bedcb798a79d0634d60613620812a760bc21803d55c18c96541c17e67d393a`  
		Last Modified: Fri, 08 Jul 2022 01:14:21 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2860df81dc9c58ab2fac5a155b75fec1e3668afdfc420f6faeed48f4ce2d11d2`  
		Last Modified: Fri, 08 Jul 2022 01:14:21 GMT  
		Size: 18.4 KB (18421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:cli-alpine3.16` - linux; arm64 variant v8

```console
$ docker pull php@sha256:b4da20a4c71815ef07a0330d2a12e1f085081a59bb1bef064ecad054f1368791
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34117717 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d50bb24212a06fcca5a41fd30fbefc22f2e39562d665def92b85a948e7903c7`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 20:06:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 20:06:19 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 20:06:20 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 20:06:21 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 20:06:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 20:06:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 20:06:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 20:06:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 20:06:26 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 22:26:43 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 22:26:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 22:26:45 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 22:26:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jul 2022 22:26:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:32:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 22:32:33 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:32:34 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 22:32:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 22:32:36 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a240d0a51bf6100803c8ce9f1ce769377fd09a2824a580ad991fb1a8a64610`  
		Last Modified: Wed, 25 May 2022 21:26:48 GMT  
		Size: 1.7 MB (1703255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d989eb157716fb2e84408b95764324504b7dd9aac628dd9a66a7f15eeb43a66`  
		Last Modified: Wed, 25 May 2022 21:26:48 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940028d0e55a77f4d9df2de18c1a76fa1058bdb66dee66fa6309f9337e500d6e`  
		Last Modified: Wed, 25 May 2022 21:26:48 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce3266979e4076dfb7e52c29c3acc19ad08c222d7e12bb1291eaefdcf8386a8`  
		Last Modified: Fri, 08 Jul 2022 00:06:52 GMT  
		Size: 11.7 MB (11742025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c79218c10d58667f9357fc9c29f91f228e827a95c62752ab4c1fd9560e3823`  
		Last Modified: Fri, 08 Jul 2022 00:06:50 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a56c6b4a1aa64ac986195bb322fdca1b1b1529b67f2b815071d17952f8072c4b`  
		Last Modified: Fri, 08 Jul 2022 00:06:53 GMT  
		Size: 18.0 MB (17955227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d85492b6391cb6017258c0e841f9308d42646b8e8d0d36514500524cd9ecb2`  
		Last Modified: Fri, 08 Jul 2022 00:06:50 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93400d803e0e11ab75fa91dfd3ebaa27ae21cfdd002061d270dab009a3fa3359`  
		Last Modified: Fri, 08 Jul 2022 00:06:50 GMT  
		Size: 18.3 KB (18340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:cli-alpine3.16` - linux; 386

```console
$ docker pull php@sha256:3e52ee391afbab163d0960e073058af9a4ddcb86e0cdb7e930c662dcda3ff76f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.9 MB (34885859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cb1ab6de774455886cdf327a6b5084d87b8ad39efb7ad953f9dd899c8f70bfd`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 19:56:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 19:56:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 19:56:28 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 19:56:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 19:56:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 19:56:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:56:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:56:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 19:56:34 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 22:52:15 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 22:52:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 22:52:17 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 22:52:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jul 2022 22:52:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:56:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 22:56:18 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 22:56:18 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 22:56:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 22:56:20 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97eb700ff81c1dbea3f8e204a809be7b7431ba817b16c87c1efe84972e2fe6c1`  
		Last Modified: Wed, 25 May 2022 20:43:18 GMT  
		Size: 1.8 MB (1807504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eaabb95698f746340e8771d50f4e356e03ad67347638c9d30dc7d3d7cdb3359`  
		Last Modified: Wed, 25 May 2022 20:43:18 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f127678bc84e9717b47e929fd82c70e9bc39b96e731eb561d466d4373561cd1`  
		Last Modified: Wed, 25 May 2022 20:43:17 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:986c99a036eb3f2cb7550f5600e945f78ed7db703558ae1e274736ad07153fbd`  
		Last Modified: Fri, 08 Jul 2022 00:24:53 GMT  
		Size: 11.7 MB (11742010 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f14f534bb01f9a8dabf379b1b2284c0a0c4691fb8311858c77c139ca06b2054`  
		Last Modified: Fri, 08 Jul 2022 00:24:51 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c216ea9e976b59483d73924ee99b826482db4c702781b257e55c82028bdd2fde`  
		Last Modified: Fri, 08 Jul 2022 00:24:54 GMT  
		Size: 18.5 MB (18511516 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34af7d72a9893d91973a80eefa3973e9fc5aa3d1d7a46f4218b14ad743344ba2`  
		Last Modified: Fri, 08 Jul 2022 00:24:51 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:773459b3abef56ecd96f1a92a5edd2c6f1801a28f5faab160790aebe09fcf279`  
		Last Modified: Fri, 08 Jul 2022 00:24:51 GMT  
		Size: 18.5 KB (18544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:cli-alpine3.16` - linux; ppc64le

```console
$ docker pull php@sha256:2f5c9030e6bbac73e038df682843aa77e9260e748f058787eb4641a1a1896596
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35157744 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee0256f7d0045025339859f2ce4e1b8712a22fec988f1d1832ee5f1d7e24769f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 19:57:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 19:57:35 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 19:57:43 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 19:57:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 19:57:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 19:57:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:57:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:57:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 19:57:56 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Fri, 08 Jul 2022 00:20:36 GMT
ENV PHP_VERSION=8.1.8
# Fri, 08 Jul 2022 00:20:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Fri, 08 Jul 2022 00:20:45 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Fri, 08 Jul 2022 00:21:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 08 Jul 2022 00:21:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 08 Jul 2022 00:26:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 08 Jul 2022 00:26:25 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Fri, 08 Jul 2022 00:26:39 GMT
RUN docker-php-ext-enable sodium
# Fri, 08 Jul 2022 00:26:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 08 Jul 2022 00:26:48 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1091cbad9101b41d3fd65de74d3265b02346722f13f77c4a456e33979dd226da`  
		Last Modified: Wed, 25 May 2022 21:08:36 GMT  
		Size: 1.8 MB (1759345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570e34510ef12ed73f2ed4ab7167c3408a7a0c69498928d0be0c6d46e2250ea3`  
		Last Modified: Wed, 25 May 2022 21:08:35 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbd0bbe87c55d5c71424cd10832856ec6580b2de2bf35112f9a41f574cef70f`  
		Last Modified: Wed, 25 May 2022 21:08:35 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:305b3063ec82e15c81424cd126fcc0b7983850de52bdddd2dbec64c77d7325cb`  
		Last Modified: Fri, 08 Jul 2022 03:22:22 GMT  
		Size: 11.7 MB (11742257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:803aa7046ad4f05b1c68c627c4064617f2c5b42d68ec68661e6c7a17f7ec52d2`  
		Last Modified: Fri, 08 Jul 2022 03:22:20 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ca373b1c5679ac62ffccbe865ba96173a6f3382a322e1036350b09ec6b66e3c`  
		Last Modified: Fri, 08 Jul 2022 03:22:24 GMT  
		Size: 18.8 MB (18843510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25e292c30e20c019e863fe503aa08e5b66af9e257afb1a3175ed59316393dcd0`  
		Last Modified: Fri, 08 Jul 2022 03:22:20 GMT  
		Size: 2.4 KB (2445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebcf401c8506b3ba42dfbf03f14aeeed7d59d80b0276833fe98d48d85184e33`  
		Last Modified: Fri, 08 Jul 2022 03:22:20 GMT  
		Size: 18.4 KB (18411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:cli-alpine3.16` - linux; s390x

```console
$ docker pull php@sha256:6544246e53d2de0ddbaa25680dc25da3904f30f7bc9188dfcf61fd3d4b6515e8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.9 MB (32916054 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2349b119065c6124b02b4db7b3fc600255b8ac989ab7eed3b59b269782aad077`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 20:06:36 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 20:06:39 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 20:06:40 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 20:06:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 20:06:42 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 20:06:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 20:06:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 20:06:43 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 20:06:43 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 07 Jul 2022 21:39:58 GMT
ENV PHP_VERSION=8.1.8
# Thu, 07 Jul 2022 21:39:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Thu, 07 Jul 2022 21:39:59 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Thu, 07 Jul 2022 21:40:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jul 2022 21:40:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jul 2022 21:42:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jul 2022 21:42:56 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 07 Jul 2022 21:42:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jul 2022 21:42:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jul 2022 21:42:57 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad757c376420c4bd689dd2059809802df6400dc63a1f808ebb6ca69780724e3`  
		Last Modified: Wed, 25 May 2022 21:13:30 GMT  
		Size: 1.8 MB (1765925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ece50bae8c0ec9d3501fc804150b9b5ad9fe9187347f2304690718df868b540`  
		Last Modified: Wed, 25 May 2022 21:13:29 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992853a158bd58244683eefc2e1a8c73fa903949f9422c6c9f2d55a4a83fc0f3`  
		Last Modified: Wed, 25 May 2022 21:13:29 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81daf7a9579c70a18bcff7396cfbbeceaecd215c895a9a0f461eb491e6b4d4e8`  
		Last Modified: Thu, 07 Jul 2022 23:11:04 GMT  
		Size: 11.7 MB (11742260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f812bd6c51a02a7c269a6b4f17cfa40e92de612461bc58b3b41e90160c37be1`  
		Last Modified: Thu, 07 Jul 2022 23:11:04 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03fa90a4bcdbcaa8369fc459a54c8534dd2ec45a7ba270c3d6646352dd499907`  
		Last Modified: Thu, 07 Jul 2022 23:11:06 GMT  
		Size: 16.8 MB (16804442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:834328dc7e8b80ed69341e4756ae3b1c00bc001d70658a94b307f79828aa3f3c`  
		Last Modified: Thu, 07 Jul 2022 23:11:03 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e1a9be632876b944573992c863d96a4b85ac2c27cd88a043d6166f26555ce6`  
		Last Modified: Thu, 07 Jul 2022 23:11:03 GMT  
		Size: 18.5 KB (18459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
