<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `composer`

-	[`composer:1`](#composer1)
-	[`composer:1.10`](#composer110)
-	[`composer:1.10.8`](#composer1108)
-	[`composer:1.9`](#composer19)
-	[`composer:1.9.3`](#composer193)
-	[`composer:2`](#composer2)
-	[`composer:2.0`](#composer20)
-	[`composer:2.0.0-alpha2`](#composer200-alpha2)
-	[`composer:latest`](#composerlatest)

## `composer:1`

```console
$ docker pull composer@sha256:68e9afcfe042a69a778ffccd2da55cf195dd5671ab14163b774f00d6da0f23c4
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

### `composer:1` - linux; amd64

```console
$ docker pull composer@sha256:6babbd3567845f5a1c6cf3a01143ddcb4abe587fd14e221e36accebf0e962e84
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63111308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433420023b60cdf98a661eab19b14714e5e1a7056ac73561a660d9727d80723c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:51:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:51:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:51:59 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:51:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:52:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:52:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:52:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:52:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:00:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:00:41 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:00:43 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:00:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:00:44 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 03:36:24 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 03:36:34 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 03:36:35 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 03:36:35 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 03:36:35 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 03:36:43 GMT
ENV COMPOSER_VERSION=1.10.7
# Fri, 12 Jun 2020 03:36:44 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 03:36:44 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 03:36:45 GMT
WORKDIR /app
# Fri, 12 Jun 2020 03:36:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 03:36:45 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358d6dbbdff5c10cbe23c608b7ff9c6d1dd13331dd7dc7644b727ca5ea8e742`  
		Last Modified: Thu, 11 Jun 2020 22:14:55 GMT  
		Size: 1.3 MB (1340817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232d962484c6b9a1caa33a12f1beed4cb20996085056b4fb1591a9fd1d8c89f`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1d3ac04d2af7a9f0eee25eccc72e586400051054ffb4aff7cdf2f4ebc993e8`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2fa029f21abccac9d1ce064bef95d56aad7de3e1079df260138622eaf8ab25`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 10.3 MB (10305445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e18722d91019f31ffd0d261959c5dd489f6d27361f221a669dbe9691a56ef9`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3659ffc4e0a4393e4597cf7a4210f863623e4e1cdf86ed3f06726aa0616108d9`  
		Last Modified: Thu, 11 Jun 2020 22:14:59 GMT  
		Size: 14.2 MB (14173631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1874d3f89152f2ab71121617a3cfdb60a30feccc88dc7806657e3b22f3ccd6`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2545369333e4aa084fbd5285c57af07bd75686c0976981a60df746089e02b75a`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 16.9 KB (16931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680b7fc10b4acd5dda859b161e18533921eb585502203fb8d90e392b990fc0ff`  
		Last Modified: Fri, 12 Jun 2020 03:37:08 GMT  
		Size: 33.8 MB (33777899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95843d9ed2bd562441ca7a2cc826205c5403bd8384507211f0d3854eb07153b8`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 189.3 KB (189338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab487c471b8cfbda88b1b5a5ea9b716442d9cae4c86413a3d3302d01f2c6b3b2`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c9a21ccbb41f0c9bc7e467ba8129c81c9c6ee9eb26efa9bf3a0ac6303da34a`  
		Last Modified: Fri, 12 Jun 2020 03:37:13 GMT  
		Size: 504.7 KB (504734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec30aea17efe54c81d4cacd55e4350577778932f8d4818b9a3ecc9706ee0e374`  
		Last Modified: Fri, 12 Jun 2020 03:37:13 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7959b1da3d37ece89d1d51098ea4a534e68b3d8311b39e6048287b4bba6250f2`  
		Last Modified: Fri, 12 Jun 2020 03:37:13 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1` - linux; arm variant v6

```console
$ docker pull composer@sha256:c99b3bde69d2f2fba1d4696ecb638d5e381c61fc1bef1be262c82eddfa17dc5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59515232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67b7073d9fbf550b58fd228a151b966b6325d38adb1c720bd8750545a3f10191`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:14:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:14:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:14:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:14:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:14:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:14:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:14:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:14:59 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:15:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:15:01 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:16:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:16:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:19:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:19:59 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:20:02 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:20:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:20:03 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 21:53:58 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 21:54:20 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 21:54:22 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 21:54:23 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 21:54:24 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 21:54:40 GMT
ENV COMPOSER_VERSION=1.10.7
# Thu, 11 Jun 2020 21:54:43 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 21:54:43 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 21:54:44 GMT
WORKDIR /app
# Thu, 11 Jun 2020 21:54:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 21:54:46 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72788d65e292354c2ce4b67441d334d0ba534db5ce71d5b8bf78011a256b566f`  
		Last Modified: Thu, 11 Jun 2020 19:29:37 GMT  
		Size: 1.3 MB (1310273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e32d62de43da999aca07cf15fdbe1cd6b03aebc88c15409c3463daadf13e01`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6701e05673b745147608cd1b6eb47a3fbc35bcfd8a65bc536e5b9f919b3d0e77`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23d338eb9977c3cc4f53684a30948f5defb783b30f97eb45447ad19c586495f`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 10.3 MB (10305474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f01a53caea7c04e7254412060a5c0cb23ff8364d565eab3d98fc0ec804c65b3`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784e930730f995fd22b8a9bdf378b989b6551ae36873db347c0d23370b99e831`  
		Last Modified: Thu, 11 Jun 2020 19:29:39 GMT  
		Size: 13.2 MB (13195114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdcd1019ed44b57cb67d664f43d95a56a032f8fbf5028ce6347443731418cb3`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f541954f527d04cef7111fa78ef9238624e7d52750cc75f73c9e0ec0d8add297`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 16.9 KB (16925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8df574460aaa4735f4c219fb58bd7ce6c6103c39e707bbd3fefdb7fda3eb15`  
		Last Modified: Thu, 11 Jun 2020 21:55:24 GMT  
		Size: 31.4 MB (31389293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d207a4c841e9986a8109779fe3f72f8a73a699ba6327cac1c3532c88c637374c`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 185.0 KB (185016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb807a0037a4bb2eea81b88d9d6bb855cd6ff3c4bb8d095679d2a08e8fd9785a`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628d2c181171c88661a79e5befe13fc7f464d8aa498dff82d835fd304f42840e`  
		Last Modified: Thu, 11 Jun 2020 21:55:33 GMT  
		Size: 504.8 KB (504761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5d325d1c74d1ed9f95a81872af98adebe1e0fcff9fa7c6cb883500dd03582e`  
		Last Modified: Thu, 11 Jun 2020 21:55:33 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19054a7d036b408c8c42f34c49a8ca70ce737a6f76c5f803d0fb8956091a4177`  
		Last Modified: Thu, 11 Jun 2020 21:55:33 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1` - linux; arm variant v7

```console
$ docker pull composer@sha256:b94ca5b5a25604233671a05014b89dfb56c3fe64f1f8200b6e71c913a2624b5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56821735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ae8665451ee2a2d4f3849bd08ad0178750f08c57ad44afeef533d24f078947b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:34:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:35:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:35:07 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:35:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:35:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:35:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:35:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:35:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:35:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:35:18 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:35:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:35:20 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:35:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:35:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:38:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:38:31 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:38:34 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:38:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:38:35 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 22:42:55 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 22:43:12 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 22:43:14 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 22:43:15 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 22:43:16 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 22:43:30 GMT
ENV COMPOSER_VERSION=1.10.7
# Thu, 11 Jun 2020 22:43:32 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 22:43:33 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 22:43:33 GMT
WORKDIR /app
# Thu, 11 Jun 2020 22:43:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 22:43:35 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5b4230297ea0028dae43acf7e134a55e11ebc15c53a61a2c0c72935dd0ed35`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.2 MB (1214376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779feafcddcba2692e3d187a609b90060e7deea16e8b629aada3a236e99c40f7`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b20c0367792ccffce00af872fa2ea0300330509fb8c15fe5c08905d7db739`  
		Last Modified: Thu, 11 Jun 2020 20:13:03 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9023ca7c2ffcb34f4e075e8f6d5001276142a28b4e0d398fa3eaddc67c4aec`  
		Last Modified: Thu, 11 Jun 2020 20:13:03 GMT  
		Size: 10.3 MB (10305461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e1f3f19383952fefc6527fb475db9a4cde57b21c9a9cb19135732e7b34d85c`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5e59fcc062532624a3a9dd675e189b78e7bce3a5b6c09ce99339dc5b014570`  
		Last Modified: Thu, 11 Jun 2020 20:13:06 GMT  
		Size: 12.4 MB (12350663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a6f7844ad0b4881ed895ba72be400c6782597448fa61bcaa58dd4fe0853836`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354514b31215294fcf1092b43467ddd5587ce6a1fefd1bd4b809cfafbfee18f7`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 16.9 KB (16913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2c7c46ccf6b4c6e523cc448dd15f5f05a0d06483d502b3b0fb72846dab717e`  
		Last Modified: Thu, 11 Jun 2020 22:44:10 GMT  
		Size: 29.8 MB (29839022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267aadf40444bd4f9132644aa6f6c0119543ca29a863cd01bfcaf3be7623cb6f`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 178.7 KB (178699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6871daa35ee6d1b5e329afbb68bf23ef665e526c054959b57f6dc1d858fa9da5`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1aac479723ca5c8c2a89d1610187c4148329bc22defdbc2a444dfc2b4cfabfd`  
		Last Modified: Thu, 11 Jun 2020 22:44:18 GMT  
		Size: 504.8 KB (504761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb738297c43fa116285317f4c78f4addf3a15382c0fd326dd4d29377ffc79d7`  
		Last Modified: Thu, 11 Jun 2020 22:44:18 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a4f6e9edfac9965af157620024a2e64e623cbad6dad720e2d44702b42327cc`  
		Last Modified: Thu, 11 Jun 2020 22:44:18 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:6c2943d8c54f865e3bbe6ea5d8968709106e67b9fbb0a79557af6286ff9e6986
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63191302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3bf68b97259926db2b63907b7b6ad33c3cb23398c5218c7e5a6cb042c608cc3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:40:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:40:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:40:31 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:40:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:40:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:40:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:40:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:40:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:40:37 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:40:38 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:40:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:40:39 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:40:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:40:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:44:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:44:41 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:44:44 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:44:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:44:46 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 22:57:10 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 22:57:28 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 22:57:30 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 22:57:31 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 22:57:31 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 22:57:45 GMT
ENV COMPOSER_VERSION=1.10.7
# Thu, 11 Jun 2020 22:57:48 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 22:57:49 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 22:57:49 GMT
WORKDIR /app
# Thu, 11 Jun 2020 22:57:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 22:57:50 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee09877319de284b8141c396485111447d75eb8cf26c68819f92f85a4de5649`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 MB (1342990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bad472a11fde1c83808bc84cc9c77da0743b9974bb8c51ab25ed0608cbb4558`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fca52dcdf28b691bbc24b2e2aff931667b865a9188287ef18af016712d3a0f`  
		Last Modified: Thu, 11 Jun 2020 20:30:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f7c9da4678b86166cb9b705a8b9505c19a0d1c24d47bb4360a5907dd28cf28`  
		Last Modified: Thu, 11 Jun 2020 20:30:04 GMT  
		Size: 10.3 MB (10305482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2aa0aa4a6988ac388d32698edfeecb7d0a24539556a4d33bc3327e5786ff0f`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39a6dec5d173eac97dd81097371b07b48982a0ab697e8ab09a40c6d4c319682`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 14.0 MB (13981145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d87e7b6f85188674dafd79fa2e34a45d6f197e8ce1ae71e2337c2534efca59`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f45b14b8adc9219dfa9399abfc7b1b753ca63bfb9a4109e4fd1c0da5caa1a0`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 16.9 KB (16938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88423514539f3ed88c3d723a4f15d7276e95e4c9f4d6c0d3864cd61e0ac8c81c`  
		Last Modified: Thu, 11 Jun 2020 22:58:31 GMT  
		Size: 34.1 MB (34138877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49e25f227bb97b88fe0ffc96fef316f6b53e7c48ef10c14f5399a7441b4ffec`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 188.1 KB (188066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3213d0d563d4eb6ff14649f7b487f46d48ae07fa7768b9ab975db0300aeb8e06`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867f1875f74e994124013a455523af4fa2ea1c18a20c999912dfef70cddf49e5`  
		Last Modified: Thu, 11 Jun 2020 22:58:39 GMT  
		Size: 504.8 KB (504760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a710d37874225c8cc6da9516d38717d9c53945a7c7eaf00c56c8764f8e532fc0`  
		Last Modified: Thu, 11 Jun 2020 22:58:39 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093b2977f90dfa6bf7e6c2dbd081d7c421ec1b69da9adf6b4d19ebe49dac79a7`  
		Last Modified: Thu, 11 Jun 2020 22:58:39 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1` - linux; 386

```console
$ docker pull composer@sha256:ca47ae35321e8e6f4572cb65f085ca1fbf08aa60d7a993ef8f314dbfc7ed12f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65188090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8034411c9bc77c35903f70e193a48739892a5ce4a31fa9f860c9205e856f6023`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:53:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:53:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:53:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:53:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:53:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:53:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:53:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:53:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:53:09 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:53:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:53:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:02:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:02:55 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:02:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:02:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:02:58 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 01:52:49 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 01:53:04 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 01:53:06 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 01:53:06 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 01:53:06 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 01:53:15 GMT
ENV COMPOSER_VERSION=1.10.7
# Fri, 12 Jun 2020 01:53:17 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 01:53:17 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 01:53:18 GMT
WORKDIR /app
# Fri, 12 Jun 2020 01:53:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 01:53:18 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380f9ca051d120d4ed72890904488f0f1e0fd0128cbd1c73adbff366e90bc2aa`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 1.4 MB (1439837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613b9419908bb5beb7365d9d340ee3071aebf8c7919f5379a7b99221fd74c78f`  
		Last Modified: Thu, 11 Jun 2020 22:28:36 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd1bd9f7e9212850ee7c4017e1d3e5ec33176a9113258688a743d871983ee8c`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055c67327ee726dcb5b4e69ca5490023191476ac33eb72e84aea00f6b00c68b7`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 10.3 MB (10305449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6b7ea2ee885f0ae987d58de97f74bb931344e2477eefb48f3d04a90751f764`  
		Last Modified: Thu, 11 Jun 2020 22:28:35 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030cdee16954ea64da3800cd137349eb9b23064bd73168050596c83095da383b`  
		Last Modified: Thu, 11 Jun 2020 22:28:40 GMT  
		Size: 14.6 MB (14564562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629202fa404c086a430dd7d7127e65b92265559980c347f282d4654381da41e8`  
		Last Modified: Thu, 11 Jun 2020 22:28:36 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9694db72218b1872d389aeb90cdae79a16b53f9dfdb334584badf8e808da9f`  
		Last Modified: Thu, 11 Jun 2020 22:28:35 GMT  
		Size: 16.9 KB (16939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4c0dbf20b6de48fdd627e0694147fc21e53c04431f7ebaaa94ec13ef6cae44`  
		Last Modified: Fri, 12 Jun 2020 01:53:45 GMT  
		Size: 35.4 MB (35355633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee96b64f9c4459a8444513a26888081669e737e3fc6eb2f028360b416b333b`  
		Last Modified: Fri, 12 Jun 2020 01:53:34 GMT  
		Size: 203.7 KB (203658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dde06329df568103704291e0b472e532ef23a2f00eadc9484c14ea9feebb8d8`  
		Last Modified: Fri, 12 Jun 2020 01:53:34 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a073f20a79e2063002071c18660e75c258c07c5cb94393ae82b4e7d51f7592b5`  
		Last Modified: Fri, 12 Jun 2020 01:53:51 GMT  
		Size: 504.7 KB (504739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872a29d49579bed85016977d1eb236f48a987c5d6cf992eb143af868d8ac2745`  
		Last Modified: Fri, 12 Jun 2020 01:53:51 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf2c57a63fa1e8a513188c0a237354c461502dbc26a5d6dda0aaa5218c816d8`  
		Last Modified: Fri, 12 Jun 2020 01:53:51 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1` - linux; ppc64le

```console
$ docker pull composer@sha256:e155573df8700733bd8bf1dce305e67622e262c4c75016d1d826624f312d75cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65449609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e574aedfcde654f9cc674ae6915ab8bc375b98c5a1b9c091e9ff77f1a4c72c58`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:45:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:45:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:45:29 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:45:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:45:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:45:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:45:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:45:52 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:45:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:45:59 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:46:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:46:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:50:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:50:07 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:50:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:50:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:50:19 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 01:52:57 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 01:53:15 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 01:53:22 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 01:53:24 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 01:53:29 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 01:54:02 GMT
ENV COMPOSER_VERSION=1.10.7
# Fri, 12 Jun 2020 01:54:10 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 01:54:11 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 01:54:15 GMT
WORKDIR /app
# Fri, 12 Jun 2020 01:54:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 01:54:19 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f98eb9049c4fcbaa1cf16ddb44aaf910a89a5471dc303198251fa25bc2a1ef`  
		Last Modified: Thu, 11 Jun 2020 20:57:07 GMT  
		Size: 1.4 MB (1383311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50cdb8e03fc1b19217cd9f80b86142d090ad3e818795b339ea4d9ef9b74555f`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4466e085b12b265fb47397c7c105fd7d78a5883beef49ab9f386393c4c3dae`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbb7594d19c6129fb268c14b9b61a062eb1509b9ee23d2d3c51e55d344b4022`  
		Last Modified: Thu, 11 Jun 2020 20:57:04 GMT  
		Size: 10.3 MB (10305491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfca2ae2dd0fa2baeaf870eb6d850ca046d8dede8bc7bd8e550139f315f0e8a1`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24693054c4d20048d5a8af6f339778f20546c2d519895fd146ed031ab08c95e8`  
		Last Modified: Thu, 11 Jun 2020 20:57:08 GMT  
		Size: 15.1 MB (15144559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91fc688a4963e2db4e23b0cf85f076b3ef08ad8cf636e48f8f6cf76f75b204`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79384080ee3a4da85e7fcf036c35abd4a72aba47f46157e5517a72aa76a2f043`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 17.0 KB (16975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9007b0e243a5a526f41b3c6df897e6cadd789dafa9075a0f6a76edf844e79dbc`  
		Last Modified: Fri, 12 Jun 2020 01:55:05 GMT  
		Size: 35.1 MB (35088531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee306131aed824d74ee7b9cd56c45cb38c0cbbf6f31360accf7310163e16e83`  
		Last Modified: Fri, 12 Jun 2020 01:54:54 GMT  
		Size: 195.7 KB (195699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e185de3b1f08c6feeb3143dac639b8e90538320cac4f19a62842f977cc1459aa`  
		Last Modified: Fri, 12 Jun 2020 01:54:54 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e9e5aadfb14bce92b646f2cc5d9e1bb48a418845cb2c5e422a6b650195444d`  
		Last Modified: Fri, 12 Jun 2020 01:55:19 GMT  
		Size: 504.8 KB (504763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3faa7594d67fbd17a8895393beeb7559f054737949d92803b2e4e52d32ea3add`  
		Last Modified: Fri, 12 Jun 2020 01:55:18 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3029d423df91b54e0ba93e32720d02228f7f5f055f6227a76d70200ee21fa7`  
		Last Modified: Fri, 12 Jun 2020 01:55:18 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1` - linux; s390x

```console
$ docker pull composer@sha256:a638d6ac9c98be9851cac68f86066ed9399324cf29b2bfe534074223796862fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62388970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf8b15a368579abfd95087125c06a1b3ce2c5b49728f3fe79b30417fc49716f5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:29:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:29:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:29:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:29:39 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:29:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:29:40 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:29:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:29:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:32:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:32:06 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:32:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:32:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:32:07 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 21:14:48 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 21:14:59 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 21:15:00 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 21:15:00 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 21:15:00 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 21:15:08 GMT
ENV COMPOSER_VERSION=1.10.7
# Thu, 11 Jun 2020 21:15:09 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 21:15:09 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 21:15:10 GMT
WORKDIR /app
# Thu, 11 Jun 2020 21:15:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 21:15:10 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057c8475c8b5e21c245ff682a57adf8970d16ccbed87694b3ec200c83e17a8fb`  
		Last Modified: Thu, 11 Jun 2020 19:32:19 GMT  
		Size: 1.4 MB (1382745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2bbd1ef5644a3638bc6f073de941463cbfceb435ea6d11ce3c7fdb9f8d2539`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b73c5118a1a42bce068c040302cb99d7a26ef9ab76544773e9ba70f28d274d3`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfeeda5adbfaef226ee75380f0826468b0bd1f4ea5142c15218b6cc328c9c9a0`  
		Last Modified: Thu, 11 Jun 2020 19:32:15 GMT  
		Size: 10.3 MB (10305469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44be4c9292a75900438b83d5e272193b11245a6bf05518dd9a7974e323661cde`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20293274603f1fbe03122151a8bea57a755d636395aad8821ca8e9495705001e`  
		Last Modified: Thu, 11 Jun 2020 19:32:17 GMT  
		Size: 13.5 MB (13477832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab300e409b143028fcd83629578c9b6c98542c1d6032fec4aa0d2ccb1e2e051c`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb729c9479eb91824cf62c8c605c0d3ab455b2a38a9d64b711b103f5dd2c20f2`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 16.9 KB (16915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa934f9e31e268cdfaf8d2cdd9036048b51a7325574c92594af08119d1ad235`  
		Last Modified: Thu, 11 Jun 2020 21:15:33 GMT  
		Size: 33.9 MB (33941742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625468e67d86014210e23c5ea7ea3619855d89e3e0d1b63de045202112042458`  
		Last Modified: Thu, 11 Jun 2020 21:15:27 GMT  
		Size: 188.2 KB (188239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdc9bfb76124ce5c12fe3ac1c9fe249e610f30b8f793016e97ac64a463138f9`  
		Last Modified: Thu, 11 Jun 2020 21:15:27 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d6e69a305ada81492d8105ec332537f82df9649eeb8be810f27e679e57ce0e`  
		Last Modified: Thu, 11 Jun 2020 21:15:49 GMT  
		Size: 504.8 KB (504760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f56ca97f5cad0a316e00feef34f27d5f0fbc5be97eacaf1f80f534151cd2df6`  
		Last Modified: Thu, 11 Jun 2020 21:15:53 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8d445cf9a9d0d80134feba5f37a8ecadbf310d18ab2caaae74a689ff9fa3be`  
		Last Modified: Thu, 11 Jun 2020 21:15:48 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `composer:1.10`

```console
$ docker pull composer@sha256:68e9afcfe042a69a778ffccd2da55cf195dd5671ab14163b774f00d6da0f23c4
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

### `composer:1.10` - linux; amd64

```console
$ docker pull composer@sha256:6babbd3567845f5a1c6cf3a01143ddcb4abe587fd14e221e36accebf0e962e84
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63111308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433420023b60cdf98a661eab19b14714e5e1a7056ac73561a660d9727d80723c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:51:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:51:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:51:59 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:51:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:52:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:52:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:52:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:52:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:00:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:00:41 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:00:43 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:00:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:00:44 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 03:36:24 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 03:36:34 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 03:36:35 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 03:36:35 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 03:36:35 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 03:36:43 GMT
ENV COMPOSER_VERSION=1.10.7
# Fri, 12 Jun 2020 03:36:44 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 03:36:44 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 03:36:45 GMT
WORKDIR /app
# Fri, 12 Jun 2020 03:36:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 03:36:45 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358d6dbbdff5c10cbe23c608b7ff9c6d1dd13331dd7dc7644b727ca5ea8e742`  
		Last Modified: Thu, 11 Jun 2020 22:14:55 GMT  
		Size: 1.3 MB (1340817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232d962484c6b9a1caa33a12f1beed4cb20996085056b4fb1591a9fd1d8c89f`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1d3ac04d2af7a9f0eee25eccc72e586400051054ffb4aff7cdf2f4ebc993e8`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2fa029f21abccac9d1ce064bef95d56aad7de3e1079df260138622eaf8ab25`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 10.3 MB (10305445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e18722d91019f31ffd0d261959c5dd489f6d27361f221a669dbe9691a56ef9`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3659ffc4e0a4393e4597cf7a4210f863623e4e1cdf86ed3f06726aa0616108d9`  
		Last Modified: Thu, 11 Jun 2020 22:14:59 GMT  
		Size: 14.2 MB (14173631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1874d3f89152f2ab71121617a3cfdb60a30feccc88dc7806657e3b22f3ccd6`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2545369333e4aa084fbd5285c57af07bd75686c0976981a60df746089e02b75a`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 16.9 KB (16931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680b7fc10b4acd5dda859b161e18533921eb585502203fb8d90e392b990fc0ff`  
		Last Modified: Fri, 12 Jun 2020 03:37:08 GMT  
		Size: 33.8 MB (33777899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95843d9ed2bd562441ca7a2cc826205c5403bd8384507211f0d3854eb07153b8`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 189.3 KB (189338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab487c471b8cfbda88b1b5a5ea9b716442d9cae4c86413a3d3302d01f2c6b3b2`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c9a21ccbb41f0c9bc7e467ba8129c81c9c6ee9eb26efa9bf3a0ac6303da34a`  
		Last Modified: Fri, 12 Jun 2020 03:37:13 GMT  
		Size: 504.7 KB (504734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec30aea17efe54c81d4cacd55e4350577778932f8d4818b9a3ecc9706ee0e374`  
		Last Modified: Fri, 12 Jun 2020 03:37:13 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7959b1da3d37ece89d1d51098ea4a534e68b3d8311b39e6048287b4bba6250f2`  
		Last Modified: Fri, 12 Jun 2020 03:37:13 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10` - linux; arm variant v6

```console
$ docker pull composer@sha256:c99b3bde69d2f2fba1d4696ecb638d5e381c61fc1bef1be262c82eddfa17dc5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59515232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67b7073d9fbf550b58fd228a151b966b6325d38adb1c720bd8750545a3f10191`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:14:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:14:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:14:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:14:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:14:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:14:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:14:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:14:59 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:15:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:15:01 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:16:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:16:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:19:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:19:59 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:20:02 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:20:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:20:03 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 21:53:58 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 21:54:20 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 21:54:22 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 21:54:23 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 21:54:24 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 21:54:40 GMT
ENV COMPOSER_VERSION=1.10.7
# Thu, 11 Jun 2020 21:54:43 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 21:54:43 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 21:54:44 GMT
WORKDIR /app
# Thu, 11 Jun 2020 21:54:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 21:54:46 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72788d65e292354c2ce4b67441d334d0ba534db5ce71d5b8bf78011a256b566f`  
		Last Modified: Thu, 11 Jun 2020 19:29:37 GMT  
		Size: 1.3 MB (1310273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e32d62de43da999aca07cf15fdbe1cd6b03aebc88c15409c3463daadf13e01`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6701e05673b745147608cd1b6eb47a3fbc35bcfd8a65bc536e5b9f919b3d0e77`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23d338eb9977c3cc4f53684a30948f5defb783b30f97eb45447ad19c586495f`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 10.3 MB (10305474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f01a53caea7c04e7254412060a5c0cb23ff8364d565eab3d98fc0ec804c65b3`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784e930730f995fd22b8a9bdf378b989b6551ae36873db347c0d23370b99e831`  
		Last Modified: Thu, 11 Jun 2020 19:29:39 GMT  
		Size: 13.2 MB (13195114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdcd1019ed44b57cb67d664f43d95a56a032f8fbf5028ce6347443731418cb3`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f541954f527d04cef7111fa78ef9238624e7d52750cc75f73c9e0ec0d8add297`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 16.9 KB (16925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8df574460aaa4735f4c219fb58bd7ce6c6103c39e707bbd3fefdb7fda3eb15`  
		Last Modified: Thu, 11 Jun 2020 21:55:24 GMT  
		Size: 31.4 MB (31389293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d207a4c841e9986a8109779fe3f72f8a73a699ba6327cac1c3532c88c637374c`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 185.0 KB (185016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb807a0037a4bb2eea81b88d9d6bb855cd6ff3c4bb8d095679d2a08e8fd9785a`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628d2c181171c88661a79e5befe13fc7f464d8aa498dff82d835fd304f42840e`  
		Last Modified: Thu, 11 Jun 2020 21:55:33 GMT  
		Size: 504.8 KB (504761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5d325d1c74d1ed9f95a81872af98adebe1e0fcff9fa7c6cb883500dd03582e`  
		Last Modified: Thu, 11 Jun 2020 21:55:33 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19054a7d036b408c8c42f34c49a8ca70ce737a6f76c5f803d0fb8956091a4177`  
		Last Modified: Thu, 11 Jun 2020 21:55:33 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10` - linux; arm variant v7

```console
$ docker pull composer@sha256:b94ca5b5a25604233671a05014b89dfb56c3fe64f1f8200b6e71c913a2624b5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56821735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ae8665451ee2a2d4f3849bd08ad0178750f08c57ad44afeef533d24f078947b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:34:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:35:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:35:07 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:35:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:35:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:35:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:35:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:35:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:35:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:35:18 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:35:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:35:20 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:35:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:35:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:38:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:38:31 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:38:34 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:38:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:38:35 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 22:42:55 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 22:43:12 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 22:43:14 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 22:43:15 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 22:43:16 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 22:43:30 GMT
ENV COMPOSER_VERSION=1.10.7
# Thu, 11 Jun 2020 22:43:32 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 22:43:33 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 22:43:33 GMT
WORKDIR /app
# Thu, 11 Jun 2020 22:43:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 22:43:35 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5b4230297ea0028dae43acf7e134a55e11ebc15c53a61a2c0c72935dd0ed35`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.2 MB (1214376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779feafcddcba2692e3d187a609b90060e7deea16e8b629aada3a236e99c40f7`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b20c0367792ccffce00af872fa2ea0300330509fb8c15fe5c08905d7db739`  
		Last Modified: Thu, 11 Jun 2020 20:13:03 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9023ca7c2ffcb34f4e075e8f6d5001276142a28b4e0d398fa3eaddc67c4aec`  
		Last Modified: Thu, 11 Jun 2020 20:13:03 GMT  
		Size: 10.3 MB (10305461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e1f3f19383952fefc6527fb475db9a4cde57b21c9a9cb19135732e7b34d85c`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5e59fcc062532624a3a9dd675e189b78e7bce3a5b6c09ce99339dc5b014570`  
		Last Modified: Thu, 11 Jun 2020 20:13:06 GMT  
		Size: 12.4 MB (12350663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a6f7844ad0b4881ed895ba72be400c6782597448fa61bcaa58dd4fe0853836`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354514b31215294fcf1092b43467ddd5587ce6a1fefd1bd4b809cfafbfee18f7`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 16.9 KB (16913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2c7c46ccf6b4c6e523cc448dd15f5f05a0d06483d502b3b0fb72846dab717e`  
		Last Modified: Thu, 11 Jun 2020 22:44:10 GMT  
		Size: 29.8 MB (29839022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267aadf40444bd4f9132644aa6f6c0119543ca29a863cd01bfcaf3be7623cb6f`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 178.7 KB (178699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6871daa35ee6d1b5e329afbb68bf23ef665e526c054959b57f6dc1d858fa9da5`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1aac479723ca5c8c2a89d1610187c4148329bc22defdbc2a444dfc2b4cfabfd`  
		Last Modified: Thu, 11 Jun 2020 22:44:18 GMT  
		Size: 504.8 KB (504761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb738297c43fa116285317f4c78f4addf3a15382c0fd326dd4d29377ffc79d7`  
		Last Modified: Thu, 11 Jun 2020 22:44:18 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a4f6e9edfac9965af157620024a2e64e623cbad6dad720e2d44702b42327cc`  
		Last Modified: Thu, 11 Jun 2020 22:44:18 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:6c2943d8c54f865e3bbe6ea5d8968709106e67b9fbb0a79557af6286ff9e6986
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63191302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3bf68b97259926db2b63907b7b6ad33c3cb23398c5218c7e5a6cb042c608cc3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:40:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:40:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:40:31 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:40:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:40:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:40:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:40:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:40:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:40:37 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:40:38 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:40:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:40:39 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:40:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:40:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:44:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:44:41 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:44:44 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:44:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:44:46 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 22:57:10 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 22:57:28 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 22:57:30 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 22:57:31 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 22:57:31 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 22:57:45 GMT
ENV COMPOSER_VERSION=1.10.7
# Thu, 11 Jun 2020 22:57:48 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 22:57:49 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 22:57:49 GMT
WORKDIR /app
# Thu, 11 Jun 2020 22:57:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 22:57:50 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee09877319de284b8141c396485111447d75eb8cf26c68819f92f85a4de5649`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 MB (1342990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bad472a11fde1c83808bc84cc9c77da0743b9974bb8c51ab25ed0608cbb4558`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fca52dcdf28b691bbc24b2e2aff931667b865a9188287ef18af016712d3a0f`  
		Last Modified: Thu, 11 Jun 2020 20:30:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f7c9da4678b86166cb9b705a8b9505c19a0d1c24d47bb4360a5907dd28cf28`  
		Last Modified: Thu, 11 Jun 2020 20:30:04 GMT  
		Size: 10.3 MB (10305482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2aa0aa4a6988ac388d32698edfeecb7d0a24539556a4d33bc3327e5786ff0f`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39a6dec5d173eac97dd81097371b07b48982a0ab697e8ab09a40c6d4c319682`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 14.0 MB (13981145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d87e7b6f85188674dafd79fa2e34a45d6f197e8ce1ae71e2337c2534efca59`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f45b14b8adc9219dfa9399abfc7b1b753ca63bfb9a4109e4fd1c0da5caa1a0`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 16.9 KB (16938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88423514539f3ed88c3d723a4f15d7276e95e4c9f4d6c0d3864cd61e0ac8c81c`  
		Last Modified: Thu, 11 Jun 2020 22:58:31 GMT  
		Size: 34.1 MB (34138877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49e25f227bb97b88fe0ffc96fef316f6b53e7c48ef10c14f5399a7441b4ffec`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 188.1 KB (188066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3213d0d563d4eb6ff14649f7b487f46d48ae07fa7768b9ab975db0300aeb8e06`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867f1875f74e994124013a455523af4fa2ea1c18a20c999912dfef70cddf49e5`  
		Last Modified: Thu, 11 Jun 2020 22:58:39 GMT  
		Size: 504.8 KB (504760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a710d37874225c8cc6da9516d38717d9c53945a7c7eaf00c56c8764f8e532fc0`  
		Last Modified: Thu, 11 Jun 2020 22:58:39 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093b2977f90dfa6bf7e6c2dbd081d7c421ec1b69da9adf6b4d19ebe49dac79a7`  
		Last Modified: Thu, 11 Jun 2020 22:58:39 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10` - linux; 386

```console
$ docker pull composer@sha256:ca47ae35321e8e6f4572cb65f085ca1fbf08aa60d7a993ef8f314dbfc7ed12f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65188090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8034411c9bc77c35903f70e193a48739892a5ce4a31fa9f860c9205e856f6023`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:53:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:53:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:53:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:53:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:53:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:53:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:53:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:53:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:53:09 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:53:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:53:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:02:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:02:55 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:02:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:02:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:02:58 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 01:52:49 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 01:53:04 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 01:53:06 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 01:53:06 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 01:53:06 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 01:53:15 GMT
ENV COMPOSER_VERSION=1.10.7
# Fri, 12 Jun 2020 01:53:17 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 01:53:17 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 01:53:18 GMT
WORKDIR /app
# Fri, 12 Jun 2020 01:53:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 01:53:18 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380f9ca051d120d4ed72890904488f0f1e0fd0128cbd1c73adbff366e90bc2aa`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 1.4 MB (1439837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613b9419908bb5beb7365d9d340ee3071aebf8c7919f5379a7b99221fd74c78f`  
		Last Modified: Thu, 11 Jun 2020 22:28:36 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd1bd9f7e9212850ee7c4017e1d3e5ec33176a9113258688a743d871983ee8c`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055c67327ee726dcb5b4e69ca5490023191476ac33eb72e84aea00f6b00c68b7`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 10.3 MB (10305449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6b7ea2ee885f0ae987d58de97f74bb931344e2477eefb48f3d04a90751f764`  
		Last Modified: Thu, 11 Jun 2020 22:28:35 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030cdee16954ea64da3800cd137349eb9b23064bd73168050596c83095da383b`  
		Last Modified: Thu, 11 Jun 2020 22:28:40 GMT  
		Size: 14.6 MB (14564562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629202fa404c086a430dd7d7127e65b92265559980c347f282d4654381da41e8`  
		Last Modified: Thu, 11 Jun 2020 22:28:36 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9694db72218b1872d389aeb90cdae79a16b53f9dfdb334584badf8e808da9f`  
		Last Modified: Thu, 11 Jun 2020 22:28:35 GMT  
		Size: 16.9 KB (16939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4c0dbf20b6de48fdd627e0694147fc21e53c04431f7ebaaa94ec13ef6cae44`  
		Last Modified: Fri, 12 Jun 2020 01:53:45 GMT  
		Size: 35.4 MB (35355633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee96b64f9c4459a8444513a26888081669e737e3fc6eb2f028360b416b333b`  
		Last Modified: Fri, 12 Jun 2020 01:53:34 GMT  
		Size: 203.7 KB (203658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dde06329df568103704291e0b472e532ef23a2f00eadc9484c14ea9feebb8d8`  
		Last Modified: Fri, 12 Jun 2020 01:53:34 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a073f20a79e2063002071c18660e75c258c07c5cb94393ae82b4e7d51f7592b5`  
		Last Modified: Fri, 12 Jun 2020 01:53:51 GMT  
		Size: 504.7 KB (504739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872a29d49579bed85016977d1eb236f48a987c5d6cf992eb143af868d8ac2745`  
		Last Modified: Fri, 12 Jun 2020 01:53:51 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf2c57a63fa1e8a513188c0a237354c461502dbc26a5d6dda0aaa5218c816d8`  
		Last Modified: Fri, 12 Jun 2020 01:53:51 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10` - linux; ppc64le

```console
$ docker pull composer@sha256:e155573df8700733bd8bf1dce305e67622e262c4c75016d1d826624f312d75cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65449609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e574aedfcde654f9cc674ae6915ab8bc375b98c5a1b9c091e9ff77f1a4c72c58`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:45:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:45:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:45:29 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:45:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:45:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:45:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:45:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:45:52 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:45:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:45:59 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:46:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:46:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:50:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:50:07 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:50:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:50:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:50:19 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 01:52:57 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 01:53:15 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 01:53:22 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 01:53:24 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 01:53:29 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 01:54:02 GMT
ENV COMPOSER_VERSION=1.10.7
# Fri, 12 Jun 2020 01:54:10 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 01:54:11 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 01:54:15 GMT
WORKDIR /app
# Fri, 12 Jun 2020 01:54:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 01:54:19 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f98eb9049c4fcbaa1cf16ddb44aaf910a89a5471dc303198251fa25bc2a1ef`  
		Last Modified: Thu, 11 Jun 2020 20:57:07 GMT  
		Size: 1.4 MB (1383311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50cdb8e03fc1b19217cd9f80b86142d090ad3e818795b339ea4d9ef9b74555f`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4466e085b12b265fb47397c7c105fd7d78a5883beef49ab9f386393c4c3dae`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbb7594d19c6129fb268c14b9b61a062eb1509b9ee23d2d3c51e55d344b4022`  
		Last Modified: Thu, 11 Jun 2020 20:57:04 GMT  
		Size: 10.3 MB (10305491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfca2ae2dd0fa2baeaf870eb6d850ca046d8dede8bc7bd8e550139f315f0e8a1`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24693054c4d20048d5a8af6f339778f20546c2d519895fd146ed031ab08c95e8`  
		Last Modified: Thu, 11 Jun 2020 20:57:08 GMT  
		Size: 15.1 MB (15144559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91fc688a4963e2db4e23b0cf85f076b3ef08ad8cf636e48f8f6cf76f75b204`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79384080ee3a4da85e7fcf036c35abd4a72aba47f46157e5517a72aa76a2f043`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 17.0 KB (16975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9007b0e243a5a526f41b3c6df897e6cadd789dafa9075a0f6a76edf844e79dbc`  
		Last Modified: Fri, 12 Jun 2020 01:55:05 GMT  
		Size: 35.1 MB (35088531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee306131aed824d74ee7b9cd56c45cb38c0cbbf6f31360accf7310163e16e83`  
		Last Modified: Fri, 12 Jun 2020 01:54:54 GMT  
		Size: 195.7 KB (195699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e185de3b1f08c6feeb3143dac639b8e90538320cac4f19a62842f977cc1459aa`  
		Last Modified: Fri, 12 Jun 2020 01:54:54 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e9e5aadfb14bce92b646f2cc5d9e1bb48a418845cb2c5e422a6b650195444d`  
		Last Modified: Fri, 12 Jun 2020 01:55:19 GMT  
		Size: 504.8 KB (504763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3faa7594d67fbd17a8895393beeb7559f054737949d92803b2e4e52d32ea3add`  
		Last Modified: Fri, 12 Jun 2020 01:55:18 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3029d423df91b54e0ba93e32720d02228f7f5f055f6227a76d70200ee21fa7`  
		Last Modified: Fri, 12 Jun 2020 01:55:18 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10` - linux; s390x

```console
$ docker pull composer@sha256:a638d6ac9c98be9851cac68f86066ed9399324cf29b2bfe534074223796862fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62388970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf8b15a368579abfd95087125c06a1b3ce2c5b49728f3fe79b30417fc49716f5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:29:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:29:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:29:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:29:39 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:29:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:29:40 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:29:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:29:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:32:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:32:06 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:32:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:32:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:32:07 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 21:14:48 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 21:14:59 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 21:15:00 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 21:15:00 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 21:15:00 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 21:15:08 GMT
ENV COMPOSER_VERSION=1.10.7
# Thu, 11 Jun 2020 21:15:09 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 21:15:09 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 21:15:10 GMT
WORKDIR /app
# Thu, 11 Jun 2020 21:15:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 21:15:10 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057c8475c8b5e21c245ff682a57adf8970d16ccbed87694b3ec200c83e17a8fb`  
		Last Modified: Thu, 11 Jun 2020 19:32:19 GMT  
		Size: 1.4 MB (1382745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2bbd1ef5644a3638bc6f073de941463cbfceb435ea6d11ce3c7fdb9f8d2539`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b73c5118a1a42bce068c040302cb99d7a26ef9ab76544773e9ba70f28d274d3`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfeeda5adbfaef226ee75380f0826468b0bd1f4ea5142c15218b6cc328c9c9a0`  
		Last Modified: Thu, 11 Jun 2020 19:32:15 GMT  
		Size: 10.3 MB (10305469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44be4c9292a75900438b83d5e272193b11245a6bf05518dd9a7974e323661cde`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20293274603f1fbe03122151a8bea57a755d636395aad8821ca8e9495705001e`  
		Last Modified: Thu, 11 Jun 2020 19:32:17 GMT  
		Size: 13.5 MB (13477832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab300e409b143028fcd83629578c9b6c98542c1d6032fec4aa0d2ccb1e2e051c`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb729c9479eb91824cf62c8c605c0d3ab455b2a38a9d64b711b103f5dd2c20f2`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 16.9 KB (16915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa934f9e31e268cdfaf8d2cdd9036048b51a7325574c92594af08119d1ad235`  
		Last Modified: Thu, 11 Jun 2020 21:15:33 GMT  
		Size: 33.9 MB (33941742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625468e67d86014210e23c5ea7ea3619855d89e3e0d1b63de045202112042458`  
		Last Modified: Thu, 11 Jun 2020 21:15:27 GMT  
		Size: 188.2 KB (188239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdc9bfb76124ce5c12fe3ac1c9fe249e610f30b8f793016e97ac64a463138f9`  
		Last Modified: Thu, 11 Jun 2020 21:15:27 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d6e69a305ada81492d8105ec332537f82df9649eeb8be810f27e679e57ce0e`  
		Last Modified: Thu, 11 Jun 2020 21:15:49 GMT  
		Size: 504.8 KB (504760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f56ca97f5cad0a316e00feef34f27d5f0fbc5be97eacaf1f80f534151cd2df6`  
		Last Modified: Thu, 11 Jun 2020 21:15:53 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8d445cf9a9d0d80134feba5f37a8ecadbf310d18ab2caaae74a689ff9fa3be`  
		Last Modified: Thu, 11 Jun 2020 21:15:48 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `composer:1.10.8`

**does not exist** (yet?)

## `composer:1.9`

```console
$ docker pull composer@sha256:27797ba529bde1deaa37043ded4978c939b30a2932f07a243c1591665b15e90a
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

### `composer:1.9` - linux; amd64

```console
$ docker pull composer@sha256:a32f2600758aa5e183ec75c2943800b9957ab74be63695d66bbdbba51dbb8b95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63103963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5dd4118e662cb31c859294da2fd942fa0a26a86d3a79e3a444983d77d401c2c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:51:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:51:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:51:59 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:51:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:52:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:52:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:52:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:52:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:00:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:00:41 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:00:43 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:00:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:00:44 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 03:36:24 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 03:36:34 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 03:36:35 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 03:36:35 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 03:36:35 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 03:36:49 GMT
ENV COMPOSER_VERSION=1.9.3
# Fri, 12 Jun 2020 03:36:50 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 03:36:50 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 03:36:51 GMT
WORKDIR /app
# Fri, 12 Jun 2020 03:36:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 03:36:51 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358d6dbbdff5c10cbe23c608b7ff9c6d1dd13331dd7dc7644b727ca5ea8e742`  
		Last Modified: Thu, 11 Jun 2020 22:14:55 GMT  
		Size: 1.3 MB (1340817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232d962484c6b9a1caa33a12f1beed4cb20996085056b4fb1591a9fd1d8c89f`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1d3ac04d2af7a9f0eee25eccc72e586400051054ffb4aff7cdf2f4ebc993e8`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2fa029f21abccac9d1ce064bef95d56aad7de3e1079df260138622eaf8ab25`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 10.3 MB (10305445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e18722d91019f31ffd0d261959c5dd489f6d27361f221a669dbe9691a56ef9`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3659ffc4e0a4393e4597cf7a4210f863623e4e1cdf86ed3f06726aa0616108d9`  
		Last Modified: Thu, 11 Jun 2020 22:14:59 GMT  
		Size: 14.2 MB (14173631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1874d3f89152f2ab71121617a3cfdb60a30feccc88dc7806657e3b22f3ccd6`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2545369333e4aa084fbd5285c57af07bd75686c0976981a60df746089e02b75a`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 16.9 KB (16931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680b7fc10b4acd5dda859b161e18533921eb585502203fb8d90e392b990fc0ff`  
		Last Modified: Fri, 12 Jun 2020 03:37:08 GMT  
		Size: 33.8 MB (33777899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95843d9ed2bd562441ca7a2cc826205c5403bd8384507211f0d3854eb07153b8`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 189.3 KB (189338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab487c471b8cfbda88b1b5a5ea9b716442d9cae4c86413a3d3302d01f2c6b3b2`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeaf4d46828ed20efa236f583ae15ec914a6ff03ca10132b91cedd9c1cc8847c`  
		Last Modified: Fri, 12 Jun 2020 03:37:19 GMT  
		Size: 497.4 KB (497387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f085f33fc10a3aa8e16831a6ba625edb0d203137653776f227d71a4d0107dd7f`  
		Last Modified: Fri, 12 Jun 2020 03:37:19 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb683f9cc423f9febcce5927901451e7a741ce606e3a1905b84d46d602caae1`  
		Last Modified: Fri, 12 Jun 2020 03:37:19 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.9` - linux; arm variant v6

```console
$ docker pull composer@sha256:3c1973fcfbb83ed7d854ea49ecfc58794e4c7b243fd25817a0260a2100a6fc66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59507886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57af769535bb8a622a630ff4693c4feb1b3a536d1bcc6df1a19e6177f7d672a5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:14:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:14:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:14:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:14:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:14:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:14:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:14:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:14:59 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:15:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:15:01 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:16:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:16:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:19:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:19:59 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:20:02 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:20:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:20:03 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 21:53:58 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 21:54:20 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 21:54:22 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 21:54:23 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 21:54:24 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 21:54:52 GMT
ENV COMPOSER_VERSION=1.9.3
# Thu, 11 Jun 2020 21:54:55 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 21:54:55 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 21:54:56 GMT
WORKDIR /app
# Thu, 11 Jun 2020 21:54:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 21:54:58 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72788d65e292354c2ce4b67441d334d0ba534db5ce71d5b8bf78011a256b566f`  
		Last Modified: Thu, 11 Jun 2020 19:29:37 GMT  
		Size: 1.3 MB (1310273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e32d62de43da999aca07cf15fdbe1cd6b03aebc88c15409c3463daadf13e01`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6701e05673b745147608cd1b6eb47a3fbc35bcfd8a65bc536e5b9f919b3d0e77`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23d338eb9977c3cc4f53684a30948f5defb783b30f97eb45447ad19c586495f`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 10.3 MB (10305474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f01a53caea7c04e7254412060a5c0cb23ff8364d565eab3d98fc0ec804c65b3`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784e930730f995fd22b8a9bdf378b989b6551ae36873db347c0d23370b99e831`  
		Last Modified: Thu, 11 Jun 2020 19:29:39 GMT  
		Size: 13.2 MB (13195114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdcd1019ed44b57cb67d664f43d95a56a032f8fbf5028ce6347443731418cb3`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f541954f527d04cef7111fa78ef9238624e7d52750cc75f73c9e0ec0d8add297`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 16.9 KB (16925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8df574460aaa4735f4c219fb58bd7ce6c6103c39e707bbd3fefdb7fda3eb15`  
		Last Modified: Thu, 11 Jun 2020 21:55:24 GMT  
		Size: 31.4 MB (31389293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d207a4c841e9986a8109779fe3f72f8a73a699ba6327cac1c3532c88c637374c`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 185.0 KB (185016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb807a0037a4bb2eea81b88d9d6bb855cd6ff3c4bb8d095679d2a08e8fd9785a`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1280d607edd8e80a14a02839c518cdac3e6adb2f4afc128be80bf4a4473b3f`  
		Last Modified: Thu, 11 Jun 2020 21:55:42 GMT  
		Size: 497.4 KB (497415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c6e36a419ab7126e696b467d11a7f60a7f76709aa921674168da7e064c7728`  
		Last Modified: Thu, 11 Jun 2020 21:55:41 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb59abd6ad91d95b5eb2d2f3b16731c0de61704d2d821c2fe313cf4ebef323c`  
		Last Modified: Thu, 11 Jun 2020 21:55:41 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.9` - linux; arm variant v7

```console
$ docker pull composer@sha256:e0f7949cc8ae3da709d085b51905816da1c63ea45f434739cc2eead84fe7e339
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56814390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00408071befc152320a08bb5cdd9dcb402a3c976445b8c6f7e5802bd177e9109`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:34:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:35:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:35:07 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:35:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:35:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:35:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:35:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:35:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:35:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:35:18 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:35:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:35:20 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:35:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:35:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:38:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:38:31 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:38:34 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:38:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:38:35 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 22:42:55 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 22:43:12 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 22:43:14 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 22:43:15 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 22:43:16 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 22:43:41 GMT
ENV COMPOSER_VERSION=1.9.3
# Thu, 11 Jun 2020 22:43:43 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 22:43:44 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 22:43:45 GMT
WORKDIR /app
# Thu, 11 Jun 2020 22:43:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 22:43:46 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5b4230297ea0028dae43acf7e134a55e11ebc15c53a61a2c0c72935dd0ed35`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.2 MB (1214376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779feafcddcba2692e3d187a609b90060e7deea16e8b629aada3a236e99c40f7`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b20c0367792ccffce00af872fa2ea0300330509fb8c15fe5c08905d7db739`  
		Last Modified: Thu, 11 Jun 2020 20:13:03 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9023ca7c2ffcb34f4e075e8f6d5001276142a28b4e0d398fa3eaddc67c4aec`  
		Last Modified: Thu, 11 Jun 2020 20:13:03 GMT  
		Size: 10.3 MB (10305461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e1f3f19383952fefc6527fb475db9a4cde57b21c9a9cb19135732e7b34d85c`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5e59fcc062532624a3a9dd675e189b78e7bce3a5b6c09ce99339dc5b014570`  
		Last Modified: Thu, 11 Jun 2020 20:13:06 GMT  
		Size: 12.4 MB (12350663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a6f7844ad0b4881ed895ba72be400c6782597448fa61bcaa58dd4fe0853836`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354514b31215294fcf1092b43467ddd5587ce6a1fefd1bd4b809cfafbfee18f7`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 16.9 KB (16913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2c7c46ccf6b4c6e523cc448dd15f5f05a0d06483d502b3b0fb72846dab717e`  
		Last Modified: Thu, 11 Jun 2020 22:44:10 GMT  
		Size: 29.8 MB (29839022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267aadf40444bd4f9132644aa6f6c0119543ca29a863cd01bfcaf3be7623cb6f`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 178.7 KB (178699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6871daa35ee6d1b5e329afbb68bf23ef665e526c054959b57f6dc1d858fa9da5`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e54386f4644a57592b31051461907b17b8084a77f38d3f77ce02175110acac`  
		Last Modified: Thu, 11 Jun 2020 22:44:26 GMT  
		Size: 497.4 KB (497415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ffdf412d8d39424e6c8915fa13b9bf7f451e806549b4dd2e2bab028c160d9`  
		Last Modified: Thu, 11 Jun 2020 22:44:26 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc10d46cbf361714c9df7cc583b27e708ad410ee72bd564ebbab695559a6a18`  
		Last Modified: Thu, 11 Jun 2020 22:44:26 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.9` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:7c433a8d2d5f393cd906d88d064823c44f0f923951b704eb4ddeae9818e43ad9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63183963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd6697c5cfbbb8f7881d6f54f65102f492c61f5b995917aeb0712118f8351bea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:40:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:40:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:40:31 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:40:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:40:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:40:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:40:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:40:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:40:37 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:40:38 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:40:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:40:39 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:40:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:40:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:44:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:44:41 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:44:44 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:44:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:44:46 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 22:57:10 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 22:57:28 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 22:57:30 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 22:57:31 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 22:57:31 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 22:57:57 GMT
ENV COMPOSER_VERSION=1.9.3
# Thu, 11 Jun 2020 22:58:00 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 22:58:00 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 22:58:02 GMT
WORKDIR /app
# Thu, 11 Jun 2020 22:58:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 22:58:06 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee09877319de284b8141c396485111447d75eb8cf26c68819f92f85a4de5649`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 MB (1342990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bad472a11fde1c83808bc84cc9c77da0743b9974bb8c51ab25ed0608cbb4558`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fca52dcdf28b691bbc24b2e2aff931667b865a9188287ef18af016712d3a0f`  
		Last Modified: Thu, 11 Jun 2020 20:30:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f7c9da4678b86166cb9b705a8b9505c19a0d1c24d47bb4360a5907dd28cf28`  
		Last Modified: Thu, 11 Jun 2020 20:30:04 GMT  
		Size: 10.3 MB (10305482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2aa0aa4a6988ac388d32698edfeecb7d0a24539556a4d33bc3327e5786ff0f`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39a6dec5d173eac97dd81097371b07b48982a0ab697e8ab09a40c6d4c319682`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 14.0 MB (13981145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d87e7b6f85188674dafd79fa2e34a45d6f197e8ce1ae71e2337c2534efca59`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f45b14b8adc9219dfa9399abfc7b1b753ca63bfb9a4109e4fd1c0da5caa1a0`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 16.9 KB (16938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88423514539f3ed88c3d723a4f15d7276e95e4c9f4d6c0d3864cd61e0ac8c81c`  
		Last Modified: Thu, 11 Jun 2020 22:58:31 GMT  
		Size: 34.1 MB (34138877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49e25f227bb97b88fe0ffc96fef316f6b53e7c48ef10c14f5399a7441b4ffec`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 188.1 KB (188066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3213d0d563d4eb6ff14649f7b487f46d48ae07fa7768b9ab975db0300aeb8e06`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9768c908bd5898f62ac4dd779c73894ddb7312b4e45972bee70068373b03ae`  
		Last Modified: Thu, 11 Jun 2020 22:58:47 GMT  
		Size: 497.4 KB (497420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d7f2cb706b08579c7adbbfca539000f236af2139c3db5e60816341200d5893`  
		Last Modified: Thu, 11 Jun 2020 22:58:48 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eee9f73a22e3032cabdf508918581a6b61f2a7c19710cdce056b3bef9306722`  
		Last Modified: Thu, 11 Jun 2020 22:58:47 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.9` - linux; 386

```console
$ docker pull composer@sha256:1e449a637863ba0e3c506ee01928b5ee5018532e1a501c54ebeb9c1e82e81adb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65180740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f3395a3815c7186932e25e01edbcd4eed4aa88280a330675eda9772c54e0c7e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:53:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:53:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:53:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:53:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:53:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:53:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:53:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:53:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:53:09 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:53:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:53:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:02:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:02:55 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:02:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:02:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:02:58 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 01:52:49 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 01:53:04 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 01:53:06 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 01:53:06 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 01:53:06 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 01:53:22 GMT
ENV COMPOSER_VERSION=1.9.3
# Fri, 12 Jun 2020 01:53:24 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 01:53:24 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 01:53:24 GMT
WORKDIR /app
# Fri, 12 Jun 2020 01:53:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 01:53:24 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380f9ca051d120d4ed72890904488f0f1e0fd0128cbd1c73adbff366e90bc2aa`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 1.4 MB (1439837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613b9419908bb5beb7365d9d340ee3071aebf8c7919f5379a7b99221fd74c78f`  
		Last Modified: Thu, 11 Jun 2020 22:28:36 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd1bd9f7e9212850ee7c4017e1d3e5ec33176a9113258688a743d871983ee8c`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055c67327ee726dcb5b4e69ca5490023191476ac33eb72e84aea00f6b00c68b7`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 10.3 MB (10305449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6b7ea2ee885f0ae987d58de97f74bb931344e2477eefb48f3d04a90751f764`  
		Last Modified: Thu, 11 Jun 2020 22:28:35 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030cdee16954ea64da3800cd137349eb9b23064bd73168050596c83095da383b`  
		Last Modified: Thu, 11 Jun 2020 22:28:40 GMT  
		Size: 14.6 MB (14564562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629202fa404c086a430dd7d7127e65b92265559980c347f282d4654381da41e8`  
		Last Modified: Thu, 11 Jun 2020 22:28:36 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9694db72218b1872d389aeb90cdae79a16b53f9dfdb334584badf8e808da9f`  
		Last Modified: Thu, 11 Jun 2020 22:28:35 GMT  
		Size: 16.9 KB (16939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4c0dbf20b6de48fdd627e0694147fc21e53c04431f7ebaaa94ec13ef6cae44`  
		Last Modified: Fri, 12 Jun 2020 01:53:45 GMT  
		Size: 35.4 MB (35355633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee96b64f9c4459a8444513a26888081669e737e3fc6eb2f028360b416b333b`  
		Last Modified: Fri, 12 Jun 2020 01:53:34 GMT  
		Size: 203.7 KB (203658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dde06329df568103704291e0b472e532ef23a2f00eadc9484c14ea9feebb8d8`  
		Last Modified: Fri, 12 Jun 2020 01:53:34 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc88f68775ade2ac7073c4fc9694e6736d6c28b837873e0c9a903a04b2ff7c87`  
		Last Modified: Fri, 12 Jun 2020 01:53:56 GMT  
		Size: 497.4 KB (497389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b5d872a7e0407450ebc5d327e0c1ac3cbc8c9d7aca5e95ff618297e912077c`  
		Last Modified: Fri, 12 Jun 2020 01:53:56 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797da76b3e10a6a1df8eb650b0634c5493e538bdc0510e21242d970d5ae82965`  
		Last Modified: Fri, 12 Jun 2020 01:53:56 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.9` - linux; ppc64le

```console
$ docker pull composer@sha256:da3d7aea9e4b7d94826973b6e15c4487d75434666cbe1be10b0807f209382ebb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65442266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17df82de18d14f06ac6fb866b506298020d6fee99da847866559f73031a3c991`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:45:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:45:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:45:29 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:45:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:45:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:45:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:45:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:45:52 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:45:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:45:59 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:46:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:46:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:50:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:50:07 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:50:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:50:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:50:19 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 01:52:57 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 01:53:15 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 01:53:22 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 01:53:24 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 01:53:29 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 01:54:24 GMT
ENV COMPOSER_VERSION=1.9.3
# Fri, 12 Jun 2020 01:54:31 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 01:54:33 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 01:54:36 GMT
WORKDIR /app
# Fri, 12 Jun 2020 01:54:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 01:54:41 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f98eb9049c4fcbaa1cf16ddb44aaf910a89a5471dc303198251fa25bc2a1ef`  
		Last Modified: Thu, 11 Jun 2020 20:57:07 GMT  
		Size: 1.4 MB (1383311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50cdb8e03fc1b19217cd9f80b86142d090ad3e818795b339ea4d9ef9b74555f`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4466e085b12b265fb47397c7c105fd7d78a5883beef49ab9f386393c4c3dae`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbb7594d19c6129fb268c14b9b61a062eb1509b9ee23d2d3c51e55d344b4022`  
		Last Modified: Thu, 11 Jun 2020 20:57:04 GMT  
		Size: 10.3 MB (10305491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfca2ae2dd0fa2baeaf870eb6d850ca046d8dede8bc7bd8e550139f315f0e8a1`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24693054c4d20048d5a8af6f339778f20546c2d519895fd146ed031ab08c95e8`  
		Last Modified: Thu, 11 Jun 2020 20:57:08 GMT  
		Size: 15.1 MB (15144559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91fc688a4963e2db4e23b0cf85f076b3ef08ad8cf636e48f8f6cf76f75b204`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79384080ee3a4da85e7fcf036c35abd4a72aba47f46157e5517a72aa76a2f043`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 17.0 KB (16975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9007b0e243a5a526f41b3c6df897e6cadd789dafa9075a0f6a76edf844e79dbc`  
		Last Modified: Fri, 12 Jun 2020 01:55:05 GMT  
		Size: 35.1 MB (35088531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee306131aed824d74ee7b9cd56c45cb38c0cbbf6f31360accf7310163e16e83`  
		Last Modified: Fri, 12 Jun 2020 01:54:54 GMT  
		Size: 195.7 KB (195699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e185de3b1f08c6feeb3143dac639b8e90538320cac4f19a62842f977cc1459aa`  
		Last Modified: Fri, 12 Jun 2020 01:54:54 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9929bf79eaa0ee5dbc430e13187d07300bb22bd2aea68d0bb6c186bc381e9dab`  
		Last Modified: Fri, 12 Jun 2020 01:55:35 GMT  
		Size: 497.4 KB (497419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492a148822497fc329c80d470f0d769aadb3204710993dd8edd2b4540e32fd55`  
		Last Modified: Fri, 12 Jun 2020 01:55:34 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68a4568fa6208a81c3d1dd0ca72b2781511b6c801685b4ec635f78e9098fabe`  
		Last Modified: Fri, 12 Jun 2020 01:55:34 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.9` - linux; s390x

```console
$ docker pull composer@sha256:85b34f732cbfdb44b0609f3f13f164521483a137a98027bba4ccf868789e5524
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62381624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c76525108c4286cf57775662980ae47841e94c9d7a7c906ed9b7f0c48f3445`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:29:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:29:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:29:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:29:39 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:29:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:29:40 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:29:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:29:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:32:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:32:06 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:32:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:32:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:32:07 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 21:14:48 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 21:14:59 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 21:15:00 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 21:15:00 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 21:15:00 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 21:15:15 GMT
ENV COMPOSER_VERSION=1.9.3
# Thu, 11 Jun 2020 21:15:16 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 21:15:17 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 21:15:17 GMT
WORKDIR /app
# Thu, 11 Jun 2020 21:15:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 21:15:17 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057c8475c8b5e21c245ff682a57adf8970d16ccbed87694b3ec200c83e17a8fb`  
		Last Modified: Thu, 11 Jun 2020 19:32:19 GMT  
		Size: 1.4 MB (1382745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2bbd1ef5644a3638bc6f073de941463cbfceb435ea6d11ce3c7fdb9f8d2539`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b73c5118a1a42bce068c040302cb99d7a26ef9ab76544773e9ba70f28d274d3`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfeeda5adbfaef226ee75380f0826468b0bd1f4ea5142c15218b6cc328c9c9a0`  
		Last Modified: Thu, 11 Jun 2020 19:32:15 GMT  
		Size: 10.3 MB (10305469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44be4c9292a75900438b83d5e272193b11245a6bf05518dd9a7974e323661cde`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20293274603f1fbe03122151a8bea57a755d636395aad8821ca8e9495705001e`  
		Last Modified: Thu, 11 Jun 2020 19:32:17 GMT  
		Size: 13.5 MB (13477832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab300e409b143028fcd83629578c9b6c98542c1d6032fec4aa0d2ccb1e2e051c`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb729c9479eb91824cf62c8c605c0d3ab455b2a38a9d64b711b103f5dd2c20f2`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 16.9 KB (16915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa934f9e31e268cdfaf8d2cdd9036048b51a7325574c92594af08119d1ad235`  
		Last Modified: Thu, 11 Jun 2020 21:15:33 GMT  
		Size: 33.9 MB (33941742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625468e67d86014210e23c5ea7ea3619855d89e3e0d1b63de045202112042458`  
		Last Modified: Thu, 11 Jun 2020 21:15:27 GMT  
		Size: 188.2 KB (188239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdc9bfb76124ce5c12fe3ac1c9fe249e610f30b8f793016e97ac64a463138f9`  
		Last Modified: Thu, 11 Jun 2020 21:15:27 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cfe0801f1d5cc57895f2a97dd2dde51296cb3101783315d0016f91417abdb8d`  
		Last Modified: Thu, 11 Jun 2020 21:16:01 GMT  
		Size: 497.4 KB (497414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcd501c915246325ce0a26fd9d77d35658e51ebf723aa4186b726013dd9a1ae`  
		Last Modified: Thu, 11 Jun 2020 21:16:06 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8538568c632698969065102fa8a60b5b87da8c3e80104f32528a8ced27527a41`  
		Last Modified: Thu, 11 Jun 2020 21:16:16 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `composer:1.9.3`

```console
$ docker pull composer@sha256:27797ba529bde1deaa37043ded4978c939b30a2932f07a243c1591665b15e90a
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

### `composer:1.9.3` - linux; amd64

```console
$ docker pull composer@sha256:a32f2600758aa5e183ec75c2943800b9957ab74be63695d66bbdbba51dbb8b95
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63103963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e5dd4118e662cb31c859294da2fd942fa0a26a86d3a79e3a444983d77d401c2c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:51:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:51:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:51:59 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:51:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:52:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:52:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:52:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:52:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:00:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:00:41 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:00:43 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:00:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:00:44 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 03:36:24 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 03:36:34 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 03:36:35 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 03:36:35 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 03:36:35 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 03:36:49 GMT
ENV COMPOSER_VERSION=1.9.3
# Fri, 12 Jun 2020 03:36:50 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 03:36:50 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 03:36:51 GMT
WORKDIR /app
# Fri, 12 Jun 2020 03:36:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 03:36:51 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358d6dbbdff5c10cbe23c608b7ff9c6d1dd13331dd7dc7644b727ca5ea8e742`  
		Last Modified: Thu, 11 Jun 2020 22:14:55 GMT  
		Size: 1.3 MB (1340817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232d962484c6b9a1caa33a12f1beed4cb20996085056b4fb1591a9fd1d8c89f`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1d3ac04d2af7a9f0eee25eccc72e586400051054ffb4aff7cdf2f4ebc993e8`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2fa029f21abccac9d1ce064bef95d56aad7de3e1079df260138622eaf8ab25`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 10.3 MB (10305445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e18722d91019f31ffd0d261959c5dd489f6d27361f221a669dbe9691a56ef9`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3659ffc4e0a4393e4597cf7a4210f863623e4e1cdf86ed3f06726aa0616108d9`  
		Last Modified: Thu, 11 Jun 2020 22:14:59 GMT  
		Size: 14.2 MB (14173631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1874d3f89152f2ab71121617a3cfdb60a30feccc88dc7806657e3b22f3ccd6`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2545369333e4aa084fbd5285c57af07bd75686c0976981a60df746089e02b75a`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 16.9 KB (16931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680b7fc10b4acd5dda859b161e18533921eb585502203fb8d90e392b990fc0ff`  
		Last Modified: Fri, 12 Jun 2020 03:37:08 GMT  
		Size: 33.8 MB (33777899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95843d9ed2bd562441ca7a2cc826205c5403bd8384507211f0d3854eb07153b8`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 189.3 KB (189338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab487c471b8cfbda88b1b5a5ea9b716442d9cae4c86413a3d3302d01f2c6b3b2`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeaf4d46828ed20efa236f583ae15ec914a6ff03ca10132b91cedd9c1cc8847c`  
		Last Modified: Fri, 12 Jun 2020 03:37:19 GMT  
		Size: 497.4 KB (497387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f085f33fc10a3aa8e16831a6ba625edb0d203137653776f227d71a4d0107dd7f`  
		Last Modified: Fri, 12 Jun 2020 03:37:19 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb683f9cc423f9febcce5927901451e7a741ce606e3a1905b84d46d602caae1`  
		Last Modified: Fri, 12 Jun 2020 03:37:19 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.9.3` - linux; arm variant v6

```console
$ docker pull composer@sha256:3c1973fcfbb83ed7d854ea49ecfc58794e4c7b243fd25817a0260a2100a6fc66
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59507886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57af769535bb8a622a630ff4693c4feb1b3a536d1bcc6df1a19e6177f7d672a5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:14:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:14:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:14:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:14:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:14:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:14:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:14:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:14:59 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:15:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:15:01 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:16:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:16:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:19:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:19:59 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:20:02 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:20:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:20:03 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 21:53:58 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 21:54:20 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 21:54:22 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 21:54:23 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 21:54:24 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 21:54:52 GMT
ENV COMPOSER_VERSION=1.9.3
# Thu, 11 Jun 2020 21:54:55 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 21:54:55 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 21:54:56 GMT
WORKDIR /app
# Thu, 11 Jun 2020 21:54:57 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 21:54:58 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72788d65e292354c2ce4b67441d334d0ba534db5ce71d5b8bf78011a256b566f`  
		Last Modified: Thu, 11 Jun 2020 19:29:37 GMT  
		Size: 1.3 MB (1310273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e32d62de43da999aca07cf15fdbe1cd6b03aebc88c15409c3463daadf13e01`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6701e05673b745147608cd1b6eb47a3fbc35bcfd8a65bc536e5b9f919b3d0e77`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23d338eb9977c3cc4f53684a30948f5defb783b30f97eb45447ad19c586495f`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 10.3 MB (10305474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f01a53caea7c04e7254412060a5c0cb23ff8364d565eab3d98fc0ec804c65b3`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784e930730f995fd22b8a9bdf378b989b6551ae36873db347c0d23370b99e831`  
		Last Modified: Thu, 11 Jun 2020 19:29:39 GMT  
		Size: 13.2 MB (13195114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdcd1019ed44b57cb67d664f43d95a56a032f8fbf5028ce6347443731418cb3`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f541954f527d04cef7111fa78ef9238624e7d52750cc75f73c9e0ec0d8add297`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 16.9 KB (16925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8df574460aaa4735f4c219fb58bd7ce6c6103c39e707bbd3fefdb7fda3eb15`  
		Last Modified: Thu, 11 Jun 2020 21:55:24 GMT  
		Size: 31.4 MB (31389293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d207a4c841e9986a8109779fe3f72f8a73a699ba6327cac1c3532c88c637374c`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 185.0 KB (185016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb807a0037a4bb2eea81b88d9d6bb855cd6ff3c4bb8d095679d2a08e8fd9785a`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e1280d607edd8e80a14a02839c518cdac3e6adb2f4afc128be80bf4a4473b3f`  
		Last Modified: Thu, 11 Jun 2020 21:55:42 GMT  
		Size: 497.4 KB (497415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c6e36a419ab7126e696b467d11a7f60a7f76709aa921674168da7e064c7728`  
		Last Modified: Thu, 11 Jun 2020 21:55:41 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbb59abd6ad91d95b5eb2d2f3b16731c0de61704d2d821c2fe313cf4ebef323c`  
		Last Modified: Thu, 11 Jun 2020 21:55:41 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.9.3` - linux; arm variant v7

```console
$ docker pull composer@sha256:e0f7949cc8ae3da709d085b51905816da1c63ea45f434739cc2eead84fe7e339
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56814390 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00408071befc152320a08bb5cdd9dcb402a3c976445b8c6f7e5802bd177e9109`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:34:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:35:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:35:07 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:35:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:35:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:35:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:35:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:35:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:35:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:35:18 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:35:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:35:20 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:35:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:35:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:38:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:38:31 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:38:34 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:38:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:38:35 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 22:42:55 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 22:43:12 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 22:43:14 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 22:43:15 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 22:43:16 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 22:43:41 GMT
ENV COMPOSER_VERSION=1.9.3
# Thu, 11 Jun 2020 22:43:43 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 22:43:44 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 22:43:45 GMT
WORKDIR /app
# Thu, 11 Jun 2020 22:43:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 22:43:46 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5b4230297ea0028dae43acf7e134a55e11ebc15c53a61a2c0c72935dd0ed35`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.2 MB (1214376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779feafcddcba2692e3d187a609b90060e7deea16e8b629aada3a236e99c40f7`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b20c0367792ccffce00af872fa2ea0300330509fb8c15fe5c08905d7db739`  
		Last Modified: Thu, 11 Jun 2020 20:13:03 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9023ca7c2ffcb34f4e075e8f6d5001276142a28b4e0d398fa3eaddc67c4aec`  
		Last Modified: Thu, 11 Jun 2020 20:13:03 GMT  
		Size: 10.3 MB (10305461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e1f3f19383952fefc6527fb475db9a4cde57b21c9a9cb19135732e7b34d85c`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5e59fcc062532624a3a9dd675e189b78e7bce3a5b6c09ce99339dc5b014570`  
		Last Modified: Thu, 11 Jun 2020 20:13:06 GMT  
		Size: 12.4 MB (12350663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a6f7844ad0b4881ed895ba72be400c6782597448fa61bcaa58dd4fe0853836`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354514b31215294fcf1092b43467ddd5587ce6a1fefd1bd4b809cfafbfee18f7`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 16.9 KB (16913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2c7c46ccf6b4c6e523cc448dd15f5f05a0d06483d502b3b0fb72846dab717e`  
		Last Modified: Thu, 11 Jun 2020 22:44:10 GMT  
		Size: 29.8 MB (29839022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267aadf40444bd4f9132644aa6f6c0119543ca29a863cd01bfcaf3be7623cb6f`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 178.7 KB (178699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6871daa35ee6d1b5e329afbb68bf23ef665e526c054959b57f6dc1d858fa9da5`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92e54386f4644a57592b31051461907b17b8084a77f38d3f77ce02175110acac`  
		Last Modified: Thu, 11 Jun 2020 22:44:26 GMT  
		Size: 497.4 KB (497415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:617ffdf412d8d39424e6c8915fa13b9bf7f451e806549b4dd2e2bab028c160d9`  
		Last Modified: Thu, 11 Jun 2020 22:44:26 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efc10d46cbf361714c9df7cc583b27e708ad410ee72bd564ebbab695559a6a18`  
		Last Modified: Thu, 11 Jun 2020 22:44:26 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.9.3` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:7c433a8d2d5f393cd906d88d064823c44f0f923951b704eb4ddeae9818e43ad9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63183963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd6697c5cfbbb8f7881d6f54f65102f492c61f5b995917aeb0712118f8351bea`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:40:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:40:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:40:31 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:40:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:40:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:40:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:40:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:40:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:40:37 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:40:38 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:40:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:40:39 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:40:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:40:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:44:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:44:41 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:44:44 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:44:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:44:46 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 22:57:10 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 22:57:28 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 22:57:30 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 22:57:31 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 22:57:31 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 22:57:57 GMT
ENV COMPOSER_VERSION=1.9.3
# Thu, 11 Jun 2020 22:58:00 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 22:58:00 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 22:58:02 GMT
WORKDIR /app
# Thu, 11 Jun 2020 22:58:04 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 22:58:06 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee09877319de284b8141c396485111447d75eb8cf26c68819f92f85a4de5649`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 MB (1342990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bad472a11fde1c83808bc84cc9c77da0743b9974bb8c51ab25ed0608cbb4558`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fca52dcdf28b691bbc24b2e2aff931667b865a9188287ef18af016712d3a0f`  
		Last Modified: Thu, 11 Jun 2020 20:30:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f7c9da4678b86166cb9b705a8b9505c19a0d1c24d47bb4360a5907dd28cf28`  
		Last Modified: Thu, 11 Jun 2020 20:30:04 GMT  
		Size: 10.3 MB (10305482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2aa0aa4a6988ac388d32698edfeecb7d0a24539556a4d33bc3327e5786ff0f`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39a6dec5d173eac97dd81097371b07b48982a0ab697e8ab09a40c6d4c319682`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 14.0 MB (13981145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d87e7b6f85188674dafd79fa2e34a45d6f197e8ce1ae71e2337c2534efca59`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f45b14b8adc9219dfa9399abfc7b1b753ca63bfb9a4109e4fd1c0da5caa1a0`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 16.9 KB (16938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88423514539f3ed88c3d723a4f15d7276e95e4c9f4d6c0d3864cd61e0ac8c81c`  
		Last Modified: Thu, 11 Jun 2020 22:58:31 GMT  
		Size: 34.1 MB (34138877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49e25f227bb97b88fe0ffc96fef316f6b53e7c48ef10c14f5399a7441b4ffec`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 188.1 KB (188066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3213d0d563d4eb6ff14649f7b487f46d48ae07fa7768b9ab975db0300aeb8e06`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae9768c908bd5898f62ac4dd779c73894ddb7312b4e45972bee70068373b03ae`  
		Last Modified: Thu, 11 Jun 2020 22:58:47 GMT  
		Size: 497.4 KB (497420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d7f2cb706b08579c7adbbfca539000f236af2139c3db5e60816341200d5893`  
		Last Modified: Thu, 11 Jun 2020 22:58:48 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2eee9f73a22e3032cabdf508918581a6b61f2a7c19710cdce056b3bef9306722`  
		Last Modified: Thu, 11 Jun 2020 22:58:47 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.9.3` - linux; 386

```console
$ docker pull composer@sha256:1e449a637863ba0e3c506ee01928b5ee5018532e1a501c54ebeb9c1e82e81adb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65180740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f3395a3815c7186932e25e01edbcd4eed4aa88280a330675eda9772c54e0c7e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:53:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:53:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:53:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:53:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:53:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:53:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:53:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:53:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:53:09 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:53:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:53:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:02:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:02:55 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:02:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:02:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:02:58 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 01:52:49 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 01:53:04 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 01:53:06 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 01:53:06 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 01:53:06 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 01:53:22 GMT
ENV COMPOSER_VERSION=1.9.3
# Fri, 12 Jun 2020 01:53:24 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 01:53:24 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 01:53:24 GMT
WORKDIR /app
# Fri, 12 Jun 2020 01:53:24 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 01:53:24 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380f9ca051d120d4ed72890904488f0f1e0fd0128cbd1c73adbff366e90bc2aa`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 1.4 MB (1439837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613b9419908bb5beb7365d9d340ee3071aebf8c7919f5379a7b99221fd74c78f`  
		Last Modified: Thu, 11 Jun 2020 22:28:36 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd1bd9f7e9212850ee7c4017e1d3e5ec33176a9113258688a743d871983ee8c`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055c67327ee726dcb5b4e69ca5490023191476ac33eb72e84aea00f6b00c68b7`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 10.3 MB (10305449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6b7ea2ee885f0ae987d58de97f74bb931344e2477eefb48f3d04a90751f764`  
		Last Modified: Thu, 11 Jun 2020 22:28:35 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030cdee16954ea64da3800cd137349eb9b23064bd73168050596c83095da383b`  
		Last Modified: Thu, 11 Jun 2020 22:28:40 GMT  
		Size: 14.6 MB (14564562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629202fa404c086a430dd7d7127e65b92265559980c347f282d4654381da41e8`  
		Last Modified: Thu, 11 Jun 2020 22:28:36 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9694db72218b1872d389aeb90cdae79a16b53f9dfdb334584badf8e808da9f`  
		Last Modified: Thu, 11 Jun 2020 22:28:35 GMT  
		Size: 16.9 KB (16939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4c0dbf20b6de48fdd627e0694147fc21e53c04431f7ebaaa94ec13ef6cae44`  
		Last Modified: Fri, 12 Jun 2020 01:53:45 GMT  
		Size: 35.4 MB (35355633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee96b64f9c4459a8444513a26888081669e737e3fc6eb2f028360b416b333b`  
		Last Modified: Fri, 12 Jun 2020 01:53:34 GMT  
		Size: 203.7 KB (203658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dde06329df568103704291e0b472e532ef23a2f00eadc9484c14ea9feebb8d8`  
		Last Modified: Fri, 12 Jun 2020 01:53:34 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc88f68775ade2ac7073c4fc9694e6736d6c28b837873e0c9a903a04b2ff7c87`  
		Last Modified: Fri, 12 Jun 2020 01:53:56 GMT  
		Size: 497.4 KB (497389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81b5d872a7e0407450ebc5d327e0c1ac3cbc8c9d7aca5e95ff618297e912077c`  
		Last Modified: Fri, 12 Jun 2020 01:53:56 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:797da76b3e10a6a1df8eb650b0634c5493e538bdc0510e21242d970d5ae82965`  
		Last Modified: Fri, 12 Jun 2020 01:53:56 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.9.3` - linux; ppc64le

```console
$ docker pull composer@sha256:da3d7aea9e4b7d94826973b6e15c4487d75434666cbe1be10b0807f209382ebb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65442266 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17df82de18d14f06ac6fb866b506298020d6fee99da847866559f73031a3c991`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:45:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:45:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:45:29 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:45:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:45:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:45:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:45:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:45:52 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:45:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:45:59 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:46:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:46:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:50:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:50:07 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:50:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:50:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:50:19 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 01:52:57 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 01:53:15 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 01:53:22 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 01:53:24 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 01:53:29 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 01:54:24 GMT
ENV COMPOSER_VERSION=1.9.3
# Fri, 12 Jun 2020 01:54:31 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 01:54:33 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 01:54:36 GMT
WORKDIR /app
# Fri, 12 Jun 2020 01:54:39 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 01:54:41 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f98eb9049c4fcbaa1cf16ddb44aaf910a89a5471dc303198251fa25bc2a1ef`  
		Last Modified: Thu, 11 Jun 2020 20:57:07 GMT  
		Size: 1.4 MB (1383311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50cdb8e03fc1b19217cd9f80b86142d090ad3e818795b339ea4d9ef9b74555f`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4466e085b12b265fb47397c7c105fd7d78a5883beef49ab9f386393c4c3dae`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbb7594d19c6129fb268c14b9b61a062eb1509b9ee23d2d3c51e55d344b4022`  
		Last Modified: Thu, 11 Jun 2020 20:57:04 GMT  
		Size: 10.3 MB (10305491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfca2ae2dd0fa2baeaf870eb6d850ca046d8dede8bc7bd8e550139f315f0e8a1`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24693054c4d20048d5a8af6f339778f20546c2d519895fd146ed031ab08c95e8`  
		Last Modified: Thu, 11 Jun 2020 20:57:08 GMT  
		Size: 15.1 MB (15144559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91fc688a4963e2db4e23b0cf85f076b3ef08ad8cf636e48f8f6cf76f75b204`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79384080ee3a4da85e7fcf036c35abd4a72aba47f46157e5517a72aa76a2f043`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 17.0 KB (16975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9007b0e243a5a526f41b3c6df897e6cadd789dafa9075a0f6a76edf844e79dbc`  
		Last Modified: Fri, 12 Jun 2020 01:55:05 GMT  
		Size: 35.1 MB (35088531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee306131aed824d74ee7b9cd56c45cb38c0cbbf6f31360accf7310163e16e83`  
		Last Modified: Fri, 12 Jun 2020 01:54:54 GMT  
		Size: 195.7 KB (195699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e185de3b1f08c6feeb3143dac639b8e90538320cac4f19a62842f977cc1459aa`  
		Last Modified: Fri, 12 Jun 2020 01:54:54 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9929bf79eaa0ee5dbc430e13187d07300bb22bd2aea68d0bb6c186bc381e9dab`  
		Last Modified: Fri, 12 Jun 2020 01:55:35 GMT  
		Size: 497.4 KB (497419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:492a148822497fc329c80d470f0d769aadb3204710993dd8edd2b4540e32fd55`  
		Last Modified: Fri, 12 Jun 2020 01:55:34 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c68a4568fa6208a81c3d1dd0ca72b2781511b6c801685b4ec635f78e9098fabe`  
		Last Modified: Fri, 12 Jun 2020 01:55:34 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.9.3` - linux; s390x

```console
$ docker pull composer@sha256:85b34f732cbfdb44b0609f3f13f164521483a137a98027bba4ccf868789e5524
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62381624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87c76525108c4286cf57775662980ae47841e94c9d7a7c906ed9b7f0c48f3445`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:29:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:29:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:29:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:29:39 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:29:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:29:40 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:29:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:29:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:32:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:32:06 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:32:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:32:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:32:07 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 21:14:48 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 21:14:59 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 21:15:00 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 21:15:00 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 21:15:00 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 21:15:15 GMT
ENV COMPOSER_VERSION=1.9.3
# Thu, 11 Jun 2020 21:15:16 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 21:15:17 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 21:15:17 GMT
WORKDIR /app
# Thu, 11 Jun 2020 21:15:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 21:15:17 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057c8475c8b5e21c245ff682a57adf8970d16ccbed87694b3ec200c83e17a8fb`  
		Last Modified: Thu, 11 Jun 2020 19:32:19 GMT  
		Size: 1.4 MB (1382745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2bbd1ef5644a3638bc6f073de941463cbfceb435ea6d11ce3c7fdb9f8d2539`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b73c5118a1a42bce068c040302cb99d7a26ef9ab76544773e9ba70f28d274d3`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfeeda5adbfaef226ee75380f0826468b0bd1f4ea5142c15218b6cc328c9c9a0`  
		Last Modified: Thu, 11 Jun 2020 19:32:15 GMT  
		Size: 10.3 MB (10305469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44be4c9292a75900438b83d5e272193b11245a6bf05518dd9a7974e323661cde`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20293274603f1fbe03122151a8bea57a755d636395aad8821ca8e9495705001e`  
		Last Modified: Thu, 11 Jun 2020 19:32:17 GMT  
		Size: 13.5 MB (13477832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab300e409b143028fcd83629578c9b6c98542c1d6032fec4aa0d2ccb1e2e051c`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb729c9479eb91824cf62c8c605c0d3ab455b2a38a9d64b711b103f5dd2c20f2`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 16.9 KB (16915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa934f9e31e268cdfaf8d2cdd9036048b51a7325574c92594af08119d1ad235`  
		Last Modified: Thu, 11 Jun 2020 21:15:33 GMT  
		Size: 33.9 MB (33941742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625468e67d86014210e23c5ea7ea3619855d89e3e0d1b63de045202112042458`  
		Last Modified: Thu, 11 Jun 2020 21:15:27 GMT  
		Size: 188.2 KB (188239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdc9bfb76124ce5c12fe3ac1c9fe249e610f30b8f793016e97ac64a463138f9`  
		Last Modified: Thu, 11 Jun 2020 21:15:27 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cfe0801f1d5cc57895f2a97dd2dde51296cb3101783315d0016f91417abdb8d`  
		Last Modified: Thu, 11 Jun 2020 21:16:01 GMT  
		Size: 497.4 KB (497414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bcd501c915246325ce0a26fd9d77d35658e51ebf723aa4186b726013dd9a1ae`  
		Last Modified: Thu, 11 Jun 2020 21:16:06 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8538568c632698969065102fa8a60b5b87da8c3e80104f32528a8ced27527a41`  
		Last Modified: Thu, 11 Jun 2020 21:16:16 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `composer:2`

```console
$ docker pull composer@sha256:da70d020cf2f2434af48004656ac5972eef6a364fd4f4d61844c64dc9677ca3a
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

### `composer:2` - linux; amd64

```console
$ docker pull composer@sha256:3657116bfe53d797acf316f3184cd826cbc9088f15aa6ec053f5e98d8a6c0361
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63135947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd13398d47d6b2e07de39c131c14508600729f151b0e5a9edfdb510518fce841`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:51:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:51:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:51:59 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:51:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:52:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:52:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:52:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:52:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:00:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:00:41 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:00:43 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:00:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:00:44 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 03:36:24 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 03:36:34 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 03:36:35 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 03:36:35 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 03:36:35 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 03:36:36 GMT
ENV COMPOSER_VERSION=2.0.0-alpha1
# Fri, 12 Jun 2020 03:36:37 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 03:36:37 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 03:36:38 GMT
WORKDIR /app
# Fri, 12 Jun 2020 03:36:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 03:36:38 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358d6dbbdff5c10cbe23c608b7ff9c6d1dd13331dd7dc7644b727ca5ea8e742`  
		Last Modified: Thu, 11 Jun 2020 22:14:55 GMT  
		Size: 1.3 MB (1340817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232d962484c6b9a1caa33a12f1beed4cb20996085056b4fb1591a9fd1d8c89f`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1d3ac04d2af7a9f0eee25eccc72e586400051054ffb4aff7cdf2f4ebc993e8`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2fa029f21abccac9d1ce064bef95d56aad7de3e1079df260138622eaf8ab25`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 10.3 MB (10305445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e18722d91019f31ffd0d261959c5dd489f6d27361f221a669dbe9691a56ef9`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3659ffc4e0a4393e4597cf7a4210f863623e4e1cdf86ed3f06726aa0616108d9`  
		Last Modified: Thu, 11 Jun 2020 22:14:59 GMT  
		Size: 14.2 MB (14173631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1874d3f89152f2ab71121617a3cfdb60a30feccc88dc7806657e3b22f3ccd6`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2545369333e4aa084fbd5285c57af07bd75686c0976981a60df746089e02b75a`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 16.9 KB (16931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680b7fc10b4acd5dda859b161e18533921eb585502203fb8d90e392b990fc0ff`  
		Last Modified: Fri, 12 Jun 2020 03:37:08 GMT  
		Size: 33.8 MB (33777899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95843d9ed2bd562441ca7a2cc826205c5403bd8384507211f0d3854eb07153b8`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 189.3 KB (189338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab487c471b8cfbda88b1b5a5ea9b716442d9cae4c86413a3d3302d01f2c6b3b2`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ee5ea0f15ee900a335e5589287be41936859a3ca691f63f2635e7ffc9f4291`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 529.4 KB (529373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4dc01fdf0009e85d27fb10fa3a5f414922f01a06f5dcaeba4b7564e6c6c922`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3302bba508780bbcd4b76d70f0bbcf59a823fff91fb356d9a7b84c6b001a7fe`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2` - linux; arm variant v6

```console
$ docker pull composer@sha256:c207db84af4dc9592179a78a8f3eace6e5b5301f05f780ca02e67bfe50e10a33
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59539880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d361bce8aea95297eb2aab6c7b43ef37ed844becf272358a26241180f908dc27`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:14:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:14:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:14:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:14:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:14:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:14:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:14:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:14:59 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:15:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:15:01 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:16:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:16:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:19:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:19:59 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:20:02 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:20:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:20:03 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 21:53:58 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 21:54:20 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 21:54:22 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 21:54:23 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 21:54:24 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 21:54:25 GMT
ENV COMPOSER_VERSION=2.0.0-alpha1
# Thu, 11 Jun 2020 21:54:28 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 21:54:29 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 21:54:30 GMT
WORKDIR /app
# Thu, 11 Jun 2020 21:54:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 21:54:31 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72788d65e292354c2ce4b67441d334d0ba534db5ce71d5b8bf78011a256b566f`  
		Last Modified: Thu, 11 Jun 2020 19:29:37 GMT  
		Size: 1.3 MB (1310273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e32d62de43da999aca07cf15fdbe1cd6b03aebc88c15409c3463daadf13e01`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6701e05673b745147608cd1b6eb47a3fbc35bcfd8a65bc536e5b9f919b3d0e77`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23d338eb9977c3cc4f53684a30948f5defb783b30f97eb45447ad19c586495f`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 10.3 MB (10305474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f01a53caea7c04e7254412060a5c0cb23ff8364d565eab3d98fc0ec804c65b3`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784e930730f995fd22b8a9bdf378b989b6551ae36873db347c0d23370b99e831`  
		Last Modified: Thu, 11 Jun 2020 19:29:39 GMT  
		Size: 13.2 MB (13195114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdcd1019ed44b57cb67d664f43d95a56a032f8fbf5028ce6347443731418cb3`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f541954f527d04cef7111fa78ef9238624e7d52750cc75f73c9e0ec0d8add297`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 16.9 KB (16925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8df574460aaa4735f4c219fb58bd7ce6c6103c39e707bbd3fefdb7fda3eb15`  
		Last Modified: Thu, 11 Jun 2020 21:55:24 GMT  
		Size: 31.4 MB (31389293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d207a4c841e9986a8109779fe3f72f8a73a699ba6327cac1c3532c88c637374c`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 185.0 KB (185016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb807a0037a4bb2eea81b88d9d6bb855cd6ff3c4bb8d095679d2a08e8fd9785a`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3838e2f4cafccf01c6fee22559d9d9e8a3db040ec54cfc8aa7c00bfc0107e15`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 529.4 KB (529410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462e92e05b974146a65c65f38024cb06dea4872dfc740b66cbd46f20446efe9c`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129d656e55526674b58a0c5e7dc84be5604fa0812e86de089c01bf892a4c6fae`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2` - linux; arm variant v7

```console
$ docker pull composer@sha256:ad6e4c739c756c9d4a50339ff243e48586bb81bb948d45400de700330d3b40d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56846383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1489d5f182e7810d051ca9dfba3e0b9ca08e08d35f7cb6e05bcbdfc5b4940d80`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:34:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:35:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:35:07 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:35:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:35:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:35:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:35:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:35:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:35:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:35:18 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:35:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:35:20 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:35:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:35:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:38:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:38:31 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:38:34 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:38:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:38:35 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 22:42:55 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 22:43:12 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 22:43:14 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 22:43:15 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 22:43:16 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 22:43:16 GMT
ENV COMPOSER_VERSION=2.0.0-alpha1
# Thu, 11 Jun 2020 22:43:19 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 22:43:19 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 22:43:20 GMT
WORKDIR /app
# Thu, 11 Jun 2020 22:43:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 22:43:22 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5b4230297ea0028dae43acf7e134a55e11ebc15c53a61a2c0c72935dd0ed35`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.2 MB (1214376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779feafcddcba2692e3d187a609b90060e7deea16e8b629aada3a236e99c40f7`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b20c0367792ccffce00af872fa2ea0300330509fb8c15fe5c08905d7db739`  
		Last Modified: Thu, 11 Jun 2020 20:13:03 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9023ca7c2ffcb34f4e075e8f6d5001276142a28b4e0d398fa3eaddc67c4aec`  
		Last Modified: Thu, 11 Jun 2020 20:13:03 GMT  
		Size: 10.3 MB (10305461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e1f3f19383952fefc6527fb475db9a4cde57b21c9a9cb19135732e7b34d85c`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5e59fcc062532624a3a9dd675e189b78e7bce3a5b6c09ce99339dc5b014570`  
		Last Modified: Thu, 11 Jun 2020 20:13:06 GMT  
		Size: 12.4 MB (12350663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a6f7844ad0b4881ed895ba72be400c6782597448fa61bcaa58dd4fe0853836`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354514b31215294fcf1092b43467ddd5587ce6a1fefd1bd4b809cfafbfee18f7`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 16.9 KB (16913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2c7c46ccf6b4c6e523cc448dd15f5f05a0d06483d502b3b0fb72846dab717e`  
		Last Modified: Thu, 11 Jun 2020 22:44:10 GMT  
		Size: 29.8 MB (29839022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267aadf40444bd4f9132644aa6f6c0119543ca29a863cd01bfcaf3be7623cb6f`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 178.7 KB (178699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6871daa35ee6d1b5e329afbb68bf23ef665e526c054959b57f6dc1d858fa9da5`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be16fcfd5362aee76b71dc123b9964109a10bc20c92d393dae9afb97e8dfd788`  
		Last Modified: Thu, 11 Jun 2020 22:43:59 GMT  
		Size: 529.4 KB (529407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c403575f2c0a52309de4977f71514d5b6daaae6c656246352b983a1f2e5b307f`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6bffff0f6c287c63425e0158b26f395db6cda35e35f46191e10fef1a791cf4`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:bf95cc2f6faba08800ce33f3b6dc091b92c84e60dcbafdefd95d84adc589d2a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63215956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e063d288a6bdf775ddf084508f4681c8d044afe018713605a0afae38071850b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:40:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:40:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:40:31 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:40:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:40:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:40:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:40:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:40:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:40:37 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:40:38 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:40:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:40:39 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:40:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:40:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:44:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:44:41 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:44:44 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:44:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:44:46 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 22:57:10 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 22:57:28 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 22:57:30 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 22:57:31 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 22:57:31 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 22:57:32 GMT
ENV COMPOSER_VERSION=2.0.0-alpha1
# Thu, 11 Jun 2020 22:57:35 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 22:57:35 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 22:57:36 GMT
WORKDIR /app
# Thu, 11 Jun 2020 22:57:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 22:57:37 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee09877319de284b8141c396485111447d75eb8cf26c68819f92f85a4de5649`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 MB (1342990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bad472a11fde1c83808bc84cc9c77da0743b9974bb8c51ab25ed0608cbb4558`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fca52dcdf28b691bbc24b2e2aff931667b865a9188287ef18af016712d3a0f`  
		Last Modified: Thu, 11 Jun 2020 20:30:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f7c9da4678b86166cb9b705a8b9505c19a0d1c24d47bb4360a5907dd28cf28`  
		Last Modified: Thu, 11 Jun 2020 20:30:04 GMT  
		Size: 10.3 MB (10305482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2aa0aa4a6988ac388d32698edfeecb7d0a24539556a4d33bc3327e5786ff0f`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39a6dec5d173eac97dd81097371b07b48982a0ab697e8ab09a40c6d4c319682`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 14.0 MB (13981145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d87e7b6f85188674dafd79fa2e34a45d6f197e8ce1ae71e2337c2534efca59`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f45b14b8adc9219dfa9399abfc7b1b753ca63bfb9a4109e4fd1c0da5caa1a0`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 16.9 KB (16938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88423514539f3ed88c3d723a4f15d7276e95e4c9f4d6c0d3864cd61e0ac8c81c`  
		Last Modified: Thu, 11 Jun 2020 22:58:31 GMT  
		Size: 34.1 MB (34138877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49e25f227bb97b88fe0ffc96fef316f6b53e7c48ef10c14f5399a7441b4ffec`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 188.1 KB (188066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3213d0d563d4eb6ff14649f7b487f46d48ae07fa7768b9ab975db0300aeb8e06`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee53b136300beaa8a9bb4032aad6effa57f9390832b94d0e9929a2679966e35a`  
		Last Modified: Thu, 11 Jun 2020 22:58:20 GMT  
		Size: 529.4 KB (529411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6443b7b0969b18ad433d42484a8b6b40dbd2f39edfde938ef389f5df3b56a0a1`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e384ac93dd3c4bb33efe851aa3067400a5a27edbf3303caec333d5b2e35d024`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2` - linux; 386

```console
$ docker pull composer@sha256:0a3d6a4737cbc6ef541b6a47b1da22cccb4d3b8e964667e22fddf6d99a2a2271
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65212738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a6f152bee8c132bff31b82a7dbb01f97bfd917bcd474f687a71ef849c304ebd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:53:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:53:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:53:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:53:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:53:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:53:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:53:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:53:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:53:09 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:53:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:53:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:02:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:02:55 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:02:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:02:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:02:58 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 01:52:49 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 01:53:04 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 01:53:06 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 01:53:06 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 01:53:06 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 01:53:06 GMT
ENV COMPOSER_VERSION=2.0.0-alpha1
# Fri, 12 Jun 2020 01:53:08 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 01:53:08 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 01:53:09 GMT
WORKDIR /app
# Fri, 12 Jun 2020 01:53:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 01:53:09 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380f9ca051d120d4ed72890904488f0f1e0fd0128cbd1c73adbff366e90bc2aa`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 1.4 MB (1439837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613b9419908bb5beb7365d9d340ee3071aebf8c7919f5379a7b99221fd74c78f`  
		Last Modified: Thu, 11 Jun 2020 22:28:36 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd1bd9f7e9212850ee7c4017e1d3e5ec33176a9113258688a743d871983ee8c`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055c67327ee726dcb5b4e69ca5490023191476ac33eb72e84aea00f6b00c68b7`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 10.3 MB (10305449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6b7ea2ee885f0ae987d58de97f74bb931344e2477eefb48f3d04a90751f764`  
		Last Modified: Thu, 11 Jun 2020 22:28:35 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030cdee16954ea64da3800cd137349eb9b23064bd73168050596c83095da383b`  
		Last Modified: Thu, 11 Jun 2020 22:28:40 GMT  
		Size: 14.6 MB (14564562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629202fa404c086a430dd7d7127e65b92265559980c347f282d4654381da41e8`  
		Last Modified: Thu, 11 Jun 2020 22:28:36 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9694db72218b1872d389aeb90cdae79a16b53f9dfdb334584badf8e808da9f`  
		Last Modified: Thu, 11 Jun 2020 22:28:35 GMT  
		Size: 16.9 KB (16939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4c0dbf20b6de48fdd627e0694147fc21e53c04431f7ebaaa94ec13ef6cae44`  
		Last Modified: Fri, 12 Jun 2020 01:53:45 GMT  
		Size: 35.4 MB (35355633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee96b64f9c4459a8444513a26888081669e737e3fc6eb2f028360b416b333b`  
		Last Modified: Fri, 12 Jun 2020 01:53:34 GMT  
		Size: 203.7 KB (203658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dde06329df568103704291e0b472e532ef23a2f00eadc9484c14ea9feebb8d8`  
		Last Modified: Fri, 12 Jun 2020 01:53:34 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973e661b3007d25ebf1996c4a564c5af978345f4e967ede4b4644566f922b0d6`  
		Last Modified: Fri, 12 Jun 2020 01:53:33 GMT  
		Size: 529.4 KB (529387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89c86766ee1c89a125e5e90b5b41f8140016f193982945f1489dbea16bcd840`  
		Last Modified: Fri, 12 Jun 2020 01:53:34 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44013a073fc009001cf9b6413765f77619d1cd818f0f0fa29af7deb134b8137b`  
		Last Modified: Fri, 12 Jun 2020 01:53:33 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2` - linux; ppc64le

```console
$ docker pull composer@sha256:fec312e300025e24c356c391352d5c3be326ec773471b1cd78d781586c247336
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.5 MB (65474252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:486b99edb8e67eb98cce32e22aa41b2a5a32fdeab660263c2c9debd19922a4e1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:45:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:45:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:45:29 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:45:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:45:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:45:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:45:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:45:52 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:45:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:45:59 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:46:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:46:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:50:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:50:07 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:50:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:50:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:50:19 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 01:52:57 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 01:53:15 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 01:53:22 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 01:53:24 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 01:53:29 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 01:53:32 GMT
ENV COMPOSER_VERSION=2.0.0-alpha1
# Fri, 12 Jun 2020 01:53:41 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 01:53:42 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 01:53:45 GMT
WORKDIR /app
# Fri, 12 Jun 2020 01:53:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 01:53:49 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f98eb9049c4fcbaa1cf16ddb44aaf910a89a5471dc303198251fa25bc2a1ef`  
		Last Modified: Thu, 11 Jun 2020 20:57:07 GMT  
		Size: 1.4 MB (1383311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50cdb8e03fc1b19217cd9f80b86142d090ad3e818795b339ea4d9ef9b74555f`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4466e085b12b265fb47397c7c105fd7d78a5883beef49ab9f386393c4c3dae`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbb7594d19c6129fb268c14b9b61a062eb1509b9ee23d2d3c51e55d344b4022`  
		Last Modified: Thu, 11 Jun 2020 20:57:04 GMT  
		Size: 10.3 MB (10305491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfca2ae2dd0fa2baeaf870eb6d850ca046d8dede8bc7bd8e550139f315f0e8a1`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24693054c4d20048d5a8af6f339778f20546c2d519895fd146ed031ab08c95e8`  
		Last Modified: Thu, 11 Jun 2020 20:57:08 GMT  
		Size: 15.1 MB (15144559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91fc688a4963e2db4e23b0cf85f076b3ef08ad8cf636e48f8f6cf76f75b204`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79384080ee3a4da85e7fcf036c35abd4a72aba47f46157e5517a72aa76a2f043`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 17.0 KB (16975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9007b0e243a5a526f41b3c6df897e6cadd789dafa9075a0f6a76edf844e79dbc`  
		Last Modified: Fri, 12 Jun 2020 01:55:05 GMT  
		Size: 35.1 MB (35088531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee306131aed824d74ee7b9cd56c45cb38c0cbbf6f31360accf7310163e16e83`  
		Last Modified: Fri, 12 Jun 2020 01:54:54 GMT  
		Size: 195.7 KB (195699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e185de3b1f08c6feeb3143dac639b8e90538320cac4f19a62842f977cc1459aa`  
		Last Modified: Fri, 12 Jun 2020 01:54:54 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87c7859acba14a10e08ac909806772cf7ecbece0b84531fb03475c97b910bc6`  
		Last Modified: Fri, 12 Jun 2020 01:54:55 GMT  
		Size: 529.4 KB (529406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36209a6e65503d5d917b4cdb10c6fb22668715f5f08967ca1ad194b78527b1e5`  
		Last Modified: Fri, 12 Jun 2020 01:54:54 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ed43153dfd0e77c96243f060e2e73ebb6a520d4736d61a47294c843d1e26dc`  
		Last Modified: Fri, 12 Jun 2020 01:54:55 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2` - linux; s390x

```console
$ docker pull composer@sha256:ce99e518d2dd9ad4770616140716477d4bc5632b59df03e637626401aaa95708
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62413618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82aa252a8d19e37a054b720b4cce550471c55e05e1b9eb5f1252f28a6dd83d8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:29:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:29:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:29:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:29:39 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:29:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:29:40 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:29:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:29:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:32:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:32:06 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:32:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:32:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:32:07 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 21:14:48 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 21:14:59 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 21:15:00 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 21:15:00 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 21:15:00 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 21:15:00 GMT
ENV COMPOSER_VERSION=2.0.0-alpha1
# Thu, 11 Jun 2020 21:15:02 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 21:15:02 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 21:15:02 GMT
WORKDIR /app
# Thu, 11 Jun 2020 21:15:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 21:15:02 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057c8475c8b5e21c245ff682a57adf8970d16ccbed87694b3ec200c83e17a8fb`  
		Last Modified: Thu, 11 Jun 2020 19:32:19 GMT  
		Size: 1.4 MB (1382745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2bbd1ef5644a3638bc6f073de941463cbfceb435ea6d11ce3c7fdb9f8d2539`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b73c5118a1a42bce068c040302cb99d7a26ef9ab76544773e9ba70f28d274d3`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfeeda5adbfaef226ee75380f0826468b0bd1f4ea5142c15218b6cc328c9c9a0`  
		Last Modified: Thu, 11 Jun 2020 19:32:15 GMT  
		Size: 10.3 MB (10305469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44be4c9292a75900438b83d5e272193b11245a6bf05518dd9a7974e323661cde`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20293274603f1fbe03122151a8bea57a755d636395aad8821ca8e9495705001e`  
		Last Modified: Thu, 11 Jun 2020 19:32:17 GMT  
		Size: 13.5 MB (13477832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab300e409b143028fcd83629578c9b6c98542c1d6032fec4aa0d2ccb1e2e051c`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb729c9479eb91824cf62c8c605c0d3ab455b2a38a9d64b711b103f5dd2c20f2`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 16.9 KB (16915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa934f9e31e268cdfaf8d2cdd9036048b51a7325574c92594af08119d1ad235`  
		Last Modified: Thu, 11 Jun 2020 21:15:33 GMT  
		Size: 33.9 MB (33941742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625468e67d86014210e23c5ea7ea3619855d89e3e0d1b63de045202112042458`  
		Last Modified: Thu, 11 Jun 2020 21:15:27 GMT  
		Size: 188.2 KB (188239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdc9bfb76124ce5c12fe3ac1c9fe249e610f30b8f793016e97ac64a463138f9`  
		Last Modified: Thu, 11 Jun 2020 21:15:27 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f42881c1a5a8a439c5797420022d3a2b9acc48a45cd081ef89aa7f465db132`  
		Last Modified: Thu, 11 Jun 2020 21:15:27 GMT  
		Size: 529.4 KB (529406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800710402d7e8e60725a9c1597e4b9e939f600b35ed41e5a19f6ebf6780df135`  
		Last Modified: Thu, 11 Jun 2020 21:15:42 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92016695d233f249b7054ff58d8ee3d2fc2359b00527b17065935911b4db1311`  
		Last Modified: Thu, 11 Jun 2020 21:15:42 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `composer:2.0`

```console
$ docker pull composer@sha256:da70d020cf2f2434af48004656ac5972eef6a364fd4f4d61844c64dc9677ca3a
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

### `composer:2.0` - linux; amd64

```console
$ docker pull composer@sha256:3657116bfe53d797acf316f3184cd826cbc9088f15aa6ec053f5e98d8a6c0361
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63135947 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd13398d47d6b2e07de39c131c14508600729f151b0e5a9edfdb510518fce841`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:51:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:51:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:51:59 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:51:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:52:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:52:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:52:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:52:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:00:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:00:41 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:00:43 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:00:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:00:44 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 03:36:24 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 03:36:34 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 03:36:35 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 03:36:35 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 03:36:35 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 03:36:36 GMT
ENV COMPOSER_VERSION=2.0.0-alpha1
# Fri, 12 Jun 2020 03:36:37 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 03:36:37 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 03:36:38 GMT
WORKDIR /app
# Fri, 12 Jun 2020 03:36:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 03:36:38 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358d6dbbdff5c10cbe23c608b7ff9c6d1dd13331dd7dc7644b727ca5ea8e742`  
		Last Modified: Thu, 11 Jun 2020 22:14:55 GMT  
		Size: 1.3 MB (1340817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232d962484c6b9a1caa33a12f1beed4cb20996085056b4fb1591a9fd1d8c89f`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1d3ac04d2af7a9f0eee25eccc72e586400051054ffb4aff7cdf2f4ebc993e8`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2fa029f21abccac9d1ce064bef95d56aad7de3e1079df260138622eaf8ab25`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 10.3 MB (10305445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e18722d91019f31ffd0d261959c5dd489f6d27361f221a669dbe9691a56ef9`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3659ffc4e0a4393e4597cf7a4210f863623e4e1cdf86ed3f06726aa0616108d9`  
		Last Modified: Thu, 11 Jun 2020 22:14:59 GMT  
		Size: 14.2 MB (14173631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1874d3f89152f2ab71121617a3cfdb60a30feccc88dc7806657e3b22f3ccd6`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2545369333e4aa084fbd5285c57af07bd75686c0976981a60df746089e02b75a`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 16.9 KB (16931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680b7fc10b4acd5dda859b161e18533921eb585502203fb8d90e392b990fc0ff`  
		Last Modified: Fri, 12 Jun 2020 03:37:08 GMT  
		Size: 33.8 MB (33777899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95843d9ed2bd562441ca7a2cc826205c5403bd8384507211f0d3854eb07153b8`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 189.3 KB (189338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab487c471b8cfbda88b1b5a5ea9b716442d9cae4c86413a3d3302d01f2c6b3b2`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ee5ea0f15ee900a335e5589287be41936859a3ca691f63f2635e7ffc9f4291`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 529.4 KB (529373 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4dc01fdf0009e85d27fb10fa3a5f414922f01a06f5dcaeba4b7564e6c6c922`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3302bba508780bbcd4b76d70f0bbcf59a823fff91fb356d9a7b84c6b001a7fe`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0` - linux; arm variant v6

```console
$ docker pull composer@sha256:c207db84af4dc9592179a78a8f3eace6e5b5301f05f780ca02e67bfe50e10a33
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59539880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d361bce8aea95297eb2aab6c7b43ef37ed844becf272358a26241180f908dc27`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:14:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:14:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:14:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:14:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:14:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:14:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:14:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:14:59 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:15:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:15:01 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:16:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:16:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:19:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:19:59 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:20:02 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:20:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:20:03 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 21:53:58 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 21:54:20 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 21:54:22 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 21:54:23 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 21:54:24 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 21:54:25 GMT
ENV COMPOSER_VERSION=2.0.0-alpha1
# Thu, 11 Jun 2020 21:54:28 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 21:54:29 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 21:54:30 GMT
WORKDIR /app
# Thu, 11 Jun 2020 21:54:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 21:54:31 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72788d65e292354c2ce4b67441d334d0ba534db5ce71d5b8bf78011a256b566f`  
		Last Modified: Thu, 11 Jun 2020 19:29:37 GMT  
		Size: 1.3 MB (1310273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e32d62de43da999aca07cf15fdbe1cd6b03aebc88c15409c3463daadf13e01`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6701e05673b745147608cd1b6eb47a3fbc35bcfd8a65bc536e5b9f919b3d0e77`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23d338eb9977c3cc4f53684a30948f5defb783b30f97eb45447ad19c586495f`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 10.3 MB (10305474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f01a53caea7c04e7254412060a5c0cb23ff8364d565eab3d98fc0ec804c65b3`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784e930730f995fd22b8a9bdf378b989b6551ae36873db347c0d23370b99e831`  
		Last Modified: Thu, 11 Jun 2020 19:29:39 GMT  
		Size: 13.2 MB (13195114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdcd1019ed44b57cb67d664f43d95a56a032f8fbf5028ce6347443731418cb3`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f541954f527d04cef7111fa78ef9238624e7d52750cc75f73c9e0ec0d8add297`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 16.9 KB (16925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8df574460aaa4735f4c219fb58bd7ce6c6103c39e707bbd3fefdb7fda3eb15`  
		Last Modified: Thu, 11 Jun 2020 21:55:24 GMT  
		Size: 31.4 MB (31389293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d207a4c841e9986a8109779fe3f72f8a73a699ba6327cac1c3532c88c637374c`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 185.0 KB (185016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb807a0037a4bb2eea81b88d9d6bb855cd6ff3c4bb8d095679d2a08e8fd9785a`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3838e2f4cafccf01c6fee22559d9d9e8a3db040ec54cfc8aa7c00bfc0107e15`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 529.4 KB (529410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462e92e05b974146a65c65f38024cb06dea4872dfc740b66cbd46f20446efe9c`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:129d656e55526674b58a0c5e7dc84be5604fa0812e86de089c01bf892a4c6fae`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0` - linux; arm variant v7

```console
$ docker pull composer@sha256:ad6e4c739c756c9d4a50339ff243e48586bb81bb948d45400de700330d3b40d1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56846383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1489d5f182e7810d051ca9dfba3e0b9ca08e08d35f7cb6e05bcbdfc5b4940d80`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:34:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:35:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:35:07 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:35:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:35:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:35:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:35:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:35:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:35:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:35:18 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:35:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:35:20 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:35:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:35:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:38:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:38:31 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:38:34 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:38:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:38:35 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 22:42:55 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 22:43:12 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 22:43:14 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 22:43:15 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 22:43:16 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 22:43:16 GMT
ENV COMPOSER_VERSION=2.0.0-alpha1
# Thu, 11 Jun 2020 22:43:19 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 22:43:19 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 22:43:20 GMT
WORKDIR /app
# Thu, 11 Jun 2020 22:43:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 22:43:22 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5b4230297ea0028dae43acf7e134a55e11ebc15c53a61a2c0c72935dd0ed35`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.2 MB (1214376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779feafcddcba2692e3d187a609b90060e7deea16e8b629aada3a236e99c40f7`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b20c0367792ccffce00af872fa2ea0300330509fb8c15fe5c08905d7db739`  
		Last Modified: Thu, 11 Jun 2020 20:13:03 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9023ca7c2ffcb34f4e075e8f6d5001276142a28b4e0d398fa3eaddc67c4aec`  
		Last Modified: Thu, 11 Jun 2020 20:13:03 GMT  
		Size: 10.3 MB (10305461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e1f3f19383952fefc6527fb475db9a4cde57b21c9a9cb19135732e7b34d85c`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5e59fcc062532624a3a9dd675e189b78e7bce3a5b6c09ce99339dc5b014570`  
		Last Modified: Thu, 11 Jun 2020 20:13:06 GMT  
		Size: 12.4 MB (12350663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a6f7844ad0b4881ed895ba72be400c6782597448fa61bcaa58dd4fe0853836`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354514b31215294fcf1092b43467ddd5587ce6a1fefd1bd4b809cfafbfee18f7`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 16.9 KB (16913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2c7c46ccf6b4c6e523cc448dd15f5f05a0d06483d502b3b0fb72846dab717e`  
		Last Modified: Thu, 11 Jun 2020 22:44:10 GMT  
		Size: 29.8 MB (29839022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267aadf40444bd4f9132644aa6f6c0119543ca29a863cd01bfcaf3be7623cb6f`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 178.7 KB (178699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6871daa35ee6d1b5e329afbb68bf23ef665e526c054959b57f6dc1d858fa9da5`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be16fcfd5362aee76b71dc123b9964109a10bc20c92d393dae9afb97e8dfd788`  
		Last Modified: Thu, 11 Jun 2020 22:43:59 GMT  
		Size: 529.4 KB (529407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c403575f2c0a52309de4977f71514d5b6daaae6c656246352b983a1f2e5b307f`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6bffff0f6c287c63425e0158b26f395db6cda35e35f46191e10fef1a791cf4`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:bf95cc2f6faba08800ce33f3b6dc091b92c84e60dcbafdefd95d84adc589d2a7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63215956 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e063d288a6bdf775ddf084508f4681c8d044afe018713605a0afae38071850b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:40:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:40:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:40:31 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:40:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:40:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:40:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:40:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:40:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:40:37 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:40:38 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:40:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:40:39 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:40:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:40:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:44:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:44:41 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:44:44 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:44:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:44:46 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 22:57:10 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 22:57:28 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 22:57:30 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 22:57:31 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 22:57:31 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 22:57:32 GMT
ENV COMPOSER_VERSION=2.0.0-alpha1
# Thu, 11 Jun 2020 22:57:35 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 22:57:35 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 22:57:36 GMT
WORKDIR /app
# Thu, 11 Jun 2020 22:57:37 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 22:57:37 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee09877319de284b8141c396485111447d75eb8cf26c68819f92f85a4de5649`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 MB (1342990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bad472a11fde1c83808bc84cc9c77da0743b9974bb8c51ab25ed0608cbb4558`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fca52dcdf28b691bbc24b2e2aff931667b865a9188287ef18af016712d3a0f`  
		Last Modified: Thu, 11 Jun 2020 20:30:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f7c9da4678b86166cb9b705a8b9505c19a0d1c24d47bb4360a5907dd28cf28`  
		Last Modified: Thu, 11 Jun 2020 20:30:04 GMT  
		Size: 10.3 MB (10305482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2aa0aa4a6988ac388d32698edfeecb7d0a24539556a4d33bc3327e5786ff0f`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39a6dec5d173eac97dd81097371b07b48982a0ab697e8ab09a40c6d4c319682`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 14.0 MB (13981145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d87e7b6f85188674dafd79fa2e34a45d6f197e8ce1ae71e2337c2534efca59`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f45b14b8adc9219dfa9399abfc7b1b753ca63bfb9a4109e4fd1c0da5caa1a0`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 16.9 KB (16938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88423514539f3ed88c3d723a4f15d7276e95e4c9f4d6c0d3864cd61e0ac8c81c`  
		Last Modified: Thu, 11 Jun 2020 22:58:31 GMT  
		Size: 34.1 MB (34138877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49e25f227bb97b88fe0ffc96fef316f6b53e7c48ef10c14f5399a7441b4ffec`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 188.1 KB (188066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3213d0d563d4eb6ff14649f7b487f46d48ae07fa7768b9ab975db0300aeb8e06`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee53b136300beaa8a9bb4032aad6effa57f9390832b94d0e9929a2679966e35a`  
		Last Modified: Thu, 11 Jun 2020 22:58:20 GMT  
		Size: 529.4 KB (529411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6443b7b0969b18ad433d42484a8b6b40dbd2f39edfde938ef389f5df3b56a0a1`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e384ac93dd3c4bb33efe851aa3067400a5a27edbf3303caec333d5b2e35d024`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0` - linux; 386

```console
$ docker pull composer@sha256:0a3d6a4737cbc6ef541b6a47b1da22cccb4d3b8e964667e22fddf6d99a2a2271
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65212738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a6f152bee8c132bff31b82a7dbb01f97bfd917bcd474f687a71ef849c304ebd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:53:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:53:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:53:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:53:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:53:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:53:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:53:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:53:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:53:09 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:53:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:53:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:02:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:02:55 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:02:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:02:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:02:58 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 01:52:49 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 01:53:04 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 01:53:06 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 01:53:06 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 01:53:06 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 01:53:06 GMT
ENV COMPOSER_VERSION=2.0.0-alpha1
# Fri, 12 Jun 2020 01:53:08 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 01:53:08 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 01:53:09 GMT
WORKDIR /app
# Fri, 12 Jun 2020 01:53:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 01:53:09 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380f9ca051d120d4ed72890904488f0f1e0fd0128cbd1c73adbff366e90bc2aa`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 1.4 MB (1439837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613b9419908bb5beb7365d9d340ee3071aebf8c7919f5379a7b99221fd74c78f`  
		Last Modified: Thu, 11 Jun 2020 22:28:36 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd1bd9f7e9212850ee7c4017e1d3e5ec33176a9113258688a743d871983ee8c`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055c67327ee726dcb5b4e69ca5490023191476ac33eb72e84aea00f6b00c68b7`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 10.3 MB (10305449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6b7ea2ee885f0ae987d58de97f74bb931344e2477eefb48f3d04a90751f764`  
		Last Modified: Thu, 11 Jun 2020 22:28:35 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030cdee16954ea64da3800cd137349eb9b23064bd73168050596c83095da383b`  
		Last Modified: Thu, 11 Jun 2020 22:28:40 GMT  
		Size: 14.6 MB (14564562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629202fa404c086a430dd7d7127e65b92265559980c347f282d4654381da41e8`  
		Last Modified: Thu, 11 Jun 2020 22:28:36 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9694db72218b1872d389aeb90cdae79a16b53f9dfdb334584badf8e808da9f`  
		Last Modified: Thu, 11 Jun 2020 22:28:35 GMT  
		Size: 16.9 KB (16939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4c0dbf20b6de48fdd627e0694147fc21e53c04431f7ebaaa94ec13ef6cae44`  
		Last Modified: Fri, 12 Jun 2020 01:53:45 GMT  
		Size: 35.4 MB (35355633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee96b64f9c4459a8444513a26888081669e737e3fc6eb2f028360b416b333b`  
		Last Modified: Fri, 12 Jun 2020 01:53:34 GMT  
		Size: 203.7 KB (203658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dde06329df568103704291e0b472e532ef23a2f00eadc9484c14ea9feebb8d8`  
		Last Modified: Fri, 12 Jun 2020 01:53:34 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:973e661b3007d25ebf1996c4a564c5af978345f4e967ede4b4644566f922b0d6`  
		Last Modified: Fri, 12 Jun 2020 01:53:33 GMT  
		Size: 529.4 KB (529387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b89c86766ee1c89a125e5e90b5b41f8140016f193982945f1489dbea16bcd840`  
		Last Modified: Fri, 12 Jun 2020 01:53:34 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44013a073fc009001cf9b6413765f77619d1cd818f0f0fa29af7deb134b8137b`  
		Last Modified: Fri, 12 Jun 2020 01:53:33 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0` - linux; ppc64le

```console
$ docker pull composer@sha256:fec312e300025e24c356c391352d5c3be326ec773471b1cd78d781586c247336
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.5 MB (65474252 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:486b99edb8e67eb98cce32e22aa41b2a5a32fdeab660263c2c9debd19922a4e1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:45:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:45:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:45:29 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:45:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:45:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:45:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:45:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:45:52 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:45:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:45:59 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:46:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:46:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:50:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:50:07 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:50:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:50:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:50:19 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 01:52:57 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 01:53:15 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 01:53:22 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 01:53:24 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 01:53:29 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 01:53:32 GMT
ENV COMPOSER_VERSION=2.0.0-alpha1
# Fri, 12 Jun 2020 01:53:41 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 01:53:42 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 01:53:45 GMT
WORKDIR /app
# Fri, 12 Jun 2020 01:53:47 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 01:53:49 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f98eb9049c4fcbaa1cf16ddb44aaf910a89a5471dc303198251fa25bc2a1ef`  
		Last Modified: Thu, 11 Jun 2020 20:57:07 GMT  
		Size: 1.4 MB (1383311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50cdb8e03fc1b19217cd9f80b86142d090ad3e818795b339ea4d9ef9b74555f`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4466e085b12b265fb47397c7c105fd7d78a5883beef49ab9f386393c4c3dae`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbb7594d19c6129fb268c14b9b61a062eb1509b9ee23d2d3c51e55d344b4022`  
		Last Modified: Thu, 11 Jun 2020 20:57:04 GMT  
		Size: 10.3 MB (10305491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfca2ae2dd0fa2baeaf870eb6d850ca046d8dede8bc7bd8e550139f315f0e8a1`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24693054c4d20048d5a8af6f339778f20546c2d519895fd146ed031ab08c95e8`  
		Last Modified: Thu, 11 Jun 2020 20:57:08 GMT  
		Size: 15.1 MB (15144559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91fc688a4963e2db4e23b0cf85f076b3ef08ad8cf636e48f8f6cf76f75b204`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79384080ee3a4da85e7fcf036c35abd4a72aba47f46157e5517a72aa76a2f043`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 17.0 KB (16975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9007b0e243a5a526f41b3c6df897e6cadd789dafa9075a0f6a76edf844e79dbc`  
		Last Modified: Fri, 12 Jun 2020 01:55:05 GMT  
		Size: 35.1 MB (35088531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee306131aed824d74ee7b9cd56c45cb38c0cbbf6f31360accf7310163e16e83`  
		Last Modified: Fri, 12 Jun 2020 01:54:54 GMT  
		Size: 195.7 KB (195699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e185de3b1f08c6feeb3143dac639b8e90538320cac4f19a62842f977cc1459aa`  
		Last Modified: Fri, 12 Jun 2020 01:54:54 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a87c7859acba14a10e08ac909806772cf7ecbece0b84531fb03475c97b910bc6`  
		Last Modified: Fri, 12 Jun 2020 01:54:55 GMT  
		Size: 529.4 KB (529406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36209a6e65503d5d917b4cdb10c6fb22668715f5f08967ca1ad194b78527b1e5`  
		Last Modified: Fri, 12 Jun 2020 01:54:54 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11ed43153dfd0e77c96243f060e2e73ebb6a520d4736d61a47294c843d1e26dc`  
		Last Modified: Fri, 12 Jun 2020 01:54:55 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0` - linux; s390x

```console
$ docker pull composer@sha256:ce99e518d2dd9ad4770616140716477d4bc5632b59df03e637626401aaa95708
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62413618 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82aa252a8d19e37a054b720b4cce550471c55e05e1b9eb5f1252f28a6dd83d8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:29:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:29:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:29:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:29:39 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:29:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:29:40 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:29:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:29:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:32:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:32:06 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:32:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:32:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:32:07 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 21:14:48 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 21:14:59 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 21:15:00 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 21:15:00 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 21:15:00 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 21:15:00 GMT
ENV COMPOSER_VERSION=2.0.0-alpha1
# Thu, 11 Jun 2020 21:15:02 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 21:15:02 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 21:15:02 GMT
WORKDIR /app
# Thu, 11 Jun 2020 21:15:02 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 21:15:02 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057c8475c8b5e21c245ff682a57adf8970d16ccbed87694b3ec200c83e17a8fb`  
		Last Modified: Thu, 11 Jun 2020 19:32:19 GMT  
		Size: 1.4 MB (1382745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2bbd1ef5644a3638bc6f073de941463cbfceb435ea6d11ce3c7fdb9f8d2539`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b73c5118a1a42bce068c040302cb99d7a26ef9ab76544773e9ba70f28d274d3`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfeeda5adbfaef226ee75380f0826468b0bd1f4ea5142c15218b6cc328c9c9a0`  
		Last Modified: Thu, 11 Jun 2020 19:32:15 GMT  
		Size: 10.3 MB (10305469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44be4c9292a75900438b83d5e272193b11245a6bf05518dd9a7974e323661cde`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20293274603f1fbe03122151a8bea57a755d636395aad8821ca8e9495705001e`  
		Last Modified: Thu, 11 Jun 2020 19:32:17 GMT  
		Size: 13.5 MB (13477832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab300e409b143028fcd83629578c9b6c98542c1d6032fec4aa0d2ccb1e2e051c`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb729c9479eb91824cf62c8c605c0d3ab455b2a38a9d64b711b103f5dd2c20f2`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 16.9 KB (16915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa934f9e31e268cdfaf8d2cdd9036048b51a7325574c92594af08119d1ad235`  
		Last Modified: Thu, 11 Jun 2020 21:15:33 GMT  
		Size: 33.9 MB (33941742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625468e67d86014210e23c5ea7ea3619855d89e3e0d1b63de045202112042458`  
		Last Modified: Thu, 11 Jun 2020 21:15:27 GMT  
		Size: 188.2 KB (188239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdc9bfb76124ce5c12fe3ac1c9fe249e610f30b8f793016e97ac64a463138f9`  
		Last Modified: Thu, 11 Jun 2020 21:15:27 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10f42881c1a5a8a439c5797420022d3a2b9acc48a45cd081ef89aa7f465db132`  
		Last Modified: Thu, 11 Jun 2020 21:15:27 GMT  
		Size: 529.4 KB (529406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:800710402d7e8e60725a9c1597e4b9e939f600b35ed41e5a19f6ebf6780df135`  
		Last Modified: Thu, 11 Jun 2020 21:15:42 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92016695d233f249b7054ff58d8ee3d2fc2359b00527b17065935911b4db1311`  
		Last Modified: Thu, 11 Jun 2020 21:15:42 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `composer:2.0.0-alpha2`

**does not exist** (yet?)

## `composer:latest`

```console
$ docker pull composer@sha256:68e9afcfe042a69a778ffccd2da55cf195dd5671ab14163b774f00d6da0f23c4
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

### `composer:latest` - linux; amd64

```console
$ docker pull composer@sha256:6babbd3567845f5a1c6cf3a01143ddcb4abe587fd14e221e36accebf0e962e84
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.1 MB (63111308 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:433420023b60cdf98a661eab19b14714e5e1a7056ac73561a660d9727d80723c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:51:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:51:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:51:59 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:51:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:52:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:52:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:52:01 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:52:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:52:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:00:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:00:41 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:00:43 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:00:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:00:44 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 03:36:24 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 03:36:34 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 03:36:35 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 03:36:35 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 03:36:35 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 03:36:43 GMT
ENV COMPOSER_VERSION=1.10.7
# Fri, 12 Jun 2020 03:36:44 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 03:36:44 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 03:36:45 GMT
WORKDIR /app
# Fri, 12 Jun 2020 03:36:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 03:36:45 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358d6dbbdff5c10cbe23c608b7ff9c6d1dd13331dd7dc7644b727ca5ea8e742`  
		Last Modified: Thu, 11 Jun 2020 22:14:55 GMT  
		Size: 1.3 MB (1340817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232d962484c6b9a1caa33a12f1beed4cb20996085056b4fb1591a9fd1d8c89f`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1d3ac04d2af7a9f0eee25eccc72e586400051054ffb4aff7cdf2f4ebc993e8`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f2fa029f21abccac9d1ce064bef95d56aad7de3e1079df260138622eaf8ab25`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 10.3 MB (10305445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13e18722d91019f31ffd0d261959c5dd489f6d27361f221a669dbe9691a56ef9`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3659ffc4e0a4393e4597cf7a4210f863623e4e1cdf86ed3f06726aa0616108d9`  
		Last Modified: Thu, 11 Jun 2020 22:14:59 GMT  
		Size: 14.2 MB (14173631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1874d3f89152f2ab71121617a3cfdb60a30feccc88dc7806657e3b22f3ccd6`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2545369333e4aa084fbd5285c57af07bd75686c0976981a60df746089e02b75a`  
		Last Modified: Thu, 11 Jun 2020 22:14:53 GMT  
		Size: 16.9 KB (16931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680b7fc10b4acd5dda859b161e18533921eb585502203fb8d90e392b990fc0ff`  
		Last Modified: Fri, 12 Jun 2020 03:37:08 GMT  
		Size: 33.8 MB (33777899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95843d9ed2bd562441ca7a2cc826205c5403bd8384507211f0d3854eb07153b8`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 189.3 KB (189338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab487c471b8cfbda88b1b5a5ea9b716442d9cae4c86413a3d3302d01f2c6b3b2`  
		Last Modified: Fri, 12 Jun 2020 03:37:00 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17c9a21ccbb41f0c9bc7e467ba8129c81c9c6ee9eb26efa9bf3a0ac6303da34a`  
		Last Modified: Fri, 12 Jun 2020 03:37:13 GMT  
		Size: 504.7 KB (504734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec30aea17efe54c81d4cacd55e4350577778932f8d4818b9a3ecc9706ee0e374`  
		Last Modified: Fri, 12 Jun 2020 03:37:13 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7959b1da3d37ece89d1d51098ea4a534e68b3d8311b39e6048287b4bba6250f2`  
		Last Modified: Fri, 12 Jun 2020 03:37:13 GMT  
		Size: 90.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; arm variant v6

```console
$ docker pull composer@sha256:c99b3bde69d2f2fba1d4696ecb638d5e381c61fc1bef1be262c82eddfa17dc5e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.5 MB (59515232 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67b7073d9fbf550b58fd228a151b966b6325d38adb1c720bd8750545a3f10191`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:14:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:14:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:14:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:14:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:14:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:14:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:14:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:14:59 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:15:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:15:01 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:16:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:16:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:19:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:19:59 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:20:02 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:20:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:20:03 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 21:53:58 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 21:54:20 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 21:54:22 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 21:54:23 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 21:54:24 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 21:54:40 GMT
ENV COMPOSER_VERSION=1.10.7
# Thu, 11 Jun 2020 21:54:43 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 21:54:43 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 21:54:44 GMT
WORKDIR /app
# Thu, 11 Jun 2020 21:54:45 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 21:54:46 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72788d65e292354c2ce4b67441d334d0ba534db5ce71d5b8bf78011a256b566f`  
		Last Modified: Thu, 11 Jun 2020 19:29:37 GMT  
		Size: 1.3 MB (1310273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e32d62de43da999aca07cf15fdbe1cd6b03aebc88c15409c3463daadf13e01`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6701e05673b745147608cd1b6eb47a3fbc35bcfd8a65bc536e5b9f919b3d0e77`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23d338eb9977c3cc4f53684a30948f5defb783b30f97eb45447ad19c586495f`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 10.3 MB (10305474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f01a53caea7c04e7254412060a5c0cb23ff8364d565eab3d98fc0ec804c65b3`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:784e930730f995fd22b8a9bdf378b989b6551ae36873db347c0d23370b99e831`  
		Last Modified: Thu, 11 Jun 2020 19:29:39 GMT  
		Size: 13.2 MB (13195114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccdcd1019ed44b57cb67d664f43d95a56a032f8fbf5028ce6347443731418cb3`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f541954f527d04cef7111fa78ef9238624e7d52750cc75f73c9e0ec0d8add297`  
		Last Modified: Thu, 11 Jun 2020 19:29:35 GMT  
		Size: 16.9 KB (16925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a8df574460aaa4735f4c219fb58bd7ce6c6103c39e707bbd3fefdb7fda3eb15`  
		Last Modified: Thu, 11 Jun 2020 21:55:24 GMT  
		Size: 31.4 MB (31389293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d207a4c841e9986a8109779fe3f72f8a73a699ba6327cac1c3532c88c637374c`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 185.0 KB (185016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb807a0037a4bb2eea81b88d9d6bb855cd6ff3c4bb8d095679d2a08e8fd9785a`  
		Last Modified: Thu, 11 Jun 2020 21:55:11 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628d2c181171c88661a79e5befe13fc7f464d8aa498dff82d835fd304f42840e`  
		Last Modified: Thu, 11 Jun 2020 21:55:33 GMT  
		Size: 504.8 KB (504761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab5d325d1c74d1ed9f95a81872af98adebe1e0fcff9fa7c6cb883500dd03582e`  
		Last Modified: Thu, 11 Jun 2020 21:55:33 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19054a7d036b408c8c42f34c49a8ca70ce737a6f76c5f803d0fb8956091a4177`  
		Last Modified: Thu, 11 Jun 2020 21:55:33 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; arm variant v7

```console
$ docker pull composer@sha256:b94ca5b5a25604233671a05014b89dfb56c3fe64f1f8200b6e71c913a2624b5f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.8 MB (56821735 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ae8665451ee2a2d4f3849bd08ad0178750f08c57ad44afeef533d24f078947b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:34:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:35:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:35:07 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:35:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:35:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:35:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:35:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:35:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:35:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:35:18 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:35:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:35:20 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:35:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:35:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:38:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:38:31 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:38:34 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:38:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:38:35 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 22:42:55 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 22:43:12 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 22:43:14 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 22:43:15 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 22:43:16 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 22:43:30 GMT
ENV COMPOSER_VERSION=1.10.7
# Thu, 11 Jun 2020 22:43:32 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 22:43:33 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 22:43:33 GMT
WORKDIR /app
# Thu, 11 Jun 2020 22:43:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 22:43:35 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5b4230297ea0028dae43acf7e134a55e11ebc15c53a61a2c0c72935dd0ed35`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.2 MB (1214376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779feafcddcba2692e3d187a609b90060e7deea16e8b629aada3a236e99c40f7`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b20c0367792ccffce00af872fa2ea0300330509fb8c15fe5c08905d7db739`  
		Last Modified: Thu, 11 Jun 2020 20:13:03 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b9023ca7c2ffcb34f4e075e8f6d5001276142a28b4e0d398fa3eaddc67c4aec`  
		Last Modified: Thu, 11 Jun 2020 20:13:03 GMT  
		Size: 10.3 MB (10305461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5e1f3f19383952fefc6527fb475db9a4cde57b21c9a9cb19135732e7b34d85c`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5e59fcc062532624a3a9dd675e189b78e7bce3a5b6c09ce99339dc5b014570`  
		Last Modified: Thu, 11 Jun 2020 20:13:06 GMT  
		Size: 12.4 MB (12350663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a6f7844ad0b4881ed895ba72be400c6782597448fa61bcaa58dd4fe0853836`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354514b31215294fcf1092b43467ddd5587ce6a1fefd1bd4b809cfafbfee18f7`  
		Last Modified: Thu, 11 Jun 2020 20:13:02 GMT  
		Size: 16.9 KB (16913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2c7c46ccf6b4c6e523cc448dd15f5f05a0d06483d502b3b0fb72846dab717e`  
		Last Modified: Thu, 11 Jun 2020 22:44:10 GMT  
		Size: 29.8 MB (29839022 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267aadf40444bd4f9132644aa6f6c0119543ca29a863cd01bfcaf3be7623cb6f`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 178.7 KB (178699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6871daa35ee6d1b5e329afbb68bf23ef665e526c054959b57f6dc1d858fa9da5`  
		Last Modified: Thu, 11 Jun 2020 22:43:58 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1aac479723ca5c8c2a89d1610187c4148329bc22defdbc2a444dfc2b4cfabfd`  
		Last Modified: Thu, 11 Jun 2020 22:44:18 GMT  
		Size: 504.8 KB (504761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb738297c43fa116285317f4c78f4addf3a15382c0fd326dd4d29377ffc79d7`  
		Last Modified: Thu, 11 Jun 2020 22:44:18 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a4f6e9edfac9965af157620024a2e64e623cbad6dad720e2d44702b42327cc`  
		Last Modified: Thu, 11 Jun 2020 22:44:18 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:6c2943d8c54f865e3bbe6ea5d8968709106e67b9fbb0a79557af6286ff9e6986
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.2 MB (63191302 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3bf68b97259926db2b63907b7b6ad33c3cb23398c5218c7e5a6cb042c608cc3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:40:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:40:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:40:31 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:40:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:40:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:40:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:40:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:40:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:40:37 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:40:38 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:40:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:40:39 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:40:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:40:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:44:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:44:41 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:44:44 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:44:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:44:46 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 22:57:10 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 22:57:28 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 22:57:30 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 22:57:31 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 22:57:31 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 22:57:45 GMT
ENV COMPOSER_VERSION=1.10.7
# Thu, 11 Jun 2020 22:57:48 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 22:57:49 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 22:57:49 GMT
WORKDIR /app
# Thu, 11 Jun 2020 22:57:50 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 22:57:50 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee09877319de284b8141c396485111447d75eb8cf26c68819f92f85a4de5649`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 MB (1342990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bad472a11fde1c83808bc84cc9c77da0743b9974bb8c51ab25ed0608cbb4558`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fca52dcdf28b691bbc24b2e2aff931667b865a9188287ef18af016712d3a0f`  
		Last Modified: Thu, 11 Jun 2020 20:30:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f7c9da4678b86166cb9b705a8b9505c19a0d1c24d47bb4360a5907dd28cf28`  
		Last Modified: Thu, 11 Jun 2020 20:30:04 GMT  
		Size: 10.3 MB (10305482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd2aa0aa4a6988ac388d32698edfeecb7d0a24539556a4d33bc3327e5786ff0f`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39a6dec5d173eac97dd81097371b07b48982a0ab697e8ab09a40c6d4c319682`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 14.0 MB (13981145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d87e7b6f85188674dafd79fa2e34a45d6f197e8ce1ae71e2337c2534efca59`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f45b14b8adc9219dfa9399abfc7b1b753ca63bfb9a4109e4fd1c0da5caa1a0`  
		Last Modified: Thu, 11 Jun 2020 20:30:03 GMT  
		Size: 16.9 KB (16938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88423514539f3ed88c3d723a4f15d7276e95e4c9f4d6c0d3864cd61e0ac8c81c`  
		Last Modified: Thu, 11 Jun 2020 22:58:31 GMT  
		Size: 34.1 MB (34138877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49e25f227bb97b88fe0ffc96fef316f6b53e7c48ef10c14f5399a7441b4ffec`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 188.1 KB (188066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3213d0d563d4eb6ff14649f7b487f46d48ae07fa7768b9ab975db0300aeb8e06`  
		Last Modified: Thu, 11 Jun 2020 22:58:19 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:867f1875f74e994124013a455523af4fa2ea1c18a20c999912dfef70cddf49e5`  
		Last Modified: Thu, 11 Jun 2020 22:58:39 GMT  
		Size: 504.8 KB (504760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a710d37874225c8cc6da9516d38717d9c53945a7c7eaf00c56c8764f8e532fc0`  
		Last Modified: Thu, 11 Jun 2020 22:58:39 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:093b2977f90dfa6bf7e6c2dbd081d7c421ec1b69da9adf6b4d19ebe49dac79a7`  
		Last Modified: Thu, 11 Jun 2020 22:58:39 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; 386

```console
$ docker pull composer@sha256:ca47ae35321e8e6f4572cb65f085ca1fbf08aa60d7a993ef8f314dbfc7ed12f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.2 MB (65188090 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8034411c9bc77c35903f70e193a48739892a5ce4a31fa9f860c9205e856f6023`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:53:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:53:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:53:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:53:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:53:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:53:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:53:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:53:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:53:09 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:53:10 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:53:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:53:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:02:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 19:02:55 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 19:02:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 19:02:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 19:02:58 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 01:52:49 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 01:53:04 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 01:53:06 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 01:53:06 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 01:53:06 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 01:53:15 GMT
ENV COMPOSER_VERSION=1.10.7
# Fri, 12 Jun 2020 01:53:17 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 01:53:17 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 01:53:18 GMT
WORKDIR /app
# Fri, 12 Jun 2020 01:53:18 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 01:53:18 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380f9ca051d120d4ed72890904488f0f1e0fd0128cbd1c73adbff366e90bc2aa`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 1.4 MB (1439837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613b9419908bb5beb7365d9d340ee3071aebf8c7919f5379a7b99221fd74c78f`  
		Last Modified: Thu, 11 Jun 2020 22:28:36 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd1bd9f7e9212850ee7c4017e1d3e5ec33176a9113258688a743d871983ee8c`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:055c67327ee726dcb5b4e69ca5490023191476ac33eb72e84aea00f6b00c68b7`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 10.3 MB (10305449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af6b7ea2ee885f0ae987d58de97f74bb931344e2477eefb48f3d04a90751f764`  
		Last Modified: Thu, 11 Jun 2020 22:28:35 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030cdee16954ea64da3800cd137349eb9b23064bd73168050596c83095da383b`  
		Last Modified: Thu, 11 Jun 2020 22:28:40 GMT  
		Size: 14.6 MB (14564562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629202fa404c086a430dd7d7127e65b92265559980c347f282d4654381da41e8`  
		Last Modified: Thu, 11 Jun 2020 22:28:36 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d9694db72218b1872d389aeb90cdae79a16b53f9dfdb334584badf8e808da9f`  
		Last Modified: Thu, 11 Jun 2020 22:28:35 GMT  
		Size: 16.9 KB (16939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a4c0dbf20b6de48fdd627e0694147fc21e53c04431f7ebaaa94ec13ef6cae44`  
		Last Modified: Fri, 12 Jun 2020 01:53:45 GMT  
		Size: 35.4 MB (35355633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57ee96b64f9c4459a8444513a26888081669e737e3fc6eb2f028360b416b333b`  
		Last Modified: Fri, 12 Jun 2020 01:53:34 GMT  
		Size: 203.7 KB (203658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dde06329df568103704291e0b472e532ef23a2f00eadc9484c14ea9feebb8d8`  
		Last Modified: Fri, 12 Jun 2020 01:53:34 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a073f20a79e2063002071c18660e75c258c07c5cb94393ae82b4e7d51f7592b5`  
		Last Modified: Fri, 12 Jun 2020 01:53:51 GMT  
		Size: 504.7 KB (504739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:872a29d49579bed85016977d1eb236f48a987c5d6cf992eb143af868d8ac2745`  
		Last Modified: Fri, 12 Jun 2020 01:53:51 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf2c57a63fa1e8a513188c0a237354c461502dbc26a5d6dda0aaa5218c816d8`  
		Last Modified: Fri, 12 Jun 2020 01:53:51 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; ppc64le

```console
$ docker pull composer@sha256:e155573df8700733bd8bf1dce305e67622e262c4c75016d1d826624f312d75cd
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65449609 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e574aedfcde654f9cc674ae6915ab8bc375b98c5a1b9c091e9ff77f1a4c72c58`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:45:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:45:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:45:29 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:45:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:45:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:45:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:45:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:45:52 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:45:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:45:59 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:46:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:46:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:50:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:50:07 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:50:14 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:50:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:50:19 GMT
CMD ["php" "-a"]
# Fri, 12 Jun 2020 01:52:57 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 12 Jun 2020 01:53:15 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 12 Jun 2020 01:53:22 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 12 Jun 2020 01:53:24 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 12 Jun 2020 01:53:29 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 12 Jun 2020 01:54:02 GMT
ENV COMPOSER_VERSION=1.10.7
# Fri, 12 Jun 2020 01:54:10 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 12 Jun 2020 01:54:11 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Fri, 12 Jun 2020 01:54:15 GMT
WORKDIR /app
# Fri, 12 Jun 2020 01:54:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Fri, 12 Jun 2020 01:54:19 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f98eb9049c4fcbaa1cf16ddb44aaf910a89a5471dc303198251fa25bc2a1ef`  
		Last Modified: Thu, 11 Jun 2020 20:57:07 GMT  
		Size: 1.4 MB (1383311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50cdb8e03fc1b19217cd9f80b86142d090ad3e818795b339ea4d9ef9b74555f`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4466e085b12b265fb47397c7c105fd7d78a5883beef49ab9f386393c4c3dae`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cbb7594d19c6129fb268c14b9b61a062eb1509b9ee23d2d3c51e55d344b4022`  
		Last Modified: Thu, 11 Jun 2020 20:57:04 GMT  
		Size: 10.3 MB (10305491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfca2ae2dd0fa2baeaf870eb6d850ca046d8dede8bc7bd8e550139f315f0e8a1`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24693054c4d20048d5a8af6f339778f20546c2d519895fd146ed031ab08c95e8`  
		Last Modified: Thu, 11 Jun 2020 20:57:08 GMT  
		Size: 15.1 MB (15144559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd91fc688a4963e2db4e23b0cf85f076b3ef08ad8cf636e48f8f6cf76f75b204`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79384080ee3a4da85e7fcf036c35abd4a72aba47f46157e5517a72aa76a2f043`  
		Last Modified: Thu, 11 Jun 2020 20:57:03 GMT  
		Size: 17.0 KB (16975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9007b0e243a5a526f41b3c6df897e6cadd789dafa9075a0f6a76edf844e79dbc`  
		Last Modified: Fri, 12 Jun 2020 01:55:05 GMT  
		Size: 35.1 MB (35088531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ee306131aed824d74ee7b9cd56c45cb38c0cbbf6f31360accf7310163e16e83`  
		Last Modified: Fri, 12 Jun 2020 01:54:54 GMT  
		Size: 195.7 KB (195699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e185de3b1f08c6feeb3143dac639b8e90538320cac4f19a62842f977cc1459aa`  
		Last Modified: Fri, 12 Jun 2020 01:54:54 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5e9e5aadfb14bce92b646f2cc5d9e1bb48a418845cb2c5e422a6b650195444d`  
		Last Modified: Fri, 12 Jun 2020 01:55:19 GMT  
		Size: 504.8 KB (504763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3faa7594d67fbd17a8895393beeb7559f054737949d92803b2e4e52d32ea3add`  
		Last Modified: Fri, 12 Jun 2020 01:55:18 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3029d423df91b54e0ba93e32720d02228f7f5f055f6227a76d70200ee21fa7`  
		Last Modified: Fri, 12 Jun 2020 01:55:18 GMT  
		Size: 125.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; s390x

```console
$ docker pull composer@sha256:a638d6ac9c98be9851cac68f86066ed9399324cf29b2bfe534074223796862fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.4 MB (62388970 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf8b15a368579abfd95087125c06a1b3ce2c5b49728f3fe79b30417fc49716f5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:29:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:29:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:29:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:29:39 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_VERSION=7.4.7
# Thu, 11 Jun 2020 18:29:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.7.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.7.tar.xz.asc
# Thu, 11 Jun 2020 18:29:40 GMT
ENV PHP_SHA256=53558f8f24cd8ab6fa0ea252ca8198e2650160649681ce5230c1df1dc2b52faf PHP_MD5=
# Thu, 11 Jun 2020 18:29:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 11 Jun 2020 18:29:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:32:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 11 Jun 2020 18:32:06 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 11 Jun 2020 18:32:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 11 Jun 2020 18:32:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 11 Jun 2020 18:32:07 GMT
CMD ["php" "-a"]
# Thu, 11 Jun 2020 21:14:48 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 11 Jun 2020 21:14:59 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 11 Jun 2020 21:15:00 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 11 Jun 2020 21:15:00 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 11 Jun 2020 21:15:00 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 11 Jun 2020 21:15:08 GMT
ENV COMPOSER_VERSION=1.10.7
# Thu, 11 Jun 2020 21:15:09 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 11 Jun 2020 21:15:09 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 11 Jun 2020 21:15:10 GMT
WORKDIR /app
# Thu, 11 Jun 2020 21:15:10 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 11 Jun 2020 21:15:10 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057c8475c8b5e21c245ff682a57adf8970d16ccbed87694b3ec200c83e17a8fb`  
		Last Modified: Thu, 11 Jun 2020 19:32:19 GMT  
		Size: 1.4 MB (1382745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2bbd1ef5644a3638bc6f073de941463cbfceb435ea6d11ce3c7fdb9f8d2539`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b73c5118a1a42bce068c040302cb99d7a26ef9ab76544773e9ba70f28d274d3`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfeeda5adbfaef226ee75380f0826468b0bd1f4ea5142c15218b6cc328c9c9a0`  
		Last Modified: Thu, 11 Jun 2020 19:32:15 GMT  
		Size: 10.3 MB (10305469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44be4c9292a75900438b83d5e272193b11245a6bf05518dd9a7974e323661cde`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20293274603f1fbe03122151a8bea57a755d636395aad8821ca8e9495705001e`  
		Last Modified: Thu, 11 Jun 2020 19:32:17 GMT  
		Size: 13.5 MB (13477832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab300e409b143028fcd83629578c9b6c98542c1d6032fec4aa0d2ccb1e2e051c`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb729c9479eb91824cf62c8c605c0d3ab455b2a38a9d64b711b103f5dd2c20f2`  
		Last Modified: Thu, 11 Jun 2020 19:32:20 GMT  
		Size: 16.9 KB (16915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fa934f9e31e268cdfaf8d2cdd9036048b51a7325574c92594af08119d1ad235`  
		Last Modified: Thu, 11 Jun 2020 21:15:33 GMT  
		Size: 33.9 MB (33941742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:625468e67d86014210e23c5ea7ea3619855d89e3e0d1b63de045202112042458`  
		Last Modified: Thu, 11 Jun 2020 21:15:27 GMT  
		Size: 188.2 KB (188239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdc9bfb76124ce5c12fe3ac1c9fe249e610f30b8f793016e97ac64a463138f9`  
		Last Modified: Thu, 11 Jun 2020 21:15:27 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d6e69a305ada81492d8105ec332537f82df9649eeb8be810f27e679e57ce0e`  
		Last Modified: Thu, 11 Jun 2020 21:15:49 GMT  
		Size: 504.8 KB (504760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f56ca97f5cad0a316e00feef34f27d5f0fbc5be97eacaf1f80f534151cd2df6`  
		Last Modified: Thu, 11 Jun 2020 21:15:53 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8d445cf9a9d0d80134feba5f37a8ecadbf310d18ab2caaae74a689ff9fa3be`  
		Last Modified: Thu, 11 Jun 2020 21:15:48 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
