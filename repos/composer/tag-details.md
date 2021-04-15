<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `composer`

-	[`composer:1`](#composer1)
-	[`composer:1.10`](#composer110)
-	[`composer:1.10.21`](#composer11021)
-	[`composer:2`](#composer2)
-	[`composer:2.0`](#composer20)
-	[`composer:2.0.12`](#composer2012)
-	[`composer:latest`](#composerlatest)

## `composer:1`

```console
$ docker pull composer@sha256:00806e406b7b162ee1cd32c3861f65195b270096fbfb2e9c6990168d2d1cd8aa
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
$ docker pull composer@sha256:cf2cb5b748f1cbd1f70fdc7da2e98c6286263298e750633c431068fdbfbcb2b7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62129524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:323c90397b6462cb7c8c0f975b008c19254e918895a090bd2dc1ba7b389ef9ec`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 23:59:24 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 23:59:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 23:59:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:08:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 00:08:23 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:08:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 00:08:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 00:08:24 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 10:15:35 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 10:15:45 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 10:15:46 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 10:15:46 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 10:15:46 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 10:15:57 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 10:16:00 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 10:16:00 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 10:16:00 GMT
WORKDIR /app
# Thu, 15 Apr 2021 10:16:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 10:16:01 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e582385a5d67543612fd95df7b619a8572c549e16543153bf264ad3459de5d0`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 10.8 MB (10775177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19324c9462cc1b74101165f6e7a7cfc384c6be4378ad98522841c48586380e46`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e94dc0b377148e2f02341f71c676a50265f14e42eda33d323024c1fbf07215`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 15.0 MB (14950314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da582f37592e6a319e1d4f97ce5a0e1cf3d19cd7307747c2c07f6abaafcda759`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f821502d3ad8cce566cd0aae6d9b755c841ec8d0e26ef357c746410e3c2777e5`  
		Last Modified: Thu, 15 Apr 2021 02:15:21 GMT  
		Size: 17.5 KB (17535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e24ebb98a1ce7def46c39cfc32402e1be33d692ddafa8ccaef827bde3747ac`  
		Last Modified: Thu, 15 Apr 2021 10:16:23 GMT  
		Size: 31.2 MB (31159862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efaa46072d9058afcc9a9dfd299bb0dcb820c6aa8b2dff42a8cc26933e659d6`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 198.3 KB (198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e430c6f8c1e75e9188c61b5c734cd9f1fb0629eac403ba4eae56eea95fd85ee`  
		Last Modified: Thu, 15 Apr 2021 10:16:18 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e269293d44e5bce846250e01e7d45ffbf8f8923a312b80907a416c2c15740`  
		Last Modified: Thu, 15 Apr 2021 10:16:41 GMT  
		Size: 509.1 KB (509072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1572f4dcdb6c0af4c92ac18eb08c24047d24107814a5708aa8150f93db3927a`  
		Last Modified: Thu, 15 Apr 2021 10:16:41 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dafe4568a4ed5913c7091df12b690dd1c085fa77bde35f279ef0c9cd0f7e3f8`  
		Last Modified: Thu, 15 Apr 2021 10:16:41 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1` - linux; arm variant v6

```console
$ docker pull composer@sha256:ac71ad6109874a35561f44ae8c1137b6ac15480c1cbd0c3e2fd5606e4569f40b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58365234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:499a576c9fbf90a2f68cf0d20b78262df97f094a0223533dabcb8f04a67af54e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:06:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:07:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:07:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:07:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:07:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:07:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:07:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 01:07:33 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 01:07:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 01:07:37 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 01:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 01:07:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:12:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 01:12:53 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:12:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 01:12:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 01:12:59 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 07:11:04 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 07:11:25 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 07:11:27 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 07:11:28 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 07:11:29 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 07:11:44 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 07:11:47 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 07:11:47 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 07:11:48 GMT
WORKDIR /app
# Thu, 15 Apr 2021 07:11:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:11:49 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726cd3e9e578579e631e21133870b656f3938f6a87797a842254b274d8b76e8`  
		Last Modified: Thu, 15 Apr 2021 02:33:02 GMT  
		Size: 1.7 MB (1690998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db188e87a6ea4fd0959949208b039a0d9facc96183df8dc346c6d0d3368b77e`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73dce0ed56811623cd40b786e95b951ce9d6341d9bfefded4f8aa12574283`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d5ea4d59593d016379b8d7cf9d074ab74527314a70c4ab2224e030bcce918`  
		Last Modified: Thu, 15 Apr 2021 02:33:04 GMT  
		Size: 10.8 MB (10775163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09c200324804241421da31f3b8cb8c3d7b006322de86d71d500fbdba136a885`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c0a1a831eaec187029e84f1bb7de5acc585a3b96fbfceaf583a3b36731c083`  
		Last Modified: Thu, 15 Apr 2021 02:33:14 GMT  
		Size: 13.6 MB (13585216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ad658b06066f3e4c692de9e3e1d8dbdd37dd05e3c3863e2f7cc8e6947e4df8`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e563207cd5c65809f0cb70dc82a30fb3ff8a2bb948740cd511ad08fa51a0d38`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 17.5 KB (17533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7322cd551e2d84436e4a4730a66208de66ff94b2946927fc56b146a5b180e41`  
		Last Modified: Thu, 15 Apr 2021 07:12:19 GMT  
		Size: 29.0 MB (28966488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed30edea345eb014ce9274ab7e0c12d0e6b1bf113bb2832146ab41759202280`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 193.6 KB (193560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7850310f2473f2085694f0ae25645d1dbeed617879390675b835e24400817d0c`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7ead7ebdb8b68a7cf27f3d38579f342dd1bf2041e311f31efd4ae587915d7`  
		Last Modified: Thu, 15 Apr 2021 07:12:29 GMT  
		Size: 509.1 KB (509073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d096f30b7d7abe7e2dbaeca56096f5bd93c1f3b56e855acfe8da9bce8110abe2`  
		Last Modified: Thu, 15 Apr 2021 07:12:28 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93864ba8dfd1f9f4a4cd8f01e816da8e71b86d309ac31866ad2c6de101dfed06`  
		Last Modified: Thu, 15 Apr 2021 07:12:28 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1` - linux; arm variant v7

```console
$ docker pull composer@sha256:dd9d7459623ed977ba6c414aafbf04570c125fd98209b463771b8860bad10675
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55847510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d010b225eec14156d7ad086d08030f1554b553c1824cea06bf2d6c4f7c30be7b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:08:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:08:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:08:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:08:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:08:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:08:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:08:54 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 02:09:03 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 02:09:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 02:09:29 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 02:10:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 02:11:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 02:15:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 02:16:01 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 02:16:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 02:16:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 02:16:08 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:32:23 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:32:41 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:32:43 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:32:44 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:32:45 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:33:03 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 08:33:06 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:33:07 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:33:08 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:33:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:33:09 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc6d3f07b2e440bf9a8e52a0a5bba0f27637990ee4976424cef6aae97e169f`  
		Last Modified: Thu, 15 Apr 2021 03:38:53 GMT  
		Size: 1.6 MB (1559061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9000ca9dcd92a2066a3a2c4031e677c3998cd82a3ecbc68468d11255ecbdb62`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d102949f174ecad1044574e45dded8368eb7451bf66b3bdac6e367c7f415d3`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92da8c0a1f3fbf1d4e02eaa533a5058c129447984212a6ff3c72bcc9cad8ab61`  
		Last Modified: Thu, 15 Apr 2021 03:38:54 GMT  
		Size: 10.8 MB (10775172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e011c8a33e544331ac43001738b66a746be18150ffd02e029e1781842dcc4706`  
		Last Modified: Thu, 15 Apr 2021 03:38:48 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61492dda820b711430b6f09aeb0af17f5efb9740a6147244fe1bcf9351a077b`  
		Last Modified: Thu, 15 Apr 2021 03:38:56 GMT  
		Size: 12.7 MB (12733009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e0a3051e72edd5461eda9dc5ad8e0d0b59e55fa0aee85a35da5251839f7f48`  
		Last Modified: Thu, 15 Apr 2021 03:38:47 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e451143ba28ebc0296ff08f6566c5e1d12c219c54351d23e2cb6cd545e2e009a`  
		Last Modified: Thu, 15 Apr 2021 03:38:47 GMT  
		Size: 17.5 KB (17537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3ae47db92bb3e5c1668c4815a02f3a46f82c32e59aa4e9317ea9a4d808399c`  
		Last Modified: Thu, 15 Apr 2021 08:33:40 GMT  
		Size: 27.6 MB (27638087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cacea819616d21dfc105f33ca411a910a2f359b1ab8bad9f43943880dc2a76`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 186.4 KB (186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64cc5abdecaef6df8f69965b45b6b83a146dac9487e208895b0bc28bbf32525`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f1ab5bf857c1204297d5e8cba9b34ada460782276c25949c2cb08387d3272d`  
		Last Modified: Thu, 15 Apr 2021 08:33:55 GMT  
		Size: 509.1 KB (509065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7c8e1240d5f2f131a2c5ac764636779c09822df19755585d580e27c4362b8f`  
		Last Modified: Thu, 15 Apr 2021 08:33:53 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8bbc76f44b37307fc8f7e652d7d8e97485c5d4d32cf8a2c0b2c77a421a9bad`  
		Last Modified: Thu, 15 Apr 2021 08:33:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:6c4c69ffc7001b776707d174b46637bd3eefff2cef16c8f372f5dd56ea6e5f4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61648074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35125c1cd444bbcee806cf6d736e71fbc46d40718ee77ebb1f6a8fa45a9b2cd1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:27:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:28:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:28:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:28:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:28:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:28:27 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 00:28:29 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 00:28:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 00:28:33 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 00:28:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 00:28:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:34:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 00:34:40 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:34:47 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 00:34:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 00:34:50 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:56:13 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:56:38 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:56:41 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:56:42 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:56:43 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:57:11 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 08:57:15 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:57:16 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:57:18 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:57:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:57:23 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea792edc0a65854bc13c90079b9e33a399c351b73e194d9df4f2cf5a0efeb2`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 1.7 MB (1700262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31bbfcb500579a0c450809a6b082c564c3ce4873732c1b62d8dab52ed0a11ac`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22841fe152c1fe4ec2048ebca3b9c0db9d29773b0d0670167a848d87fcfe83f3`  
		Last Modified: Thu, 15 Apr 2021 01:59:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61644ef55a78b8c8188acffca32263b12c8684a851a14a3fadc9f9c81d83c6e`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 10.8 MB (10775183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512fc0b44c8ccf1bcd4977baa78bd06876049fbefea93ca3a60d8406b53192c2`  
		Last Modified: Thu, 15 Apr 2021 01:59:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e853e5eed6ac911854cde2862e6607daf5c31850a72c856823616ad5ab566d`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 14.4 MB (14377741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bf5108bfbb40bc73cdd1e0df396ea55f8551e26c78af8e0b455b6bb2f0792e`  
		Last Modified: Thu, 15 Apr 2021 01:59:49 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127cb6e69cb6e4805c0d326498d5b9ebf45069ce7dd5c5cb94558188945baa9b`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad50c34e5614c2df0de39bfe9e05281b6b88a4cdb3c4783d80b00d4e72de6d33`  
		Last Modified: Thu, 15 Apr 2021 08:57:51 GMT  
		Size: 31.4 MB (31355216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d5b566318e8b07a0e09bffb639f37240aa5b1afbf68d7bb3aa7d9ee722e8c`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 195.9 KB (195947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9624473eddbb2b7517d6b3ec640bc13c5deae479b44cfdc7781a6dd517ff06`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c0c102804b45b89956f17345d35e267be6d92abe4dedb263adc4b12da754d`  
		Last Modified: Thu, 15 Apr 2021 08:58:02 GMT  
		Size: 509.1 KB (509073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c2202f0e19859603dc11bf86fad1338d0cf13525f28880d69a04a032e26344`  
		Last Modified: Thu, 15 Apr 2021 08:58:02 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac194e59eff9a4ec9478d567f69fd0755c64bf1cf8af48ae10d5f4f71d51959`  
		Last Modified: Thu, 15 Apr 2021 08:58:03 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1` - linux; 386

```console
$ docker pull composer@sha256:6d71b70591ed2b83cfc7681caed9f6fb8c0a1a368ea6bc96272cc0dbcb95730a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63413545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab63aedb84628cde2b29d7b0123002093c5b2844093ad4877b8ea27b0b03187`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 03:38:49 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 03:39:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 03:39:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:45:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 03:45:10 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:45:12 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 03:45:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 03:45:13 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:52:55 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:53:10 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:53:11 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:53:11 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:53:12 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:53:22 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 08:53:25 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:53:26 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:53:26 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:53:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:53:26 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeccee8de2519293816e97d37497a11495840e4c2edb7ad1254ce80fc59737a`  
		Last Modified: Thu, 15 Apr 2021 05:57:42 GMT  
		Size: 10.8 MB (10775154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962c132cc514121c8ad9862e99f06f647cbc70e07305e12cde1c0e8986f4de2d`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf4252825c42e4fc0d1dd2328fc4fbae3271919571b76a5dd55b1a5a63f3c8b`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 15.0 MB (14974551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7085eb2c648a88168bff8bcfeb7ef1f366a6c134a86b2e22fb7b2dc37479ea38`  
		Last Modified: Thu, 15 Apr 2021 05:57:40 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7ddb662add691a4ef54081ad454d11303541f3b4398453b7c72070b39bbeee`  
		Last Modified: Thu, 15 Apr 2021 05:57:40 GMT  
		Size: 17.5 KB (17533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d4448c8736ab950ed57d33c37776a00fe02282664f5316431b408f76ebccef`  
		Last Modified: Thu, 15 Apr 2021 08:54:02 GMT  
		Size: 32.3 MB (32300139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadf752d16c9b4f5ebcbf8f8ee774377e7e479e31c9900f14d6e8252b89e9686`  
		Last Modified: Thu, 15 Apr 2021 08:53:53 GMT  
		Size: 213.8 KB (213841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30932fd99a342f62c81464b27cb9398d3638e9caeaf2d233d5cf3bbde4114028`  
		Last Modified: Thu, 15 Apr 2021 08:53:53 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e099917a5878c0aef95d1eef8e6679df38cdce1af078c6618e667b67e5647b`  
		Last Modified: Thu, 15 Apr 2021 08:54:26 GMT  
		Size: 509.1 KB (509080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47392a002656e27ea395560092a247409593dcc2bfd72743c2d26cfb312a25ad`  
		Last Modified: Thu, 15 Apr 2021 08:54:26 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef5f935dd4950962716971ccfdaadb40fda3780da832dc35c44c82483871ade`  
		Last Modified: Thu, 15 Apr 2021 08:54:26 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1` - linux; ppc64le

```console
$ docker pull composer@sha256:037a83df126f1088051ae6d1973048a7c3b90d18abcae97cb0285fbf1adff379
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63743552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51e276f53c453a6216d861b799d743b20c52485dd568432e5ad64694d02530a8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:16:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:16:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 20:16:59 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 20:17:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 20:17:24 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 20:17:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:23:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Apr 2021 20:23:31 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:23:50 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Apr 2021 20:23:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Apr 2021 20:24:03 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:44:10 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:44:50 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:45:13 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:45:19 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:45:26 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:46:33 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 08:46:51 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:46:52 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:46:57 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:47:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:47:04 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6431deb07f4adae4be0bd4b93d784bb08ec63d03daa512d835bbc0230e05cf3`  
		Last Modified: Wed, 14 Apr 2021 22:00:57 GMT  
		Size: 10.8 MB (10775172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3ef816305c1c138c8c7ce8fbacf23f59654a7422858f578711604d0819539d`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171f3408ea103656d215c6b47106245684e915481a4ae3bc5b613d2f98f6b219`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 15.7 MB (15673187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5517add7dc81698b49a4430b992ab0bb4a012fbd04792d17b4754fe392f24014`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4888f0381bb3c52192f3c448b3bf6fd7906a41b23b8ac854a82340a8aa6171`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 17.6 KB (17556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f596040cc5835db2f0e35314704e491260222aa43948cc3c84967912a555a993`  
		Last Modified: Thu, 15 Apr 2021 08:47:37 GMT  
		Size: 32.0 MB (31997694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc29da636c9f65c118437157394b275676967a063d7b8cbf33ab5faca6c591c`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 204.0 KB (204005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef3767002a509df55f5149f3fb25a788238d75bd23a9cb0d17af0ae11ec7a0c`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1276d258715ae36f49d4067065fccda5c039cc9735d070cac5411faa0b4d8b`  
		Last Modified: Thu, 15 Apr 2021 08:47:56 GMT  
		Size: 509.1 KB (509081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6b87ab913b0b585c4096e95ddf29112ce5ae14e0578da714d32f99f45f325a`  
		Last Modified: Thu, 15 Apr 2021 08:47:55 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33bfd4544c699a0b940376f384092387fc38be8d436154138d6f70ea4400b7`  
		Last Modified: Thu, 15 Apr 2021 08:47:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1` - linux; s390x

```console
$ docker pull composer@sha256:db11d5d46b43801d057284e4c9deff4f7b38adfde85f1c505db8accbabb8853c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61231529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e370cbbb927d377156360639e028e49332ca8821f65b1966c0179fcde9c74352`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:00:59 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 19:01:00 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 19:01:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 19:01:01 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 19:01:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 19:01:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Apr 2021 19:06:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Apr 2021 19:06:26 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 14 Apr 2021 19:06:27 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Apr 2021 19:06:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Apr 2021 19:06:28 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 07:30:47 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 07:30:58 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 07:30:58 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 07:31:12 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 07:31:14 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 07:31:14 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 07:31:14 GMT
WORKDIR /app
# Thu, 15 Apr 2021 07:31:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:31:15 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbe2d3d9b1efb815eb614a3488743bc95ac05e1ae4b0b1e2b488a057a9697f2`  
		Last Modified: Wed, 14 Apr 2021 20:01:03 GMT  
		Size: 10.8 MB (10775158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42d806dde82abd1fa888745f98a91c4a389d70968f69ee9fb1d467acf94c233`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3407c21d5517a5fe9bee65ffefce1b436496f08d54e5ec826713de143cc769a1`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 14.0 MB (13972054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673772f281ad30fa5e8f68f1b2cc7246eb505f77b1304eeffee4ed02e2ac0025`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887ade51969a265f267fab2842da16aee5c3746eebee780035a2e8e30b486de`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 17.6 KB (17552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827a7ecf83cc085e8c067e3fb91cc8be53232ed95c0f1344337b305382d525d5`  
		Last Modified: Thu, 15 Apr 2021 07:31:34 GMT  
		Size: 31.4 MB (31391511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ddcc417205411563d9531ffab3b6e85ece64c95e6e494b9a7eac77bf621e25`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 197.8 KB (197750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f23536fe9ce1e18934446f30900cd733051f3573df86ecd7dd71a23e7047420`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c134254d1377437df67d8fa8b1af51445904e43d85c946e60b05c05bec838e7e`  
		Last Modified: Thu, 15 Apr 2021 07:31:43 GMT  
		Size: 509.1 KB (509072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9135caba7125abe2422a715bc957fe9aaeb89317d448614ef41b9acf67c1ecab`  
		Last Modified: Thu, 15 Apr 2021 07:31:42 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1bc1533a825b7fade5107526bfac27baff866a0f7b1aff17ad761b6c3aa145`  
		Last Modified: Thu, 15 Apr 2021 07:31:42 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `composer:1.10`

```console
$ docker pull composer@sha256:00806e406b7b162ee1cd32c3861f65195b270096fbfb2e9c6990168d2d1cd8aa
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
$ docker pull composer@sha256:cf2cb5b748f1cbd1f70fdc7da2e98c6286263298e750633c431068fdbfbcb2b7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62129524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:323c90397b6462cb7c8c0f975b008c19254e918895a090bd2dc1ba7b389ef9ec`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 23:59:24 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 23:59:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 23:59:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:08:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 00:08:23 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:08:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 00:08:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 00:08:24 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 10:15:35 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 10:15:45 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 10:15:46 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 10:15:46 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 10:15:46 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 10:15:57 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 10:16:00 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 10:16:00 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 10:16:00 GMT
WORKDIR /app
# Thu, 15 Apr 2021 10:16:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 10:16:01 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e582385a5d67543612fd95df7b619a8572c549e16543153bf264ad3459de5d0`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 10.8 MB (10775177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19324c9462cc1b74101165f6e7a7cfc384c6be4378ad98522841c48586380e46`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e94dc0b377148e2f02341f71c676a50265f14e42eda33d323024c1fbf07215`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 15.0 MB (14950314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da582f37592e6a319e1d4f97ce5a0e1cf3d19cd7307747c2c07f6abaafcda759`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f821502d3ad8cce566cd0aae6d9b755c841ec8d0e26ef357c746410e3c2777e5`  
		Last Modified: Thu, 15 Apr 2021 02:15:21 GMT  
		Size: 17.5 KB (17535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e24ebb98a1ce7def46c39cfc32402e1be33d692ddafa8ccaef827bde3747ac`  
		Last Modified: Thu, 15 Apr 2021 10:16:23 GMT  
		Size: 31.2 MB (31159862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efaa46072d9058afcc9a9dfd299bb0dcb820c6aa8b2dff42a8cc26933e659d6`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 198.3 KB (198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e430c6f8c1e75e9188c61b5c734cd9f1fb0629eac403ba4eae56eea95fd85ee`  
		Last Modified: Thu, 15 Apr 2021 10:16:18 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e269293d44e5bce846250e01e7d45ffbf8f8923a312b80907a416c2c15740`  
		Last Modified: Thu, 15 Apr 2021 10:16:41 GMT  
		Size: 509.1 KB (509072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1572f4dcdb6c0af4c92ac18eb08c24047d24107814a5708aa8150f93db3927a`  
		Last Modified: Thu, 15 Apr 2021 10:16:41 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dafe4568a4ed5913c7091df12b690dd1c085fa77bde35f279ef0c9cd0f7e3f8`  
		Last Modified: Thu, 15 Apr 2021 10:16:41 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10` - linux; arm variant v6

```console
$ docker pull composer@sha256:ac71ad6109874a35561f44ae8c1137b6ac15480c1cbd0c3e2fd5606e4569f40b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58365234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:499a576c9fbf90a2f68cf0d20b78262df97f094a0223533dabcb8f04a67af54e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:06:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:07:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:07:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:07:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:07:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:07:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:07:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 01:07:33 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 01:07:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 01:07:37 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 01:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 01:07:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:12:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 01:12:53 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:12:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 01:12:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 01:12:59 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 07:11:04 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 07:11:25 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 07:11:27 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 07:11:28 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 07:11:29 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 07:11:44 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 07:11:47 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 07:11:47 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 07:11:48 GMT
WORKDIR /app
# Thu, 15 Apr 2021 07:11:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:11:49 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726cd3e9e578579e631e21133870b656f3938f6a87797a842254b274d8b76e8`  
		Last Modified: Thu, 15 Apr 2021 02:33:02 GMT  
		Size: 1.7 MB (1690998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db188e87a6ea4fd0959949208b039a0d9facc96183df8dc346c6d0d3368b77e`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73dce0ed56811623cd40b786e95b951ce9d6341d9bfefded4f8aa12574283`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d5ea4d59593d016379b8d7cf9d074ab74527314a70c4ab2224e030bcce918`  
		Last Modified: Thu, 15 Apr 2021 02:33:04 GMT  
		Size: 10.8 MB (10775163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09c200324804241421da31f3b8cb8c3d7b006322de86d71d500fbdba136a885`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c0a1a831eaec187029e84f1bb7de5acc585a3b96fbfceaf583a3b36731c083`  
		Last Modified: Thu, 15 Apr 2021 02:33:14 GMT  
		Size: 13.6 MB (13585216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ad658b06066f3e4c692de9e3e1d8dbdd37dd05e3c3863e2f7cc8e6947e4df8`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e563207cd5c65809f0cb70dc82a30fb3ff8a2bb948740cd511ad08fa51a0d38`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 17.5 KB (17533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7322cd551e2d84436e4a4730a66208de66ff94b2946927fc56b146a5b180e41`  
		Last Modified: Thu, 15 Apr 2021 07:12:19 GMT  
		Size: 29.0 MB (28966488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed30edea345eb014ce9274ab7e0c12d0e6b1bf113bb2832146ab41759202280`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 193.6 KB (193560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7850310f2473f2085694f0ae25645d1dbeed617879390675b835e24400817d0c`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7ead7ebdb8b68a7cf27f3d38579f342dd1bf2041e311f31efd4ae587915d7`  
		Last Modified: Thu, 15 Apr 2021 07:12:29 GMT  
		Size: 509.1 KB (509073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d096f30b7d7abe7e2dbaeca56096f5bd93c1f3b56e855acfe8da9bce8110abe2`  
		Last Modified: Thu, 15 Apr 2021 07:12:28 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93864ba8dfd1f9f4a4cd8f01e816da8e71b86d309ac31866ad2c6de101dfed06`  
		Last Modified: Thu, 15 Apr 2021 07:12:28 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10` - linux; arm variant v7

```console
$ docker pull composer@sha256:dd9d7459623ed977ba6c414aafbf04570c125fd98209b463771b8860bad10675
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55847510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d010b225eec14156d7ad086d08030f1554b553c1824cea06bf2d6c4f7c30be7b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:08:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:08:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:08:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:08:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:08:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:08:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:08:54 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 02:09:03 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 02:09:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 02:09:29 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 02:10:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 02:11:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 02:15:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 02:16:01 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 02:16:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 02:16:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 02:16:08 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:32:23 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:32:41 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:32:43 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:32:44 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:32:45 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:33:03 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 08:33:06 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:33:07 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:33:08 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:33:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:33:09 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc6d3f07b2e440bf9a8e52a0a5bba0f27637990ee4976424cef6aae97e169f`  
		Last Modified: Thu, 15 Apr 2021 03:38:53 GMT  
		Size: 1.6 MB (1559061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9000ca9dcd92a2066a3a2c4031e677c3998cd82a3ecbc68468d11255ecbdb62`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d102949f174ecad1044574e45dded8368eb7451bf66b3bdac6e367c7f415d3`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92da8c0a1f3fbf1d4e02eaa533a5058c129447984212a6ff3c72bcc9cad8ab61`  
		Last Modified: Thu, 15 Apr 2021 03:38:54 GMT  
		Size: 10.8 MB (10775172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e011c8a33e544331ac43001738b66a746be18150ffd02e029e1781842dcc4706`  
		Last Modified: Thu, 15 Apr 2021 03:38:48 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61492dda820b711430b6f09aeb0af17f5efb9740a6147244fe1bcf9351a077b`  
		Last Modified: Thu, 15 Apr 2021 03:38:56 GMT  
		Size: 12.7 MB (12733009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e0a3051e72edd5461eda9dc5ad8e0d0b59e55fa0aee85a35da5251839f7f48`  
		Last Modified: Thu, 15 Apr 2021 03:38:47 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e451143ba28ebc0296ff08f6566c5e1d12c219c54351d23e2cb6cd545e2e009a`  
		Last Modified: Thu, 15 Apr 2021 03:38:47 GMT  
		Size: 17.5 KB (17537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3ae47db92bb3e5c1668c4815a02f3a46f82c32e59aa4e9317ea9a4d808399c`  
		Last Modified: Thu, 15 Apr 2021 08:33:40 GMT  
		Size: 27.6 MB (27638087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cacea819616d21dfc105f33ca411a910a2f359b1ab8bad9f43943880dc2a76`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 186.4 KB (186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64cc5abdecaef6df8f69965b45b6b83a146dac9487e208895b0bc28bbf32525`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f1ab5bf857c1204297d5e8cba9b34ada460782276c25949c2cb08387d3272d`  
		Last Modified: Thu, 15 Apr 2021 08:33:55 GMT  
		Size: 509.1 KB (509065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7c8e1240d5f2f131a2c5ac764636779c09822df19755585d580e27c4362b8f`  
		Last Modified: Thu, 15 Apr 2021 08:33:53 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8bbc76f44b37307fc8f7e652d7d8e97485c5d4d32cf8a2c0b2c77a421a9bad`  
		Last Modified: Thu, 15 Apr 2021 08:33:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:6c4c69ffc7001b776707d174b46637bd3eefff2cef16c8f372f5dd56ea6e5f4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61648074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35125c1cd444bbcee806cf6d736e71fbc46d40718ee77ebb1f6a8fa45a9b2cd1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:27:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:28:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:28:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:28:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:28:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:28:27 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 00:28:29 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 00:28:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 00:28:33 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 00:28:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 00:28:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:34:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 00:34:40 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:34:47 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 00:34:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 00:34:50 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:56:13 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:56:38 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:56:41 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:56:42 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:56:43 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:57:11 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 08:57:15 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:57:16 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:57:18 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:57:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:57:23 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea792edc0a65854bc13c90079b9e33a399c351b73e194d9df4f2cf5a0efeb2`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 1.7 MB (1700262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31bbfcb500579a0c450809a6b082c564c3ce4873732c1b62d8dab52ed0a11ac`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22841fe152c1fe4ec2048ebca3b9c0db9d29773b0d0670167a848d87fcfe83f3`  
		Last Modified: Thu, 15 Apr 2021 01:59:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61644ef55a78b8c8188acffca32263b12c8684a851a14a3fadc9f9c81d83c6e`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 10.8 MB (10775183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512fc0b44c8ccf1bcd4977baa78bd06876049fbefea93ca3a60d8406b53192c2`  
		Last Modified: Thu, 15 Apr 2021 01:59:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e853e5eed6ac911854cde2862e6607daf5c31850a72c856823616ad5ab566d`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 14.4 MB (14377741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bf5108bfbb40bc73cdd1e0df396ea55f8551e26c78af8e0b455b6bb2f0792e`  
		Last Modified: Thu, 15 Apr 2021 01:59:49 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127cb6e69cb6e4805c0d326498d5b9ebf45069ce7dd5c5cb94558188945baa9b`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad50c34e5614c2df0de39bfe9e05281b6b88a4cdb3c4783d80b00d4e72de6d33`  
		Last Modified: Thu, 15 Apr 2021 08:57:51 GMT  
		Size: 31.4 MB (31355216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d5b566318e8b07a0e09bffb639f37240aa5b1afbf68d7bb3aa7d9ee722e8c`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 195.9 KB (195947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9624473eddbb2b7517d6b3ec640bc13c5deae479b44cfdc7781a6dd517ff06`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c0c102804b45b89956f17345d35e267be6d92abe4dedb263adc4b12da754d`  
		Last Modified: Thu, 15 Apr 2021 08:58:02 GMT  
		Size: 509.1 KB (509073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c2202f0e19859603dc11bf86fad1338d0cf13525f28880d69a04a032e26344`  
		Last Modified: Thu, 15 Apr 2021 08:58:02 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac194e59eff9a4ec9478d567f69fd0755c64bf1cf8af48ae10d5f4f71d51959`  
		Last Modified: Thu, 15 Apr 2021 08:58:03 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10` - linux; 386

```console
$ docker pull composer@sha256:6d71b70591ed2b83cfc7681caed9f6fb8c0a1a368ea6bc96272cc0dbcb95730a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63413545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab63aedb84628cde2b29d7b0123002093c5b2844093ad4877b8ea27b0b03187`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 03:38:49 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 03:39:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 03:39:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:45:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 03:45:10 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:45:12 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 03:45:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 03:45:13 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:52:55 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:53:10 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:53:11 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:53:11 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:53:12 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:53:22 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 08:53:25 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:53:26 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:53:26 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:53:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:53:26 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeccee8de2519293816e97d37497a11495840e4c2edb7ad1254ce80fc59737a`  
		Last Modified: Thu, 15 Apr 2021 05:57:42 GMT  
		Size: 10.8 MB (10775154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962c132cc514121c8ad9862e99f06f647cbc70e07305e12cde1c0e8986f4de2d`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf4252825c42e4fc0d1dd2328fc4fbae3271919571b76a5dd55b1a5a63f3c8b`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 15.0 MB (14974551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7085eb2c648a88168bff8bcfeb7ef1f366a6c134a86b2e22fb7b2dc37479ea38`  
		Last Modified: Thu, 15 Apr 2021 05:57:40 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7ddb662add691a4ef54081ad454d11303541f3b4398453b7c72070b39bbeee`  
		Last Modified: Thu, 15 Apr 2021 05:57:40 GMT  
		Size: 17.5 KB (17533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d4448c8736ab950ed57d33c37776a00fe02282664f5316431b408f76ebccef`  
		Last Modified: Thu, 15 Apr 2021 08:54:02 GMT  
		Size: 32.3 MB (32300139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadf752d16c9b4f5ebcbf8f8ee774377e7e479e31c9900f14d6e8252b89e9686`  
		Last Modified: Thu, 15 Apr 2021 08:53:53 GMT  
		Size: 213.8 KB (213841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30932fd99a342f62c81464b27cb9398d3638e9caeaf2d233d5cf3bbde4114028`  
		Last Modified: Thu, 15 Apr 2021 08:53:53 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e099917a5878c0aef95d1eef8e6679df38cdce1af078c6618e667b67e5647b`  
		Last Modified: Thu, 15 Apr 2021 08:54:26 GMT  
		Size: 509.1 KB (509080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47392a002656e27ea395560092a247409593dcc2bfd72743c2d26cfb312a25ad`  
		Last Modified: Thu, 15 Apr 2021 08:54:26 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef5f935dd4950962716971ccfdaadb40fda3780da832dc35c44c82483871ade`  
		Last Modified: Thu, 15 Apr 2021 08:54:26 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10` - linux; ppc64le

```console
$ docker pull composer@sha256:037a83df126f1088051ae6d1973048a7c3b90d18abcae97cb0285fbf1adff379
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63743552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51e276f53c453a6216d861b799d743b20c52485dd568432e5ad64694d02530a8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:16:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:16:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 20:16:59 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 20:17:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 20:17:24 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 20:17:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:23:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Apr 2021 20:23:31 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:23:50 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Apr 2021 20:23:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Apr 2021 20:24:03 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:44:10 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:44:50 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:45:13 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:45:19 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:45:26 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:46:33 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 08:46:51 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:46:52 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:46:57 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:47:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:47:04 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6431deb07f4adae4be0bd4b93d784bb08ec63d03daa512d835bbc0230e05cf3`  
		Last Modified: Wed, 14 Apr 2021 22:00:57 GMT  
		Size: 10.8 MB (10775172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3ef816305c1c138c8c7ce8fbacf23f59654a7422858f578711604d0819539d`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171f3408ea103656d215c6b47106245684e915481a4ae3bc5b613d2f98f6b219`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 15.7 MB (15673187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5517add7dc81698b49a4430b992ab0bb4a012fbd04792d17b4754fe392f24014`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4888f0381bb3c52192f3c448b3bf6fd7906a41b23b8ac854a82340a8aa6171`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 17.6 KB (17556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f596040cc5835db2f0e35314704e491260222aa43948cc3c84967912a555a993`  
		Last Modified: Thu, 15 Apr 2021 08:47:37 GMT  
		Size: 32.0 MB (31997694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc29da636c9f65c118437157394b275676967a063d7b8cbf33ab5faca6c591c`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 204.0 KB (204005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef3767002a509df55f5149f3fb25a788238d75bd23a9cb0d17af0ae11ec7a0c`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1276d258715ae36f49d4067065fccda5c039cc9735d070cac5411faa0b4d8b`  
		Last Modified: Thu, 15 Apr 2021 08:47:56 GMT  
		Size: 509.1 KB (509081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6b87ab913b0b585c4096e95ddf29112ce5ae14e0578da714d32f99f45f325a`  
		Last Modified: Thu, 15 Apr 2021 08:47:55 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33bfd4544c699a0b940376f384092387fc38be8d436154138d6f70ea4400b7`  
		Last Modified: Thu, 15 Apr 2021 08:47:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10` - linux; s390x

```console
$ docker pull composer@sha256:db11d5d46b43801d057284e4c9deff4f7b38adfde85f1c505db8accbabb8853c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61231529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e370cbbb927d377156360639e028e49332ca8821f65b1966c0179fcde9c74352`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:00:59 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 19:01:00 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 19:01:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 19:01:01 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 19:01:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 19:01:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Apr 2021 19:06:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Apr 2021 19:06:26 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 14 Apr 2021 19:06:27 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Apr 2021 19:06:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Apr 2021 19:06:28 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 07:30:47 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 07:30:58 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 07:30:58 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 07:31:12 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 07:31:14 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 07:31:14 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 07:31:14 GMT
WORKDIR /app
# Thu, 15 Apr 2021 07:31:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:31:15 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbe2d3d9b1efb815eb614a3488743bc95ac05e1ae4b0b1e2b488a057a9697f2`  
		Last Modified: Wed, 14 Apr 2021 20:01:03 GMT  
		Size: 10.8 MB (10775158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42d806dde82abd1fa888745f98a91c4a389d70968f69ee9fb1d467acf94c233`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3407c21d5517a5fe9bee65ffefce1b436496f08d54e5ec826713de143cc769a1`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 14.0 MB (13972054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673772f281ad30fa5e8f68f1b2cc7246eb505f77b1304eeffee4ed02e2ac0025`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887ade51969a265f267fab2842da16aee5c3746eebee780035a2e8e30b486de`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 17.6 KB (17552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827a7ecf83cc085e8c067e3fb91cc8be53232ed95c0f1344337b305382d525d5`  
		Last Modified: Thu, 15 Apr 2021 07:31:34 GMT  
		Size: 31.4 MB (31391511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ddcc417205411563d9531ffab3b6e85ece64c95e6e494b9a7eac77bf621e25`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 197.8 KB (197750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f23536fe9ce1e18934446f30900cd733051f3573df86ecd7dd71a23e7047420`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c134254d1377437df67d8fa8b1af51445904e43d85c946e60b05c05bec838e7e`  
		Last Modified: Thu, 15 Apr 2021 07:31:43 GMT  
		Size: 509.1 KB (509072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9135caba7125abe2422a715bc957fe9aaeb89317d448614ef41b9acf67c1ecab`  
		Last Modified: Thu, 15 Apr 2021 07:31:42 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1bc1533a825b7fade5107526bfac27baff866a0f7b1aff17ad761b6c3aa145`  
		Last Modified: Thu, 15 Apr 2021 07:31:42 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `composer:1.10.21`

```console
$ docker pull composer@sha256:00806e406b7b162ee1cd32c3861f65195b270096fbfb2e9c6990168d2d1cd8aa
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

### `composer:1.10.21` - linux; amd64

```console
$ docker pull composer@sha256:cf2cb5b748f1cbd1f70fdc7da2e98c6286263298e750633c431068fdbfbcb2b7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.1 MB (62129524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:323c90397b6462cb7c8c0f975b008c19254e918895a090bd2dc1ba7b389ef9ec`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 23:59:24 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 23:59:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 23:59:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:08:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 00:08:23 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:08:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 00:08:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 00:08:24 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 10:15:35 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 10:15:45 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 10:15:46 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 10:15:46 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 10:15:46 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 10:15:57 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 10:16:00 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 10:16:00 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 10:16:00 GMT
WORKDIR /app
# Thu, 15 Apr 2021 10:16:01 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 10:16:01 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e582385a5d67543612fd95df7b619a8572c549e16543153bf264ad3459de5d0`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 10.8 MB (10775177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19324c9462cc1b74101165f6e7a7cfc384c6be4378ad98522841c48586380e46`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e94dc0b377148e2f02341f71c676a50265f14e42eda33d323024c1fbf07215`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 15.0 MB (14950314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da582f37592e6a319e1d4f97ce5a0e1cf3d19cd7307747c2c07f6abaafcda759`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f821502d3ad8cce566cd0aae6d9b755c841ec8d0e26ef357c746410e3c2777e5`  
		Last Modified: Thu, 15 Apr 2021 02:15:21 GMT  
		Size: 17.5 KB (17535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e24ebb98a1ce7def46c39cfc32402e1be33d692ddafa8ccaef827bde3747ac`  
		Last Modified: Thu, 15 Apr 2021 10:16:23 GMT  
		Size: 31.2 MB (31159862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efaa46072d9058afcc9a9dfd299bb0dcb820c6aa8b2dff42a8cc26933e659d6`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 198.3 KB (198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e430c6f8c1e75e9188c61b5c734cd9f1fb0629eac403ba4eae56eea95fd85ee`  
		Last Modified: Thu, 15 Apr 2021 10:16:18 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a08e269293d44e5bce846250e01e7d45ffbf8f8923a312b80907a416c2c15740`  
		Last Modified: Thu, 15 Apr 2021 10:16:41 GMT  
		Size: 509.1 KB (509072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1572f4dcdb6c0af4c92ac18eb08c24047d24107814a5708aa8150f93db3927a`  
		Last Modified: Thu, 15 Apr 2021 10:16:41 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dafe4568a4ed5913c7091df12b690dd1c085fa77bde35f279ef0c9cd0f7e3f8`  
		Last Modified: Thu, 15 Apr 2021 10:16:41 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10.21` - linux; arm variant v6

```console
$ docker pull composer@sha256:ac71ad6109874a35561f44ae8c1137b6ac15480c1cbd0c3e2fd5606e4569f40b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58365234 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:499a576c9fbf90a2f68cf0d20b78262df97f094a0223533dabcb8f04a67af54e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:06:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:07:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:07:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:07:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:07:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:07:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:07:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 01:07:33 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 01:07:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 01:07:37 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 01:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 01:07:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:12:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 01:12:53 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:12:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 01:12:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 01:12:59 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 07:11:04 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 07:11:25 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 07:11:27 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 07:11:28 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 07:11:29 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 07:11:44 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 07:11:47 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 07:11:47 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 07:11:48 GMT
WORKDIR /app
# Thu, 15 Apr 2021 07:11:49 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:11:49 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726cd3e9e578579e631e21133870b656f3938f6a87797a842254b274d8b76e8`  
		Last Modified: Thu, 15 Apr 2021 02:33:02 GMT  
		Size: 1.7 MB (1690998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db188e87a6ea4fd0959949208b039a0d9facc96183df8dc346c6d0d3368b77e`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73dce0ed56811623cd40b786e95b951ce9d6341d9bfefded4f8aa12574283`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d5ea4d59593d016379b8d7cf9d074ab74527314a70c4ab2224e030bcce918`  
		Last Modified: Thu, 15 Apr 2021 02:33:04 GMT  
		Size: 10.8 MB (10775163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09c200324804241421da31f3b8cb8c3d7b006322de86d71d500fbdba136a885`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c0a1a831eaec187029e84f1bb7de5acc585a3b96fbfceaf583a3b36731c083`  
		Last Modified: Thu, 15 Apr 2021 02:33:14 GMT  
		Size: 13.6 MB (13585216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ad658b06066f3e4c692de9e3e1d8dbdd37dd05e3c3863e2f7cc8e6947e4df8`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e563207cd5c65809f0cb70dc82a30fb3ff8a2bb948740cd511ad08fa51a0d38`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 17.5 KB (17533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7322cd551e2d84436e4a4730a66208de66ff94b2946927fc56b146a5b180e41`  
		Last Modified: Thu, 15 Apr 2021 07:12:19 GMT  
		Size: 29.0 MB (28966488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed30edea345eb014ce9274ab7e0c12d0e6b1bf113bb2832146ab41759202280`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 193.6 KB (193560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7850310f2473f2085694f0ae25645d1dbeed617879390675b835e24400817d0c`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db7ead7ebdb8b68a7cf27f3d38579f342dd1bf2041e311f31efd4ae587915d7`  
		Last Modified: Thu, 15 Apr 2021 07:12:29 GMT  
		Size: 509.1 KB (509073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d096f30b7d7abe7e2dbaeca56096f5bd93c1f3b56e855acfe8da9bce8110abe2`  
		Last Modified: Thu, 15 Apr 2021 07:12:28 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93864ba8dfd1f9f4a4cd8f01e816da8e71b86d309ac31866ad2c6de101dfed06`  
		Last Modified: Thu, 15 Apr 2021 07:12:28 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10.21` - linux; arm variant v7

```console
$ docker pull composer@sha256:dd9d7459623ed977ba6c414aafbf04570c125fd98209b463771b8860bad10675
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.8 MB (55847510 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d010b225eec14156d7ad086d08030f1554b553c1824cea06bf2d6c4f7c30be7b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:08:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:08:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:08:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:08:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:08:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:08:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:08:54 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 02:09:03 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 02:09:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 02:09:29 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 02:10:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 02:11:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 02:15:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 02:16:01 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 02:16:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 02:16:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 02:16:08 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:32:23 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:32:41 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:32:43 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:32:44 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:32:45 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:33:03 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 08:33:06 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:33:07 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:33:08 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:33:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:33:09 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc6d3f07b2e440bf9a8e52a0a5bba0f27637990ee4976424cef6aae97e169f`  
		Last Modified: Thu, 15 Apr 2021 03:38:53 GMT  
		Size: 1.6 MB (1559061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9000ca9dcd92a2066a3a2c4031e677c3998cd82a3ecbc68468d11255ecbdb62`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d102949f174ecad1044574e45dded8368eb7451bf66b3bdac6e367c7f415d3`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92da8c0a1f3fbf1d4e02eaa533a5058c129447984212a6ff3c72bcc9cad8ab61`  
		Last Modified: Thu, 15 Apr 2021 03:38:54 GMT  
		Size: 10.8 MB (10775172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e011c8a33e544331ac43001738b66a746be18150ffd02e029e1781842dcc4706`  
		Last Modified: Thu, 15 Apr 2021 03:38:48 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61492dda820b711430b6f09aeb0af17f5efb9740a6147244fe1bcf9351a077b`  
		Last Modified: Thu, 15 Apr 2021 03:38:56 GMT  
		Size: 12.7 MB (12733009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e0a3051e72edd5461eda9dc5ad8e0d0b59e55fa0aee85a35da5251839f7f48`  
		Last Modified: Thu, 15 Apr 2021 03:38:47 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e451143ba28ebc0296ff08f6566c5e1d12c219c54351d23e2cb6cd545e2e009a`  
		Last Modified: Thu, 15 Apr 2021 03:38:47 GMT  
		Size: 17.5 KB (17537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3ae47db92bb3e5c1668c4815a02f3a46f82c32e59aa4e9317ea9a4d808399c`  
		Last Modified: Thu, 15 Apr 2021 08:33:40 GMT  
		Size: 27.6 MB (27638087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cacea819616d21dfc105f33ca411a910a2f359b1ab8bad9f43943880dc2a76`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 186.4 KB (186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64cc5abdecaef6df8f69965b45b6b83a146dac9487e208895b0bc28bbf32525`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f1ab5bf857c1204297d5e8cba9b34ada460782276c25949c2cb08387d3272d`  
		Last Modified: Thu, 15 Apr 2021 08:33:55 GMT  
		Size: 509.1 KB (509065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf7c8e1240d5f2f131a2c5ac764636779c09822df19755585d580e27c4362b8f`  
		Last Modified: Thu, 15 Apr 2021 08:33:53 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db8bbc76f44b37307fc8f7e652d7d8e97485c5d4d32cf8a2c0b2c77a421a9bad`  
		Last Modified: Thu, 15 Apr 2021 08:33:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10.21` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:6c4c69ffc7001b776707d174b46637bd3eefff2cef16c8f372f5dd56ea6e5f4e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.6 MB (61648074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35125c1cd444bbcee806cf6d736e71fbc46d40718ee77ebb1f6a8fa45a9b2cd1`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:27:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:28:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:28:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:28:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:28:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:28:27 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 00:28:29 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 00:28:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 00:28:33 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 00:28:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 00:28:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:34:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 00:34:40 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:34:47 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 00:34:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 00:34:50 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:56:13 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:56:38 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:56:41 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:56:42 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:56:43 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:57:11 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 08:57:15 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:57:16 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:57:18 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:57:21 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:57:23 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea792edc0a65854bc13c90079b9e33a399c351b73e194d9df4f2cf5a0efeb2`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 1.7 MB (1700262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31bbfcb500579a0c450809a6b082c564c3ce4873732c1b62d8dab52ed0a11ac`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22841fe152c1fe4ec2048ebca3b9c0db9d29773b0d0670167a848d87fcfe83f3`  
		Last Modified: Thu, 15 Apr 2021 01:59:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61644ef55a78b8c8188acffca32263b12c8684a851a14a3fadc9f9c81d83c6e`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 10.8 MB (10775183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512fc0b44c8ccf1bcd4977baa78bd06876049fbefea93ca3a60d8406b53192c2`  
		Last Modified: Thu, 15 Apr 2021 01:59:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e853e5eed6ac911854cde2862e6607daf5c31850a72c856823616ad5ab566d`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 14.4 MB (14377741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bf5108bfbb40bc73cdd1e0df396ea55f8551e26c78af8e0b455b6bb2f0792e`  
		Last Modified: Thu, 15 Apr 2021 01:59:49 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127cb6e69cb6e4805c0d326498d5b9ebf45069ce7dd5c5cb94558188945baa9b`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad50c34e5614c2df0de39bfe9e05281b6b88a4cdb3c4783d80b00d4e72de6d33`  
		Last Modified: Thu, 15 Apr 2021 08:57:51 GMT  
		Size: 31.4 MB (31355216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d5b566318e8b07a0e09bffb639f37240aa5b1afbf68d7bb3aa7d9ee722e8c`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 195.9 KB (195947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9624473eddbb2b7517d6b3ec640bc13c5deae479b44cfdc7781a6dd517ff06`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a41c0c102804b45b89956f17345d35e267be6d92abe4dedb263adc4b12da754d`  
		Last Modified: Thu, 15 Apr 2021 08:58:02 GMT  
		Size: 509.1 KB (509073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c2202f0e19859603dc11bf86fad1338d0cf13525f28880d69a04a032e26344`  
		Last Modified: Thu, 15 Apr 2021 08:58:02 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ac194e59eff9a4ec9478d567f69fd0755c64bf1cf8af48ae10d5f4f71d51959`  
		Last Modified: Thu, 15 Apr 2021 08:58:03 GMT  
		Size: 123.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10.21` - linux; 386

```console
$ docker pull composer@sha256:6d71b70591ed2b83cfc7681caed9f6fb8c0a1a368ea6bc96272cc0dbcb95730a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.4 MB (63413545 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ab63aedb84628cde2b29d7b0123002093c5b2844093ad4877b8ea27b0b03187`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 03:38:49 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 03:39:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 03:39:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:45:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 03:45:10 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:45:12 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 03:45:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 03:45:13 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:52:55 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:53:10 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:53:11 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:53:11 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:53:12 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:53:22 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 08:53:25 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:53:26 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:53:26 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:53:26 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:53:26 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeccee8de2519293816e97d37497a11495840e4c2edb7ad1254ce80fc59737a`  
		Last Modified: Thu, 15 Apr 2021 05:57:42 GMT  
		Size: 10.8 MB (10775154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962c132cc514121c8ad9862e99f06f647cbc70e07305e12cde1c0e8986f4de2d`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf4252825c42e4fc0d1dd2328fc4fbae3271919571b76a5dd55b1a5a63f3c8b`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 15.0 MB (14974551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7085eb2c648a88168bff8bcfeb7ef1f366a6c134a86b2e22fb7b2dc37479ea38`  
		Last Modified: Thu, 15 Apr 2021 05:57:40 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7ddb662add691a4ef54081ad454d11303541f3b4398453b7c72070b39bbeee`  
		Last Modified: Thu, 15 Apr 2021 05:57:40 GMT  
		Size: 17.5 KB (17533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d4448c8736ab950ed57d33c37776a00fe02282664f5316431b408f76ebccef`  
		Last Modified: Thu, 15 Apr 2021 08:54:02 GMT  
		Size: 32.3 MB (32300139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadf752d16c9b4f5ebcbf8f8ee774377e7e479e31c9900f14d6e8252b89e9686`  
		Last Modified: Thu, 15 Apr 2021 08:53:53 GMT  
		Size: 213.8 KB (213841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30932fd99a342f62c81464b27cb9398d3638e9caeaf2d233d5cf3bbde4114028`  
		Last Modified: Thu, 15 Apr 2021 08:53:53 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e099917a5878c0aef95d1eef8e6679df38cdce1af078c6618e667b67e5647b`  
		Last Modified: Thu, 15 Apr 2021 08:54:26 GMT  
		Size: 509.1 KB (509080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47392a002656e27ea395560092a247409593dcc2bfd72743c2d26cfb312a25ad`  
		Last Modified: Thu, 15 Apr 2021 08:54:26 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef5f935dd4950962716971ccfdaadb40fda3780da832dc35c44c82483871ade`  
		Last Modified: Thu, 15 Apr 2021 08:54:26 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10.21` - linux; ppc64le

```console
$ docker pull composer@sha256:037a83df126f1088051ae6d1973048a7c3b90d18abcae97cb0285fbf1adff379
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63743552 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51e276f53c453a6216d861b799d743b20c52485dd568432e5ad64694d02530a8`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:16:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:16:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 20:16:59 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 20:17:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 20:17:24 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 20:17:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:23:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Apr 2021 20:23:31 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:23:50 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Apr 2021 20:23:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Apr 2021 20:24:03 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:44:10 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:44:50 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:45:13 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:45:19 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:45:26 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:46:33 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 08:46:51 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:46:52 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:46:57 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:47:00 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:47:04 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6431deb07f4adae4be0bd4b93d784bb08ec63d03daa512d835bbc0230e05cf3`  
		Last Modified: Wed, 14 Apr 2021 22:00:57 GMT  
		Size: 10.8 MB (10775172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3ef816305c1c138c8c7ce8fbacf23f59654a7422858f578711604d0819539d`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171f3408ea103656d215c6b47106245684e915481a4ae3bc5b613d2f98f6b219`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 15.7 MB (15673187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5517add7dc81698b49a4430b992ab0bb4a012fbd04792d17b4754fe392f24014`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4888f0381bb3c52192f3c448b3bf6fd7906a41b23b8ac854a82340a8aa6171`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 17.6 KB (17556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f596040cc5835db2f0e35314704e491260222aa43948cc3c84967912a555a993`  
		Last Modified: Thu, 15 Apr 2021 08:47:37 GMT  
		Size: 32.0 MB (31997694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc29da636c9f65c118437157394b275676967a063d7b8cbf33ab5faca6c591c`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 204.0 KB (204005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef3767002a509df55f5149f3fb25a788238d75bd23a9cb0d17af0ae11ec7a0c`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1276d258715ae36f49d4067065fccda5c039cc9735d070cac5411faa0b4d8b`  
		Last Modified: Thu, 15 Apr 2021 08:47:56 GMT  
		Size: 509.1 KB (509081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6b87ab913b0b585c4096e95ddf29112ce5ae14e0578da714d32f99f45f325a`  
		Last Modified: Thu, 15 Apr 2021 08:47:55 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c33bfd4544c699a0b940376f384092387fc38be8d436154138d6f70ea4400b7`  
		Last Modified: Thu, 15 Apr 2021 08:47:55 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:1.10.21` - linux; s390x

```console
$ docker pull composer@sha256:db11d5d46b43801d057284e4c9deff4f7b38adfde85f1c505db8accbabb8853c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.2 MB (61231529 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e370cbbb927d377156360639e028e49332ca8821f65b1966c0179fcde9c74352`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:00:59 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 19:01:00 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 19:01:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 19:01:01 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 19:01:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 19:01:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Apr 2021 19:06:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Apr 2021 19:06:26 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 14 Apr 2021 19:06:27 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Apr 2021 19:06:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Apr 2021 19:06:28 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 07:30:47 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 07:30:58 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 07:30:58 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 07:31:12 GMT
ENV COMPOSER_VERSION=1.10.21
# Thu, 15 Apr 2021 07:31:14 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 07:31:14 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 07:31:14 GMT
WORKDIR /app
# Thu, 15 Apr 2021 07:31:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:31:15 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbe2d3d9b1efb815eb614a3488743bc95ac05e1ae4b0b1e2b488a057a9697f2`  
		Last Modified: Wed, 14 Apr 2021 20:01:03 GMT  
		Size: 10.8 MB (10775158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42d806dde82abd1fa888745f98a91c4a389d70968f69ee9fb1d467acf94c233`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3407c21d5517a5fe9bee65ffefce1b436496f08d54e5ec826713de143cc769a1`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 14.0 MB (13972054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673772f281ad30fa5e8f68f1b2cc7246eb505f77b1304eeffee4ed02e2ac0025`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887ade51969a265f267fab2842da16aee5c3746eebee780035a2e8e30b486de`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 17.6 KB (17552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827a7ecf83cc085e8c067e3fb91cc8be53232ed95c0f1344337b305382d525d5`  
		Last Modified: Thu, 15 Apr 2021 07:31:34 GMT  
		Size: 31.4 MB (31391511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ddcc417205411563d9531ffab3b6e85ece64c95e6e494b9a7eac77bf621e25`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 197.8 KB (197750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f23536fe9ce1e18934446f30900cd733051f3573df86ecd7dd71a23e7047420`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c134254d1377437df67d8fa8b1af51445904e43d85c946e60b05c05bec838e7e`  
		Last Modified: Thu, 15 Apr 2021 07:31:43 GMT  
		Size: 509.1 KB (509072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9135caba7125abe2422a715bc957fe9aaeb89317d448614ef41b9acf67c1ecab`  
		Last Modified: Thu, 15 Apr 2021 07:31:42 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad1bc1533a825b7fade5107526bfac27baff866a0f7b1aff17ad761b6c3aa145`  
		Last Modified: Thu, 15 Apr 2021 07:31:42 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `composer:2`

```console
$ docker pull composer@sha256:f9aeec5f62e0f46cd92b2cfa54dff3243a9e1d05ab5ae27f034611955b14c4f2
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
$ docker pull composer@sha256:16c5c79db16eb9818aa6fa5012249e0fc4227afd5c161a3629d24de2ebb3ec6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62175820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee1fb424607c015745450cb9649f91855516264b22a6130a6ece9d49c234129`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 23:59:24 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 23:59:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 23:59:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:08:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 00:08:23 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:08:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 00:08:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 00:08:24 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 10:15:35 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 10:15:45 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 10:15:46 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 10:15:46 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 10:15:46 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 10:15:47 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 10:15:50 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 10:15:50 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 10:15:50 GMT
WORKDIR /app
# Thu, 15 Apr 2021 10:15:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 10:15:51 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e582385a5d67543612fd95df7b619a8572c549e16543153bf264ad3459de5d0`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 10.8 MB (10775177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19324c9462cc1b74101165f6e7a7cfc384c6be4378ad98522841c48586380e46`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e94dc0b377148e2f02341f71c676a50265f14e42eda33d323024c1fbf07215`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 15.0 MB (14950314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da582f37592e6a319e1d4f97ce5a0e1cf3d19cd7307747c2c07f6abaafcda759`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f821502d3ad8cce566cd0aae6d9b755c841ec8d0e26ef357c746410e3c2777e5`  
		Last Modified: Thu, 15 Apr 2021 02:15:21 GMT  
		Size: 17.5 KB (17535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e24ebb98a1ce7def46c39cfc32402e1be33d692ddafa8ccaef827bde3747ac`  
		Last Modified: Thu, 15 Apr 2021 10:16:23 GMT  
		Size: 31.2 MB (31159862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efaa46072d9058afcc9a9dfd299bb0dcb820c6aa8b2dff42a8cc26933e659d6`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 198.3 KB (198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e430c6f8c1e75e9188c61b5c734cd9f1fb0629eac403ba4eae56eea95fd85ee`  
		Last Modified: Thu, 15 Apr 2021 10:16:18 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366029d47da932cfa6bd72678d28a15f9006a7d6e70e8f61de4188c45b7a5371`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 555.4 KB (555370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5331243868df570248b0a1bc44a53c37e3e3b1d814c046a30ea3672fc12e8faf`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1c5eae9bf5060077bf987273f9a2691a7b1c9d138a0ca47edac68ea5e84490`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2` - linux; arm variant v6

```console
$ docker pull composer@sha256:e8fed4e7a57e97c313a8eb81ba749be03bd3e0d3e10e48115f416ea2fc695a6b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58411527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d89e493f7388277d91d3933bfa3e164bacb732cfd8b0b583b7b739554066908a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:06:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:07:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:07:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:07:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:07:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:07:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:07:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 01:07:33 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 01:07:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 01:07:37 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 01:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 01:07:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:12:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 01:12:53 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:12:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 01:12:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 01:12:59 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 07:11:04 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 07:11:25 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 07:11:27 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 07:11:28 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 07:11:29 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 07:11:29 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 07:11:33 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 07:11:34 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 07:11:34 GMT
WORKDIR /app
# Thu, 15 Apr 2021 07:11:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:11:36 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726cd3e9e578579e631e21133870b656f3938f6a87797a842254b274d8b76e8`  
		Last Modified: Thu, 15 Apr 2021 02:33:02 GMT  
		Size: 1.7 MB (1690998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db188e87a6ea4fd0959949208b039a0d9facc96183df8dc346c6d0d3368b77e`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73dce0ed56811623cd40b786e95b951ce9d6341d9bfefded4f8aa12574283`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d5ea4d59593d016379b8d7cf9d074ab74527314a70c4ab2224e030bcce918`  
		Last Modified: Thu, 15 Apr 2021 02:33:04 GMT  
		Size: 10.8 MB (10775163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09c200324804241421da31f3b8cb8c3d7b006322de86d71d500fbdba136a885`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c0a1a831eaec187029e84f1bb7de5acc585a3b96fbfceaf583a3b36731c083`  
		Last Modified: Thu, 15 Apr 2021 02:33:14 GMT  
		Size: 13.6 MB (13585216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ad658b06066f3e4c692de9e3e1d8dbdd37dd05e3c3863e2f7cc8e6947e4df8`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e563207cd5c65809f0cb70dc82a30fb3ff8a2bb948740cd511ad08fa51a0d38`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 17.5 KB (17533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7322cd551e2d84436e4a4730a66208de66ff94b2946927fc56b146a5b180e41`  
		Last Modified: Thu, 15 Apr 2021 07:12:19 GMT  
		Size: 29.0 MB (28966488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed30edea345eb014ce9274ab7e0c12d0e6b1bf113bb2832146ab41759202280`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 193.6 KB (193560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7850310f2473f2085694f0ae25645d1dbeed617879390675b835e24400817d0c`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e685f6d884207cd5821b189eb07436155ade2322ac14aa66466867f752d8b7`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 555.4 KB (555368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f80e0514909b04305b8652003c9f83308cdab5d4a3ff3ed6fdc75f92c7f6a8`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a531f1e7eee172868524f968eab1cd50d794e2f51df222f44024e4b4569fb004`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2` - linux; arm variant v7

```console
$ docker pull composer@sha256:f47db64626aa0085a31f4f87332a4c85e1f1b0e6dab6bbd9e0e6d59cbebc17b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55893814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f41fa048e70a27fbd80e3aebb25f5d2a785e4172c8675a1375062fd4af23fe4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:08:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:08:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:08:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:08:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:08:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:08:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:08:54 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 02:09:03 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 02:09:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 02:09:29 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 02:10:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 02:11:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 02:15:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 02:16:01 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 02:16:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 02:16:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 02:16:08 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:32:23 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:32:41 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:32:43 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:32:44 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:32:45 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:32:45 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 08:32:49 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:32:50 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:32:50 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:32:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:32:52 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc6d3f07b2e440bf9a8e52a0a5bba0f27637990ee4976424cef6aae97e169f`  
		Last Modified: Thu, 15 Apr 2021 03:38:53 GMT  
		Size: 1.6 MB (1559061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9000ca9dcd92a2066a3a2c4031e677c3998cd82a3ecbc68468d11255ecbdb62`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d102949f174ecad1044574e45dded8368eb7451bf66b3bdac6e367c7f415d3`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92da8c0a1f3fbf1d4e02eaa533a5058c129447984212a6ff3c72bcc9cad8ab61`  
		Last Modified: Thu, 15 Apr 2021 03:38:54 GMT  
		Size: 10.8 MB (10775172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e011c8a33e544331ac43001738b66a746be18150ffd02e029e1781842dcc4706`  
		Last Modified: Thu, 15 Apr 2021 03:38:48 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61492dda820b711430b6f09aeb0af17f5efb9740a6147244fe1bcf9351a077b`  
		Last Modified: Thu, 15 Apr 2021 03:38:56 GMT  
		Size: 12.7 MB (12733009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e0a3051e72edd5461eda9dc5ad8e0d0b59e55fa0aee85a35da5251839f7f48`  
		Last Modified: Thu, 15 Apr 2021 03:38:47 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e451143ba28ebc0296ff08f6566c5e1d12c219c54351d23e2cb6cd545e2e009a`  
		Last Modified: Thu, 15 Apr 2021 03:38:47 GMT  
		Size: 17.5 KB (17537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3ae47db92bb3e5c1668c4815a02f3a46f82c32e59aa4e9317ea9a4d808399c`  
		Last Modified: Thu, 15 Apr 2021 08:33:40 GMT  
		Size: 27.6 MB (27638087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cacea819616d21dfc105f33ca411a910a2f359b1ab8bad9f43943880dc2a76`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 186.4 KB (186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64cc5abdecaef6df8f69965b45b6b83a146dac9487e208895b0bc28bbf32525`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8f3a04e083b38b70dd19677baec0ff048eb0fd89827dec3a96c132afe5e282`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 555.4 KB (555369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196939056fb545323ea4219e28a3234097584c6fb32bd88616623aeabd5950bd`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83917393c8cb3c21a26875ace50b2b0b932c89355a39682da0c90b692ff404cb`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:58f7fcb3ddaf67e05162f3b09b0ee5652e65ff73ec9bcb794ed2d924caccee0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61694374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e3dec03a7d85bd434ed450c0bb62fd938a7fb193544337828c665e6480fffa`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:27:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:28:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:28:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:28:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:28:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:28:27 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 00:28:29 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 00:28:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 00:28:33 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 00:28:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 00:28:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:34:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 00:34:40 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:34:47 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 00:34:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 00:34:50 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:56:13 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:56:38 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:56:41 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:56:42 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:56:43 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:56:45 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 08:56:50 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:56:52 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:56:55 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:56:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:56:58 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea792edc0a65854bc13c90079b9e33a399c351b73e194d9df4f2cf5a0efeb2`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 1.7 MB (1700262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31bbfcb500579a0c450809a6b082c564c3ce4873732c1b62d8dab52ed0a11ac`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22841fe152c1fe4ec2048ebca3b9c0db9d29773b0d0670167a848d87fcfe83f3`  
		Last Modified: Thu, 15 Apr 2021 01:59:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61644ef55a78b8c8188acffca32263b12c8684a851a14a3fadc9f9c81d83c6e`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 10.8 MB (10775183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512fc0b44c8ccf1bcd4977baa78bd06876049fbefea93ca3a60d8406b53192c2`  
		Last Modified: Thu, 15 Apr 2021 01:59:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e853e5eed6ac911854cde2862e6607daf5c31850a72c856823616ad5ab566d`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 14.4 MB (14377741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bf5108bfbb40bc73cdd1e0df396ea55f8551e26c78af8e0b455b6bb2f0792e`  
		Last Modified: Thu, 15 Apr 2021 01:59:49 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127cb6e69cb6e4805c0d326498d5b9ebf45069ce7dd5c5cb94558188945baa9b`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad50c34e5614c2df0de39bfe9e05281b6b88a4cdb3c4783d80b00d4e72de6d33`  
		Last Modified: Thu, 15 Apr 2021 08:57:51 GMT  
		Size: 31.4 MB (31355216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d5b566318e8b07a0e09bffb639f37240aa5b1afbf68d7bb3aa7d9ee722e8c`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 195.9 KB (195947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9624473eddbb2b7517d6b3ec640bc13c5deae479b44cfdc7781a6dd517ff06`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0ea7aee59bc8c381ebf13e07f17a0a905147840a2a9813ba638e539f1f73e7`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 555.4 KB (555369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b9b6647561cc710659eec729f81d22f355bff35620854e6fe9e38b390b1a9a`  
		Last Modified: Thu, 15 Apr 2021 08:57:42 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bfd31c2ac4ef646c259c246c3ede82c00cd5aa28d34cad3b5ef2b2bba4bf25`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2` - linux; 386

```console
$ docker pull composer@sha256:70bc0657ac9d955ed89d5ea044768e0bf45b3a7226170ff6d48325a9d9787d9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.5 MB (63459840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8dd0b260971d5fcb96c0533acb7fa361b9d87ba87d71a3bfb54d32177317ef2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 03:38:49 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 03:39:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 03:39:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:45:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 03:45:10 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:45:12 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 03:45:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 03:45:13 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:52:55 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:53:10 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:53:11 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:53:11 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:53:12 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:53:12 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 08:53:15 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:53:15 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:53:15 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:53:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:53:16 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeccee8de2519293816e97d37497a11495840e4c2edb7ad1254ce80fc59737a`  
		Last Modified: Thu, 15 Apr 2021 05:57:42 GMT  
		Size: 10.8 MB (10775154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962c132cc514121c8ad9862e99f06f647cbc70e07305e12cde1c0e8986f4de2d`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf4252825c42e4fc0d1dd2328fc4fbae3271919571b76a5dd55b1a5a63f3c8b`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 15.0 MB (14974551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7085eb2c648a88168bff8bcfeb7ef1f366a6c134a86b2e22fb7b2dc37479ea38`  
		Last Modified: Thu, 15 Apr 2021 05:57:40 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7ddb662add691a4ef54081ad454d11303541f3b4398453b7c72070b39bbeee`  
		Last Modified: Thu, 15 Apr 2021 05:57:40 GMT  
		Size: 17.5 KB (17533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d4448c8736ab950ed57d33c37776a00fe02282664f5316431b408f76ebccef`  
		Last Modified: Thu, 15 Apr 2021 08:54:02 GMT  
		Size: 32.3 MB (32300139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadf752d16c9b4f5ebcbf8f8ee774377e7e479e31c9900f14d6e8252b89e9686`  
		Last Modified: Thu, 15 Apr 2021 08:53:53 GMT  
		Size: 213.8 KB (213841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30932fd99a342f62c81464b27cb9398d3638e9caeaf2d233d5cf3bbde4114028`  
		Last Modified: Thu, 15 Apr 2021 08:53:53 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359d5d64671b2b5de602c4f62ad00c7bad415822942d43fdbaff23995c637c83`  
		Last Modified: Thu, 15 Apr 2021 08:53:52 GMT  
		Size: 555.4 KB (555376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1662864d2b5ac55354e0d61fcefc60ae2f41afe4349fc86c0df7e756bb512f`  
		Last Modified: Thu, 15 Apr 2021 08:53:51 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff352cc745257d9f7c02042f4f03cc762fc0ee9c0f45d3d10657b26ff0395ad`  
		Last Modified: Thu, 15 Apr 2021 08:53:50 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2` - linux; ppc64le

```console
$ docker pull composer@sha256:ca8bcb0fad3c8c75791a7321ccbadd72dc179e18cfbf95b820714ce1d7affde1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63789841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9ee919c2f8f85644a637e78d057398a9759a722d8e5025c7b9fbc39b93004a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:16:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:16:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 20:16:59 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 20:17:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 20:17:24 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 20:17:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:23:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Apr 2021 20:23:31 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:23:50 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Apr 2021 20:23:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Apr 2021 20:24:03 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:44:10 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:44:50 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:45:13 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:45:19 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:45:26 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:45:35 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 08:45:55 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:46:00 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:46:08 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:46:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:46:16 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6431deb07f4adae4be0bd4b93d784bb08ec63d03daa512d835bbc0230e05cf3`  
		Last Modified: Wed, 14 Apr 2021 22:00:57 GMT  
		Size: 10.8 MB (10775172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3ef816305c1c138c8c7ce8fbacf23f59654a7422858f578711604d0819539d`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171f3408ea103656d215c6b47106245684e915481a4ae3bc5b613d2f98f6b219`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 15.7 MB (15673187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5517add7dc81698b49a4430b992ab0bb4a012fbd04792d17b4754fe392f24014`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4888f0381bb3c52192f3c448b3bf6fd7906a41b23b8ac854a82340a8aa6171`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 17.6 KB (17556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f596040cc5835db2f0e35314704e491260222aa43948cc3c84967912a555a993`  
		Last Modified: Thu, 15 Apr 2021 08:47:37 GMT  
		Size: 32.0 MB (31997694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc29da636c9f65c118437157394b275676967a063d7b8cbf33ab5faca6c591c`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 204.0 KB (204005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef3767002a509df55f5149f3fb25a788238d75bd23a9cb0d17af0ae11ec7a0c`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871523e4535d7b29028c6ba393e95315523bbd18d9ad4f6a313a36a3afb70d82`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 555.4 KB (555372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9b40f1162d15bc30f530fac32dbe79c562e0264f9378dd49e1e74bcda62fd0`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656cf3e249e69c2dd27fc4f38787633f612acbb71cb7645068b1946df2fb17de`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2` - linux; s390x

```console
$ docker pull composer@sha256:c8c4b8992d176fba657c9fed5cdbee13cf76d0fa9fa791ea1abaf59866bce2f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61277823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb15eb7b90d1e5576f452170f25168185d47f8d957f0fc34c6712e8e1d41df12`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:00:59 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 19:01:00 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 19:01:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 19:01:01 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 19:01:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 19:01:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Apr 2021 19:06:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Apr 2021 19:06:26 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 14 Apr 2021 19:06:27 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Apr 2021 19:06:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Apr 2021 19:06:28 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 07:30:47 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 07:30:58 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 07:30:58 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 07:31:01 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 07:31:02 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 07:31:02 GMT
WORKDIR /app
# Thu, 15 Apr 2021 07:31:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:31:03 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbe2d3d9b1efb815eb614a3488743bc95ac05e1ae4b0b1e2b488a057a9697f2`  
		Last Modified: Wed, 14 Apr 2021 20:01:03 GMT  
		Size: 10.8 MB (10775158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42d806dde82abd1fa888745f98a91c4a389d70968f69ee9fb1d467acf94c233`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3407c21d5517a5fe9bee65ffefce1b436496f08d54e5ec826713de143cc769a1`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 14.0 MB (13972054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673772f281ad30fa5e8f68f1b2cc7246eb505f77b1304eeffee4ed02e2ac0025`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887ade51969a265f267fab2842da16aee5c3746eebee780035a2e8e30b486de`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 17.6 KB (17552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827a7ecf83cc085e8c067e3fb91cc8be53232ed95c0f1344337b305382d525d5`  
		Last Modified: Thu, 15 Apr 2021 07:31:34 GMT  
		Size: 31.4 MB (31391511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ddcc417205411563d9531ffab3b6e85ece64c95e6e494b9a7eac77bf621e25`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 197.8 KB (197750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f23536fe9ce1e18934446f30900cd733051f3573df86ecd7dd71a23e7047420`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92975974c01eb23ef0604971c31c1552e1f9ba01d8712691b66b89e178d2cec4`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 555.4 KB (555366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd0d197e8c109ca4c634e2e48a35bd63c4dec1e95e8fc1c94dab6c3ad043992`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901dc3c5be755d5e73ffd749eb62730c29440327d1bfe3fa7a0546c20bd09dfe`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `composer:2.0`

```console
$ docker pull composer@sha256:f9aeec5f62e0f46cd92b2cfa54dff3243a9e1d05ab5ae27f034611955b14c4f2
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
$ docker pull composer@sha256:16c5c79db16eb9818aa6fa5012249e0fc4227afd5c161a3629d24de2ebb3ec6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62175820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee1fb424607c015745450cb9649f91855516264b22a6130a6ece9d49c234129`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 23:59:24 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 23:59:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 23:59:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:08:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 00:08:23 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:08:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 00:08:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 00:08:24 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 10:15:35 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 10:15:45 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 10:15:46 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 10:15:46 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 10:15:46 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 10:15:47 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 10:15:50 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 10:15:50 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 10:15:50 GMT
WORKDIR /app
# Thu, 15 Apr 2021 10:15:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 10:15:51 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e582385a5d67543612fd95df7b619a8572c549e16543153bf264ad3459de5d0`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 10.8 MB (10775177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19324c9462cc1b74101165f6e7a7cfc384c6be4378ad98522841c48586380e46`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e94dc0b377148e2f02341f71c676a50265f14e42eda33d323024c1fbf07215`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 15.0 MB (14950314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da582f37592e6a319e1d4f97ce5a0e1cf3d19cd7307747c2c07f6abaafcda759`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f821502d3ad8cce566cd0aae6d9b755c841ec8d0e26ef357c746410e3c2777e5`  
		Last Modified: Thu, 15 Apr 2021 02:15:21 GMT  
		Size: 17.5 KB (17535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e24ebb98a1ce7def46c39cfc32402e1be33d692ddafa8ccaef827bde3747ac`  
		Last Modified: Thu, 15 Apr 2021 10:16:23 GMT  
		Size: 31.2 MB (31159862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efaa46072d9058afcc9a9dfd299bb0dcb820c6aa8b2dff42a8cc26933e659d6`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 198.3 KB (198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e430c6f8c1e75e9188c61b5c734cd9f1fb0629eac403ba4eae56eea95fd85ee`  
		Last Modified: Thu, 15 Apr 2021 10:16:18 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366029d47da932cfa6bd72678d28a15f9006a7d6e70e8f61de4188c45b7a5371`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 555.4 KB (555370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5331243868df570248b0a1bc44a53c37e3e3b1d814c046a30ea3672fc12e8faf`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1c5eae9bf5060077bf987273f9a2691a7b1c9d138a0ca47edac68ea5e84490`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0` - linux; arm variant v6

```console
$ docker pull composer@sha256:e8fed4e7a57e97c313a8eb81ba749be03bd3e0d3e10e48115f416ea2fc695a6b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58411527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d89e493f7388277d91d3933bfa3e164bacb732cfd8b0b583b7b739554066908a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:06:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:07:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:07:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:07:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:07:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:07:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:07:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 01:07:33 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 01:07:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 01:07:37 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 01:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 01:07:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:12:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 01:12:53 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:12:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 01:12:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 01:12:59 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 07:11:04 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 07:11:25 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 07:11:27 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 07:11:28 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 07:11:29 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 07:11:29 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 07:11:33 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 07:11:34 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 07:11:34 GMT
WORKDIR /app
# Thu, 15 Apr 2021 07:11:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:11:36 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726cd3e9e578579e631e21133870b656f3938f6a87797a842254b274d8b76e8`  
		Last Modified: Thu, 15 Apr 2021 02:33:02 GMT  
		Size: 1.7 MB (1690998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db188e87a6ea4fd0959949208b039a0d9facc96183df8dc346c6d0d3368b77e`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73dce0ed56811623cd40b786e95b951ce9d6341d9bfefded4f8aa12574283`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d5ea4d59593d016379b8d7cf9d074ab74527314a70c4ab2224e030bcce918`  
		Last Modified: Thu, 15 Apr 2021 02:33:04 GMT  
		Size: 10.8 MB (10775163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09c200324804241421da31f3b8cb8c3d7b006322de86d71d500fbdba136a885`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c0a1a831eaec187029e84f1bb7de5acc585a3b96fbfceaf583a3b36731c083`  
		Last Modified: Thu, 15 Apr 2021 02:33:14 GMT  
		Size: 13.6 MB (13585216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ad658b06066f3e4c692de9e3e1d8dbdd37dd05e3c3863e2f7cc8e6947e4df8`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e563207cd5c65809f0cb70dc82a30fb3ff8a2bb948740cd511ad08fa51a0d38`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 17.5 KB (17533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7322cd551e2d84436e4a4730a66208de66ff94b2946927fc56b146a5b180e41`  
		Last Modified: Thu, 15 Apr 2021 07:12:19 GMT  
		Size: 29.0 MB (28966488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed30edea345eb014ce9274ab7e0c12d0e6b1bf113bb2832146ab41759202280`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 193.6 KB (193560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7850310f2473f2085694f0ae25645d1dbeed617879390675b835e24400817d0c`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e685f6d884207cd5821b189eb07436155ade2322ac14aa66466867f752d8b7`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 555.4 KB (555368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f80e0514909b04305b8652003c9f83308cdab5d4a3ff3ed6fdc75f92c7f6a8`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a531f1e7eee172868524f968eab1cd50d794e2f51df222f44024e4b4569fb004`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0` - linux; arm variant v7

```console
$ docker pull composer@sha256:f47db64626aa0085a31f4f87332a4c85e1f1b0e6dab6bbd9e0e6d59cbebc17b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55893814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f41fa048e70a27fbd80e3aebb25f5d2a785e4172c8675a1375062fd4af23fe4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:08:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:08:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:08:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:08:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:08:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:08:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:08:54 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 02:09:03 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 02:09:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 02:09:29 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 02:10:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 02:11:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 02:15:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 02:16:01 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 02:16:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 02:16:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 02:16:08 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:32:23 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:32:41 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:32:43 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:32:44 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:32:45 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:32:45 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 08:32:49 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:32:50 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:32:50 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:32:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:32:52 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc6d3f07b2e440bf9a8e52a0a5bba0f27637990ee4976424cef6aae97e169f`  
		Last Modified: Thu, 15 Apr 2021 03:38:53 GMT  
		Size: 1.6 MB (1559061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9000ca9dcd92a2066a3a2c4031e677c3998cd82a3ecbc68468d11255ecbdb62`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d102949f174ecad1044574e45dded8368eb7451bf66b3bdac6e367c7f415d3`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92da8c0a1f3fbf1d4e02eaa533a5058c129447984212a6ff3c72bcc9cad8ab61`  
		Last Modified: Thu, 15 Apr 2021 03:38:54 GMT  
		Size: 10.8 MB (10775172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e011c8a33e544331ac43001738b66a746be18150ffd02e029e1781842dcc4706`  
		Last Modified: Thu, 15 Apr 2021 03:38:48 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61492dda820b711430b6f09aeb0af17f5efb9740a6147244fe1bcf9351a077b`  
		Last Modified: Thu, 15 Apr 2021 03:38:56 GMT  
		Size: 12.7 MB (12733009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e0a3051e72edd5461eda9dc5ad8e0d0b59e55fa0aee85a35da5251839f7f48`  
		Last Modified: Thu, 15 Apr 2021 03:38:47 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e451143ba28ebc0296ff08f6566c5e1d12c219c54351d23e2cb6cd545e2e009a`  
		Last Modified: Thu, 15 Apr 2021 03:38:47 GMT  
		Size: 17.5 KB (17537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3ae47db92bb3e5c1668c4815a02f3a46f82c32e59aa4e9317ea9a4d808399c`  
		Last Modified: Thu, 15 Apr 2021 08:33:40 GMT  
		Size: 27.6 MB (27638087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cacea819616d21dfc105f33ca411a910a2f359b1ab8bad9f43943880dc2a76`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 186.4 KB (186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64cc5abdecaef6df8f69965b45b6b83a146dac9487e208895b0bc28bbf32525`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8f3a04e083b38b70dd19677baec0ff048eb0fd89827dec3a96c132afe5e282`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 555.4 KB (555369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196939056fb545323ea4219e28a3234097584c6fb32bd88616623aeabd5950bd`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83917393c8cb3c21a26875ace50b2b0b932c89355a39682da0c90b692ff404cb`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:58f7fcb3ddaf67e05162f3b09b0ee5652e65ff73ec9bcb794ed2d924caccee0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61694374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e3dec03a7d85bd434ed450c0bb62fd938a7fb193544337828c665e6480fffa`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:27:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:28:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:28:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:28:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:28:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:28:27 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 00:28:29 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 00:28:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 00:28:33 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 00:28:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 00:28:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:34:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 00:34:40 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:34:47 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 00:34:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 00:34:50 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:56:13 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:56:38 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:56:41 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:56:42 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:56:43 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:56:45 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 08:56:50 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:56:52 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:56:55 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:56:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:56:58 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea792edc0a65854bc13c90079b9e33a399c351b73e194d9df4f2cf5a0efeb2`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 1.7 MB (1700262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31bbfcb500579a0c450809a6b082c564c3ce4873732c1b62d8dab52ed0a11ac`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22841fe152c1fe4ec2048ebca3b9c0db9d29773b0d0670167a848d87fcfe83f3`  
		Last Modified: Thu, 15 Apr 2021 01:59:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61644ef55a78b8c8188acffca32263b12c8684a851a14a3fadc9f9c81d83c6e`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 10.8 MB (10775183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512fc0b44c8ccf1bcd4977baa78bd06876049fbefea93ca3a60d8406b53192c2`  
		Last Modified: Thu, 15 Apr 2021 01:59:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e853e5eed6ac911854cde2862e6607daf5c31850a72c856823616ad5ab566d`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 14.4 MB (14377741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bf5108bfbb40bc73cdd1e0df396ea55f8551e26c78af8e0b455b6bb2f0792e`  
		Last Modified: Thu, 15 Apr 2021 01:59:49 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127cb6e69cb6e4805c0d326498d5b9ebf45069ce7dd5c5cb94558188945baa9b`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad50c34e5614c2df0de39bfe9e05281b6b88a4cdb3c4783d80b00d4e72de6d33`  
		Last Modified: Thu, 15 Apr 2021 08:57:51 GMT  
		Size: 31.4 MB (31355216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d5b566318e8b07a0e09bffb639f37240aa5b1afbf68d7bb3aa7d9ee722e8c`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 195.9 KB (195947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9624473eddbb2b7517d6b3ec640bc13c5deae479b44cfdc7781a6dd517ff06`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0ea7aee59bc8c381ebf13e07f17a0a905147840a2a9813ba638e539f1f73e7`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 555.4 KB (555369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b9b6647561cc710659eec729f81d22f355bff35620854e6fe9e38b390b1a9a`  
		Last Modified: Thu, 15 Apr 2021 08:57:42 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bfd31c2ac4ef646c259c246c3ede82c00cd5aa28d34cad3b5ef2b2bba4bf25`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0` - linux; 386

```console
$ docker pull composer@sha256:70bc0657ac9d955ed89d5ea044768e0bf45b3a7226170ff6d48325a9d9787d9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.5 MB (63459840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8dd0b260971d5fcb96c0533acb7fa361b9d87ba87d71a3bfb54d32177317ef2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 03:38:49 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 03:39:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 03:39:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:45:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 03:45:10 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:45:12 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 03:45:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 03:45:13 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:52:55 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:53:10 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:53:11 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:53:11 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:53:12 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:53:12 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 08:53:15 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:53:15 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:53:15 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:53:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:53:16 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeccee8de2519293816e97d37497a11495840e4c2edb7ad1254ce80fc59737a`  
		Last Modified: Thu, 15 Apr 2021 05:57:42 GMT  
		Size: 10.8 MB (10775154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962c132cc514121c8ad9862e99f06f647cbc70e07305e12cde1c0e8986f4de2d`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf4252825c42e4fc0d1dd2328fc4fbae3271919571b76a5dd55b1a5a63f3c8b`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 15.0 MB (14974551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7085eb2c648a88168bff8bcfeb7ef1f366a6c134a86b2e22fb7b2dc37479ea38`  
		Last Modified: Thu, 15 Apr 2021 05:57:40 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7ddb662add691a4ef54081ad454d11303541f3b4398453b7c72070b39bbeee`  
		Last Modified: Thu, 15 Apr 2021 05:57:40 GMT  
		Size: 17.5 KB (17533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d4448c8736ab950ed57d33c37776a00fe02282664f5316431b408f76ebccef`  
		Last Modified: Thu, 15 Apr 2021 08:54:02 GMT  
		Size: 32.3 MB (32300139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadf752d16c9b4f5ebcbf8f8ee774377e7e479e31c9900f14d6e8252b89e9686`  
		Last Modified: Thu, 15 Apr 2021 08:53:53 GMT  
		Size: 213.8 KB (213841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30932fd99a342f62c81464b27cb9398d3638e9caeaf2d233d5cf3bbde4114028`  
		Last Modified: Thu, 15 Apr 2021 08:53:53 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359d5d64671b2b5de602c4f62ad00c7bad415822942d43fdbaff23995c637c83`  
		Last Modified: Thu, 15 Apr 2021 08:53:52 GMT  
		Size: 555.4 KB (555376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1662864d2b5ac55354e0d61fcefc60ae2f41afe4349fc86c0df7e756bb512f`  
		Last Modified: Thu, 15 Apr 2021 08:53:51 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff352cc745257d9f7c02042f4f03cc762fc0ee9c0f45d3d10657b26ff0395ad`  
		Last Modified: Thu, 15 Apr 2021 08:53:50 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0` - linux; ppc64le

```console
$ docker pull composer@sha256:ca8bcb0fad3c8c75791a7321ccbadd72dc179e18cfbf95b820714ce1d7affde1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63789841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9ee919c2f8f85644a637e78d057398a9759a722d8e5025c7b9fbc39b93004a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:16:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:16:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 20:16:59 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 20:17:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 20:17:24 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 20:17:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:23:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Apr 2021 20:23:31 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:23:50 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Apr 2021 20:23:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Apr 2021 20:24:03 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:44:10 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:44:50 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:45:13 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:45:19 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:45:26 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:45:35 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 08:45:55 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:46:00 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:46:08 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:46:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:46:16 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6431deb07f4adae4be0bd4b93d784bb08ec63d03daa512d835bbc0230e05cf3`  
		Last Modified: Wed, 14 Apr 2021 22:00:57 GMT  
		Size: 10.8 MB (10775172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3ef816305c1c138c8c7ce8fbacf23f59654a7422858f578711604d0819539d`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171f3408ea103656d215c6b47106245684e915481a4ae3bc5b613d2f98f6b219`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 15.7 MB (15673187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5517add7dc81698b49a4430b992ab0bb4a012fbd04792d17b4754fe392f24014`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4888f0381bb3c52192f3c448b3bf6fd7906a41b23b8ac854a82340a8aa6171`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 17.6 KB (17556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f596040cc5835db2f0e35314704e491260222aa43948cc3c84967912a555a993`  
		Last Modified: Thu, 15 Apr 2021 08:47:37 GMT  
		Size: 32.0 MB (31997694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc29da636c9f65c118437157394b275676967a063d7b8cbf33ab5faca6c591c`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 204.0 KB (204005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef3767002a509df55f5149f3fb25a788238d75bd23a9cb0d17af0ae11ec7a0c`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871523e4535d7b29028c6ba393e95315523bbd18d9ad4f6a313a36a3afb70d82`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 555.4 KB (555372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9b40f1162d15bc30f530fac32dbe79c562e0264f9378dd49e1e74bcda62fd0`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656cf3e249e69c2dd27fc4f38787633f612acbb71cb7645068b1946df2fb17de`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0` - linux; s390x

```console
$ docker pull composer@sha256:c8c4b8992d176fba657c9fed5cdbee13cf76d0fa9fa791ea1abaf59866bce2f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61277823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb15eb7b90d1e5576f452170f25168185d47f8d957f0fc34c6712e8e1d41df12`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:00:59 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 19:01:00 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 19:01:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 19:01:01 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 19:01:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 19:01:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Apr 2021 19:06:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Apr 2021 19:06:26 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 14 Apr 2021 19:06:27 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Apr 2021 19:06:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Apr 2021 19:06:28 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 07:30:47 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 07:30:58 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 07:30:58 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 07:31:01 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 07:31:02 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 07:31:02 GMT
WORKDIR /app
# Thu, 15 Apr 2021 07:31:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:31:03 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbe2d3d9b1efb815eb614a3488743bc95ac05e1ae4b0b1e2b488a057a9697f2`  
		Last Modified: Wed, 14 Apr 2021 20:01:03 GMT  
		Size: 10.8 MB (10775158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42d806dde82abd1fa888745f98a91c4a389d70968f69ee9fb1d467acf94c233`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3407c21d5517a5fe9bee65ffefce1b436496f08d54e5ec826713de143cc769a1`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 14.0 MB (13972054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673772f281ad30fa5e8f68f1b2cc7246eb505f77b1304eeffee4ed02e2ac0025`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887ade51969a265f267fab2842da16aee5c3746eebee780035a2e8e30b486de`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 17.6 KB (17552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827a7ecf83cc085e8c067e3fb91cc8be53232ed95c0f1344337b305382d525d5`  
		Last Modified: Thu, 15 Apr 2021 07:31:34 GMT  
		Size: 31.4 MB (31391511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ddcc417205411563d9531ffab3b6e85ece64c95e6e494b9a7eac77bf621e25`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 197.8 KB (197750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f23536fe9ce1e18934446f30900cd733051f3573df86ecd7dd71a23e7047420`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92975974c01eb23ef0604971c31c1552e1f9ba01d8712691b66b89e178d2cec4`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 555.4 KB (555366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd0d197e8c109ca4c634e2e48a35bd63c4dec1e95e8fc1c94dab6c3ad043992`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901dc3c5be755d5e73ffd749eb62730c29440327d1bfe3fa7a0546c20bd09dfe`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `composer:2.0.12`

```console
$ docker pull composer@sha256:f9aeec5f62e0f46cd92b2cfa54dff3243a9e1d05ab5ae27f034611955b14c4f2
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

### `composer:2.0.12` - linux; amd64

```console
$ docker pull composer@sha256:16c5c79db16eb9818aa6fa5012249e0fc4227afd5c161a3629d24de2ebb3ec6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62175820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee1fb424607c015745450cb9649f91855516264b22a6130a6ece9d49c234129`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 23:59:24 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 23:59:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 23:59:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:08:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 00:08:23 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:08:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 00:08:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 00:08:24 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 10:15:35 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 10:15:45 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 10:15:46 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 10:15:46 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 10:15:46 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 10:15:47 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 10:15:50 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 10:15:50 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 10:15:50 GMT
WORKDIR /app
# Thu, 15 Apr 2021 10:15:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 10:15:51 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e582385a5d67543612fd95df7b619a8572c549e16543153bf264ad3459de5d0`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 10.8 MB (10775177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19324c9462cc1b74101165f6e7a7cfc384c6be4378ad98522841c48586380e46`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e94dc0b377148e2f02341f71c676a50265f14e42eda33d323024c1fbf07215`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 15.0 MB (14950314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da582f37592e6a319e1d4f97ce5a0e1cf3d19cd7307747c2c07f6abaafcda759`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f821502d3ad8cce566cd0aae6d9b755c841ec8d0e26ef357c746410e3c2777e5`  
		Last Modified: Thu, 15 Apr 2021 02:15:21 GMT  
		Size: 17.5 KB (17535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e24ebb98a1ce7def46c39cfc32402e1be33d692ddafa8ccaef827bde3747ac`  
		Last Modified: Thu, 15 Apr 2021 10:16:23 GMT  
		Size: 31.2 MB (31159862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efaa46072d9058afcc9a9dfd299bb0dcb820c6aa8b2dff42a8cc26933e659d6`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 198.3 KB (198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e430c6f8c1e75e9188c61b5c734cd9f1fb0629eac403ba4eae56eea95fd85ee`  
		Last Modified: Thu, 15 Apr 2021 10:16:18 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366029d47da932cfa6bd72678d28a15f9006a7d6e70e8f61de4188c45b7a5371`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 555.4 KB (555370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5331243868df570248b0a1bc44a53c37e3e3b1d814c046a30ea3672fc12e8faf`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1c5eae9bf5060077bf987273f9a2691a7b1c9d138a0ca47edac68ea5e84490`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0.12` - linux; arm variant v6

```console
$ docker pull composer@sha256:e8fed4e7a57e97c313a8eb81ba749be03bd3e0d3e10e48115f416ea2fc695a6b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58411527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d89e493f7388277d91d3933bfa3e164bacb732cfd8b0b583b7b739554066908a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:06:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:07:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:07:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:07:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:07:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:07:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:07:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 01:07:33 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 01:07:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 01:07:37 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 01:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 01:07:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:12:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 01:12:53 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:12:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 01:12:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 01:12:59 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 07:11:04 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 07:11:25 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 07:11:27 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 07:11:28 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 07:11:29 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 07:11:29 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 07:11:33 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 07:11:34 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 07:11:34 GMT
WORKDIR /app
# Thu, 15 Apr 2021 07:11:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:11:36 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726cd3e9e578579e631e21133870b656f3938f6a87797a842254b274d8b76e8`  
		Last Modified: Thu, 15 Apr 2021 02:33:02 GMT  
		Size: 1.7 MB (1690998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db188e87a6ea4fd0959949208b039a0d9facc96183df8dc346c6d0d3368b77e`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73dce0ed56811623cd40b786e95b951ce9d6341d9bfefded4f8aa12574283`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d5ea4d59593d016379b8d7cf9d074ab74527314a70c4ab2224e030bcce918`  
		Last Modified: Thu, 15 Apr 2021 02:33:04 GMT  
		Size: 10.8 MB (10775163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09c200324804241421da31f3b8cb8c3d7b006322de86d71d500fbdba136a885`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c0a1a831eaec187029e84f1bb7de5acc585a3b96fbfceaf583a3b36731c083`  
		Last Modified: Thu, 15 Apr 2021 02:33:14 GMT  
		Size: 13.6 MB (13585216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ad658b06066f3e4c692de9e3e1d8dbdd37dd05e3c3863e2f7cc8e6947e4df8`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e563207cd5c65809f0cb70dc82a30fb3ff8a2bb948740cd511ad08fa51a0d38`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 17.5 KB (17533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7322cd551e2d84436e4a4730a66208de66ff94b2946927fc56b146a5b180e41`  
		Last Modified: Thu, 15 Apr 2021 07:12:19 GMT  
		Size: 29.0 MB (28966488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed30edea345eb014ce9274ab7e0c12d0e6b1bf113bb2832146ab41759202280`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 193.6 KB (193560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7850310f2473f2085694f0ae25645d1dbeed617879390675b835e24400817d0c`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e685f6d884207cd5821b189eb07436155ade2322ac14aa66466867f752d8b7`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 555.4 KB (555368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f80e0514909b04305b8652003c9f83308cdab5d4a3ff3ed6fdc75f92c7f6a8`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a531f1e7eee172868524f968eab1cd50d794e2f51df222f44024e4b4569fb004`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0.12` - linux; arm variant v7

```console
$ docker pull composer@sha256:f47db64626aa0085a31f4f87332a4c85e1f1b0e6dab6bbd9e0e6d59cbebc17b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55893814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f41fa048e70a27fbd80e3aebb25f5d2a785e4172c8675a1375062fd4af23fe4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:08:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:08:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:08:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:08:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:08:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:08:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:08:54 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 02:09:03 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 02:09:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 02:09:29 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 02:10:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 02:11:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 02:15:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 02:16:01 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 02:16:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 02:16:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 02:16:08 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:32:23 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:32:41 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:32:43 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:32:44 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:32:45 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:32:45 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 08:32:49 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:32:50 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:32:50 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:32:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:32:52 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc6d3f07b2e440bf9a8e52a0a5bba0f27637990ee4976424cef6aae97e169f`  
		Last Modified: Thu, 15 Apr 2021 03:38:53 GMT  
		Size: 1.6 MB (1559061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9000ca9dcd92a2066a3a2c4031e677c3998cd82a3ecbc68468d11255ecbdb62`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d102949f174ecad1044574e45dded8368eb7451bf66b3bdac6e367c7f415d3`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92da8c0a1f3fbf1d4e02eaa533a5058c129447984212a6ff3c72bcc9cad8ab61`  
		Last Modified: Thu, 15 Apr 2021 03:38:54 GMT  
		Size: 10.8 MB (10775172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e011c8a33e544331ac43001738b66a746be18150ffd02e029e1781842dcc4706`  
		Last Modified: Thu, 15 Apr 2021 03:38:48 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61492dda820b711430b6f09aeb0af17f5efb9740a6147244fe1bcf9351a077b`  
		Last Modified: Thu, 15 Apr 2021 03:38:56 GMT  
		Size: 12.7 MB (12733009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e0a3051e72edd5461eda9dc5ad8e0d0b59e55fa0aee85a35da5251839f7f48`  
		Last Modified: Thu, 15 Apr 2021 03:38:47 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e451143ba28ebc0296ff08f6566c5e1d12c219c54351d23e2cb6cd545e2e009a`  
		Last Modified: Thu, 15 Apr 2021 03:38:47 GMT  
		Size: 17.5 KB (17537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3ae47db92bb3e5c1668c4815a02f3a46f82c32e59aa4e9317ea9a4d808399c`  
		Last Modified: Thu, 15 Apr 2021 08:33:40 GMT  
		Size: 27.6 MB (27638087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cacea819616d21dfc105f33ca411a910a2f359b1ab8bad9f43943880dc2a76`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 186.4 KB (186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64cc5abdecaef6df8f69965b45b6b83a146dac9487e208895b0bc28bbf32525`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8f3a04e083b38b70dd19677baec0ff048eb0fd89827dec3a96c132afe5e282`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 555.4 KB (555369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196939056fb545323ea4219e28a3234097584c6fb32bd88616623aeabd5950bd`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83917393c8cb3c21a26875ace50b2b0b932c89355a39682da0c90b692ff404cb`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0.12` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:58f7fcb3ddaf67e05162f3b09b0ee5652e65ff73ec9bcb794ed2d924caccee0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61694374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e3dec03a7d85bd434ed450c0bb62fd938a7fb193544337828c665e6480fffa`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:27:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:28:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:28:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:28:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:28:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:28:27 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 00:28:29 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 00:28:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 00:28:33 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 00:28:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 00:28:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:34:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 00:34:40 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:34:47 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 00:34:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 00:34:50 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:56:13 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:56:38 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:56:41 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:56:42 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:56:43 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:56:45 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 08:56:50 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:56:52 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:56:55 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:56:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:56:58 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea792edc0a65854bc13c90079b9e33a399c351b73e194d9df4f2cf5a0efeb2`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 1.7 MB (1700262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31bbfcb500579a0c450809a6b082c564c3ce4873732c1b62d8dab52ed0a11ac`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22841fe152c1fe4ec2048ebca3b9c0db9d29773b0d0670167a848d87fcfe83f3`  
		Last Modified: Thu, 15 Apr 2021 01:59:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61644ef55a78b8c8188acffca32263b12c8684a851a14a3fadc9f9c81d83c6e`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 10.8 MB (10775183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512fc0b44c8ccf1bcd4977baa78bd06876049fbefea93ca3a60d8406b53192c2`  
		Last Modified: Thu, 15 Apr 2021 01:59:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e853e5eed6ac911854cde2862e6607daf5c31850a72c856823616ad5ab566d`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 14.4 MB (14377741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bf5108bfbb40bc73cdd1e0df396ea55f8551e26c78af8e0b455b6bb2f0792e`  
		Last Modified: Thu, 15 Apr 2021 01:59:49 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127cb6e69cb6e4805c0d326498d5b9ebf45069ce7dd5c5cb94558188945baa9b`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad50c34e5614c2df0de39bfe9e05281b6b88a4cdb3c4783d80b00d4e72de6d33`  
		Last Modified: Thu, 15 Apr 2021 08:57:51 GMT  
		Size: 31.4 MB (31355216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d5b566318e8b07a0e09bffb639f37240aa5b1afbf68d7bb3aa7d9ee722e8c`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 195.9 KB (195947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9624473eddbb2b7517d6b3ec640bc13c5deae479b44cfdc7781a6dd517ff06`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0ea7aee59bc8c381ebf13e07f17a0a905147840a2a9813ba638e539f1f73e7`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 555.4 KB (555369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b9b6647561cc710659eec729f81d22f355bff35620854e6fe9e38b390b1a9a`  
		Last Modified: Thu, 15 Apr 2021 08:57:42 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bfd31c2ac4ef646c259c246c3ede82c00cd5aa28d34cad3b5ef2b2bba4bf25`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0.12` - linux; 386

```console
$ docker pull composer@sha256:70bc0657ac9d955ed89d5ea044768e0bf45b3a7226170ff6d48325a9d9787d9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.5 MB (63459840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8dd0b260971d5fcb96c0533acb7fa361b9d87ba87d71a3bfb54d32177317ef2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 03:38:49 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 03:39:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 03:39:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:45:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 03:45:10 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:45:12 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 03:45:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 03:45:13 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:52:55 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:53:10 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:53:11 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:53:11 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:53:12 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:53:12 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 08:53:15 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:53:15 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:53:15 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:53:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:53:16 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeccee8de2519293816e97d37497a11495840e4c2edb7ad1254ce80fc59737a`  
		Last Modified: Thu, 15 Apr 2021 05:57:42 GMT  
		Size: 10.8 MB (10775154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962c132cc514121c8ad9862e99f06f647cbc70e07305e12cde1c0e8986f4de2d`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf4252825c42e4fc0d1dd2328fc4fbae3271919571b76a5dd55b1a5a63f3c8b`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 15.0 MB (14974551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7085eb2c648a88168bff8bcfeb7ef1f366a6c134a86b2e22fb7b2dc37479ea38`  
		Last Modified: Thu, 15 Apr 2021 05:57:40 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7ddb662add691a4ef54081ad454d11303541f3b4398453b7c72070b39bbeee`  
		Last Modified: Thu, 15 Apr 2021 05:57:40 GMT  
		Size: 17.5 KB (17533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d4448c8736ab950ed57d33c37776a00fe02282664f5316431b408f76ebccef`  
		Last Modified: Thu, 15 Apr 2021 08:54:02 GMT  
		Size: 32.3 MB (32300139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadf752d16c9b4f5ebcbf8f8ee774377e7e479e31c9900f14d6e8252b89e9686`  
		Last Modified: Thu, 15 Apr 2021 08:53:53 GMT  
		Size: 213.8 KB (213841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30932fd99a342f62c81464b27cb9398d3638e9caeaf2d233d5cf3bbde4114028`  
		Last Modified: Thu, 15 Apr 2021 08:53:53 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359d5d64671b2b5de602c4f62ad00c7bad415822942d43fdbaff23995c637c83`  
		Last Modified: Thu, 15 Apr 2021 08:53:52 GMT  
		Size: 555.4 KB (555376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1662864d2b5ac55354e0d61fcefc60ae2f41afe4349fc86c0df7e756bb512f`  
		Last Modified: Thu, 15 Apr 2021 08:53:51 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff352cc745257d9f7c02042f4f03cc762fc0ee9c0f45d3d10657b26ff0395ad`  
		Last Modified: Thu, 15 Apr 2021 08:53:50 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0.12` - linux; ppc64le

```console
$ docker pull composer@sha256:ca8bcb0fad3c8c75791a7321ccbadd72dc179e18cfbf95b820714ce1d7affde1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63789841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9ee919c2f8f85644a637e78d057398a9759a722d8e5025c7b9fbc39b93004a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:16:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:16:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 20:16:59 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 20:17:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 20:17:24 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 20:17:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:23:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Apr 2021 20:23:31 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:23:50 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Apr 2021 20:23:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Apr 2021 20:24:03 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:44:10 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:44:50 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:45:13 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:45:19 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:45:26 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:45:35 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 08:45:55 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:46:00 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:46:08 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:46:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:46:16 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6431deb07f4adae4be0bd4b93d784bb08ec63d03daa512d835bbc0230e05cf3`  
		Last Modified: Wed, 14 Apr 2021 22:00:57 GMT  
		Size: 10.8 MB (10775172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3ef816305c1c138c8c7ce8fbacf23f59654a7422858f578711604d0819539d`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171f3408ea103656d215c6b47106245684e915481a4ae3bc5b613d2f98f6b219`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 15.7 MB (15673187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5517add7dc81698b49a4430b992ab0bb4a012fbd04792d17b4754fe392f24014`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4888f0381bb3c52192f3c448b3bf6fd7906a41b23b8ac854a82340a8aa6171`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 17.6 KB (17556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f596040cc5835db2f0e35314704e491260222aa43948cc3c84967912a555a993`  
		Last Modified: Thu, 15 Apr 2021 08:47:37 GMT  
		Size: 32.0 MB (31997694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc29da636c9f65c118437157394b275676967a063d7b8cbf33ab5faca6c591c`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 204.0 KB (204005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef3767002a509df55f5149f3fb25a788238d75bd23a9cb0d17af0ae11ec7a0c`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871523e4535d7b29028c6ba393e95315523bbd18d9ad4f6a313a36a3afb70d82`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 555.4 KB (555372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9b40f1162d15bc30f530fac32dbe79c562e0264f9378dd49e1e74bcda62fd0`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656cf3e249e69c2dd27fc4f38787633f612acbb71cb7645068b1946df2fb17de`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:2.0.12` - linux; s390x

```console
$ docker pull composer@sha256:c8c4b8992d176fba657c9fed5cdbee13cf76d0fa9fa791ea1abaf59866bce2f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61277823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb15eb7b90d1e5576f452170f25168185d47f8d957f0fc34c6712e8e1d41df12`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:00:59 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 19:01:00 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 19:01:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 19:01:01 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 19:01:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 19:01:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Apr 2021 19:06:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Apr 2021 19:06:26 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 14 Apr 2021 19:06:27 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Apr 2021 19:06:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Apr 2021 19:06:28 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 07:30:47 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 07:30:58 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 07:30:58 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 07:31:01 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 07:31:02 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 07:31:02 GMT
WORKDIR /app
# Thu, 15 Apr 2021 07:31:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:31:03 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbe2d3d9b1efb815eb614a3488743bc95ac05e1ae4b0b1e2b488a057a9697f2`  
		Last Modified: Wed, 14 Apr 2021 20:01:03 GMT  
		Size: 10.8 MB (10775158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42d806dde82abd1fa888745f98a91c4a389d70968f69ee9fb1d467acf94c233`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3407c21d5517a5fe9bee65ffefce1b436496f08d54e5ec826713de143cc769a1`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 14.0 MB (13972054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673772f281ad30fa5e8f68f1b2cc7246eb505f77b1304eeffee4ed02e2ac0025`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887ade51969a265f267fab2842da16aee5c3746eebee780035a2e8e30b486de`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 17.6 KB (17552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827a7ecf83cc085e8c067e3fb91cc8be53232ed95c0f1344337b305382d525d5`  
		Last Modified: Thu, 15 Apr 2021 07:31:34 GMT  
		Size: 31.4 MB (31391511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ddcc417205411563d9531ffab3b6e85ece64c95e6e494b9a7eac77bf621e25`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 197.8 KB (197750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f23536fe9ce1e18934446f30900cd733051f3573df86ecd7dd71a23e7047420`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92975974c01eb23ef0604971c31c1552e1f9ba01d8712691b66b89e178d2cec4`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 555.4 KB (555366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd0d197e8c109ca4c634e2e48a35bd63c4dec1e95e8fc1c94dab6c3ad043992`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901dc3c5be755d5e73ffd749eb62730c29440327d1bfe3fa7a0546c20bd09dfe`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `composer:latest`

```console
$ docker pull composer@sha256:f9aeec5f62e0f46cd92b2cfa54dff3243a9e1d05ab5ae27f034611955b14c4f2
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
$ docker pull composer@sha256:16c5c79db16eb9818aa6fa5012249e0fc4227afd5c161a3629d24de2ebb3ec6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.2 MB (62175820 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fee1fb424607c015745450cb9649f91855516264b22a6130a6ece9d49c234129`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 23:59:24 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 23:59:25 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 23:59:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 23:59:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:08:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 00:08:23 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:08:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 00:08:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 00:08:24 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 10:15:35 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 10:15:45 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 10:15:46 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 10:15:46 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 10:15:46 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 10:15:47 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 10:15:50 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 10:15:50 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 10:15:50 GMT
WORKDIR /app
# Thu, 15 Apr 2021 10:15:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 10:15:51 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e582385a5d67543612fd95df7b619a8572c549e16543153bf264ad3459de5d0`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 10.8 MB (10775177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19324c9462cc1b74101165f6e7a7cfc384c6be4378ad98522841c48586380e46`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e94dc0b377148e2f02341f71c676a50265f14e42eda33d323024c1fbf07215`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 15.0 MB (14950314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da582f37592e6a319e1d4f97ce5a0e1cf3d19cd7307747c2c07f6abaafcda759`  
		Last Modified: Thu, 15 Apr 2021 02:15:20 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f821502d3ad8cce566cd0aae6d9b755c841ec8d0e26ef357c746410e3c2777e5`  
		Last Modified: Thu, 15 Apr 2021 02:15:21 GMT  
		Size: 17.5 KB (17535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e24ebb98a1ce7def46c39cfc32402e1be33d692ddafa8ccaef827bde3747ac`  
		Last Modified: Thu, 15 Apr 2021 10:16:23 GMT  
		Size: 31.2 MB (31159862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0efaa46072d9058afcc9a9dfd299bb0dcb820c6aa8b2dff42a8cc26933e659d6`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 198.3 KB (198330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e430c6f8c1e75e9188c61b5c734cd9f1fb0629eac403ba4eae56eea95fd85ee`  
		Last Modified: Thu, 15 Apr 2021 10:16:18 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:366029d47da932cfa6bd72678d28a15f9006a7d6e70e8f61de4188c45b7a5371`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 555.4 KB (555370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5331243868df570248b0a1bc44a53c37e3e3b1d814c046a30ea3672fc12e8faf`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1c5eae9bf5060077bf987273f9a2691a7b1c9d138a0ca47edac68ea5e84490`  
		Last Modified: Thu, 15 Apr 2021 10:16:15 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; arm variant v6

```console
$ docker pull composer@sha256:e8fed4e7a57e97c313a8eb81ba749be03bd3e0d3e10e48115f416ea2fc695a6b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.4 MB (58411527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d89e493f7388277d91d3933bfa3e164bacb732cfd8b0b583b7b739554066908a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:06:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:07:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:07:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:07:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:07:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:07:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:07:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 01:07:33 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 01:07:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 01:07:37 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 01:07:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 01:07:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:12:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 01:12:53 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 01:12:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 01:12:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 01:12:59 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 07:11:04 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 07:11:25 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 07:11:27 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 07:11:28 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 07:11:29 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 07:11:29 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 07:11:33 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 07:11:34 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 07:11:34 GMT
WORKDIR /app
# Thu, 15 Apr 2021 07:11:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:11:36 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726cd3e9e578579e631e21133870b656f3938f6a87797a842254b274d8b76e8`  
		Last Modified: Thu, 15 Apr 2021 02:33:02 GMT  
		Size: 1.7 MB (1690998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db188e87a6ea4fd0959949208b039a0d9facc96183df8dc346c6d0d3368b77e`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73dce0ed56811623cd40b786e95b951ce9d6341d9bfefded4f8aa12574283`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:794d5ea4d59593d016379b8d7cf9d074ab74527314a70c4ab2224e030bcce918`  
		Last Modified: Thu, 15 Apr 2021 02:33:04 GMT  
		Size: 10.8 MB (10775163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09c200324804241421da31f3b8cb8c3d7b006322de86d71d500fbdba136a885`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c0a1a831eaec187029e84f1bb7de5acc585a3b96fbfceaf583a3b36731c083`  
		Last Modified: Thu, 15 Apr 2021 02:33:14 GMT  
		Size: 13.6 MB (13585216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ad658b06066f3e4c692de9e3e1d8dbdd37dd05e3c3863e2f7cc8e6947e4df8`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e563207cd5c65809f0cb70dc82a30fb3ff8a2bb948740cd511ad08fa51a0d38`  
		Last Modified: Thu, 15 Apr 2021 02:32:59 GMT  
		Size: 17.5 KB (17533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7322cd551e2d84436e4a4730a66208de66ff94b2946927fc56b146a5b180e41`  
		Last Modified: Thu, 15 Apr 2021 07:12:19 GMT  
		Size: 29.0 MB (28966488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed30edea345eb014ce9274ab7e0c12d0e6b1bf113bb2832146ab41759202280`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 193.6 KB (193560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7850310f2473f2085694f0ae25645d1dbeed617879390675b835e24400817d0c`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 257.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73e685f6d884207cd5821b189eb07436155ade2322ac14aa66466867f752d8b7`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 555.4 KB (555368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95f80e0514909b04305b8652003c9f83308cdab5d4a3ff3ed6fdc75f92c7f6a8`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a531f1e7eee172868524f968eab1cd50d794e2f51df222f44024e4b4569fb004`  
		Last Modified: Thu, 15 Apr 2021 07:12:06 GMT  
		Size: 124.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; arm variant v7

```console
$ docker pull composer@sha256:f47db64626aa0085a31f4f87332a4c85e1f1b0e6dab6bbd9e0e6d59cbebc17b8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.9 MB (55893814 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f41fa048e70a27fbd80e3aebb25f5d2a785e4172c8675a1375062fd4af23fe4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:08:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:08:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:08:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:08:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:08:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:08:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:08:54 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 02:09:03 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 02:09:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 02:09:29 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 02:10:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 02:11:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 02:15:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 02:16:01 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 02:16:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 02:16:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 02:16:08 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:32:23 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:32:41 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:32:43 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:32:44 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:32:45 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:32:45 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 08:32:49 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:32:50 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:32:50 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:32:51 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:32:52 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc6d3f07b2e440bf9a8e52a0a5bba0f27637990ee4976424cef6aae97e169f`  
		Last Modified: Thu, 15 Apr 2021 03:38:53 GMT  
		Size: 1.6 MB (1559061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9000ca9dcd92a2066a3a2c4031e677c3998cd82a3ecbc68468d11255ecbdb62`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d102949f174ecad1044574e45dded8368eb7451bf66b3bdac6e367c7f415d3`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92da8c0a1f3fbf1d4e02eaa533a5058c129447984212a6ff3c72bcc9cad8ab61`  
		Last Modified: Thu, 15 Apr 2021 03:38:54 GMT  
		Size: 10.8 MB (10775172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e011c8a33e544331ac43001738b66a746be18150ffd02e029e1781842dcc4706`  
		Last Modified: Thu, 15 Apr 2021 03:38:48 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61492dda820b711430b6f09aeb0af17f5efb9740a6147244fe1bcf9351a077b`  
		Last Modified: Thu, 15 Apr 2021 03:38:56 GMT  
		Size: 12.7 MB (12733009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e0a3051e72edd5461eda9dc5ad8e0d0b59e55fa0aee85a35da5251839f7f48`  
		Last Modified: Thu, 15 Apr 2021 03:38:47 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e451143ba28ebc0296ff08f6566c5e1d12c219c54351d23e2cb6cd545e2e009a`  
		Last Modified: Thu, 15 Apr 2021 03:38:47 GMT  
		Size: 17.5 KB (17537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3ae47db92bb3e5c1668c4815a02f3a46f82c32e59aa4e9317ea9a4d808399c`  
		Last Modified: Thu, 15 Apr 2021 08:33:40 GMT  
		Size: 27.6 MB (27638087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83cacea819616d21dfc105f33ca411a910a2f359b1ab8bad9f43943880dc2a76`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 186.4 KB (186352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64cc5abdecaef6df8f69965b45b6b83a146dac9487e208895b0bc28bbf32525`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f8f3a04e083b38b70dd19677baec0ff048eb0fd89827dec3a96c132afe5e282`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 555.4 KB (555369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:196939056fb545323ea4219e28a3234097584c6fb32bd88616623aeabd5950bd`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83917393c8cb3c21a26875ace50b2b0b932c89355a39682da0c90b692ff404cb`  
		Last Modified: Thu, 15 Apr 2021 08:33:29 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; arm64 variant v8

```console
$ docker pull composer@sha256:58f7fcb3ddaf67e05162f3b09b0ee5652e65ff73ec9bcb794ed2d924caccee0b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.7 MB (61694374 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4e3dec03a7d85bd434ed450c0bb62fd938a7fb193544337828c665e6480fffa`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:27:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:28:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:28:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:28:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:28:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:28:27 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 00:28:29 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 00:28:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 00:28:33 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 00:28:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 00:28:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:34:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 00:34:40 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 00:34:47 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 00:34:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 00:34:50 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:56:13 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:56:38 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:56:41 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:56:42 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:56:43 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:56:45 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 08:56:50 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:56:52 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:56:55 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:56:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:56:58 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea792edc0a65854bc13c90079b9e33a399c351b73e194d9df4f2cf5a0efeb2`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 1.7 MB (1700262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31bbfcb500579a0c450809a6b082c564c3ce4873732c1b62d8dab52ed0a11ac`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22841fe152c1fe4ec2048ebca3b9c0db9d29773b0d0670167a848d87fcfe83f3`  
		Last Modified: Thu, 15 Apr 2021 01:59:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e61644ef55a78b8c8188acffca32263b12c8684a851a14a3fadc9f9c81d83c6e`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 10.8 MB (10775183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512fc0b44c8ccf1bcd4977baa78bd06876049fbefea93ca3a60d8406b53192c2`  
		Last Modified: Thu, 15 Apr 2021 01:59:49 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e853e5eed6ac911854cde2862e6607daf5c31850a72c856823616ad5ab566d`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 14.4 MB (14377741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7bf5108bfbb40bc73cdd1e0df396ea55f8551e26c78af8e0b455b6bb2f0792e`  
		Last Modified: Thu, 15 Apr 2021 01:59:49 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127cb6e69cb6e4805c0d326498d5b9ebf45069ce7dd5c5cb94558188945baa9b`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad50c34e5614c2df0de39bfe9e05281b6b88a4cdb3c4783d80b00d4e72de6d33`  
		Last Modified: Thu, 15 Apr 2021 08:57:51 GMT  
		Size: 31.4 MB (31355216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c37d5b566318e8b07a0e09bffb639f37240aa5b1afbf68d7bb3aa7d9ee722e8c`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 195.9 KB (195947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a9624473eddbb2b7517d6b3ec640bc13c5deae479b44cfdc7781a6dd517ff06`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 260.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0ea7aee59bc8c381ebf13e07f17a0a905147840a2a9813ba638e539f1f73e7`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 555.4 KB (555369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b9b6647561cc710659eec729f81d22f355bff35620854e6fe9e38b390b1a9a`  
		Last Modified: Thu, 15 Apr 2021 08:57:42 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bfd31c2ac4ef646c259c246c3ede82c00cd5aa28d34cad3b5ef2b2bba4bf25`  
		Last Modified: Thu, 15 Apr 2021 08:57:41 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; 386

```console
$ docker pull composer@sha256:70bc0657ac9d955ed89d5ea044768e0bf45b3a7226170ff6d48325a9d9787d9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.5 MB (63459840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8dd0b260971d5fcb96c0533acb7fa361b9d87ba87d71a3bfb54d32177317ef2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 03:38:49 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_VERSION=8.0.3
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 15 Apr 2021 03:38:49 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 15 Apr 2021 03:39:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 15 Apr 2021 03:39:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:45:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 15 Apr 2021 03:45:10 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 15 Apr 2021 03:45:12 GMT
RUN docker-php-ext-enable sodium
# Thu, 15 Apr 2021 03:45:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 15 Apr 2021 03:45:13 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:52:55 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:53:10 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:53:11 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:53:11 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:53:12 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:53:12 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 08:53:15 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:53:15 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:53:15 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:53:16 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:53:16 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeccee8de2519293816e97d37497a11495840e4c2edb7ad1254ce80fc59737a`  
		Last Modified: Thu, 15 Apr 2021 05:57:42 GMT  
		Size: 10.8 MB (10775154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:962c132cc514121c8ad9862e99f06f647cbc70e07305e12cde1c0e8986f4de2d`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bf4252825c42e4fc0d1dd2328fc4fbae3271919571b76a5dd55b1a5a63f3c8b`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 15.0 MB (14974551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7085eb2c648a88168bff8bcfeb7ef1f366a6c134a86b2e22fb7b2dc37479ea38`  
		Last Modified: Thu, 15 Apr 2021 05:57:40 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c7ddb662add691a4ef54081ad454d11303541f3b4398453b7c72070b39bbeee`  
		Last Modified: Thu, 15 Apr 2021 05:57:40 GMT  
		Size: 17.5 KB (17533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d4448c8736ab950ed57d33c37776a00fe02282664f5316431b408f76ebccef`  
		Last Modified: Thu, 15 Apr 2021 08:54:02 GMT  
		Size: 32.3 MB (32300139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aadf752d16c9b4f5ebcbf8f8ee774377e7e479e31c9900f14d6e8252b89e9686`  
		Last Modified: Thu, 15 Apr 2021 08:53:53 GMT  
		Size: 213.8 KB (213841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30932fd99a342f62c81464b27cb9398d3638e9caeaf2d233d5cf3bbde4114028`  
		Last Modified: Thu, 15 Apr 2021 08:53:53 GMT  
		Size: 254.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359d5d64671b2b5de602c4f62ad00c7bad415822942d43fdbaff23995c637c83`  
		Last Modified: Thu, 15 Apr 2021 08:53:52 GMT  
		Size: 555.4 KB (555376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec1662864d2b5ac55354e0d61fcefc60ae2f41afe4349fc86c0df7e756bb512f`  
		Last Modified: Thu, 15 Apr 2021 08:53:51 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff352cc745257d9f7c02042f4f03cc762fc0ee9c0f45d3d10657b26ff0395ad`  
		Last Modified: Thu, 15 Apr 2021 08:53:50 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; ppc64le

```console
$ docker pull composer@sha256:ca8bcb0fad3c8c75791a7321ccbadd72dc179e18cfbf95b820714ce1d7affde1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.8 MB (63789841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f9ee919c2f8f85644a637e78d057398a9759a722d8e5025c7b9fbc39b93004a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:16:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:16:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 20:16:59 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 20:17:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 20:17:24 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 20:17:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 20:17:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:23:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Apr 2021 20:23:31 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 14 Apr 2021 20:23:50 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Apr 2021 20:23:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Apr 2021 20:24:03 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 08:44:10 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 08:44:50 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 08:45:13 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 08:45:19 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 08:45:26 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 08:45:35 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 08:45:55 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 08:46:00 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 08:46:08 GMT
WORKDIR /app
# Thu, 15 Apr 2021 08:46:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 08:46:16 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6431deb07f4adae4be0bd4b93d784bb08ec63d03daa512d835bbc0230e05cf3`  
		Last Modified: Wed, 14 Apr 2021 22:00:57 GMT  
		Size: 10.8 MB (10775172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3ef816305c1c138c8c7ce8fbacf23f59654a7422858f578711604d0819539d`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171f3408ea103656d215c6b47106245684e915481a4ae3bc5b613d2f98f6b219`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 15.7 MB (15673187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5517add7dc81698b49a4430b992ab0bb4a012fbd04792d17b4754fe392f24014`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4888f0381bb3c52192f3c448b3bf6fd7906a41b23b8ac854a82340a8aa6171`  
		Last Modified: Wed, 14 Apr 2021 22:00:56 GMT  
		Size: 17.6 KB (17556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f596040cc5835db2f0e35314704e491260222aa43948cc3c84967912a555a993`  
		Last Modified: Thu, 15 Apr 2021 08:47:37 GMT  
		Size: 32.0 MB (31997694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cc29da636c9f65c118437157394b275676967a063d7b8cbf33ab5faca6c591c`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 204.0 KB (204005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef3767002a509df55f5149f3fb25a788238d75bd23a9cb0d17af0ae11ec7a0c`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 258.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871523e4535d7b29028c6ba393e95315523bbd18d9ad4f6a313a36a3afb70d82`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 555.4 KB (555372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9b40f1162d15bc30f530fac32dbe79c562e0264f9378dd49e1e74bcda62fd0`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 406.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656cf3e249e69c2dd27fc4f38787633f612acbb71cb7645068b1946df2fb17de`  
		Last Modified: Thu, 15 Apr 2021 08:47:21 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `composer:latest` - linux; s390x

```console
$ docker pull composer@sha256:c8c4b8992d176fba657c9fed5cdbee13cf76d0fa9fa791ea1abaf59866bce2f6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.3 MB (61277823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb15eb7b90d1e5576f452170f25168185d47f8d957f0fc34c6712e8e1d41df12`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["composer"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:00:59 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 14 Apr 2021 19:01:00 GMT
ENV PHP_VERSION=8.0.3
# Wed, 14 Apr 2021 19:01:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 14 Apr 2021 19:01:01 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 14 Apr 2021 19:01:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 14 Apr 2021 19:01:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 14 Apr 2021 19:06:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 14 Apr 2021 19:06:26 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 14 Apr 2021 19:06:27 GMT
RUN docker-php-ext-enable sodium
# Wed, 14 Apr 2021 19:06:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 14 Apr 2021 19:06:28 GMT
CMD ["php" "-a"]
# Thu, 15 Apr 2021 07:30:47 GMT
RUN set -eux;   apk add --no-cache --virtual .composer-rundeps     bash     coreutils     git     make     mercurial     openssh-client     patch     subversion     tini     unzip     zip
# Thu, 15 Apr 2021 07:30:58 GMT
RUN set -eux;   apk add --no-cache --virtual .build-deps     libzip-dev     zlib-dev   ;   docker-php-ext-install -j "$(nproc)"     zip   ;   runDeps="$(     scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions       | tr ',' '\n'       | sort -u       | awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }'     )";   apk add --no-cache --virtual .composer-phpext-rundeps $runDeps;   apk del .build-deps
# Thu, 15 Apr 2021 07:30:58 GMT
RUN printf "# composer php cli ini settings\ndate.timezone=UTC\nmemory_limit=-1\n" > $PHP_INI_DIR/php-cli.ini
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_ALLOW_SUPERUSER=1
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_HOME=/tmp
# Thu, 15 Apr 2021 07:30:59 GMT
ENV COMPOSER_VERSION=2.0.12
# Thu, 15 Apr 2021 07:31:01 GMT
RUN set -eux;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.dev.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/snapshots.pub   ;   php -r "     \$signature = '4ac45767e5ec22652f0c1167cbbb8a2b0c708369153e328cad90147dafe50952';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.dev.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, dev public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/keys.tags.pub     --url https://raw.githubusercontent.com/composer/composer.github.io/e7f28b7200249f8e5bc912b42837d4598c74153a/releases.pub   ;   php -r "     \$signature = '57815ba27e54dc317ecc7cc5573090d087719ba68f3bb7234e5d42d084a14642';     \$hash = hash('sha256', preg_replace('{\s}', '', file_get_contents('/tmp/keys.tags.pub')));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, tags public key is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   curl     --silent     --fail     --location     --retry 3     --output /tmp/installer.php     --url https://raw.githubusercontent.com/composer/getcomposer.org/cb19f2aa3aeaa2006c0cd69a7ef011eb31463067/web/installer   ;   php -r "     \$signature = '48e3236262b34d30969dca3c37281b3b4bbe3221bda826ac6a9a62d6444cdb0dcd0615698a5cbe587c3f0fe57a54d8f5';     \$hash = hash('sha384', file_get_contents('/tmp/installer.php'));     if (!hash_equals(\$signature, \$hash)) {       echo 'Integrity check failed, installer is either corrupt or worse.' . PHP_EOL;       exit(1);     }"   ;   php /tmp/installer.php --no-ansi --install-dir=/usr/bin --filename=composer --version=${COMPOSER_VERSION};   composer --ansi --version --no-interaction;   composer diagnose;   rm -f /tmp/installer.php;   find /tmp -type d -exec chmod -v 1777 {} +
# Thu, 15 Apr 2021 07:31:02 GMT
COPY file:fec7a37c0f859c3b5da390e40fa6f3ea8445ed26f54be61f4bce40efcaad57ee in /docker-entrypoint.sh 
# Thu, 15 Apr 2021 07:31:02 GMT
WORKDIR /app
# Thu, 15 Apr 2021 07:31:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 15 Apr 2021 07:31:03 GMT
CMD ["composer"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfbe2d3d9b1efb815eb614a3488743bc95ac05e1ae4b0b1e2b488a057a9697f2`  
		Last Modified: Wed, 14 Apr 2021 20:01:03 GMT  
		Size: 10.8 MB (10775158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e42d806dde82abd1fa888745f98a91c4a389d70968f69ee9fb1d467acf94c233`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3407c21d5517a5fe9bee65ffefce1b436496f08d54e5ec826713de143cc769a1`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 14.0 MB (13972054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673772f281ad30fa5e8f68f1b2cc7246eb505f77b1304eeffee4ed02e2ac0025`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b887ade51969a265f267fab2842da16aee5c3746eebee780035a2e8e30b486de`  
		Last Modified: Wed, 14 Apr 2021 20:01:02 GMT  
		Size: 17.6 KB (17552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:827a7ecf83cc085e8c067e3fb91cc8be53232ed95c0f1344337b305382d525d5`  
		Last Modified: Thu, 15 Apr 2021 07:31:34 GMT  
		Size: 31.4 MB (31391511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21ddcc417205411563d9531ffab3b6e85ece64c95e6e494b9a7eac77bf621e25`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 197.8 KB (197750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f23536fe9ce1e18934446f30900cd733051f3573df86ecd7dd71a23e7047420`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 259.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92975974c01eb23ef0604971c31c1552e1f9ba01d8712691b66b89e178d2cec4`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 555.4 KB (555366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd0d197e8c109ca4c634e2e48a35bd63c4dec1e95e8fc1c94dab6c3ad043992`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:901dc3c5be755d5e73ffd749eb62730c29440327d1bfe3fa7a0546c20bd09dfe`  
		Last Modified: Thu, 15 Apr 2021 07:31:28 GMT  
		Size: 126.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
