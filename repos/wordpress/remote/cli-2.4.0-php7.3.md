## `wordpress:cli-2.4.0-php7.3`

```console
$ docker pull wordpress@sha256:50cbfbbd1ff195f3ab02e8221ab3342315a08175f82567b665691b57bf1ab9e7
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

### `wordpress:cli-2.4.0-php7.3` - linux; amd64

```console
$ docker pull wordpress@sha256:ab225cdea5f9d62f13eaade43445592146c4534e55d98880fa007a29069e43ca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46314866 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f45e048c2e397c9d69fb4549d57573fd9d2928c158af4e35a6c79cc1e6dcebf4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Thu, 25 Mar 2021 22:19:32 GMT
ADD file:6b081cabb4b256ee07587d249c4989b5b679375529542b81550a65b6f19f274e in / 
# Thu, 25 Mar 2021 22:19:32 GMT
CMD ["/bin/sh"]
# Thu, 25 Mar 2021 22:51:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 25 Mar 2021 22:52:01 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 25 Mar 2021 22:52:02 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 25 Mar 2021 22:52:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 25 Mar 2021 22:52:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 25 Mar 2021 22:52:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 25 Mar 2021 22:52:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 25 Mar 2021 22:52:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 26 Mar 2021 00:02:41 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 26 Mar 2021 00:02:41 GMT
ENV PHP_VERSION=7.3.27
# Fri, 26 Mar 2021 00:02:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.27.tar.xz.asc
# Fri, 26 Mar 2021 00:02:42 GMT
ENV PHP_SHA256=65f616e2d5b6faacedf62830fa047951b0136d5da34ae59e6744cbaf5dca148d
# Fri, 26 Mar 2021 00:02:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 26 Mar 2021 00:02:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Mar 2021 00:10:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 26 Mar 2021 00:10:46 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 26 Mar 2021 00:10:48 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Mar 2021 00:10:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Mar 2021 00:10:48 GMT
CMD ["php" "-a"]
# Fri, 26 Mar 2021 18:13:35 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 26 Mar 2021 18:13:36 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 26 Mar 2021 18:13:37 GMT
WORKDIR /var/www/html
# Sat, 27 Mar 2021 14:01:53 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 27 Mar 2021 14:01:54 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 27 Mar 2021 14:01:54 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Sat, 27 Mar 2021 14:01:54 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Sat, 27 Mar 2021 14:01:54 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Sat, 27 Mar 2021 14:01:57 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Sat, 27 Mar 2021 14:01:57 GMT
VOLUME [/var/www/html]
# Sat, 27 Mar 2021 14:01:57 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Sat, 27 Mar 2021 14:01:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 14:01:57 GMT
USER www-data
# Sat, 27 Mar 2021 14:01:58 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:9aae54b2144e5b2b00c610f8805128f4f86822e1e52d3714c463744a431f0f4a`  
		Last Modified: Thu, 25 Mar 2021 22:20:18 GMT  
		Size: 2.8 MB (2811681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0552190813ec45fbb7d7734d1ea62c2e2ecb18e81204b0942ae40e8de25eebdc`  
		Last Modified: Fri, 26 Mar 2021 01:05:20 GMT  
		Size: 1.7 MB (1694828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6abf49ad7ff9971373cb1a72865aec4f8a294be34c53b85066fd626d97ae3d0`  
		Last Modified: Fri, 26 Mar 2021 01:05:19 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a7b791901cf28e74ddce41fce7b81e07c2a11ca345ad6eeea21aa321ce9fd84`  
		Last Modified: Fri, 26 Mar 2021 01:05:19 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7a91f50f2ee1ec1203eff482bef218e8f6be94b57bcde551cac36444d41aaa2`  
		Last Modified: Fri, 26 Mar 2021 01:11:23 GMT  
		Size: 12.2 MB (12157792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9575c9ff9c211971b8f1b125b24b538e3a6724f69ebb6b0154dd6b9d26c5cffc`  
		Last Modified: Fri, 26 Mar 2021 01:11:20 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5bdfb8baf0dd534a2b7b6e75e5831ad56a7a7d4c75cf2c906a1a33f14d448ae`  
		Last Modified: Fri, 26 Mar 2021 01:11:24 GMT  
		Size: 14.5 MB (14456790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e8ac8666bd52fa6e8f947d2d7cfe306e8118dc3fe52006c6cf9ad32b6a9519b`  
		Last Modified: Fri, 26 Mar 2021 01:11:20 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69034f4dd97794865aa7be12bc4059d6a22284bdf418ac0fe60f3895c3ada49c`  
		Last Modified: Fri, 26 Mar 2021 01:11:21 GMT  
		Size: 17.3 KB (17332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b3cc7c323718fb704d35df8324a35fd566a8f6d11bb8b3483c2ddde46b3e1d`  
		Last Modified: Fri, 26 Mar 2021 18:20:57 GMT  
		Size: 9.3 MB (9335106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d8d6bea1b9b875cf9e1ce632ae5979fffc31506039edd72b9344888d85086db`  
		Last Modified: Fri, 26 Mar 2021 18:20:51 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d80bae426ca9d654b0ccd56680d6f09ca6b3a8ce94d0034ce6e4d82d9d4f9619`  
		Last Modified: Sat, 27 Mar 2021 14:09:18 GMT  
		Size: 4.6 MB (4630303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bacf373c25a5b0d977ef577df17327bbc8a82de1ddc7d197b5aee09456106f9`  
		Last Modified: Sat, 27 Mar 2021 14:09:17 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9187783722cb007b8ee728632812e9626e63c0f5bb8fa4322b2e689b50a2a2f9`  
		Last Modified: Sat, 27 Mar 2021 14:09:17 GMT  
		Size: 1.2 MB (1205804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af9470123fd27b7ddfaddcb48f2e58ae7fd56a51f1aea40684526f2345eaed8`  
		Last Modified: Sat, 27 Mar 2021 14:09:17 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4.0-php7.3` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:be043321da33f7bc7790a6fbb55844cf456ef7176560ac0d5f9da46cfffe4d9d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44473423 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a63a253a342bcdf17f19494f8e8a554d1c8a4746006b4d6f17e0ee3d99fd1633`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Wed, 31 Mar 2021 22:37:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 31 Mar 2021 22:37:10 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 31 Mar 2021 22:37:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 31 Mar 2021 22:37:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 31 Mar 2021 22:37:17 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 31 Mar 2021 22:37:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 22:37:20 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 31 Mar 2021 22:37:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 31 Mar 2021 23:30:08 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Wed, 31 Mar 2021 23:30:09 GMT
ENV PHP_VERSION=7.3.27
# Wed, 31 Mar 2021 23:30:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.27.tar.xz.asc
# Wed, 31 Mar 2021 23:30:12 GMT
ENV PHP_SHA256=65f616e2d5b6faacedf62830fa047951b0136d5da34ae59e6744cbaf5dca148d
# Wed, 31 Mar 2021 23:30:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 31 Mar 2021 23:30:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 23:33:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 23:33:39 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 31 Mar 2021 23:33:46 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 23:33:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 23:33:49 GMT
CMD ["php" "-a"]
# Thu, 01 Apr 2021 06:05:07 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 01 Apr 2021 06:05:10 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 01 Apr 2021 06:05:10 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 06:06:57 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 06:07:01 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 01 Apr 2021 06:07:03 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 01 Apr 2021 06:07:04 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 01 Apr 2021 06:07:05 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 01 Apr 2021 06:07:11 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 01 Apr 2021 06:07:12 GMT
VOLUME [/var/www/html]
# Thu, 01 Apr 2021 06:07:13 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 01 Apr 2021 06:07:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 06:07:15 GMT
USER www-data
# Thu, 01 Apr 2021 06:07:16 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db6e43e67e5babad459f6f197992a26d77e745ef3b9a9ffac78e944ac250c167`  
		Last Modified: Thu, 01 Apr 2021 00:01:46 GMT  
		Size: 1.7 MB (1684700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a574a3d26078380134181643d6542608f6e510e2cce4119361f1df09b617dcb2`  
		Last Modified: Thu, 01 Apr 2021 00:01:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90716c38f3f1c30424f0b486ba18c8c8c630b62f6858c89513c20968dfb91bd`  
		Last Modified: Thu, 01 Apr 2021 00:01:43 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:029c66aca063471eef104c032d9c9271735438580768c5859498c349d6ac1ff7`  
		Last Modified: Thu, 01 Apr 2021 00:06:50 GMT  
		Size: 12.2 MB (12157776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f49b1e175a0cf1db27328094909ecb6199d09804a8740360f7fd5ff3935e37a`  
		Last Modified: Thu, 01 Apr 2021 00:06:46 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:088424208cdde140e0ce392630f6f9e47525aa8d830e7c75086e76f507f91fd1`  
		Last Modified: Thu, 01 Apr 2021 00:06:54 GMT  
		Size: 13.4 MB (13388877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010a580db7513747e8732e6e3f7803af1b908f44249ee7b08a0fdf8d9791f87b`  
		Last Modified: Thu, 01 Apr 2021 00:06:45 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8281d327c7e89a747b25774ebb3565e03f63b183d53b0285c8b31266626193a7`  
		Last Modified: Thu, 01 Apr 2021 00:06:45 GMT  
		Size: 17.3 KB (17316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76a1432e9528f8d6c965298492038a373b2d942a5e5f8e7eae6ad662e7c6587e`  
		Last Modified: Thu, 01 Apr 2021 06:11:20 GMT  
		Size: 8.9 MB (8943847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302f181ed068a147ffb521de096f653ef4333ff2642dfe70ac6c41a17310e050`  
		Last Modified: Thu, 01 Apr 2021 06:11:15 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db271c58252be0110878368fb1149dc10560f4e4b87ec8ee1e3874cb11e2f892`  
		Last Modified: Thu, 01 Apr 2021 06:11:15 GMT  
		Size: 4.4 MB (4447745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca13e6fa2d915d661624632c1a78c3bbf949874fb1c012c6a6b5aa0a7a171d72`  
		Last Modified: Thu, 01 Apr 2021 06:11:13 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71185f53cc43332f9f3e0759706f5aab737197e92ffe5b086dbad806cf4584b`  
		Last Modified: Thu, 01 Apr 2021 06:11:17 GMT  
		Size: 1.2 MB (1205808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd512fe6eaf1a48ffa3d254f55a67066bdf05d7b17b64eec62b5a504d30fb81`  
		Last Modified: Thu, 01 Apr 2021 06:11:16 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4.0-php7.3` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:3f5348497e15b49acfe7bf36099bc5c764d03abcb874a629444a06b6bf0f6d83
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.7 MB (42704466 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2547ff2b7adff365edd64b41862b73cf4fb777bb1adde0072fe484e3dc74bfa`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Thu, 25 Mar 2021 22:05:53 GMT
ADD file:44ef6cff6e7d37a67c5846eb792fec65025702c00c56ff96801ac79bf81b0cc3 in / 
# Thu, 25 Mar 2021 22:05:55 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 06:56:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 26 Mar 2021 06:56:57 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 26 Mar 2021 06:57:00 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 26 Mar 2021 06:57:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 26 Mar 2021 06:57:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 26 Mar 2021 06:57:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 06:57:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 06:57:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 26 Mar 2021 07:32:44 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 26 Mar 2021 07:32:45 GMT
ENV PHP_VERSION=7.3.27
# Fri, 26 Mar 2021 07:32:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.27.tar.xz.asc
# Fri, 26 Mar 2021 07:32:47 GMT
ENV PHP_SHA256=65f616e2d5b6faacedf62830fa047951b0136d5da34ae59e6744cbaf5dca148d
# Fri, 26 Mar 2021 07:32:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 26 Mar 2021 07:32:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:35:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 26 Mar 2021 07:36:01 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:36:04 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Mar 2021 07:36:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Mar 2021 07:36:06 GMT
CMD ["php" "-a"]
# Fri, 26 Mar 2021 11:54:03 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 26 Mar 2021 11:54:07 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 26 Mar 2021 11:54:09 GMT
WORKDIR /var/www/html
# Sat, 27 Mar 2021 15:19:12 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 27 Mar 2021 15:19:15 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 27 Mar 2021 15:19:16 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Sat, 27 Mar 2021 15:19:17 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Sat, 27 Mar 2021 15:19:18 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Sat, 27 Mar 2021 15:19:23 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Sat, 27 Mar 2021 15:19:24 GMT
VOLUME [/var/www/html]
# Sat, 27 Mar 2021 15:19:25 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Sat, 27 Mar 2021 15:19:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 15:19:28 GMT
USER www-data
# Sat, 27 Mar 2021 15:19:28 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:6c1162af251f0d5ab4945f8506f3265b86d0a03cda37f703c2446a71a233bc20`  
		Last Modified: Thu, 25 Mar 2021 22:07:21 GMT  
		Size: 2.4 MB (2423999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ce0e5f49a9711e3c44eca8e360bc4f1652954226f8f66f4e9f7802de3ddc4c`  
		Last Modified: Fri, 26 Mar 2021 07:56:02 GMT  
		Size: 1.6 MB (1555137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717384b7374c999b528c18425465cf28f272790b8eaba5b8c8ec65859b96e26e`  
		Last Modified: Fri, 26 Mar 2021 07:56:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7638befde742a0a93dc501fb76875f103a283c69c5270049b296bca16eeedc58`  
		Last Modified: Fri, 26 Mar 2021 07:56:02 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49769df201a6324d1622c951e150b823c91d3c7df7bcedc8f607d76783f7f97`  
		Last Modified: Fri, 26 Mar 2021 07:59:58 GMT  
		Size: 12.2 MB (12157778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2998df5827c4b3e24e05a16b89493d71052274f41247fc16229e54ddda7af141`  
		Last Modified: Fri, 26 Mar 2021 07:59:59 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f485dd6f38a9a4231b029e15911058ea94fd81395d06035fce0a22380d4ff77`  
		Last Modified: Fri, 26 Mar 2021 08:00:01 GMT  
		Size: 12.5 MB (12534695 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f0f0f26dc11446915efe63ce06004f7dc565c0321e18e6c1c802352fa47be78`  
		Last Modified: Fri, 26 Mar 2021 07:59:59 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d721362e554a13fe56d04fbd54abe699a12168c1b1f4a263891b64c4929502`  
		Last Modified: Fri, 26 Mar 2021 07:59:57 GMT  
		Size: 17.3 KB (17324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa2126727ec618204432384bdc865c5e24d17d5d8fb6c3804085f776b5856d1c`  
		Last Modified: Fri, 26 Mar 2021 12:01:15 GMT  
		Size: 8.7 MB (8660707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d940fe6d0000772f826afb8ea2af652918e6b54c679e712d11d54e0db6149f6`  
		Last Modified: Fri, 26 Mar 2021 12:01:11 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b1aa59bcb2372408dd2edd5b990b4cb41f0de7e15c6b08776c88c7ff92935ae`  
		Last Modified: Sat, 27 Mar 2021 15:24:31 GMT  
		Size: 4.1 MB (4143786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1af1e80627a22e78ae4843d5344a00425dcb89fef173671e39183c8225f3ece`  
		Last Modified: Sat, 27 Mar 2021 15:24:30 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6378c0101219c909972d03eccf8393a8725c32de7122d429e3ce88d200c1cf`  
		Last Modified: Sat, 27 Mar 2021 15:24:30 GMT  
		Size: 1.2 MB (1205811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2b08687029aa35010b99f216ee8905febf165b35c520cc9d6b94c40c78e2f7e`  
		Last Modified: Sat, 27 Mar 2021 15:24:30 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4.0-php7.3` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:caf962cc111212ff728c12d3f2884c3ae6844327790236e8d0e407d63466c6a2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45797418 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03adcf864192d96bc94fabeefe79b4c9fe6e58bfa293f502faa5d21de101697e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Thu, 25 Mar 2021 22:40:10 GMT
ADD file:8d7431f7e3e42b162a1626e7abf4ef7605146671dccc753d490de6b7fe429261 in / 
# Thu, 25 Mar 2021 22:40:23 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 03:47:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 26 Mar 2021 03:48:01 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 26 Mar 2021 03:48:03 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 26 Mar 2021 03:48:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 26 Mar 2021 03:48:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 26 Mar 2021 03:48:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 03:48:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 03:48:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 26 Mar 2021 04:33:32 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 26 Mar 2021 04:33:33 GMT
ENV PHP_VERSION=7.3.27
# Fri, 26 Mar 2021 04:33:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.27.tar.xz.asc
# Fri, 26 Mar 2021 04:33:35 GMT
ENV PHP_SHA256=65f616e2d5b6faacedf62830fa047951b0136d5da34ae59e6744cbaf5dca148d
# Fri, 26 Mar 2021 04:33:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 26 Mar 2021 04:33:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:37:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 26 Mar 2021 04:37:23 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:37:26 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Mar 2021 04:37:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Mar 2021 04:37:28 GMT
CMD ["php" "-a"]
# Fri, 26 Mar 2021 18:06:16 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 26 Mar 2021 18:06:19 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 26 Mar 2021 18:06:19 GMT
WORKDIR /var/www/html
# Sat, 27 Mar 2021 11:58:20 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 27 Mar 2021 11:58:24 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 27 Mar 2021 11:58:26 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Sat, 27 Mar 2021 11:58:27 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Sat, 27 Mar 2021 11:58:28 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Sat, 27 Mar 2021 11:58:41 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Sat, 27 Mar 2021 11:58:45 GMT
VOLUME [/var/www/html]
# Sat, 27 Mar 2021 11:58:47 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Sat, 27 Mar 2021 11:58:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 11:58:50 GMT
USER www-data
# Sat, 27 Mar 2021 11:58:52 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:5ceb5101e3b0d54efb5f18318982508a04b181b4d5ae52b096dd35dea3a006cc`  
		Last Modified: Thu, 25 Mar 2021 22:44:41 GMT  
		Size: 2.7 MB (2711898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d060b906a189f871d2750341d5225b1dc4b31011947c63e0fa6e23177a3b1879`  
		Last Modified: Fri, 26 Mar 2021 05:10:49 GMT  
		Size: 1.7 MB (1694521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2837359c696419bd4d3c7fe859fbba2bac672084b48e6338599c23210a14666d`  
		Last Modified: Fri, 26 Mar 2021 05:10:48 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:890e1b8d57d77fde9bbea8d93e5851a1e2e7156bce307a803addd6871a63697b`  
		Last Modified: Fri, 26 Mar 2021 05:10:48 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791f568b8fd5f72d098937e8bf1ca1f702ef3ee57e1b8f146e5112231e9f55e5`  
		Last Modified: Fri, 26 Mar 2021 05:15:28 GMT  
		Size: 12.2 MB (12157806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577a8bb27ac58228aeb532c0fcfea753e1868bd8a352d5bb66a57be9932c9185`  
		Last Modified: Fri, 26 Mar 2021 05:15:26 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b0f2256ad97f58d5097c11d4e46bf45d12dda48e644409bb2c10d75713d27a5`  
		Last Modified: Fri, 26 Mar 2021 05:15:32 GMT  
		Size: 14.1 MB (14145475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f82ab5b718f0f1726fb57348a58253569c71778004a04987d39f52b649db3e80`  
		Last Modified: Fri, 26 Mar 2021 05:15:26 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4aecc580306041cb4f39437357ba44cf7dfcc4aedccbd0ab6ce3d5d9e4bd5e86`  
		Last Modified: Fri, 26 Mar 2021 05:15:26 GMT  
		Size: 17.3 KB (17341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c54b2f6b5a3723b48ea5e38653a61876250d9b83991376b9c5b8fffbc433cd0`  
		Last Modified: Fri, 26 Mar 2021 18:13:02 GMT  
		Size: 9.4 MB (9403532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5be6b501abb40336c8c7b7dc7fcab1afbb454d59d2ca68743be29e10d01757`  
		Last Modified: Fri, 26 Mar 2021 18:12:58 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:654f4295239dcd65dbda7a50ce80ddf17ea3cf2398906b842b0e2c7020781cc5`  
		Last Modified: Sat, 27 Mar 2021 12:03:54 GMT  
		Size: 4.5 MB (4455792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce1617b9f2b64766d0736f4c72bcbfdd0ee720734321934996efee1e860ef0e`  
		Last Modified: Sat, 27 Mar 2021 12:03:53 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb8b685cc0e55ced5f21a03efc74b1cdcf0972d25eb564abe08ff26ecec4172`  
		Last Modified: Sat, 27 Mar 2021 12:03:53 GMT  
		Size: 1.2 MB (1205817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ef7ef50a31d4897778990d799673d875d890f76030361fb0591912171c689f7`  
		Last Modified: Sat, 27 Mar 2021 12:03:53 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4.0-php7.3` - linux; 386

```console
$ docker pull wordpress@sha256:d01ad0c31e74e155369d90bbced3ffab922a5becd376898655b31a29c689480e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.1 MB (47067452 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:393554218d12f115870a7a851f4794dbfeb0ad9ecced496b99540404a66b6e3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 02:49:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 02:49:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 02:49:03 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 02:49:03 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 02:49:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 02:49:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 02:49:05 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 02:49:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 03:54:41 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 01 Apr 2021 03:54:41 GMT
ENV PHP_VERSION=7.3.27
# Thu, 01 Apr 2021 03:54:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.27.tar.xz.asc
# Thu, 01 Apr 2021 03:54:41 GMT
ENV PHP_SHA256=65f616e2d5b6faacedf62830fa047951b0136d5da34ae59e6744cbaf5dca148d
# Thu, 01 Apr 2021 03:55:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 03:55:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 04:01:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 04:01:36 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 01 Apr 2021 04:01:37 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 04:01:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 04:01:37 GMT
CMD ["php" "-a"]
# Thu, 01 Apr 2021 10:37:55 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 01 Apr 2021 10:37:55 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 01 Apr 2021 10:37:56 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 10:38:47 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 10:38:48 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 01 Apr 2021 10:38:48 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 01 Apr 2021 10:38:48 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 01 Apr 2021 10:38:48 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 01 Apr 2021 10:38:51 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 01 Apr 2021 10:38:51 GMT
VOLUME [/var/www/html]
# Thu, 01 Apr 2021 10:38:51 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 01 Apr 2021 10:38:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 10:38:52 GMT
USER www-data
# Thu, 01 Apr 2021 10:38:52 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4303b3cd022ad91251e7495aeed4896d9bb7f6fa0dcb18e18234a628ef5cfeec`  
		Last Modified: Thu, 01 Apr 2021 04:41:12 GMT  
		Size: 1.8 MB (1793710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:526e185ad2b26faab26d003f328b965c1bbcb1058eae28cb5cb132c7ea7f0c09`  
		Last Modified: Thu, 01 Apr 2021 04:41:11 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e9b82cb292af1dd42fbdda274111233ed643f3515fe3b67e1c212c10f26daa`  
		Last Modified: Thu, 01 Apr 2021 04:41:11 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59dd8fa335e56046872fb90846a7b6d151a8afc410e54dc2ac0ff38b1aef8203`  
		Last Modified: Thu, 01 Apr 2021 04:48:09 GMT  
		Size: 12.2 MB (12157772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b966e2bacc5b88ef7b4a2fed4557175d692c35c74df9cd5327cc1a39a39549f4`  
		Last Modified: Thu, 01 Apr 2021 04:48:06 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9939bcecb15e1c574db774e9dcb96db3ac272739a66b099560cce24e8af1dca`  
		Last Modified: Thu, 01 Apr 2021 04:48:10 GMT  
		Size: 14.8 MB (14780212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f51065e521a0477241cba869da66fdd671f1a4f0c07909ca09514946a107290`  
		Last Modified: Thu, 01 Apr 2021 04:48:06 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c00b515deb1732adb9a3ca5d3f197d26f0934e3b2e51d89d23c3425111156a2f`  
		Last Modified: Thu, 01 Apr 2021 04:48:07 GMT  
		Size: 17.3 KB (17323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64d7b817f6aaedd84b3084793a1e75ba08210e9456a959a9db4c3f2d71c47d67`  
		Last Modified: Thu, 01 Apr 2021 10:47:57 GMT  
		Size: 9.5 MB (9498460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f1fe5a99caedf46c7ca63c0ed1913394c9de9bd8372a8389832c6e31c8addd`  
		Last Modified: Thu, 01 Apr 2021 10:47:52 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ec7e613148dc7abc1bd17d1b593ce298a260b42a8ec8582742a84444f3b7ff`  
		Last Modified: Thu, 01 Apr 2021 10:47:56 GMT  
		Size: 4.8 MB (4790162 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955d6fb3d5036519ac7e7b4f06adbfb5e54d679aa6d4c8a9d8332628bed6dfab`  
		Last Modified: Thu, 01 Apr 2021 10:47:52 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4722e6fe5d91ca3b21d5a3e4cf6ec373bc115456e694ed0363fd720637376a6`  
		Last Modified: Thu, 01 Apr 2021 10:47:52 GMT  
		Size: 1.2 MB (1205787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ccf48cf01cb30ba2635236d7f2fc18d28ef8128f4c7835fcaef8946f8996b75`  
		Last Modified: Thu, 01 Apr 2021 10:47:52 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4.0-php7.3` - linux; ppc64le

```console
$ docker pull wordpress@sha256:1d37dfaa900f7382af34d0e99a726ffd1b99634c3e97772a28c3ead0321d24fd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47706858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d340dc532c782c8c1cd8fe1275504bc18624e22b09992613fd85a20896bc6687`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Thu, 25 Mar 2021 22:22:28 GMT
ADD file:f91f8e0aa646cb847f6e210056280f9332382ad2f8d6a8839fd9aa69b81c4a2a in / 
# Thu, 25 Mar 2021 22:22:30 GMT
CMD ["/bin/sh"]
# Fri, 26 Mar 2021 12:16:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 26 Mar 2021 12:17:00 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 26 Mar 2021 12:17:20 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 26 Mar 2021 12:17:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 26 Mar 2021 12:17:44 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 26 Mar 2021 12:17:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 12:17:59 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 26 Mar 2021 12:18:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 26 Mar 2021 13:23:14 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 26 Mar 2021 13:23:18 GMT
ENV PHP_VERSION=7.3.27
# Fri, 26 Mar 2021 13:23:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.27.tar.xz.asc
# Fri, 26 Mar 2021 13:23:29 GMT
ENV PHP_SHA256=65f616e2d5b6faacedf62830fa047951b0136d5da34ae59e6744cbaf5dca148d
# Fri, 26 Mar 2021 13:23:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 26 Mar 2021 13:23:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Mar 2021 13:28:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 26 Mar 2021 13:28:48 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 26 Mar 2021 13:29:00 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Mar 2021 13:29:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Mar 2021 13:29:15 GMT
CMD ["php" "-a"]
# Sat, 27 Mar 2021 04:33:29 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Sat, 27 Mar 2021 04:33:42 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Sat, 27 Mar 2021 04:33:45 GMT
WORKDIR /var/www/html
# Sat, 27 Mar 2021 04:35:03 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 27 Mar 2021 04:35:21 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 27 Mar 2021 04:35:29 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Sat, 27 Mar 2021 04:35:40 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Sat, 27 Mar 2021 04:35:46 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Sat, 27 Mar 2021 04:35:59 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Sat, 27 Mar 2021 04:36:05 GMT
VOLUME [/var/www/html]
# Sat, 27 Mar 2021 04:36:07 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Sat, 27 Mar 2021 04:36:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 04:36:15 GMT
USER www-data
# Sat, 27 Mar 2021 04:36:21 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:f3b2866c25f0a9167af050d646a7a740ccc88d46e068c90ff28a5c2ec2ee0030`  
		Last Modified: Thu, 25 Mar 2021 22:24:08 GMT  
		Size: 2.8 MB (2813115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:daca8c363f7712061682fe7d66e2ffc7b799dc3eeda331a052371fb1d4e035f4`  
		Last Modified: Fri, 26 Mar 2021 14:03:41 GMT  
		Size: 1.7 MB (1741748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:424805b3da287757ac21e21b913464a51a7f769315aa3d315509d358f2abe2d9`  
		Last Modified: Fri, 26 Mar 2021 14:03:40 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:264372d3d9e7f169e6bae54417834eaa26d51761308cbd903403393d376a6e94`  
		Last Modified: Fri, 26 Mar 2021 14:03:39 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:325e9355a5fc284df5be5702d4ac0f920d8798e8af561bc00bd2480eafdf0855`  
		Last Modified: Fri, 26 Mar 2021 14:09:13 GMT  
		Size: 12.2 MB (12157776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2849e0e562561225a898517645254cb3f2416639b571649e772f07ac50d241c4`  
		Last Modified: Fri, 26 Mar 2021 14:09:12 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6df4665d977c27d7e4e02a21a144d932ac793c9991e59ec270690bca65837976`  
		Last Modified: Fri, 26 Mar 2021 14:09:18 GMT  
		Size: 15.5 MB (15517930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae754b9a49684c23cfd1ae6728090a171f504045379ce4d7e104fcba6502acc`  
		Last Modified: Fri, 26 Mar 2021 14:09:12 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca327dd8db6e2a5ce0a8b6ad55a727e5b73e1c1cb313907c70864c59684946a`  
		Last Modified: Fri, 26 Mar 2021 14:09:12 GMT  
		Size: 17.3 KB (17332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d67b96470b86b7346015d5cd22b0ea14188ee125c71fe8344d5bb2bdf0da3e6`  
		Last Modified: Sat, 27 Mar 2021 04:46:18 GMT  
		Size: 9.5 MB (9530530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e47cf443fedda4127b2ecd3fcc4a16b2edd991b457f995dd8c23c09a2f41360`  
		Last Modified: Sat, 27 Mar 2021 04:46:13 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d6b2d559ece3a4be65552423984ea1ddb860e4144f6d74dc942d825966e54f6`  
		Last Modified: Sat, 27 Mar 2021 04:46:14 GMT  
		Size: 4.7 MB (4717356 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45a1be8f831ca31bc4e596a2547c09800ae74bdd69d1dc4b842560dd9bacec67`  
		Last Modified: Sat, 27 Mar 2021 04:46:13 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d456dab1b92528b6bd59958750f647cd51d6675cd18cf78a8ed24c5fd0b4c665`  
		Last Modified: Sat, 27 Mar 2021 04:46:14 GMT  
		Size: 1.2 MB (1205818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f417e3634d9bde24f15e7668351e4741b54b7b83c54aa0f961f919cec0b72e58`  
		Last Modified: Sat, 27 Mar 2021 04:46:13 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4.0-php7.3` - linux; s390x

```console
$ docker pull wordpress@sha256:ff71c6e61af44df80da4f2d2044041fe08a80931a92f9d6666297d298256bffa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (46012240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b4e3d114339c0bcf49ad06767ede86bb21db91ed5c174491f91307489b26dbb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Wed, 31 Mar 2021 17:14:58 GMT
ADD file:3f5fe04867af3c9f2cfc5b315d97097145ae11343399985386321a8db21d7786 in / 
# Wed, 31 Mar 2021 17:14:58 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 01:11:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 01 Apr 2021 01:11:52 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 01 Apr 2021 01:11:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 01 Apr 2021 01:11:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 01 Apr 2021 01:11:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 01 Apr 2021 01:11:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 01:11:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 01 Apr 2021 01:11:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 01 Apr 2021 01:49:51 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 01 Apr 2021 01:49:51 GMT
ENV PHP_VERSION=7.3.27
# Thu, 01 Apr 2021 01:49:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.27.tar.xz.asc
# Thu, 01 Apr 2021 01:49:51 GMT
ENV PHP_SHA256=65f616e2d5b6faacedf62830fa047951b0136d5da34ae59e6744cbaf5dca148d
# Thu, 01 Apr 2021 01:49:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 01:49:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 01:54:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 01:54:08 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 01 Apr 2021 01:54:10 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 01:54:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 01:54:11 GMT
CMD ["php" "-a"]
# Thu, 01 Apr 2021 05:19:49 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 01 Apr 2021 05:19:50 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 01 Apr 2021 05:19:51 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 05:20:28 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 05:20:29 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 01 Apr 2021 05:20:29 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 01 Apr 2021 05:20:29 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 01 Apr 2021 05:20:29 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 01 Apr 2021 05:20:31 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 01 Apr 2021 05:20:31 GMT
VOLUME [/var/www/html]
# Thu, 01 Apr 2021 05:20:32 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 01 Apr 2021 05:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 05:20:32 GMT
USER www-data
# Thu, 01 Apr 2021 05:20:32 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:1d4058bbeedf5296bcaf5ae8f37c8cd58152acad3ec45a536e08b83f5d3abe83`  
		Last Modified: Wed, 31 Mar 2021 17:15:36 GMT  
		Size: 2.6 MB (2602591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a4c07ec00cdaafa92f3d601111e0e944457d2558ae06e4ce2e67960618fc651`  
		Last Modified: Thu, 01 Apr 2021 02:24:49 GMT  
		Size: 1.8 MB (1756492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5489cbeafa33cd33ad47e4fd6c7340503c898fb03a500adea4bb365316c28b9`  
		Last Modified: Thu, 01 Apr 2021 02:24:48 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1315fe5c5d5b17d21ea40b00f7ec9504f46655b7a4b0d3ca770546a572162af`  
		Last Modified: Thu, 01 Apr 2021 02:24:48 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f65253eb52504ddee66f5a28eea5031b9d272c343afe188eeea66d6ad5cd0cd`  
		Last Modified: Thu, 01 Apr 2021 02:28:56 GMT  
		Size: 12.2 MB (12157779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:920f0032be7959c7e3838695b3a9cf63101cdebbcbcb68a24f8ced067ae90b73`  
		Last Modified: Thu, 01 Apr 2021 02:28:58 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cf0067e1c826403ae5d0209dd4a4d149fc07afce604beb6b887629af5149d87`  
		Last Modified: Thu, 01 Apr 2021 02:28:57 GMT  
		Size: 13.8 MB (13836086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2f6dae4d2a61de63ccb0a2424d2b6ed2b9d7094677bdde665eb7f6b341b08e`  
		Last Modified: Thu, 01 Apr 2021 02:28:55 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90dbf97d523412521151fadd8544684f9bab5a324eb501072f91535cf204c92e`  
		Last Modified: Thu, 01 Apr 2021 02:28:55 GMT  
		Size: 17.3 KB (17331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c48a61e970d71b4d1f622c4f0942d5ebbd7a3211d9d1f44fe90c8a04eb4b68`  
		Last Modified: Thu, 01 Apr 2021 05:23:53 GMT  
		Size: 9.8 MB (9829975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07583ae47bef9793bd92a831c3428533bb2c1b6f7437f0193a5082bef61b47bf`  
		Last Modified: Thu, 01 Apr 2021 05:23:50 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1995b5bc04362a7c8ea6eb9445bb1aab2c671be6376fc65eb060c0a768fc2aa9`  
		Last Modified: Thu, 01 Apr 2021 05:23:50 GMT  
		Size: 4.6 MB (4600963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64ea6cbaaab6823b46d246c0f2d5079cefd12ef0736ff31f48a68b7e0097602`  
		Last Modified: Thu, 01 Apr 2021 05:23:50 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92f80da2964752bc85e4bc6d7e216ec05a8867e0c6da4c89dd9e31d35ada829`  
		Last Modified: Thu, 01 Apr 2021 05:23:50 GMT  
		Size: 1.2 MB (1205788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9b81a74eff11a45da57c5db51b371d7e74a37e8611f84ef7dcef1c31a1f0db`  
		Last Modified: Thu, 01 Apr 2021 05:23:50 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
