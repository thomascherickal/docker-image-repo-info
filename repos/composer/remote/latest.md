## `composer:latest`

```console
$ docker pull composer@sha256:be48a5151b396fbe56d3cbbb75ffa6d8a80dc922ab869f3c73a4ef91fd4bd9ad
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
$ docker pull composer@sha256:c2c6ccb0988e7be6acde712b0d31f7126cfd5a0abc1ff8eb97ccfb8634ac3b1c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.3 MB (63277708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6207092f41307553938f66a3bff2a1821cf7de961a46b4adf7a4441ad012475`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Thu, 22 Oct 2020 02:19:24 GMT
ADD file:f17f65714f703db9012f00e5ec98d0b2541ff6147c2633f7ab9ba659d0c507f4 in / 
# Thu, 22 Oct 2020 02:19:24 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 06:30:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 22 Oct 2020 06:30:14 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 22 Oct 2020 06:30:15 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 22 Oct 2020 06:30:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Oct 2020 06:30:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Oct 2020 06:30:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 06:30:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 06:30:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Oct 2020 06:43:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Oct 2020 22:35:02 GMT
ENV PHP_VERSION=7.4.12
# Thu, 29 Oct 2020 22:35:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.12.tar.xz.asc
# Thu, 05 Nov 2020 20:35:06 GMT
ENV PHP_SHA256=e82d2bcead05255f6b7d2ff4e2561bc334204955820cabc2457b5239fde96b76
# Thu, 05 Nov 2020 20:35:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 05 Nov 2020 20:35:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Nov 2020 20:43:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Nov 2020 20:43:36 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 05 Nov 2020 20:43:37 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Nov 2020 20:43:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Nov 2020 20:43:37 GMT
CMD ["php" "-a"]
# Fri, 06 Nov 2020 02:49:32 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 06 Nov 2020 02:49:42 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 06 Nov 2020 02:49:43 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 06 Nov 2020 02:49:43 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 06 Nov 2020 02:49:43 GMT
ENV COMPOSER_HOME=/tmp
# Mon, 16 Nov 2020 19:23:18 GMT
ENV COMPOSER_VERSION=2.0.7
# Mon, 16 Nov 2020 19:23:19 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Mon, 16 Nov 2020 19:23:19 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Mon, 16 Nov 2020 19:23:20 GMT
WORKDIR /app
# Mon, 16 Nov 2020 19:23:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Nov 2020 19:23:20 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:188c0c94c7c576fff0792aca7ec73d67a2f7f4cb3a6e53a84559337260b36964`  
		Last Modified: Thu, 22 Oct 2020 02:19:57 GMT  
		Size: 2.8 MB (2796860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45f8bf6cfdbe614fef94f982905079c16e27b3de2d24eb1ff513d3d83e656ca2`  
		Last Modified: Thu, 22 Oct 2020 07:36:55 GMT  
		Size: 1.3 MB (1340771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce5be79740125b9e74a77885bf6ee2b0d25ac7ed9e9432c5aa7210bb3b00458a`  
		Last Modified: Thu, 22 Oct 2020 07:36:55 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99dd6507fe563b66ba35badf706e1bbb2d39eb5d0a3c0d5a86a45d2af7e89c1`  
		Last Modified: Thu, 22 Oct 2020 07:36:55 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84ab7a98c2ef9382ba6cf0fc5a9987d6e32a81832e54241be956471c98ce2088`  
		Last Modified: Fri, 06 Nov 2020 01:29:54 GMT  
		Size: 10.3 MB (10330812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07fa46c284ad61140e5ce3ac01798895f0edecbbbce228b86ccfc667dad36d6b`  
		Last Modified: Fri, 06 Nov 2020 01:29:53 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ae9397c88ea7dfdab00f9699013044c2631ee7c62c839411c1c111c3408c324`  
		Last Modified: Fri, 06 Nov 2020 01:29:58 GMT  
		Size: 14.2 MB (14183042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4748577090d68f9af19983928b0fb9fb2323318240fb214c4c7f1e2b42279b`  
		Last Modified: Fri, 06 Nov 2020 01:29:53 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36fcf1c47c045c21c5c9a53d4cefd85e291836fcea324b721d0b802f566bb1c2`  
		Last Modified: Fri, 06 Nov 2020 01:29:53 GMT  
		Size: 16.9 KB (16894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e7ab985a9bda3eaa74105e5c5275bbb1907152463c919d389a6399eea368b41`  
		Last Modified: Fri, 06 Nov 2020 02:50:13 GMT  
		Size: 33.9 MB (33862856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587323d75f78e9e8213c235befaccf69ddd6b86ec9b5677fab5e32709a3e181f`  
		Last Modified: Fri, 06 Nov 2020 02:50:05 GMT  
		Size: 189.3 KB (189279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d927604c025a4d1bc228608c30d3556822c5e59db33c49f1780e70976b68ca0`  
		Last Modified: Fri, 06 Nov 2020 02:50:05 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:083992f957e512f5d364f6161af9cd438bee25869ed4e6f54c2bb441da8da4cb`  
		Last Modified: Mon, 16 Nov 2020 19:23:33 GMT  
		Size: 552.2 KB (552225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e563cb1d5fd63759a5a565efadef1175e9a81c0c9742d577491bcc4e48f7ac8`  
		Last Modified: Mon, 16 Nov 2020 19:23:33 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef10c81512098b0e5decc878803026a0f62bb780cb18d75cf8d442641af1452`  
		Last Modified: Mon, 16 Nov 2020 19:23:33 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; arm variant v6

```console
$ docker pull composer@sha256:e09391cd49758a728452bbe232f1c67eb7fa23169c4e0a2f552742c2b6eb307b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.1 MB (60083802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:92e93cfbe482ac3ddad07a6c75ffc6399360734d27aeb22a32f1c76e628f7b35`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:09 GMT
ADD file:dec4d3b6cf21c59820d1d74a554d0a193b5f4859e00b932f31ffe73f554d5afb in / 
# Thu, 22 Oct 2020 02:01:12 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 06:41:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 22 Oct 2020 06:41:56 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 22 Oct 2020 06:42:00 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 22 Oct 2020 06:42:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Oct 2020 06:42:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Oct 2020 06:42:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 06:42:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 06:42:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Oct 2020 06:50:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 01 Dec 2020 01:59:03 GMT
ENV PHP_VERSION=7.4.13
# Tue, 01 Dec 2020 01:59:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.13.tar.xz.asc
# Tue, 01 Dec 2020 01:59:08 GMT
ENV PHP_SHA256=aead303e3abac23106529560547baebbedba0bb2943b91d5aa08fff1f41680f4
# Tue, 01 Dec 2020 01:59:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 01 Dec 2020 01:59:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Dec 2020 02:02:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Dec 2020 02:02:54 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Tue, 01 Dec 2020 02:02:57 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Dec 2020 02:02:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Dec 2020 02:03:02 GMT
CMD ["php" "-a"]
# Tue, 01 Dec 2020 03:12:11 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Tue, 01 Dec 2020 03:12:37 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Tue, 01 Dec 2020 03:12:41 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Tue, 01 Dec 2020 03:12:42 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Tue, 01 Dec 2020 03:12:43 GMT
ENV COMPOSER_HOME=/tmp
# Tue, 01 Dec 2020 03:12:44 GMT
ENV COMPOSER_VERSION=2.0.7
# Tue, 01 Dec 2020 03:12:47 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Tue, 01 Dec 2020 03:12:48 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Tue, 01 Dec 2020 03:12:48 GMT
WORKDIR /app
# Tue, 01 Dec 2020 03:12:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 01 Dec 2020 03:12:50 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:bad30e7b45c14f784ef29a828b5fc69db0ebdefebcde6a7c98f4f77ffc93a546`  
		Last Modified: Thu, 22 Oct 2020 02:01:42 GMT  
		Size: 2.6 MB (2601912 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba9bf946cf0a5f710967e36dd17cee52857cd6bda3def477e4f23823071a310d`  
		Last Modified: Thu, 22 Oct 2020 07:36:00 GMT  
		Size: 1.3 MB (1310155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fedfce6787031ac99140460dc123850a8ced1bdf113b93150f3c0a99891a588`  
		Last Modified: Thu, 22 Oct 2020 07:35:58 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2498251eae8b7a8b7d6fae9311ceec47f607cc852ba45c073a4fe55bf917b819`  
		Last Modified: Thu, 22 Oct 2020 07:35:58 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e674e6efb9d069a0159ccc3c4941a5f08d20360aba50d7e232c471e26ca607d8`  
		Last Modified: Tue, 01 Dec 2020 02:53:05 GMT  
		Size: 10.3 MB (10338595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a02b648f7778bfa410ed3adc8a6adf9af5a1d60272d3324d62d91c415185361`  
		Last Modified: Tue, 01 Dec 2020 02:53:03 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b62f92d21d14f0171b42a23823e14a5b4c991c050e74ab201677a756ea6e9b8f`  
		Last Modified: Tue, 01 Dec 2020 02:53:09 GMT  
		Size: 13.6 MB (13583295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f15f32492fdfa7bd7fe7400e832df4050c35c4dfafcceb8ea7003939b26f302`  
		Last Modified: Tue, 01 Dec 2020 02:53:03 GMT  
		Size: 2.3 KB (2260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:279191cd3478b6f6c4be4c2196ea47d7ae11bd2dc5c8c31d430d7da4b53990ed`  
		Last Modified: Tue, 01 Dec 2020 02:53:03 GMT  
		Size: 16.9 KB (16924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127dab053d505004930ec7b80e090e4830073dcc0d6ade49e47c4cee36b9c849`  
		Last Modified: Tue, 01 Dec 2020 03:13:30 GMT  
		Size: 31.5 MB (31490591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ac68c1f7da271e8359b207c8f63fb2dd37bc8f4ddf99ddc04f3e5c608fad14`  
		Last Modified: Tue, 01 Dec 2020 03:13:17 GMT  
		Size: 185.0 KB (184997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e824b220051307f1b162a42431c076073ed0e4b10015051c08ca29a4a290dd7`  
		Last Modified: Tue, 01 Dec 2020 03:13:17 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744037e6fbab35cac2f1d061176449d66b16b6a22365c270093d7a2ffa5f97eb`  
		Last Modified: Tue, 01 Dec 2020 03:13:18 GMT  
		Size: 552.3 KB (552256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b620d648a964fc9b3f5a9a66c1de18f992c790ad139528dd1aa35db62b884048`  
		Last Modified: Tue, 01 Dec 2020 03:13:17 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e8b50f0b48ea8badda25b67850ace5d5b827fb097647d45a04828c59228dbf`  
		Last Modified: Tue, 01 Dec 2020 03:13:18 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; arm variant v7

```console
$ docker pull composer@sha256:48a3df94666ab8a3591d8efceb90845028510210fd71506648e1a7ba89c1ce9e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.4 MB (57362004 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:562eec41de4ee6cd07fb6935b409db46c6fa6a913412fde4ab42bce0b981c1f5`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Thu, 22 Oct 2020 01:58:13 GMT
ADD file:46f89172426e9f5b1d669a2ca7ab218fc2deaef1caeeab88f2b5bd443ac9773d in / 
# Thu, 22 Oct 2020 01:58:14 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 06:47:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 22 Oct 2020 06:47:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 22 Oct 2020 06:47:45 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 22 Oct 2020 06:47:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Oct 2020 06:47:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Oct 2020 06:47:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 06:47:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 06:48:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Oct 2020 06:56:26 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 01 Dec 2020 02:39:45 GMT
ENV PHP_VERSION=7.4.13
# Tue, 01 Dec 2020 02:39:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.13.tar.xz.asc
# Tue, 01 Dec 2020 02:39:46 GMT
ENV PHP_SHA256=aead303e3abac23106529560547baebbedba0bb2943b91d5aa08fff1f41680f4
# Tue, 01 Dec 2020 02:39:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 01 Dec 2020 02:39:53 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Dec 2020 02:42:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Dec 2020 02:42:32 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Tue, 01 Dec 2020 02:42:37 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Dec 2020 02:42:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Dec 2020 02:42:40 GMT
CMD ["php" "-a"]
# Tue, 01 Dec 2020 04:25:49 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Tue, 01 Dec 2020 04:26:07 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Tue, 01 Dec 2020 04:26:10 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Tue, 01 Dec 2020 04:26:16 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Tue, 01 Dec 2020 04:26:19 GMT
ENV COMPOSER_HOME=/tmp
# Tue, 01 Dec 2020 04:26:21 GMT
ENV COMPOSER_VERSION=2.0.7
# Tue, 01 Dec 2020 04:26:31 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Tue, 01 Dec 2020 04:26:33 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Tue, 01 Dec 2020 04:26:34 GMT
WORKDIR /app
# Tue, 01 Dec 2020 04:26:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Tue, 01 Dec 2020 04:26:36 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:5f2023fd85a4e68f37fe41421fd89f30e69b98a645613521c57c01317561eee3`  
		Last Modified: Thu, 22 Oct 2020 01:58:45 GMT  
		Size: 2.4 MB (2405675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c60b50c98f8a8e2c6a27378dfa0f44df1844ac67c6981303675f138a42679f25`  
		Last Modified: Thu, 22 Oct 2020 07:35:57 GMT  
		Size: 1.2 MB (1214265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b472094d673b7c272085505c976192b9aaafa3157c99bade9755fbca18a24071`  
		Last Modified: Thu, 22 Oct 2020 07:35:56 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcc39e5d916c11e7eb158e72d14ab981eb45ccc7b6451c1d6d3cb627b71cdbb6`  
		Last Modified: Thu, 22 Oct 2020 07:35:55 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e834fd39435ea86b08faf9b3af2e2623e0a247fa06dfe096decdf80f7a986a`  
		Last Modified: Tue, 01 Dec 2020 04:00:44 GMT  
		Size: 10.3 MB (10338583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a458e4d5704bca7330dbfab239f74ff255f4813b58f19f50a4ad7fd7087f0c8`  
		Last Modified: Tue, 01 Dec 2020 04:00:43 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a500121bbd97abb5116b6e95bdaa9aed74160334e46aadaabef548dca0edce6`  
		Last Modified: Tue, 01 Dec 2020 04:00:46 GMT  
		Size: 12.7 MB (12706582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3321b09ca6255e6f5cb4dce9057df675dd4644a3654424c7ee95fbdcb083e9c`  
		Last Modified: Tue, 01 Dec 2020 04:00:42 GMT  
		Size: 2.3 KB (2257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:345450fde280cf49e34f7246cebd38e311d4b7bebe22415a6126c18e67899f91`  
		Last Modified: Tue, 01 Dec 2020 04:00:42 GMT  
		Size: 16.9 KB (16903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61c211566c153b566fb046b601bacfbc3f5c8bb124fee4c6a58a1cb232992185`  
		Last Modified: Tue, 01 Dec 2020 04:27:17 GMT  
		Size: 29.9 MB (29943908 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f2127cee04865b730706eaadda98cbe00cfa69690c3587ed3067377170a802`  
		Last Modified: Tue, 01 Dec 2020 04:27:06 GMT  
		Size: 178.8 KB (178754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28e1bad24086ecc1216d8c4feceb4808c923e2617519f749f03cba2ef437406c`  
		Last Modified: Tue, 01 Dec 2020 04:27:06 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d64599db79a604bedb55ba298bfb1ab035358aa8d24ed2fa2156ff98b145b2`  
		Last Modified: Tue, 01 Dec 2020 04:27:06 GMT  
		Size: 552.3 KB (552259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed748aafb9b12e3f423170800c3ace75ff173a770e2f6dd19d592422b482b12`  
		Last Modified: Tue, 01 Dec 2020 04:27:06 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91302676871ad2073c4638fa2f2ba200bdb1e34ca21bc412df3ee0916db39d1`  
		Last Modified: Tue, 01 Dec 2020 04:27:06 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:6e011372684eedab1a86355ede8e01029e6f91c10d0754f02aa5e3b53e6971ce
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63360843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aab6beb7501418a7163e8ea739ec23d85a030be1240496d084400f570e2827ec`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Thu, 22 Oct 2020 02:01:01 GMT
ADD file:55c4e9752146061a2b5f76027221329f423687987c0744ef577130c60ff0ba42 in / 
# Thu, 22 Oct 2020 02:01:06 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 07:18:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 22 Oct 2020 07:18:56 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 22 Oct 2020 07:18:59 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 22 Oct 2020 07:19:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Oct 2020 07:19:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Oct 2020 07:19:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 07:19:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 07:19:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Oct 2020 07:27:59 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Oct 2020 22:25:19 GMT
ENV PHP_VERSION=7.4.12
# Thu, 29 Oct 2020 22:25:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.12.tar.xz.asc
# Thu, 05 Nov 2020 19:51:05 GMT
ENV PHP_SHA256=e82d2bcead05255f6b7d2ff4e2561bc334204955820cabc2457b5239fde96b76
# Thu, 05 Nov 2020 19:51:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 05 Nov 2020 19:51:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Nov 2020 19:54:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Nov 2020 19:55:01 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 05 Nov 2020 19:55:04 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Nov 2020 19:55:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Nov 2020 19:55:06 GMT
CMD ["php" "-a"]
# Thu, 05 Nov 2020 22:19:49 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 05 Nov 2020 22:20:07 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 05 Nov 2020 22:20:09 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 05 Nov 2020 22:20:10 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 05 Nov 2020 22:20:11 GMT
ENV COMPOSER_HOME=/tmp
# Mon, 16 Nov 2020 19:39:32 GMT
ENV COMPOSER_VERSION=2.0.7
# Mon, 16 Nov 2020 19:39:48 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Mon, 16 Nov 2020 19:39:49 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Mon, 16 Nov 2020 19:39:50 GMT
WORKDIR /app
# Mon, 16 Nov 2020 19:39:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Nov 2020 19:39:51 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:5f621e34cdf485f410766dc9a0fc7855d17916d0f6583b58cbdce7c28831f527`  
		Last Modified: Thu, 22 Oct 2020 02:01:38 GMT  
		Size: 2.7 MB (2706555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d57dba23203172f8fffd1379aef0307e782178b62dfc684d43c546f7e874ed`  
		Last Modified: Thu, 22 Oct 2020 08:06:21 GMT  
		Size: 1.3 MB (1342784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8414edb0c9c2f7472bb6228bf691a2ddac19ddad7bad789c7cbdc147aded711`  
		Last Modified: Thu, 22 Oct 2020 08:06:20 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d26eeef0db35b2328adae38a8490c7403844452c3606dd17fbe68216f98e82`  
		Last Modified: Thu, 22 Oct 2020 08:06:19 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e318e25edf7eaf77d8a3b344dbdd4531041889f0c5ed7cd5dcacc8119556681`  
		Last Modified: Thu, 05 Nov 2020 21:50:58 GMT  
		Size: 10.3 MB (10330840 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e186db7628fb2a3edf41cf79946418d166452fd292ae64a10e2e425fce234e3`  
		Last Modified: Thu, 05 Nov 2020 21:50:56 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc28adcdc367df0e66ea09e866001068f3d4b2a4c5d31c3f83c4db9619f54ca`  
		Last Modified: Thu, 05 Nov 2020 21:51:01 GMT  
		Size: 14.0 MB (13995566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb111a3fbebad22e4be1f598dabd780a6e68931957ca53233cbb5bbd1e30b394`  
		Last Modified: Thu, 05 Nov 2020 21:50:56 GMT  
		Size: 2.3 KB (2260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a16c1fb112fd142189eac791e82bb9c1c36f886751b9bcd56ff401bf0e78b01`  
		Last Modified: Thu, 05 Nov 2020 21:50:56 GMT  
		Size: 16.9 KB (16894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dae51005a5627db9f85a2c3f5f03f4eeb0ca8639cb49fa2b776f594d33c033e9`  
		Last Modified: Thu, 05 Nov 2020 22:21:05 GMT  
		Size: 34.2 MB (34222855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f4f5694f14f9d8557fd14b1a5e6cd524bab3b5d4bbd9bd2b9c29e4c3b2d6ff`  
		Last Modified: Thu, 05 Nov 2020 22:20:55 GMT  
		Size: 188.0 KB (188012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3637e53950aaa1d4a998b36fae9f43f07921a9cac6606a3531aae0fd874b301`  
		Last Modified: Thu, 05 Nov 2020 22:20:54 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0ba08bd3e0ed1e055fe1ba4e02dee6f9d0ca783c914f69ed05929dc31ad565e`  
		Last Modified: Mon, 16 Nov 2020 19:40:08 GMT  
		Size: 552.3 KB (552263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89ad771259d34c73e7636c5c5ca230998df739b1821ffab3ae1b44e356d24c96`  
		Last Modified: Mon, 16 Nov 2020 19:40:08 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f632b6fc1a1ce12fdbd4b44e497d8ba5d46da3c5f339e475108ba051ea18315d`  
		Last Modified: Mon, 16 Nov 2020 19:39:55 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; 386

```console
$ docker pull composer@sha256:225f592d02932773d3a90334964f5be60f63d0451d98c8af9c0973a73b3d8864
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.4 MB (65367804 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6207ad6f0b79d70f3abd3b9d86c052b8bb4c3a6d9ee7df449c9060d6b90de728`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Thu, 22 Oct 2020 02:00:33 GMT
ADD file:46ad43b4984bcf49c5a888ff3628f23161f55cd1fb062f469e707100c97fa254 in / 
# Thu, 22 Oct 2020 02:00:33 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 03:36:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 22 Oct 2020 03:36:26 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 22 Oct 2020 03:36:27 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 22 Oct 2020 03:36:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Oct 2020 03:36:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Oct 2020 03:36:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 03:36:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 03:36:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Oct 2020 03:55:07 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Oct 2020 23:09:16 GMT
ENV PHP_VERSION=7.4.12
# Thu, 29 Oct 2020 23:09:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.12.tar.xz.asc
# Thu, 05 Nov 2020 21:09:24 GMT
ENV PHP_SHA256=e82d2bcead05255f6b7d2ff4e2561bc334204955820cabc2457b5239fde96b76
# Thu, 05 Nov 2020 21:09:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 05 Nov 2020 21:09:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Nov 2020 21:18:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Nov 2020 21:19:00 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 05 Nov 2020 21:19:01 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Nov 2020 21:19:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Nov 2020 21:19:01 GMT
CMD ["php" "-a"]
# Fri, 06 Nov 2020 03:41:10 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 06 Nov 2020 03:41:21 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 06 Nov 2020 03:41:21 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 06 Nov 2020 03:41:22 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 06 Nov 2020 03:41:22 GMT
ENV COMPOSER_HOME=/tmp
# Mon, 16 Nov 2020 19:38:26 GMT
ENV COMPOSER_VERSION=2.0.7
# Mon, 16 Nov 2020 19:38:27 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Mon, 16 Nov 2020 19:38:28 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Mon, 16 Nov 2020 19:38:28 GMT
WORKDIR /app
# Mon, 16 Nov 2020 19:38:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Nov 2020 19:38:28 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:d6ca64ac6f4b6382142ce9a3501652938130a6ec4bb02f3f455ee1f980834cfe`  
		Last Modified: Thu, 22 Oct 2020 02:00:57 GMT  
		Size: 2.8 MB (2791407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30be8ffd290910905a5fb7cbb70252eb0f59edb09db20bdc21f3b65456acc28f`  
		Last Modified: Thu, 22 Oct 2020 05:10:23 GMT  
		Size: 1.4 MB (1439641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8d58e2433b13446c863e85b34f8e4c93ca9d5b3b93d2bac415fd9cdf77bcec4`  
		Last Modified: Thu, 22 Oct 2020 05:10:21 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5729dcb8d303f82a7f8cf3df49048e34ce8ee89f79155fb08a475da46b64308`  
		Last Modified: Thu, 22 Oct 2020 05:10:21 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2d18f6e1563003e4112b372b0b1306a7936ca26aa28ab257b1ee7094eba114d`  
		Last Modified: Fri, 06 Nov 2020 02:13:47 GMT  
		Size: 10.3 MB (10330800 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57a4de1058294a64654dc6ab2482b2e6ac59e16603f5ef7e337feea1a1f94b92`  
		Last Modified: Fri, 06 Nov 2020 02:13:46 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5e387eefb852ad18d1623f4f7cc77473658e54aff501427c52ced9772472959`  
		Last Modified: Fri, 06 Nov 2020 02:13:53 GMT  
		Size: 14.6 MB (14566555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be3c7cd936a2573e7a67c512476449c663161bf0a5d38b4d58afe5359e643c0f`  
		Last Modified: Fri, 06 Nov 2020 02:13:46 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5d50a767bc960bbaa819f382b40f34e1ada8620ebb3567829fc549fb09c3078`  
		Last Modified: Fri, 06 Nov 2020 02:13:46 GMT  
		Size: 16.9 KB (16875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e05645ffe2af6040a65e7a64ed4d0db2a5f56b0b85d47b6ec382d9b327c881`  
		Last Modified: Fri, 06 Nov 2020 03:41:54 GMT  
		Size: 35.5 MB (35461731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:effe3bfc8dee4cce6b574dae63a647fa65f5a2a8959e5917346307d1bef1f61f`  
		Last Modified: Fri, 06 Nov 2020 03:41:43 GMT  
		Size: 203.6 KB (203610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc53bed8fd4a89c2f8539177cedff8559ffed5234fc0852aeb63a953c7ddd7a`  
		Last Modified: Fri, 06 Nov 2020 03:41:43 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbb092b227d0ac4f959bf53676f972e98966a405c3427a6d5d73d263035e40a3`  
		Last Modified: Mon, 16 Nov 2020 19:38:43 GMT  
		Size: 552.2 KB (552220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7199bab9e025f0d63769e9dafa440bf66b9c6a3b77a746b27ba26fcfbc7d7120`  
		Last Modified: Mon, 16 Nov 2020 19:38:43 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa7500542301904ff427c674ad4a0bb31e7df9db8203499fdfa39154f32db994`  
		Last Modified: Mon, 16 Nov 2020 19:38:43 GMT  
		Size: 92.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; ppc64le

```console
$ docker pull composer@sha256:46d0607e50bcd7dd192484211d8809a51800191b5b8f2404ee8f85b4947efb24
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.6 MB (65612694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9a285a1c12f2b81d5ff21ea93120bb69b7af8dea0e5903a5a564ff98328cec7`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Thu, 22 Oct 2020 11:00:06 GMT
ADD file:176e047fab2c1828575bffa6b14773efa297b7ecf312d86103c5dd4f78ec8027 in / 
# Thu, 22 Oct 2020 11:00:17 GMT
CMD ["/bin/sh"]
# Fri, 23 Oct 2020 00:21:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 23 Oct 2020 00:21:18 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 23 Oct 2020 00:21:30 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 23 Oct 2020 00:21:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 23 Oct 2020 00:21:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 23 Oct 2020 00:21:47 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 23 Oct 2020 00:21:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 23 Oct 2020 00:21:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 23 Oct 2020 00:34:37 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Oct 2020 22:58:44 GMT
ENV PHP_VERSION=7.4.12
# Thu, 29 Oct 2020 22:58:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.12.tar.xz.asc
# Thu, 05 Nov 2020 20:58:05 GMT
ENV PHP_SHA256=e82d2bcead05255f6b7d2ff4e2561bc334204955820cabc2457b5239fde96b76
# Thu, 05 Nov 2020 20:58:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 05 Nov 2020 20:58:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Nov 2020 21:02:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Nov 2020 21:02:17 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 05 Nov 2020 21:02:23 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Nov 2020 21:02:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Nov 2020 21:02:27 GMT
CMD ["php" "-a"]
# Fri, 06 Nov 2020 00:08:26 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Fri, 06 Nov 2020 00:09:06 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Fri, 06 Nov 2020 00:09:38 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Fri, 06 Nov 2020 00:09:49 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Fri, 06 Nov 2020 00:10:00 GMT
ENV COMPOSER_HOME=/tmp
# Mon, 16 Nov 2020 19:17:08 GMT
ENV COMPOSER_VERSION=2.0.7
# Mon, 16 Nov 2020 19:17:42 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Mon, 16 Nov 2020 19:17:46 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Mon, 16 Nov 2020 19:17:55 GMT
WORKDIR /app
# Mon, 16 Nov 2020 19:18:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Nov 2020 19:18:23 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:692a9d763e196c85d79fc3e45b316b1bb557c93ba88a3c8ebf679a585d1efe73`  
		Last Modified: Thu, 22 Oct 2020 11:02:06 GMT  
		Size: 2.8 MB (2803218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0285d6f06f3beb1c140c055210664c441b93dd4f2037177a5396bce94ca16ce5`  
		Last Modified: Fri, 23 Oct 2020 01:34:08 GMT  
		Size: 1.4 MB (1383187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6459a3bf272daa53ff4ba97cc849676f497de9f78d8e9378ec02552293f175`  
		Last Modified: Fri, 23 Oct 2020 01:34:07 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16cff6064dc29d3f629d353736c1cac074caa5b50738422adb84de99a019bb32`  
		Last Modified: Fri, 23 Oct 2020 01:34:08 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be0e2adb9ee15f41e12b4a620edb6754bef2f53293c42f8dd6e0ae18ca914f3`  
		Last Modified: Thu, 05 Nov 2020 23:40:25 GMT  
		Size: 10.3 MB (10330846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:731b57709a420b675b6782cb22c8cb0c5bc0b5b20926f48aae2285a45e7aec8e`  
		Last Modified: Thu, 05 Nov 2020 23:40:23 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05050fc6e5b8da8d950be3ca576071a305bac1ca44e663dd3542ff46433dc7bd`  
		Last Modified: Thu, 05 Nov 2020 23:40:30 GMT  
		Size: 15.2 MB (15156702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501d13ec8a1996615b91bb6ba0b88203c5123160040f8ef3ac7ecb2c673129e8`  
		Last Modified: Thu, 05 Nov 2020 23:40:24 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e751c7af550bf453347f25dac96de408f0557f54de7fd1d13df192103f0009c`  
		Last Modified: Thu, 05 Nov 2020 23:40:23 GMT  
		Size: 16.9 KB (16924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58a9e78d8921c22e0c86fe808e8e7d0092e67916418c94cf8c04cd3e34bfe587`  
		Last Modified: Fri, 06 Nov 2020 00:13:37 GMT  
		Size: 35.2 MB (35168906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3c8d6d418c64da300ecda25b4e1793b1549af58020b80a15492f3732a990965`  
		Last Modified: Fri, 06 Nov 2020 00:13:23 GMT  
		Size: 195.6 KB (195567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d0fc926c1bc018709d6e02f610e3fb0dc10b4f284aa2d1249d33b6f4f4b6c3`  
		Last Modified: Fri, 06 Nov 2020 00:13:23 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1cbab2a38e23b90044b0f8b0ff653ba0e12ff3a2493cd06ec7696ace1c17b0f`  
		Last Modified: Mon, 16 Nov 2020 19:19:05 GMT  
		Size: 552.3 KB (552265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9312404f11e9f9788080293f7594371cea1325d95c3f68642092721d73cb23c`  
		Last Modified: Mon, 16 Nov 2020 19:19:04 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72bd8da7ebc540592894239d16246f3a431a230ab8b213c579e4374d81567115`  
		Last Modified: Mon, 16 Nov 2020 19:19:04 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; s390x

```console
$ docker pull composer@sha256:8b57a6c53f582bdb5d33bee9b3b9b366a2192a235dad4fc72e8344601bb752e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.6 MB (62551950 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:437a66234e8014a7bf7e4de857b79970072e2f04470246c47eba1ab00dc744d6`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Thu, 22 Oct 2020 01:59:08 GMT
ADD file:e07d6f40b1afc3d3eff230bc89e84704eb762706a373a60c6bea6a45b2287464 in / 
# Thu, 22 Oct 2020 01:59:09 GMT
CMD ["/bin/sh"]
# Thu, 22 Oct 2020 04:34:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 22 Oct 2020 04:34:29 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 22 Oct 2020 04:34:31 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 22 Oct 2020 04:34:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 22 Oct 2020 04:34:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 22 Oct 2020 04:34:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 04:34:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 22 Oct 2020 04:34:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 22 Oct 2020 04:44:17 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 29 Oct 2020 22:20:50 GMT
ENV PHP_VERSION=7.4.12
# Thu, 29 Oct 2020 22:20:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.12.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.12.tar.xz.asc
# Thu, 05 Nov 2020 19:46:56 GMT
ENV PHP_SHA256=e82d2bcead05255f6b7d2ff4e2561bc334204955820cabc2457b5239fde96b76
# Thu, 05 Nov 2020 19:47:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 05 Nov 2020 19:47:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Nov 2020 19:50:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Nov 2020 19:50:53 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 05 Nov 2020 19:50:54 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Nov 2020 19:50:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Nov 2020 19:50:55 GMT
CMD ["php" "-a"]
# Thu, 05 Nov 2020 22:13:05 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 05 Nov 2020 22:13:19 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 05 Nov 2020 22:13:21 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 05 Nov 2020 22:13:21 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 05 Nov 2020 22:13:21 GMT
ENV COMPOSER_HOME=/tmp
# Mon, 16 Nov 2020 19:41:25 GMT
ENV COMPOSER_VERSION=2.0.7
# Mon, 16 Nov 2020 19:41:27 GMT
RUN set -eux;   curl --silent --fail --location --retry 3 --output /tmp/installer.php --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       unlink('/tmp/installer.php');       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }";   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Mon, 16 Nov 2020 19:41:27 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Mon, 16 Nov 2020 19:41:28 GMT
WORKDIR /app
# Mon, 16 Nov 2020 19:41:28 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Mon, 16 Nov 2020 19:41:29 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:a4c84ece3d2b98927d25f13a4f367bfd96cbfae272f6ff1117d74c84b92d11d3`  
		Last Modified: Thu, 22 Oct 2020 01:59:37 GMT  
		Size: 2.6 MB (2565829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18701639c0ce1824d9d9f426e7ad4ccdf2d7598bcb0d03c58a4c0bb7c992e3b7`  
		Last Modified: Thu, 22 Oct 2020 05:29:10 GMT  
		Size: 1.4 MB (1382560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8913bd186df85a9366fb2cdb38fcc79adf2a420106aae8406124ac8d0165e92f`  
		Last Modified: Thu, 22 Oct 2020 05:29:09 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870830cea28d819a5f749933d7ba6ce48296069aed28f02cd4d609284b3944c3`  
		Last Modified: Thu, 22 Oct 2020 05:29:09 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1102bb589a38ae090f6e986c40fcda34caf16d324363ffdde50b1495dd2ba1fe`  
		Last Modified: Thu, 05 Nov 2020 21:51:18 GMT  
		Size: 10.3 MB (10330839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c2ec46fdabdf7e196f67c2da8f9c5a7eeb5e6c1c88ba1e55cf50d47833543b`  
		Last Modified: Thu, 05 Nov 2020 21:51:18 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f307ad94d99bb17db081d88cbb593a9da80ff7c3d26cf99181673786f37025`  
		Last Modified: Thu, 05 Nov 2020 21:51:19 GMT  
		Size: 13.5 MB (13485163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:860dbdb7a9f964c29d06c5969237bb792c9a4d69cb58ffe10507538c9062ea0e`  
		Last Modified: Thu, 05 Nov 2020 21:51:19 GMT  
		Size: 2.3 KB (2255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56959c3bffd939fbf4149eec973d3331a4273b1a9d72c5add5397b1af4912e5b`  
		Last Modified: Thu, 05 Nov 2020 21:51:18 GMT  
		Size: 16.9 KB (16879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20e65a75b3879d79efe6f40b2734327716ca427b327ba34e01677c27ea78019a`  
		Last Modified: Thu, 05 Nov 2020 22:13:54 GMT  
		Size: 34.0 MB (34025112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2212e04769cf650b0f5ead7d25ca6f30dbbe7ac3514627030509060eae6248`  
		Last Modified: Thu, 05 Nov 2020 22:13:48 GMT  
		Size: 188.2 KB (188236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f707697be36d71646f6eecbad3b1385fe77c56964aaebd5e7999a3b1e4b7bbc`  
		Last Modified: Thu, 05 Nov 2020 22:13:48 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6a1062d3721c09025a4d5d3842c4cc3f902a529348d41011fedb4dcf4927df2`  
		Last Modified: Mon, 16 Nov 2020 19:41:45 GMT  
		Size: 552.3 KB (552262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9abe82a33510a6f74565307a80d16c16668e8b6eca7b8311c4b4476e0cba235`  
		Last Modified: Mon, 16 Nov 2020 19:41:45 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cda627eb3557ca89cea0c6f668bfd073042c3b289928085776cae5762424691`  
		Last Modified: Mon, 16 Nov 2020 19:41:45 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
