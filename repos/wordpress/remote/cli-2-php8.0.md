## `wordpress:cli-2-php8.0`

```console
$ docker pull wordpress@sha256:214e469f386e0872f9117ff51b1fa6812278bac54d13f9d4f9779963aacbffc2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `wordpress:cli-2-php8.0` - linux; amd64

```console
$ docker pull wordpress@sha256:6e5a3fc1b2dbdcd770b960d591f4857bb7215e1a5236879cdcb77736c1047381
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.2 MB (42211668 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:512e22a5f8198f77a5e864f55e93820bac0f33cce80d0ce68fdc3efe558690c0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Fri, 15 Jan 2021 02:23:51 GMT
ADD file:edbe213ae0c825a5bfbe569928cf20f683f334f93a093ccd0a3a014b7428e760 in / 
# Fri, 15 Jan 2021 02:23:51 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 23:43:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 23:43:24 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 23:43:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 23:43:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 23:43:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 23:43:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:43:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:43:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 23:43:30 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 15 Jan 2021 23:43:30 GMT
ENV PHP_VERSION=8.0.1
# Fri, 15 Jan 2021 23:43:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.1.tar.xz.asc
# Fri, 15 Jan 2021 23:43:31 GMT
ENV PHP_SHA256=208b3330af881b44a6a8c6858d569c72db78dab97810332978cc65206b0ec2dc
# Fri, 15 Jan 2021 23:43:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:43:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:51:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 20:17:47 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 21 Jan 2021 20:17:50 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 20:17:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 20:17:51 GMT
CMD ["php" "-a"]
# Thu, 21 Jan 2021 20:55:15 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 21 Jan 2021 20:55:16 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 21 Jan 2021 20:55:16 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 20:56:03 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Jan 2021 20:56:04 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 21 Jan 2021 20:56:05 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 21 Jan 2021 20:56:05 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 21 Jan 2021 20:56:05 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 21 Jan 2021 20:56:07 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 21 Jan 2021 20:56:08 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 20:56:08 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 21 Jan 2021 20:56:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 20:56:08 GMT
USER www-data
# Thu, 21 Jan 2021 20:56:08 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:596ba82af5aaa3e2fd9d6f955b8b94f0744a2b60710e3c243ba3e4a467f051d1`  
		Last Modified: Fri, 15 Jan 2021 02:08:10 GMT  
		Size: 2.8 MB (2810825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af74f285bb27c6623f2b5c8c3a2e487603c7dd5c51859fd6e13859542f4310c3`  
		Last Modified: Sat, 16 Jan 2021 01:00:24 GMT  
		Size: 1.7 MB (1694838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab8440e5667ccb2ffd4e62ed905a106742dfdd7dd3167d9d64b4bdeed8a4945`  
		Last Modified: Sat, 16 Jan 2021 01:00:20 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64889fa545ec919e6fe392c368b8cb41a10e7834c1ba4d4d96fd9ee2e3405cc1`  
		Last Modified: Sat, 16 Jan 2021 01:00:20 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94168e6487351b04d28db6aabb22e0c68ad3582533cf8d7e00322078720f8081`  
		Last Modified: Sat, 16 Jan 2021 01:00:19 GMT  
		Size: 10.7 MB (10661716 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3898f14298ef25ab2005e9025a88f553003a83a1b6a61765e93d78879441aa36`  
		Last Modified: Sat, 16 Jan 2021 01:00:18 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3747e5f21671eba796a4b76a6abc180c60b0ef9414e9a80b325b31aeaa1f6ca`  
		Last Modified: Sat, 16 Jan 2021 01:00:21 GMT  
		Size: 15.3 MB (15318011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c3df0f8088890764041d8dbfe574cd5bdf020400801b0b108cd6b7f965aab3a`  
		Last Modified: Thu, 21 Jan 2021 20:28:34 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f6ddeaf0bdcf495df2e7c8d72852796c1bae3d9f8ef8260058fdb43b995163`  
		Last Modified: Thu, 21 Jan 2021 20:28:34 GMT  
		Size: 17.5 KB (17539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:112505d2c53dcf98db6040079e92854ab370cbc75b5b92785a8411161181b47e`  
		Last Modified: Thu, 21 Jan 2021 21:03:13 GMT  
		Size: 9.3 MB (9334488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb196045b3f47405e5a84bab00ccdc485f8fb4a5631c16cff8eb5823c23cad6`  
		Last Modified: Thu, 21 Jan 2021 21:03:09 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5cc7cca3850b8699e4605ae363f3b133103373220c7032872608a9e9d14cb99`  
		Last Modified: Thu, 21 Jan 2021 21:03:08 GMT  
		Size: 1.2 MB (1172839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95b64fec7fd0f0f1beb1425ff88f8445f98e94f00c2890f1f173e7f6f3ca0a48`  
		Last Modified: Thu, 21 Jan 2021 21:03:08 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b374f76fd9ff5b0212f1aa75be0352943054de6984e83e0ffa487fba4ee777f4`  
		Last Modified: Thu, 21 Jan 2021 21:03:08 GMT  
		Size: 1.2 MB (1196260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5833431bbac63d295daf3764e0e5dbcf08c6d00a99a30d3fd0792cef323f1122`  
		Last Modified: Thu, 21 Jan 2021 21:03:08 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php8.0` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:0946a7c98858326675adedb3f0d602bc61c9d1d9eff653037bd33ad3e58932eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.2 MB (40158769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1905125d8f613e3b6257e28add13d1ba85ff647fc36acacdf89053d471087de5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Fri, 15 Jan 2021 01:51:19 GMT
ADD file:f2665ccfd90cf53580dc87c3e57db7c223147c686554b1d6e3fc166cce818b3e in / 
# Fri, 15 Jan 2021 01:51:20 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 22:53:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 22:53:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 22:54:00 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 22:54:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 22:54:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 22:54:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 22:54:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 22:54:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 22:54:05 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 15 Jan 2021 22:54:05 GMT
ENV PHP_VERSION=8.0.1
# Fri, 15 Jan 2021 22:54:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.1.tar.xz.asc
# Fri, 15 Jan 2021 22:54:06 GMT
ENV PHP_SHA256=208b3330af881b44a6a8c6858d569c72db78dab97810332978cc65206b0ec2dc
# Fri, 15 Jan 2021 22:54:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 22:54:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 22:57:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:02:49 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:02:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:03:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:03:01 GMT
CMD ["php" "-a"]
# Thu, 21 Jan 2021 19:49:35 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 21 Jan 2021 19:49:38 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 21 Jan 2021 19:49:38 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 19:50:40 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Jan 2021 19:50:44 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 21 Jan 2021 19:50:45 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 21 Jan 2021 19:50:46 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 21 Jan 2021 19:50:47 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 21 Jan 2021 19:50:53 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 21 Jan 2021 19:50:54 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 19:50:54 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:50:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 19:50:56 GMT
USER www-data
# Thu, 21 Jan 2021 19:50:57 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:b550170d5d44558603032e2371fa7a2fb3575b38b2c64ad8be4ab798bcad44d3`  
		Last Modified: Fri, 15 Jan 2021 01:52:01 GMT  
		Size: 2.6 MB (2621576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3110258b4da6fc6756faa0ee4ede2d02a24ff821ba8f1ba72a75739fc89161fa`  
		Last Modified: Fri, 15 Jan 2021 23:27:01 GMT  
		Size: 1.7 MB (1684838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef6d6cdd312890c0852fd22903c40d68137566e06f947a0c3461bba58aab6fb`  
		Last Modified: Fri, 15 Jan 2021 23:27:00 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61428ad89e8a3dd97317b0da99d3c4b4f36306fd1b554393af68eea521ad75c`  
		Last Modified: Fri, 15 Jan 2021 23:27:00 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff3894a3ae7e83f79c5a6f41cdf891dd272c553efa4e2352f95960dbe81ee8c5`  
		Last Modified: Fri, 15 Jan 2021 23:26:56 GMT  
		Size: 10.7 MB (10661711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9b70f7fa71db3253a5cd86c160d36b8d84b1e2e1e1e51db33beb1588b4fd4e`  
		Last Modified: Fri, 15 Jan 2021 23:26:54 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6688375eab89792d41c4aaa1a8b1c0acd0afa4b774dd657c28c51de1ce3f536`  
		Last Modified: Fri, 15 Jan 2021 23:27:00 GMT  
		Size: 14.0 MB (13964293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f32d816af29684b2734f088138ea043684a1262aacc682feebbaebb1364bd37`  
		Last Modified: Thu, 21 Jan 2021 19:09:11 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fd0328654c566f2b086391daf44b73b095d574d5613a8d7e1088be8e1a5ed5`  
		Last Modified: Thu, 21 Jan 2021 19:09:11 GMT  
		Size: 17.5 KB (17540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4278601373d3ce0b2fa68998090ea93df4341d7621d6f3406afe9c8e8342d074`  
		Last Modified: Thu, 21 Jan 2021 19:55:10 GMT  
		Size: 8.9 MB (8943832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e7a9cee69da5c7c503fc22c3d3ae46ee9b893d212788f9fdfa7fa7f867815d`  
		Last Modified: Thu, 21 Jan 2021 19:55:03 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cfb5430049f0673d6385ef1e1188717f5e527a8f4fdb7068f2ee5dd43ead52`  
		Last Modified: Thu, 21 Jan 2021 19:55:03 GMT  
		Size: 1.1 MB (1063488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad956197dd3778ea5c8faca51d16829156ea85b8d32c242e5963d7885a56e701`  
		Last Modified: Thu, 21 Jan 2021 19:55:03 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14c56c7d975bc9d2be279d12e346958b13376d6af1e5f7444fca2d6a6a095000`  
		Last Modified: Thu, 21 Jan 2021 19:55:06 GMT  
		Size: 1.2 MB (1196261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4a1c68aff38f2cffd640f87e7d691c2d5a6c17ae46f41b7d094760cf84e0e0`  
		Last Modified: Thu, 21 Jan 2021 19:55:03 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php8.0` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:31a7707d25416b13ce24558ce04a692ebf1246376d2b6765347814851c986abf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.6 MB (38558405 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5933b90119fb7419cf218401b76fdca702d63f2252ec8d7fa54c38269025fd0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Fri, 15 Jan 2021 01:58:27 GMT
ADD file:718d7c24a8d6ff0feb2843cf8c3ca4b7ef1fb523a45dea568404259a7b4e6f10 in / 
# Fri, 15 Jan 2021 01:58:29 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 23:04:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 23:04:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 23:04:07 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 23:04:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 23:04:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 23:04:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:04:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:04:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 23:04:13 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 15 Jan 2021 23:04:14 GMT
ENV PHP_VERSION=8.0.1
# Fri, 15 Jan 2021 23:04:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.1.tar.xz.asc
# Fri, 15 Jan 2021 23:04:15 GMT
ENV PHP_SHA256=208b3330af881b44a6a8c6858d569c72db78dab97810332978cc65206b0ec2dc
# Fri, 15 Jan 2021 23:04:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:04:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:07:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:10:13 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:10:16 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:10:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:10:18 GMT
CMD ["php" "-a"]
# Thu, 21 Jan 2021 20:29:40 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 21 Jan 2021 20:29:44 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 21 Jan 2021 20:29:46 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 20:30:42 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Jan 2021 20:30:44 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 21 Jan 2021 20:30:45 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 21 Jan 2021 20:30:46 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 21 Jan 2021 20:30:47 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 21 Jan 2021 20:30:51 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 21 Jan 2021 20:30:52 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 20:30:53 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 21 Jan 2021 20:30:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 20:30:55 GMT
USER www-data
# Thu, 21 Jan 2021 20:30:56 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:0f34ce5da94097b8c334f6b2065a010aced9855c3532e4462e9bd1b0a4c4b3f6`  
		Last Modified: Fri, 15 Jan 2021 01:59:13 GMT  
		Size: 2.4 MB (2422744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cecec77a7b5b50913bcb9f7bfe0c5fdcebb948b947747285290197c13902be91`  
		Last Modified: Fri, 15 Jan 2021 23:42:36 GMT  
		Size: 1.6 MB (1555130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0496082b3c55009a50b47ce80bf27dd7451aaa7e13b5b4ccbe886a780c614dd1`  
		Last Modified: Fri, 15 Jan 2021 23:42:33 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af351861d88fff830659b71d51e45b8e623d31cb86c764fab107e6c39ca5a717`  
		Last Modified: Fri, 15 Jan 2021 23:42:33 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11aa9107e62f7893b45936388317768641833b4f6b1937989fcbfc5845e1c698`  
		Last Modified: Fri, 15 Jan 2021 23:42:32 GMT  
		Size: 10.7 MB (10661711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:739d880e478996d44b501dcc056bf9f5f25909c929d579ba0c02f123be170522`  
		Last Modified: Fri, 15 Jan 2021 23:42:30 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed2a0f0dbdad0b49284a158baa86126c2b2a794ee53b82c4181378520555f1d`  
		Last Modified: Fri, 15 Jan 2021 23:42:36 GMT  
		Size: 13.1 MB (13070133 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7b9ed4df09ec14031c338ad506ba7fcc76ab6a07fc32432ad75d94867ae04d9`  
		Last Modified: Thu, 21 Jan 2021 19:23:58 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:500dd1602efbacb91e481ac3e868dadb7bca74fb6b4f73d41fb2ec82cab72f22`  
		Last Modified: Thu, 21 Jan 2021 19:23:59 GMT  
		Size: 17.5 KB (17536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8bdd0f6fd3af1f237ea4045b843dcf437542cb8c0813fad0f74e9172068bcd6`  
		Last Modified: Thu, 21 Jan 2021 20:41:26 GMT  
		Size: 8.7 MB (8661186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddc0fa1fbb964ada3bf60da5605e92f3c8a4b8d06e7c32c7c100a63ea210cd1`  
		Last Modified: Thu, 21 Jan 2021 20:41:21 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dec33ebc44d8dcc15fb3e0f80396a3069d284bf3cc402d50cff67f9bc54b5fa3`  
		Last Modified: Thu, 21 Jan 2021 20:41:21 GMT  
		Size: 968.5 KB (968487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1003d1d779bf9127ecb1c1dee6a64b5cff165e658477802d889d9363f3a550cd`  
		Last Modified: Thu, 21 Jan 2021 20:41:20 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fd6b5f12bfe4e00804b10eebd5ed88a945ae3a8126c4e0f646869b2c62bee5f`  
		Last Modified: Thu, 21 Jan 2021 20:41:21 GMT  
		Size: 1.2 MB (1196252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3cd2355890dac7fd8f0b56ba6a7ef097675e17308083ec7f27f78979dd5bae`  
		Last Modified: Thu, 21 Jan 2021 20:41:20 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php8.0` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:56b39786a35f19e9c2898287c02154bbc8619c64536bbf2c90fffdf340dcb873
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41601740 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08f30fc59f59a5347c44d8abdf94a06fb835e3fd3a0719b0631384e373ee5f9b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Fri, 15 Jan 2021 01:47:51 GMT
ADD file:95be2cec37537b3fd70aeb1d4eb3479fc4a56b00ad7180788ddd7fa772ca65e7 in / 
# Fri, 15 Jan 2021 01:47:52 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 23:04:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 23:04:24 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 23:04:28 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 23:04:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 23:04:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 23:04:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:04:37 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:04:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 23:04:39 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 15 Jan 2021 23:04:40 GMT
ENV PHP_VERSION=8.0.1
# Fri, 15 Jan 2021 23:04:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.1.tar.xz.asc
# Fri, 15 Jan 2021 23:04:41 GMT
ENV PHP_SHA256=208b3330af881b44a6a8c6858d569c72db78dab97810332978cc65206b0ec2dc
# Fri, 15 Jan 2021 23:04:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:04:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:09:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:51:20 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:51:27 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:51:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:51:31 GMT
CMD ["php" "-a"]
# Thu, 21 Jan 2021 21:16:52 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 21 Jan 2021 21:16:55 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 21 Jan 2021 21:16:56 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 21:17:52 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Jan 2021 21:17:54 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 21 Jan 2021 21:17:55 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 21 Jan 2021 21:17:56 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 21 Jan 2021 21:17:57 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 21 Jan 2021 21:18:01 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 21 Jan 2021 21:18:02 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 21:18:03 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 21 Jan 2021 21:18:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 21:18:04 GMT
USER www-data
# Thu, 21 Jan 2021 21:18:05 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:30d5333d20a68dd6ea3689e2c5692d7071f2d68e72c06f0b3b4c7e213df454e2`  
		Last Modified: Fri, 15 Jan 2021 01:48:29 GMT  
		Size: 2.7 MB (2710904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72077bc47778707d4c51904bf6932e44a09d9a5a37f1bac45ef59fe94bc54e1`  
		Last Modified: Fri, 15 Jan 2021 23:49:43 GMT  
		Size: 1.7 MB (1694577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bfc628cf72db6285835ff062834a15ee7c9067f6b7ccb55fad0a8bb0f292be`  
		Last Modified: Fri, 15 Jan 2021 23:49:41 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ab015e378a2ad2e4c345884006fc6b1678a0ebba44214fbc5e9dcb48ef7bb2`  
		Last Modified: Fri, 15 Jan 2021 23:49:41 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d24a448de09dec3ceb6bc305d0c17be120e79f5611f1e4054850e11526133cc8`  
		Last Modified: Fri, 15 Jan 2021 23:49:39 GMT  
		Size: 10.7 MB (10661733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8079f19e688581d52496f1937db9dc33ef25e597b149eb517633043678bd61d2`  
		Last Modified: Fri, 15 Jan 2021 23:49:39 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978c3da5ab542fa26ea4333b9b5c608d2ee68fa98cbf1e0d05df83ece9439e24`  
		Last Modified: Fri, 15 Jan 2021 23:49:45 GMT  
		Size: 14.8 MB (14764647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1043bb484cdf4818387523cb0c703d862e1c50b54ebe62f605c0d3b74837f39`  
		Last Modified: Thu, 21 Jan 2021 20:05:13 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c953f678545439a3b425e1dd037e3e5d5b8092e37adb1a63cb110a0a888b5300`  
		Last Modified: Thu, 21 Jan 2021 20:05:12 GMT  
		Size: 17.6 KB (17550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b088213b40ee58356582c1b860e1e869d92a8280e6ad1d5c114cd8b702a453bd`  
		Last Modified: Thu, 21 Jan 2021 21:28:41 GMT  
		Size: 9.4 MB (9403058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e00566731ec4ecb1466a552595c386df1d4f37221bf55e6e6b45723f4122b0`  
		Last Modified: Thu, 21 Jan 2021 21:28:37 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3976b84b6c9cf95e8fb904463fc6a496dd9831fe49f91e4c25a8ac8307171bb2`  
		Last Modified: Thu, 21 Jan 2021 21:28:38 GMT  
		Size: 1.1 MB (1147768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdf79423be3a1bb5c4306220a31bd2e8f14798b9d2f7cd167af6b72287919bc2`  
		Last Modified: Thu, 21 Jan 2021 21:28:36 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13d5b47c27837fa0480ccbbc52553ac1e1f45adddc8bc899eed4d340b2f9f7e`  
		Last Modified: Thu, 21 Jan 2021 21:28:37 GMT  
		Size: 1.2 MB (1196266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40af667b20cf3f8a58dff5d87a6425901cc7fc78c8e14ea2c88abb83b75ffff2`  
		Last Modified: Thu, 21 Jan 2021 21:28:37 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php8.0` - linux; 386

```console
$ docker pull wordpress@sha256:5c5c5a62703e26ce5bfa08366536119afae6148dfdee124bdccb32e239e67771
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42576078 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94e8f64599e9f95bcdfba6d2cb127ad59336f6b791afbf02dab1a27d78b2e20f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Fri, 15 Jan 2021 01:38:28 GMT
ADD file:d8723c02f1eb0efa4dadc6480a753d18d7e28d9815bff96a92ff09ff55a92b11 in / 
# Fri, 15 Jan 2021 01:38:29 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 22:42:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 22:42:22 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 22:42:23 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 22:42:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 22:42:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 22:42:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 22:42:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 22:42:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 22:42:24 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 15 Jan 2021 22:42:25 GMT
ENV PHP_VERSION=8.0.1
# Fri, 15 Jan 2021 22:42:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.1.tar.xz.asc
# Fri, 15 Jan 2021 22:42:25 GMT
ENV PHP_SHA256=208b3330af881b44a6a8c6858d569c72db78dab97810332978cc65206b0ec2dc
# Fri, 15 Jan 2021 22:42:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 22:42:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 22:49:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:44:48 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:44:51 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:44:51 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:44:51 GMT
CMD ["php" "-a"]
# Thu, 21 Jan 2021 21:09:30 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 21 Jan 2021 21:09:31 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 21 Jan 2021 21:09:31 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 21:10:17 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Jan 2021 21:10:18 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 21 Jan 2021 21:10:18 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 21 Jan 2021 21:10:18 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 21 Jan 2021 21:10:19 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 21 Jan 2021 21:10:21 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 21 Jan 2021 21:10:21 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 21:10:21 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 21 Jan 2021 21:10:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 21:10:22 GMT
USER www-data
# Thu, 21 Jan 2021 21:10:22 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:9e6a151110e36daa7a487250f98425289313f856e3a586d89d82bafc1bf322c3`  
		Last Modified: Fri, 15 Jan 2021 01:39:01 GMT  
		Size: 2.8 MB (2817152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b194694eae0c8525a66d3c56796eb37a9e263d63f03eaecf6bc83d2ab3f7c9`  
		Last Modified: Fri, 15 Jan 2021 23:50:55 GMT  
		Size: 1.8 MB (1793505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a9a95dec7f2cd3bcf6903d006a870fa7113f6a974d30ec6634ab82b0a0a792`  
		Last Modified: Fri, 15 Jan 2021 23:50:52 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ad687f5cfc54121cc70af5ff69cb844177c4325a2c14efcd144cb096ecfba2`  
		Last Modified: Fri, 15 Jan 2021 23:50:54 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ae4debbbbc31db383a639e6a7df85ebf9c2f15905a9ec2df4fb8a3998dec90`  
		Last Modified: Fri, 15 Jan 2021 23:50:56 GMT  
		Size: 10.7 MB (10661677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:900efcbd73b95b91ec42e946efd16fa2e312e57beba40e9aac2b0699baa90d1d`  
		Last Modified: Fri, 15 Jan 2021 23:50:51 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c042850cc5dcebe86c931da9e6014fe607a6c507fe5a61059ba47003a80cac2`  
		Last Modified: Fri, 15 Jan 2021 23:51:00 GMT  
		Size: 15.3 MB (15348857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a592432a0a1e356653687e23dd3c8f953d0fc904db0377fa898de0c851be229d`  
		Last Modified: Thu, 21 Jan 2021 19:55:39 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3b6898b8d491988e64358ef661f654c98cbec8cc3e36edeedea25334aae60e`  
		Last Modified: Thu, 21 Jan 2021 19:55:40 GMT  
		Size: 17.5 KB (17525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba14158326d081d231e4c538574836742d7217acee03f9cccee8c41d87764b4c`  
		Last Modified: Thu, 21 Jan 2021 21:18:21 GMT  
		Size: 9.5 MB (9498446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaeee0e22276430c90e52e30889685c6aff006aa9889c6d9b3867f5a4ee788c4`  
		Last Modified: Thu, 21 Jan 2021 21:18:13 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57c6f1c17fa3c4ce31b048413ef675fd2cfbf2a7df666ab109f1e4050608481a`  
		Last Modified: Thu, 21 Jan 2021 21:18:15 GMT  
		Size: 1.2 MB (1237519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:078b522fd7d02af85354d3da1374162f334e60efab2e1fcfed463f0fbbffaec7`  
		Last Modified: Thu, 21 Jan 2021 21:18:14 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce15c7f98abde9a48020a5147a8ee6b90f2b4989f305f0d59a90642ae3893749`  
		Last Modified: Thu, 21 Jan 2021 21:18:15 GMT  
		Size: 1.2 MB (1196241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ed35be576a56eab8eba4d22b32aed7d65b9aae58a78fdf9093e1b6d0e37322`  
		Last Modified: Thu, 21 Jan 2021 21:18:14 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php8.0` - linux; s390x

```console
$ docker pull wordpress@sha256:7b4efa093d996a3c2a93a699982bd0d4a7af226bfdb4ad2fbbd75b0358b69010
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.6 MB (41607891 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3b0a728dbb9a501894daf0c18316dd5e024a847cb0e9834f345d0bfdd3b2caf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Fri, 15 Jan 2021 01:51:34 GMT
ADD file:3ba807ca8ed73ca14224dd26a883f2399031fa32430f035cc5ae97b5e6db0ca7 in / 
# Fri, 15 Jan 2021 01:51:35 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 22:57:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 22:57:12 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 22:57:13 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 22:57:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 22:57:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 22:57:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 22:57:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 22:57:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 22:57:17 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 15 Jan 2021 22:57:17 GMT
ENV PHP_VERSION=8.0.1
# Fri, 15 Jan 2021 22:57:18 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.1.tar.xz.asc
# Fri, 15 Jan 2021 22:57:18 GMT
ENV PHP_SHA256=208b3330af881b44a6a8c6858d569c72db78dab97810332978cc65206b0ec2dc
# Fri, 15 Jan 2021 22:57:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 22:57:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:02:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:54:10 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:54:13 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:54:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:54:14 GMT
CMD ["php" "-a"]
# Thu, 21 Jan 2021 21:15:28 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 21 Jan 2021 21:15:32 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 21 Jan 2021 21:15:32 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 21:16:32 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Jan 2021 21:16:34 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 21 Jan 2021 21:16:35 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 21 Jan 2021 21:16:36 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 21 Jan 2021 21:16:36 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 21 Jan 2021 21:16:40 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 21 Jan 2021 21:16:41 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 21:16:42 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 21 Jan 2021 21:16:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 21:16:43 GMT
USER www-data
# Thu, 21 Jan 2021 21:16:44 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:3997176601fb5d5ac06922718668ede4acac00a5c0daef8a9099fd76ce93047f`  
		Last Modified: Fri, 15 Jan 2021 01:52:40 GMT  
		Size: 2.6 MB (2601720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497e79d9095f9ba4812f1150c33ad07d399f559fea8e3c4fe8553e02f2cf8b6a`  
		Last Modified: Fri, 15 Jan 2021 23:39:10 GMT  
		Size: 1.8 MB (1756352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99527660904ffc5aed1d27bb86166f189e04b5df76d7becf74efffb1836eaf5e`  
		Last Modified: Fri, 15 Jan 2021 23:39:10 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9b51111e1ef5a5156e505d6369bb2d4e21354a1203636fca6f26de34df9c15`  
		Last Modified: Fri, 15 Jan 2021 23:39:10 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b3c721a3fef9acf0bac166c45ff18e2485752ef7b86447284b7b710646d40df`  
		Last Modified: Fri, 15 Jan 2021 23:38:47 GMT  
		Size: 10.7 MB (10661723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e676c2ca01980f72daf35a53dae36e4fe10945de76af81d54618066f5204c598`  
		Last Modified: Fri, 15 Jan 2021 23:38:48 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e90c350aff0df72bb91eaa20306afe2218ac1d50242eb213d4e481f65b2a9f60`  
		Last Modified: Fri, 15 Jan 2021 23:38:48 GMT  
		Size: 14.4 MB (14364644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c91dec7c10d367e01e4907cb6c2d00b3e5b7390545c8c9499eaac3c35986507`  
		Last Modified: Thu, 21 Jan 2021 20:05:24 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e63e510378e653ab6ff71c58fc15e869877848171131d614af01c250d7a36e31`  
		Last Modified: Thu, 21 Jan 2021 20:05:20 GMT  
		Size: 17.5 KB (17541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ac6f08e30cde6a14d7c34bc7b7495ff2180a0fe799b9cf69266e2a89174940`  
		Last Modified: Thu, 21 Jan 2021 21:27:50 GMT  
		Size: 9.8 MB (9830114 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a653427ca28d9975a8be0d1b7d6cf1b51f0dace64fb18dffba4bf3cb0cf81805`  
		Last Modified: Thu, 21 Jan 2021 21:27:45 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c0015c939d0358096b446db3a2d19593a7a176eef101cc1ead2330a11fa467d`  
		Last Modified: Thu, 21 Jan 2021 21:27:46 GMT  
		Size: 1.2 MB (1174312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8777248042fd68b74cebbfbb99d8f0ade78c8136780d3013076fb8ed99e92f5a`  
		Last Modified: Thu, 21 Jan 2021 21:27:45 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c123260016c5ea2a9656a9f79daf1e061581a35e02fdc8b0b223246f8e43b30`  
		Last Modified: Thu, 21 Jan 2021 21:27:46 GMT  
		Size: 1.2 MB (1196251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ad80e6d9bb0c167882b4742cbee24800a90ea6ad60e0c285c336f6e27e4cc4e`  
		Last Modified: Thu, 21 Jan 2021 21:27:46 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
