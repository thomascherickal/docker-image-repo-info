## `php:7-cli-alpine3.13`

```console
$ docker pull php@sha256:aa43e49ff8247f41f8c10ab211b5b7ea8fa61d1723269a49d33336363230ed30
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

### `php:7-cli-alpine3.13` - linux; amd64

```console
$ docker pull php@sha256:ef74ad84de438cb5ef47ac94b507e36275c67c16ac616447ffa2bce65c44c07a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.5 MB (29476409 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6281d1f0f3ce136e0531ffad60357ac8fffec3a9dbff182a2f816503945b0642`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Tue, 31 Aug 2021 23:18:16 GMT
ADD file:ecdfb91a737d6c292265c1b77ffd3d82ba810dd43ea4ef79714b66b1da74a5aa in / 
# Tue, 31 Aug 2021 23:18:16 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 04:00:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 01 Sep 2021 04:00:18 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 01 Sep 2021 04:00:19 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Sep 2021 04:00:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Sep 2021 04:00:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Sep 2021 04:00:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Sep 2021 04:00:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Sep 2021 04:00:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Sep 2021 04:33:56 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 22 Oct 2021 18:13:08 GMT
ENV PHP_VERSION=7.4.25
# Fri, 22 Oct 2021 18:13:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.25.tar.xz.asc
# Fri, 22 Oct 2021 18:13:08 GMT
ENV PHP_SHA256=12a758f1d7fee544387a28d3cf73226f47e3a52fb3049f07fcc37d156d393c0a
# Fri, 22 Oct 2021 18:13:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 22 Oct 2021 18:13:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Oct 2021 18:20:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 22 Oct 2021 18:20:50 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 22 Oct 2021 18:20:52 GMT
RUN docker-php-ext-enable sodium
# Fri, 22 Oct 2021 18:20:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 22 Oct 2021 18:20:53 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:4e9f2cdf438714c2c4533e28c6c41a89cc6c1b46cf77e54c488db30ca4f5b6f3`  
		Last Modified: Tue, 31 Aug 2021 23:18:55 GMT  
		Size: 2.8 MB (2814079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:662f73c0505feff97099f0198262a893c7591884904c0595d39c8825c60506ac`  
		Last Modified: Wed, 01 Sep 2021 05:17:53 GMT  
		Size: 1.7 MB (1707686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d10375732079c31a31aa416c500526f9fea1b9add9764883167734b851a1e8c`  
		Last Modified: Wed, 01 Sep 2021 05:17:52 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05d05dc8bbc6681ed10a3260ac9935232133f477566735176bec3f913fec89c1`  
		Last Modified: Wed, 01 Sep 2021 05:17:52 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6f6b0e200e13a2a6eb10d70bd06bda59d907430db3181c4aec875b9d428f22e`  
		Last Modified: Fri, 22 Oct 2021 18:49:53 GMT  
		Size: 10.4 MB (10395727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801e4846f02fb620c6fc0a4a7bd2d0b08f547316c80df84960337e3c9bb1498d`  
		Last Modified: Fri, 22 Oct 2021 18:49:53 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ff7fa06e8e72f6554fda25b9a463480e89385cdc98887bd101e6df21f9bd720`  
		Last Modified: Fri, 22 Oct 2021 18:49:55 GMT  
		Size: 14.5 MB (14536950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:941ca1a8bc7ac4e33345b97380fc5ee90cd78c6be06cb9dfca2ffdcb79419cb4`  
		Last Modified: Fri, 22 Oct 2021 18:49:53 GMT  
		Size: 2.3 KB (2306 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5910a112339e0221b7c5d87de5a019103d9113f06e784b1e5427c33eda3f0b`  
		Last Modified: Fri, 22 Oct 2021 18:49:53 GMT  
		Size: 17.6 KB (17632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-alpine3.13` - linux; arm variant v6

```console
$ docker pull php@sha256:4ba10ce20d86b164bc6a277e623db44de6acf9970be328b0e00350b4acec692d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.0 MB (28044132 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d811d0ae204ed7e2354fb7dc53c2693fbf75176cb51c3f9f9a6d10ac841cb8a`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:57 GMT
ADD file:26e756fd544e28ae75be38d81452cf3266a2dabcffe9ecce3af2db9fde9edea3 in / 
# Fri, 12 Nov 2021 16:49:58 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 01:11:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 01:11:15 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 01:11:16 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 01:11:17 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 01:11:18 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 01:11:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 01:11:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 01:11:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 01:56:42 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 13 Nov 2021 01:56:42 GMT
ENV PHP_VERSION=7.4.25
# Sat, 13 Nov 2021 01:56:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.25.tar.xz.asc
# Sat, 13 Nov 2021 01:56:43 GMT
ENV PHP_SHA256=12a758f1d7fee544387a28d3cf73226f47e3a52fb3049f07fcc37d156d393c0a
# Sat, 13 Nov 2021 01:57:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 13 Nov 2021 01:57:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 13 Nov 2021 02:01:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 13 Nov 2021 02:01:36 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Sat, 13 Nov 2021 02:01:39 GMT
RUN docker-php-ext-enable sodium
# Sat, 13 Nov 2021 02:01:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 13 Nov 2021 02:01:40 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:846f3a0f3493d22f22643b6a1c057d2d37e608433cd1033d25dac92032b8b9e3`  
		Last Modified: Fri, 12 Nov 2021 16:51:54 GMT  
		Size: 2.6 MB (2633344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709a0b0ba2762467ff5cd49fe541e7bea1116a100156f40955aee70ba1c714b8`  
		Last Modified: Sat, 13 Nov 2021 02:50:36 GMT  
		Size: 1.7 MB (1701986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894f2665ecd825a26876bc3bd318a5a9e41d519d6a5ed6d3071c5a2aafbf1b69`  
		Last Modified: Sat, 13 Nov 2021 02:50:35 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f363d7c7ae87485a0a4982c1f8be83a9d0da4e4513e74c24325340688483c60`  
		Last Modified: Sat, 13 Nov 2021 02:50:35 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e757baad4e1f41050b1de4301b98dbc0f56ce0417adaabbca129333acbfcd5c2`  
		Last Modified: Sat, 13 Nov 2021 02:57:09 GMT  
		Size: 10.4 MB (10396163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebac89a61ea84a130ecb73cd53643789f82ac118dde1ef32801f1924dc08d909`  
		Last Modified: Sat, 13 Nov 2021 02:57:07 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acfaaf2f6f0556bc0c7eb980be7f4ff49d9b4fbec5a572618efffb167d046880`  
		Last Modified: Sat, 13 Nov 2021 02:57:17 GMT  
		Size: 13.3 MB (13290277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9c6e57fa5139c1769be52808f08379a8d7c6598276481c52c9adfdeea356222`  
		Last Modified: Sat, 13 Nov 2021 02:57:07 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179725e8953afeb657d04485eaf3890be4d6c5b16f6b0adc718477d9e05243c2`  
		Last Modified: Sat, 13 Nov 2021 02:57:07 GMT  
		Size: 18.0 KB (18038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-alpine3.13` - linux; arm variant v7

```console
$ docker pull php@sha256:8b0d50878d38a1bc8214214f6e13bb0c120a075091348b43f84dbf5b02d81281
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.9 MB (26856479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:75a343ab89b664b0a4ab3d3c211b84a27ecf07fdf943052afd07d524cb7e62b9`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:54 GMT
ADD file:a13993855beba2267575c54a0c6707ddda85d238e697a81046a8b1c1a34df054 in / 
# Fri, 12 Nov 2021 16:57:54 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 02:30:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 02:30:29 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 02:30:31 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 02:30:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 02:30:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 02:30:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 02:30:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 02:30:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 03:17:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 13 Nov 2021 03:17:19 GMT
ENV PHP_VERSION=7.4.25
# Sat, 13 Nov 2021 03:17:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.25.tar.xz.asc
# Sat, 13 Nov 2021 03:17:20 GMT
ENV PHP_SHA256=12a758f1d7fee544387a28d3cf73226f47e3a52fb3049f07fcc37d156d393c0a
# Sat, 13 Nov 2021 03:17:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 13 Nov 2021 03:17:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 13 Nov 2021 03:21:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 13 Nov 2021 03:21:44 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Sat, 13 Nov 2021 03:21:47 GMT
RUN docker-php-ext-enable sodium
# Sat, 13 Nov 2021 03:21:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 13 Nov 2021 03:21:48 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:767c1b67bc22761376676021ea5a310e7a7d1344b7a017bb8ede1a202340dbaf`  
		Last Modified: Fri, 12 Nov 2021 16:59:54 GMT  
		Size: 2.4 MB (2436506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a024553b7b200f7f9e627307316c58b2ef4fccac9cf20f1d5b65872b7f7e66e`  
		Last Modified: Sat, 13 Nov 2021 04:22:37 GMT  
		Size: 1.6 MB (1571087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7010fcc94ee2e996f2b2e3aec4d84f46649fc70b5db989674108c0f1637ce5e`  
		Last Modified: Sat, 13 Nov 2021 04:22:36 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23f6947b4872056b7f5857818de8c20d4c6188a8f33061cb0362b23065c9636a`  
		Last Modified: Sat, 13 Nov 2021 04:22:36 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548f2832eeea9e97b4d833687eaf663e0d5bb16c83a1fba6dd017ce0375c0657`  
		Last Modified: Sat, 13 Nov 2021 04:31:38 GMT  
		Size: 10.4 MB (10396163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2bb154028097aa29fbc4ee846c33ff83f6425dda516a0ab6c83815e666a1b40`  
		Last Modified: Sat, 13 Nov 2021 04:31:36 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1e08546b35b72623da81643a7a6ac5c1d3cbcb300b20988a2a531ddb07cae58`  
		Last Modified: Sat, 13 Nov 2021 04:31:44 GMT  
		Size: 12.4 MB (12430357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3e16acfd7f53f73277ab39bcfc84c751434931f83e2c603015867d9c364cf8`  
		Last Modified: Sat, 13 Nov 2021 04:31:36 GMT  
		Size: 2.3 KB (2300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a19178df13e53c1eb8c4290348fd6f7d64d371abf6f3057673e1a0cd4becd1f4`  
		Last Modified: Sat, 13 Nov 2021 04:31:36 GMT  
		Size: 18.0 KB (18046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-alpine3.13` - linux; arm64 variant v8

```console
$ docker pull php@sha256:2c8526aacd0a62bdb7672ff29ae284414703009f44be29fc1ec58718f2edeba8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.9 MB (28919343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:23c0ee47a8589acdfc4b9c0245df77ff80eed1a66b7cfd2f9ffdef22219445ff`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 12 Nov 2021 16:40:05 GMT
ADD file:ad85e8724ab9b90e37aadca9513807d07d557e7fc4287ca017f01f269aff3920 in / 
# Fri, 12 Nov 2021 16:40:06 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:46:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 12 Nov 2021 19:46:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 12 Nov 2021 19:46:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 12 Nov 2021 19:46:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Nov 2021 19:46:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Nov 2021 19:46:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:46:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:46:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Nov 2021 20:37:14 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 12 Nov 2021 20:37:15 GMT
ENV PHP_VERSION=7.4.25
# Fri, 12 Nov 2021 20:37:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.25.tar.xz.asc
# Fri, 12 Nov 2021 20:37:17 GMT
ENV PHP_SHA256=12a758f1d7fee544387a28d3cf73226f47e3a52fb3049f07fcc37d156d393c0a
# Fri, 12 Nov 2021 20:37:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 12 Nov 2021 20:37:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 12 Nov 2021 20:42:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 12 Nov 2021 20:42:04 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 12 Nov 2021 20:42:05 GMT
RUN docker-php-ext-enable sodium
# Fri, 12 Nov 2021 20:42:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 12 Nov 2021 20:42:07 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:06decbbdea2401b400024fb2feadd51ee381cd4b7b78a30306c3828ec9f6c760`  
		Last Modified: Fri, 12 Nov 2021 16:41:15 GMT  
		Size: 2.7 MB (2719640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50dbf8d5f017c540c631de487dec7f45c7cc2dbfa733ea07a6990bca869b3ac6`  
		Last Modified: Fri, 12 Nov 2021 21:26:44 GMT  
		Size: 1.7 MB (1712223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c69606f4bc361ce0b7763cee352c411b14688059f4026d175cdb08d2420edb86`  
		Last Modified: Fri, 12 Nov 2021 21:26:43 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ded21824f7e9205cfb4bbeb96f339cb406d13e8fae594b44e5c8296515413a`  
		Last Modified: Fri, 12 Nov 2021 21:26:44 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2a5dff52ead344dfa8adf18a4f64c482c96da3d3d0407149b74e40af4dee36`  
		Last Modified: Fri, 12 Nov 2021 21:32:25 GMT  
		Size: 10.4 MB (10395947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c24b65739691ac362621ae95b9b3a4b8b0b1aef8da99bc5cd228eca3bd5d5fa`  
		Last Modified: Fri, 12 Nov 2021 21:32:24 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a7cc52612a39dca9d958e2c55bce91488bcfc7b55979ed178809d8bd5a44e0`  
		Last Modified: Fri, 12 Nov 2021 21:32:26 GMT  
		Size: 14.1 MB (14069328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e029cc6c337f2f65b0f98373f02662ab8fad6419a46a26fb27293b34eb86b657`  
		Last Modified: Fri, 12 Nov 2021 21:32:24 GMT  
		Size: 2.3 KB (2301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa8db48dc6b0893ca3b2c583e46a41d121ca0a67765a59827b7187202613f1fa`  
		Last Modified: Fri, 12 Nov 2021 21:32:24 GMT  
		Size: 18.0 KB (17959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-alpine3.13` - linux; 386

```console
$ docker pull php@sha256:c05ed06251288d101f2c50667325bd4a15f5018b5a6154af616f03126c637e0d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.7 MB (29720935 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f7c2340e6b93523ed31178062c06abf52c3550f7c8c9c902944476166f2e006`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:50 GMT
ADD file:f6503c5a96198c02627cf7250b271ec6d49ffa83a87a588498eee61ba7f9c6fe in / 
# Fri, 12 Nov 2021 16:38:50 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 01:08:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 01:08:48 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 01:08:49 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 01:08:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 01:08:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 01:08:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 01:08:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 01:08:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 02:29:33 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 13 Nov 2021 02:29:33 GMT
ENV PHP_VERSION=7.4.25
# Sat, 13 Nov 2021 02:29:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.25.tar.xz.asc
# Sat, 13 Nov 2021 02:29:34 GMT
ENV PHP_SHA256=12a758f1d7fee544387a28d3cf73226f47e3a52fb3049f07fcc37d156d393c0a
# Sat, 13 Nov 2021 02:29:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 13 Nov 2021 02:29:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 13 Nov 2021 02:36:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 13 Nov 2021 02:36:07 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Sat, 13 Nov 2021 02:36:09 GMT
RUN docker-php-ext-enable sodium
# Sat, 13 Nov 2021 02:36:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 13 Nov 2021 02:36:10 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:afe0e1febe23918824088b45b415ce1778e92899ae26f0867294eb91de50aa4f`  
		Last Modified: Fri, 12 Nov 2021 16:39:53 GMT  
		Size: 2.8 MB (2828811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57de1e3a102dd98cbd68f18394f446a21aceaf11dd9edc7ef426daa51ee20e6`  
		Last Modified: Sat, 13 Nov 2021 04:01:42 GMT  
		Size: 1.8 MB (1812559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a67c7a80f6eafc55d33b761189aac9a8fc69d68bb03a1ff883ff61a50cedbb3`  
		Last Modified: Sat, 13 Nov 2021 04:01:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a54b005055d99a7166c269ea407d95bdc1dcdedfdbedd89dd5f07dc39dd89a`  
		Last Modified: Sat, 13 Nov 2021 04:01:39 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd5184f5257c371a55bc61bc7366a3283aae34bef67e94293bac1ec226bcfe23`  
		Last Modified: Sat, 13 Nov 2021 04:09:32 GMT  
		Size: 10.4 MB (10396171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08cbf215d003c1abce0d322d563a0231714d07bb94654165e201d4091b99f98b`  
		Last Modified: Sat, 13 Nov 2021 04:09:31 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1666defc6e6ba9b640f6ea180f30af47acb144eec5c01ef28e393d85352a9a58`  
		Last Modified: Sat, 13 Nov 2021 04:09:35 GMT  
		Size: 14.7 MB (14661033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c598a8824882d1a5dfb8e2b8df7b1c9d6a3714d03000967515dc99b064fd2754`  
		Last Modified: Sat, 13 Nov 2021 04:09:31 GMT  
		Size: 2.3 KB (2301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ba4a58d7c652d976a95b9025b2ca050742414880a536b466024392ca99d20c8`  
		Last Modified: Sat, 13 Nov 2021 04:09:31 GMT  
		Size: 18.0 KB (18036 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-alpine3.13` - linux; ppc64le

```console
$ docker pull php@sha256:455c02b1e7b8817492565e6bb8ba01b91f11086c960e5fe75f7bfd1de32994b6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.6 MB (30558548 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a7d309925548c203fee7b2ea4c1cdd9c6c09aa008f4266220e326e8f0d1a04f`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Wed, 01 Sep 2021 02:42:40 GMT
ADD file:07a51f1a2f818bd1c1651832ce63cb1e0046a57994724cda6a20ff1a2a685295 in / 
# Wed, 01 Sep 2021 02:42:41 GMT
CMD ["/bin/sh"]
# Wed, 01 Sep 2021 11:37:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 01 Sep 2021 11:37:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 01 Sep 2021 11:37:36 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Sep 2021 11:37:42 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Sep 2021 11:37:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Sep 2021 11:37:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Sep 2021 11:38:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Sep 2021 11:38:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Sep 2021 12:05:36 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 22 Oct 2021 19:09:01 GMT
ENV PHP_VERSION=7.4.25
# Fri, 22 Oct 2021 19:09:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.25.tar.xz.asc
# Fri, 22 Oct 2021 19:09:08 GMT
ENV PHP_SHA256=12a758f1d7fee544387a28d3cf73226f47e3a52fb3049f07fcc37d156d393c0a
# Fri, 22 Oct 2021 19:09:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 22 Oct 2021 19:09:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 22 Oct 2021 19:14:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 22 Oct 2021 19:14:38 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 22 Oct 2021 19:14:49 GMT
RUN docker-php-ext-enable sodium
# Fri, 22 Oct 2021 19:14:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 22 Oct 2021 19:14:54 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:39d9bf63205258fe1d085fd596101e6fc46ff796cda8d3ba2983e166a25b74db`  
		Last Modified: Wed, 01 Sep 2021 02:43:53 GMT  
		Size: 2.8 MB (2814813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:280fcf6c136467410ce39cbedb1567e6594635bcfb69b3408ebe41740112baf9`  
		Last Modified: Wed, 01 Sep 2021 12:50:23 GMT  
		Size: 1.8 MB (1753345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2ffbefc6a72f5a7251be574aaf2b8ab0a340146a826cd12dd61bfef1a34f3ea`  
		Last Modified: Wed, 01 Sep 2021 12:50:22 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698662ec601124d3e71f3d6b5953ef4d8e2a14f3ead80a153d1133e3f65ee8d7`  
		Last Modified: Wed, 01 Sep 2021 12:50:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ccd3538c0a1699816c9bd4fe23481fc9c981a0eea7d0ebcac53ab1319f4708`  
		Last Modified: Fri, 22 Oct 2021 19:42:34 GMT  
		Size: 10.4 MB (10395710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93723e91fcbd491e81658506c2a01d91ac0dd44447b635497f95aca4b1c9e84e`  
		Last Modified: Fri, 22 Oct 2021 19:42:33 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c375d1167074fc1c7bab4f76f08adc241cab6918bc4575fa618d4dc66864ce`  
		Last Modified: Fri, 22 Oct 2021 19:42:37 GMT  
		Size: 15.6 MB (15572727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f40af6257960b4e764b7d7ea0ac27296f5a4ff1562126f5b2caeeb930cc951ae`  
		Last Modified: Fri, 22 Oct 2021 19:42:33 GMT  
		Size: 2.3 KB (2301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15b73bf054b097aae27baca26c9ac390c8effc5e7fd9a60743599138077c50dd`  
		Last Modified: Fri, 22 Oct 2021 19:42:33 GMT  
		Size: 17.6 KB (17625 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:7-cli-alpine3.13` - linux; s390x

```console
$ docker pull php@sha256:14e514df0a47885f5701a6facf81b910749e31911592ad1835ad83b2d4d6e700
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **28.5 MB (28461253 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:335f1ad861e76047fd287fbaecd3ad23c458614281ff6ed7040475ec1ce04477`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 12 Nov 2021 16:41:44 GMT
ADD file:637f327c9b07758709ef7dbc42eb472c888d221acde89b1c3775553864334d5c in / 
# Fri, 12 Nov 2021 16:41:44 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 20:04:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 12 Nov 2021 20:04:13 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 12 Nov 2021 20:04:13 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 12 Nov 2021 20:04:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Nov 2021 20:04:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Nov 2021 20:04:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 20:04:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 20:04:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Nov 2021 20:34:20 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 12 Nov 2021 20:34:20 GMT
ENV PHP_VERSION=7.4.25
# Fri, 12 Nov 2021 20:34:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.25.tar.xz.asc
# Fri, 12 Nov 2021 20:34:21 GMT
ENV PHP_SHA256=12a758f1d7fee544387a28d3cf73226f47e3a52fb3049f07fcc37d156d393c0a
# Fri, 12 Nov 2021 20:34:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 12 Nov 2021 20:34:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 12 Nov 2021 20:37:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 12 Nov 2021 20:37:13 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 12 Nov 2021 20:37:14 GMT
RUN docker-php-ext-enable sodium
# Fri, 12 Nov 2021 20:37:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 12 Nov 2021 20:37:14 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:b872f056719bde6e6722091afb2a3376d720c69c142b91ac352050080dd79615`  
		Last Modified: Fri, 12 Nov 2021 16:42:54 GMT  
		Size: 2.6 MB (2611155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1000bd5a210bcbcc7c067529790c76fddbf14888fb15a116bde3ccecb80481f`  
		Last Modified: Fri, 12 Nov 2021 21:11:22 GMT  
		Size: 1.8 MB (1773886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:457496087d5e5a8ebada28b554aa221ffbaf020ce8229f4569476666ef84d673`  
		Last Modified: Fri, 12 Nov 2021 21:11:22 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f15cab968ab945b21c8387458bdf17ebd9d32e1fa97512a52e3861e4c61ec6c`  
		Last Modified: Fri, 12 Nov 2021 21:11:22 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ac4bd067c5cade7adfcfce4c7ad3a9057abb03722ce8752957bbbd3625e135e`  
		Last Modified: Fri, 12 Nov 2021 21:15:55 GMT  
		Size: 10.4 MB (10396171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39995109e506297298ecf6604a2fe1f996cc7648c92ff747c444031bfcd9ba87`  
		Last Modified: Fri, 12 Nov 2021 21:15:55 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c11c29cff3d1462d3bc30c1b227d521a5e0ecfad15ce1bab16ddd6b64559869`  
		Last Modified: Fri, 12 Nov 2021 21:15:57 GMT  
		Size: 13.7 MB (13657673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b765c2f2b7f85047dafd83ab18825d4e70de8bf928485f7978afed0144a9ee`  
		Last Modified: Fri, 12 Nov 2021 21:15:55 GMT  
		Size: 2.3 KB (2302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eda5f4d2917236de0497545a1747bd678f00da5eaad8c6410f3f72a3534d3d11`  
		Last Modified: Fri, 12 Nov 2021 21:15:55 GMT  
		Size: 18.0 KB (18045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
