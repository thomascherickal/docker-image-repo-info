## `php:zts-alpine3.11`

```console
$ docker pull php@sha256:f03bed173a537f5c96f86fa0a51dbaef05ae438c5b860823fd2268271248f13c
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

### `php:zts-alpine3.11` - linux; amd64

```console
$ docker pull php@sha256:446517726709c75f0aeae11fe74a6eaaac98e149c8d43bd9aedc0af1563c2e57
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.3 MB (25282721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c89d9fa2e6f4af9801611d975c8895b831f35ef8fe5512c8049cba0b810f4a7d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:35:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 24 Apr 2020 17:35:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 24 Apr 2020 17:35:51 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 24 Apr 2020 17:35:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 24 Apr 2020 17:35:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 24 Apr 2020 17:46:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Fri, 24 Apr 2020 17:46:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 17:46:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 17:46:27 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Apr 2020 17:46:28 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 06 Aug 2020 20:16:15 GMT
ENV PHP_VERSION=7.4.9
# Thu, 06 Aug 2020 20:16:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.9.tar.xz.asc
# Thu, 06 Aug 2020 20:16:16 GMT
ENV PHP_SHA256=23733f4a608ad1bebdcecf0138ebc5fd57cf20d6e0915f98a9444c3f747dc57b PHP_MD5=
# Thu, 06 Aug 2020 20:16:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Aug 2020 20:16:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Sep 2020 03:34:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Sep 2020 03:34:14 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Tue, 01 Sep 2020 03:34:16 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Sep 2020 03:34:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Sep 2020 03:34:17 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc86e4cff5f320d778d7412cab415d31e8e986659b5e453545b0a7afe86d472`  
		Last Modified: Fri, 24 Apr 2020 19:16:17 GMT  
		Size: 1.4 MB (1355296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be142bd33f5003d85a3e056208af127ac6c5f627f263469134baafdd011ad59`  
		Last Modified: Fri, 24 Apr 2020 19:16:16 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8132c9e52be363f64724649f370635dd54cac7b8696c6365dd2011290afbc7c0`  
		Last Modified: Fri, 24 Apr 2020 19:16:16 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdac70d12df78b7b8352d77c85dba7c76c7ee9440da1c03ada40ceab4779f868`  
		Last Modified: Fri, 07 Aug 2020 00:26:40 GMT  
		Size: 10.3 MB (10308658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ecf31e8747546964784ee38d0f1cfb3ef420c70c4c9a05a91d52106f327fa3`  
		Last Modified: Fri, 07 Aug 2020 00:26:39 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda784c05c4624f98eba3201fcefd762c48b6b5a68b1b52c889c33606cf69c02`  
		Last Modified: Tue, 01 Sep 2020 07:22:29 GMT  
		Size: 10.8 MB (10784115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96d116e3ee1b551bbe254f17aeb4eaa2640c2bcd22bfa0dbabf52f02fd01a80`  
		Last Modified: Tue, 01 Sep 2020 07:22:26 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3196bd20ad7af652f24de8c8c8a5ae058d9dbde95b59f5d2b895c6389b032d2`  
		Last Modified: Tue, 01 Sep 2020 07:22:26 GMT  
		Size: 17.1 KB (17109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:zts-alpine3.11` - linux; arm variant v6

```console
$ docker pull php@sha256:b7380a7f417f8a8fb7b2b12843468f25cab4ff6c821a17e371e4442a52f37eb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.4 MB (24433654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b70086bb6f653f2d7b0eb9e46c054c6ebfaa3c865c1d510cd4ec4bdf31d72150`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:40:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 23 Apr 2020 22:40:31 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 23 Apr 2020 22:40:34 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 23 Apr 2020 22:40:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 22:40:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 22:49:14 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Thu, 23 Apr 2020 22:49:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 22:49:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 22:49:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 22:49:18 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 06 Aug 2020 19:09:44 GMT
ENV PHP_VERSION=7.4.9
# Thu, 06 Aug 2020 19:09:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.9.tar.xz.asc
# Thu, 06 Aug 2020 19:10:10 GMT
ENV PHP_SHA256=23733f4a608ad1bebdcecf0138ebc5fd57cf20d6e0915f98a9444c3f747dc57b PHP_MD5=
# Thu, 06 Aug 2020 19:11:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Aug 2020 19:11:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Sep 2020 01:37:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Sep 2020 01:38:26 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Tue, 01 Sep 2020 01:39:29 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Sep 2020 01:39:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Sep 2020 01:40:06 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e4a0b35ae612f97f86d2cb9a5c35d9974c53c9693ed9c503293a2ed4d1f5eb`  
		Last Modified: Thu, 23 Apr 2020 23:53:32 GMT  
		Size: 1.3 MB (1321299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744673dda954515280697917b25c13df9ff57231c28643848fc80b349d6b246b`  
		Last Modified: Thu, 23 Apr 2020 23:53:31 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6829673d00afbe39285f6e4d9977770c99d7bf841436086efa137773c99fd188`  
		Last Modified: Thu, 23 Apr 2020 23:53:31 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eedf37e891da43054899210d3e59bf9e34abd40ed4fd63940a9a5d9099a44009`  
		Last Modified: Thu, 06 Aug 2020 21:07:50 GMT  
		Size: 10.3 MB (10308672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed720bd97c8dc0a775e2ddc4366f11c124bc461597bac016e7b0899f10115201`  
		Last Modified: Thu, 06 Aug 2020 21:07:47 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:542c37b41851eac2cbdb77fb6c4545c2b949f1291b435d8886d186467582eed2`  
		Last Modified: Tue, 01 Sep 2020 03:33:01 GMT  
		Size: 10.2 MB (10162344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fac110dade123a0ae45d45ae743cc57c0154a01d3a11d9c97fb1f2a5fe7ff9ed`  
		Last Modified: Tue, 01 Sep 2020 03:32:58 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0aa8f1781f9c6720834c6359d59594a35af6a74a905c93849f1740ce821c7851`  
		Last Modified: Tue, 01 Sep 2020 03:32:58 GMT  
		Size: 17.1 KB (17102 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:zts-alpine3.11` - linux; arm variant v7

```console
$ docker pull php@sha256:f4a79f1c16c6cec497a66f98e2364d582415d57c7d525fd86d24d95b85bc86be
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **23.5 MB (23476316 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00644c3c8b6ed31aca2b7d951dbdf69152d72708504295be9b3f8767015dbbb1`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:12:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 24 Apr 2020 09:12:32 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 24 Apr 2020 09:12:34 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 24 Apr 2020 09:12:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 24 Apr 2020 09:12:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 24 Apr 2020 09:18:11 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Fri, 24 Apr 2020 09:18:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 09:18:13 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 09:18:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Apr 2020 09:18:14 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 06 Aug 2020 20:08:14 GMT
ENV PHP_VERSION=7.4.9
# Thu, 06 Aug 2020 20:08:20 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.9.tar.xz.asc
# Thu, 06 Aug 2020 20:08:34 GMT
ENV PHP_SHA256=23733f4a608ad1bebdcecf0138ebc5fd57cf20d6e0915f98a9444c3f747dc57b PHP_MD5=
# Thu, 06 Aug 2020 20:09:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Aug 2020 20:09:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 06 Aug 2020 20:12:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 06 Aug 2020 20:13:29 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 06 Aug 2020 20:14:18 GMT
RUN docker-php-ext-enable sodium
# Thu, 06 Aug 2020 20:14:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 06 Aug 2020 20:14:46 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39281f57fe7d3f99c4fe23af0e5eb45caa0646180d5ff71304d26ff35a0b9856`  
		Last Modified: Fri, 24 Apr 2020 11:16:34 GMT  
		Size: 1.2 MB (1227897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df36ec4ede8343ef6e75d1f33f8dbbe0ccdfa6522152dda7801db48b8a06b85`  
		Last Modified: Fri, 24 Apr 2020 11:16:33 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e16ed34ef7f3b453ef768e1198de2318c7d1cdd60f43223f1c53df2e82119e`  
		Last Modified: Fri, 24 Apr 2020 11:16:33 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b48d32e611471be2ad7126a4497fda2c3019213f5ac749565738bc138deb3c92`  
		Last Modified: Fri, 07 Aug 2020 01:05:17 GMT  
		Size: 10.3 MB (10308678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f020df63ac6ede5d212bed519342a818d8eb226761db8274f73686ed46955726`  
		Last Modified: Fri, 07 Aug 2020 01:05:15 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a120ab1a46c665c9b67cf2508a000c760deb2861f6ead7a78c7520c37fd131ff`  
		Last Modified: Fri, 07 Aug 2020 01:05:19 GMT  
		Size: 9.5 MB (9496288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e188e28d9522c861786dfc4b9d5cb37b628cbc4638e96827f75ede966e957459`  
		Last Modified: Fri, 07 Aug 2020 01:05:16 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5b23e64aacbd64f8ad8a46a7ea1e75afd7853cf0093214ae0f80774ce820e7`  
		Last Modified: Fri, 07 Aug 2020 01:05:16 GMT  
		Size: 17.1 KB (17089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:zts-alpine3.11` - linux; arm64 variant v8

```console
$ docker pull php@sha256:7a79e8f7af58306308590e1b1753ceac1300b9ce4a244e4dd0e3eb61b40e160f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.1 MB (25118190 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcf46484514e5b2a8100983e4c244f547a56ded03e14e08ca3d967619b2415ed`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:51:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 24 Apr 2020 12:51:32 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 24 Apr 2020 12:51:35 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 24 Apr 2020 12:51:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 24 Apr 2020 12:51:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 24 Apr 2020 13:00:13 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Fri, 24 Apr 2020 13:00:14 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 13:00:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 13:00:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Apr 2020 13:00:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 06 Aug 2020 19:39:42 GMT
ENV PHP_VERSION=7.4.9
# Thu, 06 Aug 2020 19:39:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.9.tar.xz.asc
# Thu, 06 Aug 2020 19:40:00 GMT
ENV PHP_SHA256=23733f4a608ad1bebdcecf0138ebc5fd57cf20d6e0915f98a9444c3f747dc57b PHP_MD5=
# Thu, 06 Aug 2020 19:40:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Aug 2020 19:40:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Sep 2020 04:51:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Sep 2020 04:51:33 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Tue, 01 Sep 2020 04:52:04 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Sep 2020 04:52:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Sep 2020 04:52:21 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8614da4aa8d46e10af7f7788136931561b8f1d1efe1a78311b26f5cf57506f`  
		Last Modified: Fri, 24 Apr 2020 14:02:47 GMT  
		Size: 1.4 MB (1359714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ececdba1264fbd4760d671f21f71713e4038fc665ad77ae891d54cc1d8db0cc3`  
		Last Modified: Fri, 24 Apr 2020 14:02:46 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab4eb699b8d1e5be3d1e82202067c943b8869558f71be0d2557563912b0f942`  
		Last Modified: Fri, 24 Apr 2020 14:02:47 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4686ca66c7870d3e4c381baa09104ba5088a30b0219e5710c11352e9909d6644`  
		Last Modified: Thu, 06 Aug 2020 23:31:31 GMT  
		Size: 10.3 MB (10308671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18d18c86a85196e4301433f672c826004a101cd98d9900bbd749708d8a8b4bdc`  
		Last Modified: Thu, 06 Aug 2020 23:31:27 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f05821fabfd116130f339dc05f6ae60ce82dbe4314cea368a46cfae7dd745910`  
		Last Modified: Tue, 01 Sep 2020 07:07:30 GMT  
		Size: 10.7 MB (10703983 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce0f61e616131b9dab0d7509ebccf8247fe49eefc2938f329256f3f76ba8823`  
		Last Modified: Tue, 01 Sep 2020 07:07:28 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db974a49fe382de31ab86b35cc82312167d6cfc92d0057a2bca22a88fb9f1707`  
		Last Modified: Tue, 01 Sep 2020 07:07:28 GMT  
		Size: 17.1 KB (17097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:zts-alpine3.11` - linux; 386

```console
$ docker pull php@sha256:262cce2a2d0d52ff0db3fcbbba4272bb16f4a10437371451aa59ddbd83938daf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **25.7 MB (25694298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee13cd32be20fb8fd26e1bac1c08493f3a710bf7b0d82733454f170847a6c18e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 06:05:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 24 Apr 2020 06:05:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 24 Apr 2020 06:05:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 24 Apr 2020 06:05:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 24 Apr 2020 06:05:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 24 Apr 2020 06:17:25 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Fri, 24 Apr 2020 06:17:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 06:17:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 06:17:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Apr 2020 06:17:25 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 06 Aug 2020 20:25:43 GMT
ENV PHP_VERSION=7.4.9
# Thu, 06 Aug 2020 20:25:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.9.tar.xz.asc
# Thu, 06 Aug 2020 20:25:43 GMT
ENV PHP_SHA256=23733f4a608ad1bebdcecf0138ebc5fd57cf20d6e0915f98a9444c3f747dc57b PHP_MD5=
# Thu, 06 Aug 2020 20:25:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Aug 2020 20:25:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Sep 2020 01:19:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Sep 2020 01:19:56 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Tue, 01 Sep 2020 01:19:57 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Sep 2020 01:19:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Sep 2020 01:19:58 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990138137e85533c48403b0cd1aee9ac6c5f3fc3be67a74a44a22f1a30e39af6`  
		Last Modified: Fri, 24 Apr 2020 07:59:39 GMT  
		Size: 1.5 MB (1453100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d973cd3524efeb6727b2144c33f96c71896f4ee22b1a55cc0c5aa5756f9b758`  
		Last Modified: Fri, 24 Apr 2020 07:59:37 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f386ab173ce6081c15380f99f906f8ea531e5748425804a21ebb0b5c433e6782`  
		Last Modified: Fri, 24 Apr 2020 07:59:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bad6993ab1d2610b02a4129500cac031cbaff8a88003e3adbb857cf8027f6556`  
		Last Modified: Fri, 07 Aug 2020 00:49:11 GMT  
		Size: 10.3 MB (10308666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f87197bec0ea6323c9be4d6a2a0036fbf021cf8a0939c076ed4382575f143bb`  
		Last Modified: Fri, 07 Aug 2020 00:49:09 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3284de38087773157d52f79fda072ec09f6d7035724eb24cb8ee936f5c972db4`  
		Last Modified: Tue, 01 Sep 2020 05:14:15 GMT  
		Size: 11.1 MB (11102783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3abd7aa174f6f8986eef81afc6ca0069ea119544706cc710032c61e5840e62a`  
		Last Modified: Tue, 01 Sep 2020 05:14:09 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6db6a18c89003712582fa1da861590c3cb59c657a9da1e261d3064f363428f9b`  
		Last Modified: Tue, 01 Sep 2020 05:14:09 GMT  
		Size: 17.1 KB (17109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:zts-alpine3.11` - linux; ppc64le

```console
$ docker pull php@sha256:5bf62072c006df4ba6d16c4ddae324a3872d56c45f9474e8a3f5cef0f14e2fe0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **26.0 MB (26032158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4332e24338e34834be7768f3740b551fed479d1ef48cd79b54348ffef252907b`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:11:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 24 Apr 2020 07:11:47 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 24 Apr 2020 07:12:07 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 24 Apr 2020 07:12:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 24 Apr 2020 07:12:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 24 Apr 2020 07:24:30 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Fri, 24 Apr 2020 07:24:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 07:24:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 07:24:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Apr 2020 07:24:46 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 06 Aug 2020 19:54:04 GMT
ENV PHP_VERSION=7.4.9
# Thu, 06 Aug 2020 19:54:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.9.tar.xz.asc
# Thu, 06 Aug 2020 19:54:13 GMT
ENV PHP_SHA256=23733f4a608ad1bebdcecf0138ebc5fd57cf20d6e0915f98a9444c3f747dc57b PHP_MD5=
# Thu, 06 Aug 2020 19:54:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Aug 2020 19:54:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Sep 2020 04:36:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Sep 2020 04:36:30 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Tue, 01 Sep 2020 04:36:41 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Sep 2020 04:36:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Sep 2020 04:36:48 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d52f33021895c8254527a626bd23b02f5ffb7cf7d498663099bfb52bc36cb4f`  
		Last Modified: Fri, 24 Apr 2020 08:53:41 GMT  
		Size: 1.4 MB (1398496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca0df5facaec815af37eabcf3f16b8d84fbf49322219c06e6d19e7067b54f86`  
		Last Modified: Fri, 24 Apr 2020 08:53:38 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eafa9bf45f1a09b417cf061af38e982c6a4e2c77a1f1f3c59b8587f215c9208`  
		Last Modified: Fri, 24 Apr 2020 08:53:37 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bfde1fe4f392b1aef229b9ba8cb4e79fc5af6b661d5bbeadfb0e344a89b4c67`  
		Last Modified: Thu, 06 Aug 2020 22:43:02 GMT  
		Size: 10.3 MB (10308688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3354b0d408b02026b44d39cb6407b73afc231ad8a62b2104b79b16311b51de28`  
		Last Modified: Thu, 06 Aug 2020 22:42:59 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9524558ed6dcc8edd0020ff3d9eb195b215508b49890dae7c146815c21e4fcb5`  
		Last Modified: Tue, 01 Sep 2020 07:06:01 GMT  
		Size: 11.5 MB (11481736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb5fd830322540559093fb1349cfb2c036e70929c3f6d05c6063948c9977a150`  
		Last Modified: Tue, 01 Sep 2020 07:05:37 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:763d4d3a70c9e4467e2f2ed16480098168f322a1ae94cb205afe8a7d3c3e5ade`  
		Last Modified: Tue, 01 Sep 2020 07:05:39 GMT  
		Size: 17.1 KB (17092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `php:zts-alpine3.11` - linux; s390x

```console
$ docker pull php@sha256:5ba18bd33f67f4f6544db87fa510f0a58938c32019a9c1c5d392b1dd2da92797
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **24.7 MB (24746673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab5465054538ed379f0a453bb333e985b7d1b25c29d9e19d7a262d614ab62e9`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php","-a"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 23:04:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 23 Apr 2020 23:04:49 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 23 Apr 2020 23:04:50 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 23 Apr 2020 23:04:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 23:04:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 23:09:56 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-maintainer-zts --disable-cgi
# Thu, 23 Apr 2020 23:09:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 23:09:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 23:09:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 23:09:57 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 06 Aug 2020 18:44:55 GMT
ENV PHP_VERSION=7.4.9
# Thu, 06 Aug 2020 18:44:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.9.tar.xz.asc
# Thu, 06 Aug 2020 18:44:56 GMT
ENV PHP_SHA256=23733f4a608ad1bebdcecf0138ebc5fd57cf20d6e0915f98a9444c3f747dc57b PHP_MD5=
# Thu, 06 Aug 2020 18:45:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Aug 2020 18:45:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Sep 2020 00:53:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Sep 2020 00:53:39 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Tue, 01 Sep 2020 00:53:40 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Sep 2020 00:53:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Sep 2020 00:53:40 GMT
CMD ["php" "-a"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9311aad926b3cb7924b7f1bbfda3972f2b64dca32e8decf8257ba49353a285`  
		Last Modified: Thu, 23 Apr 2020 23:53:51 GMT  
		Size: 1.4 MB (1397092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77861eec55084cb75eb6742ba23b02781c9311acbf6d27f56e08d1323565fe2`  
		Last Modified: Thu, 23 Apr 2020 23:53:50 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628ed6ecb36cf955a18714674b47d5822ae7eb0372cd31f3c2edd4a3c38fce32`  
		Last Modified: Thu, 23 Apr 2020 23:53:48 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1742377729b75ed91868a4cbf76594677ab866864c8b69a5ff765c740ebed9a3`  
		Last Modified: Thu, 06 Aug 2020 19:48:52 GMT  
		Size: 10.3 MB (10308686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7e4093eb1093b9beda3e4ecaa81be7c3f50e22cf095f67ffe32a930888cab2a`  
		Last Modified: Thu, 06 Aug 2020 19:48:50 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2512a67a0a5862721ae1efb3dc2a2f9ce3028542ab9b60eb4b3f2622bdba2718`  
		Last Modified: Tue, 01 Sep 2020 02:27:28 GMT  
		Size: 10.4 MB (10436646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f2e38905584d7da0336596d9dcf91a0a4cda62c805842fb3d4c2979f757f309`  
		Last Modified: Tue, 01 Sep 2020 02:27:26 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb1dfd20ca6ded76a6d463d31a587e003fabc3deb93043746cf3cb0e075c8b0`  
		Last Modified: Tue, 01 Sep 2020 02:27:26 GMT  
		Size: 17.1 KB (17093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
