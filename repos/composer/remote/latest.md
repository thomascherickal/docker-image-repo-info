## `composer:latest`

```console
$ docker pull composer@sha256:8fbf47ea70644f7bdb6e3b55bf1c9c1b378a55112a194b5cc42a8785759d3491
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `composer:latest` - linux; amd64

```console
$ docker pull composer@sha256:16f05d29ac7f60d9dbc9daae7bf503c35926484035825ee84092994e33d6c338
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64650009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac7c61d05d5a00bdbb65a566c32eb1d50351b29fbd676e2dc9e3bfb6850eaed0`
-	Entrypoint: `["\/bin\/sh","\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:18:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 18 Jan 2020 03:18:28 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 18 Jan 2020 03:18:29 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:18:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 18 Jan 2020 03:18:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 18 Jan 2020 03:18:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 03:18:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 03:18:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 18 Jan 2020 03:18:30 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 24 Jan 2020 07:05:12 GMT
ENV PHP_VERSION=7.4.2
# Fri, 24 Jan 2020 07:05:13 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Fri, 24 Jan 2020 07:05:13 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Fri, 24 Jan 2020 07:05:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 24 Jan 2020 07:05:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 24 Jan 2020 07:13:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 24 Jan 2020 07:13:16 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Fri, 24 Jan 2020 07:13:17 GMT
RUN docker-php-ext-enable sodium
# Fri, 24 Jan 2020 07:13:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 24 Jan 2020 07:13:17 GMT
CMD ["php" "-a"]
# Fri, 24 Jan 2020 11:01:17 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 24 Jan 2020 11:01:28 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 24 Jan 2020 11:01:29 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 24 Jan 2020 11:01:29 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 24 Jan 2020 11:01:29 GMT
ENV COMPOSER_HOME=/tmp
# Wed, 05 Feb 2020 00:19:31 GMT
ENV COMPOSER_VERSION=1.9.3
# Wed, 05 Feb 2020 00:19:33 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Wed, 05 Feb 2020 00:19:33 GMT
COPY file:098af1c9d6ed00c2f357827391da1b2b0978915db35f033349301c7cbe78010d in /docker-entrypoint.sh 
# Wed, 05 Feb 2020 00:19:33 GMT
WORKDIR /app
# Wed, 05 Feb 2020 00:19:33 GMT
ENTRYPOINT ["/bin/sh" "/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 00:19:33 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c0a1817becf025301783a94fa11de700972e7d7c117ca7e45d080db0ec1a11`  
		Last Modified: Sat, 18 Jan 2020 04:09:35 GMT  
		Size: 1.4 MB (1354634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd5b3ea1fc31791c18f464b5b95dd3d9b8ff97aef4b64e0202f3da7f5550e80`  
		Last Modified: Sat, 18 Jan 2020 04:09:35 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db87396003bdeb76e6e367a5ae26be9642a89986dcda71b3491412c579cb6859`  
		Last Modified: Sat, 18 Jan 2020 04:09:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fa47f19b1e835f47f4c1273ccb215a42ee2aefafe300409d92b05b899a757d8`  
		Last Modified: Fri, 24 Jan 2020 10:39:33 GMT  
		Size: 10.3 MB (10271096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4556adb19ddcb43be3cd12b973f718e5edc74d6986ae4406a0c3011cbeb3dc93`  
		Last Modified: Fri, 24 Jan 2020 10:39:33 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:205de55b7ed0d389ac2c9777321f11ba9377a148002c2ef1d7b68d02a96472f3`  
		Last Modified: Fri, 24 Jan 2020 10:39:42 GMT  
		Size: 14.6 MB (14574023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c35aa7da966a732561c37c8b5d56949eedcb7865066b86da95c8bc58c18c48d2`  
		Last Modified: Fri, 24 Jan 2020 10:39:32 GMT  
		Size: 2.2 KB (2216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a54ca6f814c156199e3266c4297efe2f54fb83bfb1645f53582eae3d1e222e`  
		Last Modified: Fri, 24 Jan 2020 10:39:33 GMT  
		Size: 73.1 KB (73145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7814beba2ab07c91fb86d128f49942659d2bfc3d4424cfbdac5fdea74fc182b0`  
		Last Modified: Fri, 24 Jan 2020 11:02:23 GMT  
		Size: 34.8 MB (34794310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b13fbce728aec3717fa6728e30f0eaa3ccdedcc0990a924e51fb5149c56b925a`  
		Last Modified: Fri, 24 Jan 2020 11:01:53 GMT  
		Size: 277.4 KB (277393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57edc146252bda027552b3da0c9a06aee45976a1f8692d5d82727304cd43661`  
		Last Modified: Fri, 24 Jan 2020 11:01:52 GMT  
		Size: 256.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3129b3f701e31f3009bbd5a36e552b3d298ac20d3e704dc345ba4ceff446146c`  
		Last Modified: Wed, 05 Feb 2020 00:19:44 GMT  
		Size: 497.4 KB (497385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15289548f5eea10369727a861c6b41806dfbafeb6f8024b6015806afeee1047d`  
		Last Modified: Wed, 05 Feb 2020 00:19:44 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997a01e12008a7b7f9c654ede9d590c663b22a377064e29bc83375289713f51f`  
		Last Modified: Wed, 05 Feb 2020 00:19:44 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; arm variant v6

```console
$ docker pull composer@sha256:e36707baf24ea0623807617f27cfe0f849809fb1005e563aa49495f9e6ac3f31
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62788228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f548fa38c84df4e16081fd01ac0007649ce7ac26b5d46d70df578d15c0e59274`
-	Entrypoint: `["\/bin\/sh","\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:40:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 18 Jan 2020 03:40:03 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 18 Jan 2020 03:40:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:40:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 18 Jan 2020 03:40:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 18 Jan 2020 03:40:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 03:40:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 03:40:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 18 Jan 2020 03:40:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 20 Feb 2020 21:49:41 GMT
ENV PHP_VERSION=7.4.3
# Thu, 20 Feb 2020 21:49:43 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.3.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.3.tar.xz.asc/from/this/mirror
# Thu, 20 Feb 2020 21:49:44 GMT
ENV PHP_SHA256=cf1f856d877c268124ded1ede40c9fb6142b125fdaafdc54f855120b8bc6982a PHP_MD5=
# Thu, 20 Feb 2020 21:49:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 20 Feb 2020 21:49:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 20 Feb 2020 21:53:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 20 Feb 2020 21:53:50 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Thu, 20 Feb 2020 21:53:53 GMT
RUN docker-php-ext-enable sodium
# Thu, 20 Feb 2020 21:53:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 20 Feb 2020 21:53:54 GMT
CMD ["php" "-a"]
# Thu, 20 Feb 2020 23:38:44 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 20 Feb 2020 23:39:05 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 20 Feb 2020 23:39:09 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 20 Feb 2020 23:39:11 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 20 Feb 2020 23:39:12 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 20 Feb 2020 23:39:13 GMT
ENV COMPOSER_VERSION=1.9.3
# Thu, 20 Feb 2020 23:39:18 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 20 Feb 2020 23:39:19 GMT
COPY file:098af1c9d6ed00c2f357827391da1b2b0978915db35f033349301c7cbe78010d in /docker-entrypoint.sh 
# Thu, 20 Feb 2020 23:39:20 GMT
WORKDIR /app
# Thu, 20 Feb 2020 23:39:21 GMT
ENTRYPOINT ["/bin/sh" "/docker-entrypoint.sh"]
# Thu, 20 Feb 2020 23:39:23 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5c701ead53742b2a88bf4f606bd05029ec59ccaf522450bfa76be8cea0cf02`  
		Last Modified: Sat, 18 Jan 2020 04:28:12 GMT  
		Size: 1.3 MB (1321088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574e3d03f7d4228e33415f8592e7ec2a89fe1616e0ab6366ea68045b09d7f280`  
		Last Modified: Sat, 18 Jan 2020 04:28:12 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba27e9ff828195f46a3edb0b1e28b5d10451b66ae080c20794f6d005cffbd72`  
		Last Modified: Sat, 18 Jan 2020 04:28:12 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f246fe8b62d43a3f633a04898577258a2ce5dd84edf5fd464403b9a108b301e2`  
		Last Modified: Thu, 20 Feb 2020 23:10:06 GMT  
		Size: 10.3 MB (10280264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b4e0af10768397859f6f19eca4b17ee9f21d61a1cb06989aba861267cf1b6a`  
		Last Modified: Thu, 20 Feb 2020 23:10:05 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a228bdc8e070add11170637553b04b0eeab55a8af3159561b2878b3bcc00bbb`  
		Last Modified: Thu, 20 Feb 2020 23:10:11 GMT  
		Size: 13.6 MB (13600067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:936640ed543c6bb114e0374d4aa5d00b0ad989151337d4edfe6047bad672c605`  
		Last Modified: Thu, 20 Feb 2020 23:10:05 GMT  
		Size: 2.2 KB (2214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:071eed09e44daa0c7c7d337a517208fa4a3c08e02029c0970082688456496bec`  
		Last Modified: Thu, 20 Feb 2020 23:10:05 GMT  
		Size: 72.7 KB (72679 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1484b55cf2e4265f19b432a0f9703ba1942adc03e2e472e80d4888e6a97edd58`  
		Last Modified: Thu, 20 Feb 2020 23:40:18 GMT  
		Size: 34.1 MB (34123104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d975b56d19fa6555c8dc2e29c9438bca490fc5e3acc9f2c4e475b320680e3e1`  
		Last Modified: Thu, 20 Feb 2020 23:40:04 GMT  
		Size: 270.9 KB (270874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628fcd789fd80e1db05071f903233ef15a9c8df4acef1d7dd64ad731d4c6e5f1`  
		Last Modified: Thu, 20 Feb 2020 23:40:03 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6564440b0b1fad834cbf445eb9b34e28bc9b36b4db1d6f199878cd5b9abd06a`  
		Last Modified: Thu, 20 Feb 2020 23:40:03 GMT  
		Size: 497.4 KB (497413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e424bea0d4b8c7b62adf7bc8777d7f5dbaf11339a380c80b655b0023cbf9d87`  
		Last Modified: Thu, 20 Feb 2020 23:40:03 GMT  
		Size: 555.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f295e138761a8094550447848ed3453f44cca30147ed2d1059655a081dace0b`  
		Last Modified: Thu, 20 Feb 2020 23:40:04 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; arm variant v7

```console
$ docker pull composer@sha256:e465d2d7e511a179c05a0d23f275aa6fa2e2579a9dafc3633d9c9030464f029c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60149124 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f26995b67cbf60dd99f2ed49a91a5f94b24295cec520d2909d94dfff4031adec`
-	Entrypoint: `["\/bin\/sh","\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:21:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 18 Jan 2020 05:22:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 18 Jan 2020 05:22:16 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 05:22:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 18 Jan 2020 05:22:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 18 Jan 2020 05:22:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 05:22:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 05:22:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 18 Jan 2020 05:22:49 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 20 Feb 2020 21:11:31 GMT
ENV PHP_VERSION=7.4.3
# Thu, 20 Feb 2020 21:11:32 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.3.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.3.tar.xz.asc/from/this/mirror
# Thu, 20 Feb 2020 21:11:32 GMT
ENV PHP_SHA256=cf1f856d877c268124ded1ede40c9fb6142b125fdaafdc54f855120b8bc6982a PHP_MD5=
# Thu, 20 Feb 2020 21:11:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 20 Feb 2020 21:11:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 20 Feb 2020 21:13:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 20 Feb 2020 21:13:59 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Thu, 20 Feb 2020 21:14:01 GMT
RUN docker-php-ext-enable sodium
# Thu, 20 Feb 2020 21:14:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 20 Feb 2020 21:14:02 GMT
CMD ["php" "-a"]
# Fri, 21 Feb 2020 00:25:46 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 21 Feb 2020 00:26:06 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 21 Feb 2020 00:26:10 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 21 Feb 2020 00:26:12 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 21 Feb 2020 00:26:12 GMT
ENV COMPOSER_HOME=/tmp
# Fri, 21 Feb 2020 00:26:14 GMT
ENV COMPOSER_VERSION=1.9.3
# Fri, 21 Feb 2020 00:26:17 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Fri, 21 Feb 2020 00:26:18 GMT
COPY file:098af1c9d6ed00c2f357827391da1b2b0978915db35f033349301c7cbe78010d in /docker-entrypoint.sh 
# Fri, 21 Feb 2020 00:26:19 GMT
WORKDIR /app
# Fri, 21 Feb 2020 00:26:20 GMT
ENTRYPOINT ["/bin/sh" "/docker-entrypoint.sh"]
# Fri, 21 Feb 2020 00:26:21 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eecb809efefba021b07183ae486164fd475667a42a78ab308bd01b8d7dd8c1e`  
		Last Modified: Sat, 18 Jan 2020 06:09:11 GMT  
		Size: 1.2 MB (1227271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6ec95513b0eab50a07131cbee828abed358fb86fd276018e1bae6f04611ed9`  
		Last Modified: Sat, 18 Jan 2020 06:09:10 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459d1b57d2f034e68934a4116a4434479186cfce56d1235af4f1c1b9de08acbc`  
		Last Modified: Sat, 18 Jan 2020 06:09:08 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c492689366599e65cb0add947004a2dba1350bb15c7e6d5cf0926aba55ce6ec`  
		Last Modified: Thu, 20 Feb 2020 23:26:18 GMT  
		Size: 10.3 MB (10280256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e5617623e9ad0a01e633e336a37f6ff4d4a71c6cb1277692357d52303452d2f`  
		Last Modified: Thu, 20 Feb 2020 23:26:17 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4302d0c4f38943fda60770816f7eba1edb1d2f6a0c6f489e97ba67d9bdad574`  
		Last Modified: Thu, 20 Feb 2020 23:26:22 GMT  
		Size: 12.8 MB (12751449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fc244875b6924b539df26879b4496e91b8eee4f5000e1ea5b774d83b9546b93`  
		Last Modified: Thu, 20 Feb 2020 23:26:18 GMT  
		Size: 2.2 KB (2214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04543010f9cd746143ced265c7b4b63d09ddc611588a131cbafe2099993fb5eb`  
		Last Modified: Thu, 20 Feb 2020 23:26:17 GMT  
		Size: 72.7 KB (72683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f12c5ab65e2a603a37cb38a03c18050c2dbd142b9649dce2f7a64aba7b7640d8`  
		Last Modified: Fri, 21 Feb 2020 00:27:03 GMT  
		Size: 32.6 MB (32630447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af88c21669dd599df800e8d06657e64676f53a9aaf4a145253093716fc4e699e`  
		Last Modified: Fri, 21 Feb 2020 00:26:49 GMT  
		Size: 264.9 KB (264867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:407d2599e3950af3e6a6946ff942cb77334a4050a0eb5667af00b5dfabd870a8`  
		Last Modified: Fri, 21 Feb 2020 00:26:49 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc1b6f8226a00b699176d7e435c48c352b521aa6be9437d1ac40df4dd3bc107`  
		Last Modified: Fri, 21 Feb 2020 00:26:50 GMT  
		Size: 497.4 KB (497415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cee739a7af1b03efdbaaf1139d1ad1c169d6fbebb44e3c7313f0f5c4b30ef6fd`  
		Last Modified: Fri, 21 Feb 2020 00:26:49 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3956a8f2dde939b03006d4b552e251eb5adca823327190a6290d908e8c4758ae`  
		Last Modified: Fri, 21 Feb 2020 00:26:49 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:addf7b4ab545ceb2e9c95f041466c36b14827f65268d663a00a74ed7a78c0d42
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64748105 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a40d26d26c71224142f0e6c9997f8666ac483647cbac216796ce38a5415db8cc`
-	Entrypoint: `["\/bin\/sh","\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

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
# Fri, 24 Jan 2020 00:09:58 GMT
ENV PHP_VERSION=7.4.2
# Fri, 24 Jan 2020 00:10:02 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Fri, 24 Jan 2020 00:10:03 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Fri, 24 Jan 2020 00:10:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 24 Jan 2020 00:10:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 24 Jan 2020 00:14:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 24 Jan 2020 00:14:05 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Fri, 24 Jan 2020 00:14:09 GMT
RUN docker-php-ext-enable sodium
# Fri, 24 Jan 2020 00:14:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 24 Jan 2020 00:14:11 GMT
CMD ["php" "-a"]
# Fri, 24 Jan 2020 02:53:48 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 24 Jan 2020 02:54:06 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 24 Jan 2020 02:54:08 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 24 Jan 2020 02:54:09 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 24 Jan 2020 02:54:09 GMT
ENV COMPOSER_HOME=/tmp
# Wed, 05 Feb 2020 00:39:38 GMT
ENV COMPOSER_VERSION=1.9.3
# Wed, 05 Feb 2020 00:39:43 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Wed, 05 Feb 2020 00:39:43 GMT
COPY file:098af1c9d6ed00c2f357827391da1b2b0978915db35f033349301c7cbe78010d in /docker-entrypoint.sh 
# Wed, 05 Feb 2020 00:39:44 GMT
WORKDIR /app
# Wed, 05 Feb 2020 00:39:44 GMT
ENTRYPOINT ["/bin/sh" "/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 00:39:45 GMT
CMD ["composer"]
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
	-	`sha256:aa724be546925194dbbb305717c1ec1404bd825d4e768f5fa30758fc836a1dda`  
		Last Modified: Fri, 24 Jan 2020 02:37:49 GMT  
		Size: 10.3 MB (10271109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b0bc8c61926931859ef4bf710fb73b709a407ca1086dfe704e7654934b4bdd`  
		Last Modified: Fri, 24 Jan 2020 02:37:45 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07be412705d63c11275e2018adae846b8861d4f678a21f2c43e2c22ae0bcee6d`  
		Last Modified: Fri, 24 Jan 2020 02:37:49 GMT  
		Size: 14.4 MB (14366228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cafd3dde7ad30752409223dc0b26b0a5f4fa98d9a875225e2566bd99806655`  
		Last Modified: Fri, 24 Jan 2020 02:37:45 GMT  
		Size: 2.2 KB (2216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59195632759b7e9a57fb9ac253284ecbea9055d01c12f9caa49d23ca8f40bc1c`  
		Last Modified: Fri, 24 Jan 2020 02:37:45 GMT  
		Size: 72.7 KB (72676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9615657f0c002721450ed083349a10e4e4f5d642ec621cb26ab776e262dccacb`  
		Last Modified: Fri, 24 Jan 2020 02:54:59 GMT  
		Size: 35.2 MB (35177383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:922fe86012efc9b29ffe0e1f2b72c9b0957a389cc954245524f67f1b76b9254b`  
		Last Modified: Fri, 24 Jan 2020 02:54:46 GMT  
		Size: 275.6 KB (275616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f22723ecccd4084f9b254f40802a5b4580f38ac5289e4188ca324a241251089`  
		Last Modified: Fri, 24 Jan 2020 02:54:46 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdcb1294f078bfbfe1f250aeb9945ea1120356f685e60ab4fdb735e7d5de719e`  
		Last Modified: Wed, 05 Feb 2020 00:40:02 GMT  
		Size: 497.4 KB (497415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34301f0285a57957f3d334012bcf6bb69f3a3e454737d1aea18559eb12853a9`  
		Last Modified: Wed, 05 Feb 2020 00:40:00 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81a84752d23f3f01965cf6a195623db46015afd4f3e158f9ff10df1fe60e5f2`  
		Last Modified: Wed, 05 Feb 2020 00:40:00 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; 386

```console
$ docker pull composer@sha256:2dc88c8bb9a5ec3e37f8e384a0c00b808bb1d2986c9e8238420ed5014d1c7ae0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66721677 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f98137d1145162897d9780334718f359879dcd58e84afbf4a7dd7830386cf7`
-	Entrypoint: `["\/bin\/sh","\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:41:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 18 Jan 2020 05:41:36 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 18 Jan 2020 05:41:37 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 05:41:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 18 Jan 2020 05:41:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 18 Jan 2020 05:41:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 05:41:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 05:41:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 18 Jan 2020 05:41:39 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jan 2020 23:13:49 GMT
ENV PHP_VERSION=7.4.2
# Thu, 23 Jan 2020 23:13:49 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 23:13:49 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Thu, 23 Jan 2020 23:13:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 23 Jan 2020 23:13:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 23:21:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 23:21:57 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Thu, 23 Jan 2020 23:21:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 23:21:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 23:22:00 GMT
CMD ["php" "-a"]
# Fri, 24 Jan 2020 08:22:35 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 24 Jan 2020 08:22:51 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 24 Jan 2020 08:22:52 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 24 Jan 2020 08:22:53 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 24 Jan 2020 08:22:53 GMT
ENV COMPOSER_HOME=/tmp
# Wed, 05 Feb 2020 00:38:22 GMT
ENV COMPOSER_VERSION=1.9.3
# Wed, 05 Feb 2020 00:38:24 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Wed, 05 Feb 2020 00:38:25 GMT
COPY file:098af1c9d6ed00c2f357827391da1b2b0978915db35f033349301c7cbe78010d in /docker-entrypoint.sh 
# Wed, 05 Feb 2020 00:38:25 GMT
WORKDIR /app
# Wed, 05 Feb 2020 00:38:25 GMT
ENTRYPOINT ["/bin/sh" "/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 00:38:26 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6686b8c2d7ff02237fc9b12daa86e7e7328b7031b6585a20cd6b5fd618f77486`  
		Last Modified: Sat, 18 Jan 2020 06:45:55 GMT  
		Size: 1.5 MB (1452582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564ce419d6f56887ea2bd9699c37517ecd579e747f1a2698e764ad6f74e66b4c`  
		Last Modified: Sat, 18 Jan 2020 06:45:54 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694ef48cddae433ef86445fc9786eb75673c1c0c6d903fd7a81b2c56fb7e1b86`  
		Last Modified: Sat, 18 Jan 2020 06:45:54 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3628b223c4b093cf7c2d7723ccd39dfcb6977a659c9c183e7673f22f44865b`  
		Last Modified: Fri, 24 Jan 2020 02:36:11 GMT  
		Size: 10.3 MB (10271099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e167c61f346105deafdbe6bff7f521715a3d31cd4c9ca27d6dca67654d916c`  
		Last Modified: Fri, 24 Jan 2020 02:36:08 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53425617927914b1561c930b3ce2f90644de41394e731ca71a5d66feeba55d5b`  
		Last Modified: Fri, 24 Jan 2020 02:36:19 GMT  
		Size: 15.0 MB (14974599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809347a8b4ae69caee1b666ac61ec86e0f2dd5d64744592a59f65fd9bb49c7c9`  
		Last Modified: Fri, 24 Jan 2020 02:36:10 GMT  
		Size: 2.2 KB (2216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31917077d16c99b9c58e44f9267cbda55763d759a59379d7e4ca1f9fd6acf60a`  
		Last Modified: Fri, 24 Jan 2020 02:36:09 GMT  
		Size: 72.3 KB (72331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edbb819400a4408b8ee64894de00a5e9665d253fa003d1f63f0b9d96f114ff6d`  
		Last Modified: Fri, 24 Jan 2020 08:23:42 GMT  
		Size: 36.3 MB (36349747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ad7ee897f84efc8378a059a418c1026db0c674ffd33fb66b3886409622db7d`  
		Last Modified: Fri, 24 Jan 2020 08:23:18 GMT  
		Size: 292.3 KB (292291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc4f29430e372325c9d2467e48b0c59094feb4c82f8a1efae605753eea36da9c`  
		Last Modified: Fri, 24 Jan 2020 08:23:18 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68de0e93252fbd06b13a637c87060690e039fdefb5e3022aaafc6e9d9e4b7971`  
		Last Modified: Wed, 05 Feb 2020 00:38:41 GMT  
		Size: 497.4 KB (497398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfc7c1fc1916f608623a218251459aa48ec97b74637ae54b4062fda54eb7dabe`  
		Last Modified: Wed, 05 Feb 2020 00:38:41 GMT  
		Size: 554.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad7fba29d1184ca7929ab1f0ea1f09e3c52a6fd2caf37b74696f3eb12d7e69f0`  
		Last Modified: Wed, 05 Feb 2020 00:38:41 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; ppc64le

```console
$ docker pull composer@sha256:42f5a5425d8fcd1a6d756f5edaf70517986ed2be2ad77a4e4eeb85aa136d5cc3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66895004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc6b0d6196eecb61a182270f30a5b80b8617a51fb5e5c759ff37b3c276c9e8f3`
-	Entrypoint: `["\/bin\/sh","\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:24:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 18 Jan 2020 03:24:16 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 18 Jan 2020 03:24:20 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:24:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 18 Jan 2020 03:24:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 18 Jan 2020 03:24:28 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 03:24:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 03:24:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 18 Jan 2020 03:24:34 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jan 2020 23:32:44 GMT
ENV PHP_VERSION=7.4.2
# Thu, 23 Jan 2020 23:32:47 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 23:32:50 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Thu, 23 Jan 2020 23:33:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 23 Jan 2020 23:33:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 23:36:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 23:36:54 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Thu, 23 Jan 2020 23:37:00 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 23:37:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 23:37:04 GMT
CMD ["php" "-a"]
# Fri, 24 Jan 2020 05:49:01 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 24 Jan 2020 05:49:18 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 24 Jan 2020 05:49:23 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 24 Jan 2020 05:49:26 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 24 Jan 2020 05:49:28 GMT
ENV COMPOSER_HOME=/tmp
# Wed, 05 Feb 2020 00:16:59 GMT
ENV COMPOSER_VERSION=1.9.3
# Wed, 05 Feb 2020 00:17:09 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Wed, 05 Feb 2020 00:17:11 GMT
COPY file:098af1c9d6ed00c2f357827391da1b2b0978915db35f033349301c7cbe78010d in /docker-entrypoint.sh 
# Wed, 05 Feb 2020 00:17:14 GMT
WORKDIR /app
# Wed, 05 Feb 2020 00:17:15 GMT
ENTRYPOINT ["/bin/sh" "/docker-entrypoint.sh"]
# Wed, 05 Feb 2020 00:17:17 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccdcd97be351ef8da754f6efea3745b7060b1fe92ab96e4b8f5ff85b6322da9`  
		Last Modified: Sat, 18 Jan 2020 04:12:49 GMT  
		Size: 1.4 MB (1397881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea78a138902aeee431e9b31b236dfea5d4f95a1e155aada946ca57f6650a4da9`  
		Last Modified: Sat, 18 Jan 2020 04:12:49 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda899b5dd7be53564e6266c17b869d98468c50bc887279c51acacfa831de39f`  
		Last Modified: Sat, 18 Jan 2020 04:12:49 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24c1e693453ad6efa656fcfa28e76c0786f80b4467d83c277d1116117942973`  
		Last Modified: Fri, 24 Jan 2020 02:32:44 GMT  
		Size: 10.3 MB (10271124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb71fc05f0fe0d365d8b9891f304e0cf2c1f6f0d2200ecdc0ea9a1c569117a1d`  
		Last Modified: Fri, 24 Jan 2020 02:32:41 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf26116548345ee1f676a6c1fabb768cd60750eb7a3a0ac7f09724350dde3b1`  
		Last Modified: Fri, 24 Jan 2020 02:32:54 GMT  
		Size: 15.5 MB (15539990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4f870d6f2e6bbade33c0f28534b50765c4b56a093dc7565bd3ec3b37a7c603`  
		Last Modified: Fri, 24 Jan 2020 02:32:41 GMT  
		Size: 2.2 KB (2211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a738ee51d709e4c4db983f9206a240500a2fc0dbaf3c76f6da2f99e5f6eb3b`  
		Last Modified: Fri, 24 Jan 2020 02:32:41 GMT  
		Size: 73.0 KB (72992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dc5fc293a477499359971379d717f39675d5561f43d20385550b8957b1ab64e`  
		Last Modified: Fri, 24 Jan 2020 05:50:27 GMT  
		Size: 36.0 MB (35996362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a0c3b736bfb90c202775534c83c62fd8bf5aec90e784dc6e6be2b7e339692a5`  
		Last Modified: Fri, 24 Jan 2020 05:50:16 GMT  
		Size: 291.9 KB (291935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab440fd903567aa43375d7420843dbcb66394234442e5f38645e12166c6ee550`  
		Last Modified: Fri, 24 Jan 2020 05:50:16 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340c463507efcd04da3ce58cc918251b42318191d117b4f411caaf16bfa3ae7e`  
		Last Modified: Wed, 05 Feb 2020 00:17:34 GMT  
		Size: 497.4 KB (497423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d37b91d28b0c9120110fc0887baddbb8af128fdc5a138a0849bf3852ef3920`  
		Last Modified: Wed, 05 Feb 2020 00:17:34 GMT  
		Size: 556.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cd84842520fe40bbe8a752eeee5e6b68d58fc1e872d3d2a7b0737f082442314`  
		Last Modified: Wed, 05 Feb 2020 00:17:34 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
