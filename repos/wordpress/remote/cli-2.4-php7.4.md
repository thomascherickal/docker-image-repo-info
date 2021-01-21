## `wordpress:cli-2.4-php7.4`

```console
$ docker pull wordpress@sha256:569cb9a65591f635300b325c46aefcf3c347f997d89ff7e5ba973bc611c79363
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

### `wordpress:cli-2.4-php7.4` - linux; amd64

```console
$ docker pull wordpress@sha256:c864e4b3d27279ddea00d12510ce007b480c06062c37bebfd07bd165277f81eb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44935034 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcc343113a792dd63ec1fda1c44f904bc34e3c20ddd1b5483ac50759954b611e`
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
# Sat, 16 Jan 2021 00:02:53 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 16 Jan 2021 00:02:53 GMT
ENV PHP_VERSION=7.4.14
# Sat, 16 Jan 2021 00:02:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Sat, 16 Jan 2021 00:02:54 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Sat, 16 Jan 2021 00:03:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 16 Jan 2021 00:03:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 16 Jan 2021 00:12:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 20:19:38 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 21 Jan 2021 20:19:41 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 20:19:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 20:19:42 GMT
CMD ["php" "-a"]
# Thu, 21 Jan 2021 20:52:41 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 21 Jan 2021 20:52:42 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 21 Jan 2021 20:52:42 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 20:53:41 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Jan 2021 20:53:42 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 21 Jan 2021 20:53:42 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 21 Jan 2021 20:53:43 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 21 Jan 2021 20:53:43 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 21 Jan 2021 20:53:46 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 21 Jan 2021 20:53:46 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 20:53:46 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 21 Jan 2021 20:53:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 20:53:47 GMT
USER www-data
# Thu, 21 Jan 2021 20:53:47 GMT
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
	-	`sha256:f807504c7162d8c8a01c4ed7719eddf9c0987d1522e53e0cca55d25a811b46a3`  
		Last Modified: Sat, 16 Jan 2021 01:01:27 GMT  
		Size: 10.3 MB (10346229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3950d3df66cb25d8d95f1e080f7c320434a6c03b4e5ca3f53f050955a905cb69`  
		Last Modified: Sat, 16 Jan 2021 01:01:26 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09a3aba4cdc0fa6208a0d3994a2a072a87164f53a4e7ad140668b9ee8751d262`  
		Last Modified: Sat, 16 Jan 2021 01:01:29 GMT  
		Size: 14.6 MB (14626667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177ad834d54fe6b8023f36d21b2ef7f96dba2f99ac5502d3224d47aab40180d1`  
		Last Modified: Thu, 21 Jan 2021 20:31:07 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9356474b59dbf533b938f104e562640901bf2be9ff90ff7d0c094f80e7d6ae8f`  
		Last Modified: Thu, 21 Jan 2021 20:31:07 GMT  
		Size: 17.5 KB (17541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06d9f9db8d161cb7160ee627d79125fd8558cc1c4e8ba44f5ebfdd2104910de`  
		Last Modified: Thu, 21 Jan 2021 21:02:40 GMT  
		Size: 9.3 MB (9334441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d268eff95a4935e68cb4861a73006dd698c893ee002538e10369d63ac7dd4b0`  
		Last Modified: Sat, 16 Jan 2021 02:57:12 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c6fb6635b6998166b2dae0c1049a36a57d3660c7cc6f83e71cfd22ff038d6d`  
		Last Modified: Thu, 21 Jan 2021 21:02:39 GMT  
		Size: 4.9 MB (4893231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30fbf526a0c05b96f6bc4188ad06174db88399846cad9c49e54080b31acb5523`  
		Last Modified: Thu, 21 Jan 2021 21:02:38 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24bb8bca049db06f9f01c3b38d596e8d694789d8bbf1feb03ae7ca3e9ba5ecfe`  
		Last Modified: Thu, 21 Jan 2021 21:02:38 GMT  
		Size: 1.2 MB (1206104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c3b40a73f97d7b534fe6f67d4c472de328bc711c7207aacbd9174f08221b10c`  
		Last Modified: Thu, 21 Jan 2021 21:02:38 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4-php7.4` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:e4160ded74c866041ffc49938a8e1077d29431a852b4b3ef27ca9d6e10af3fcf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.2 MB (43161605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6c027869ce20cd178d4305232a8164e3c3d1fb01dba69c5ffbf599ddceacb7a`
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
# Fri, 15 Jan 2021 23:01:32 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 15 Jan 2021 23:01:33 GMT
ENV PHP_VERSION=7.4.14
# Fri, 15 Jan 2021 23:01:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 15 Jan 2021 23:01:34 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 15 Jan 2021 23:01:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:01:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:04:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:04:31 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:04:35 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:04:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:04:38 GMT
CMD ["php" "-a"]
# Thu, 21 Jan 2021 19:45:42 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 21 Jan 2021 19:45:45 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 21 Jan 2021 19:45:48 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 19:47:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Jan 2021 19:47:07 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 21 Jan 2021 19:47:07 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 21 Jan 2021 19:47:08 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 21 Jan 2021 19:47:08 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 21 Jan 2021 19:47:12 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 21 Jan 2021 19:47:13 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 19:47:13 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:47:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 19:47:15 GMT
USER www-data
# Thu, 21 Jan 2021 19:47:15 GMT
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
	-	`sha256:5068d337aadde6ab5c5030548e4cfad9daeb349600f59048ab1694e1d05e30c4`  
		Last Modified: Fri, 15 Jan 2021 23:28:23 GMT  
		Size: 10.3 MB (10346237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcec7f541445bb5d87df482628532d9371128934f433a8c1ef4846129ffaf180`  
		Last Modified: Fri, 15 Jan 2021 23:28:22 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83bd10c9c1eadd08db33d9e3671f6b06234a6786a77dec628b51f202c5d4e96e`  
		Last Modified: Fri, 15 Jan 2021 23:28:27 GMT  
		Size: 13.6 MB (13622892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58c4516237eb9f3837effadff5447447e696372ca597e8265a1f142055a1b23b`  
		Last Modified: Thu, 21 Jan 2021 19:10:45 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56bcae3fb8b0c47ef6aafaee80d4e8e39d934dfa1628b49abdc7daaad0c7559c`  
		Last Modified: Thu, 21 Jan 2021 19:10:46 GMT  
		Size: 17.5 KB (17541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:656e07c27f9804c6887644e062bfd21dab55331bffeafd07780e93ed7d16f8fb`  
		Last Modified: Thu, 21 Jan 2021 19:54:16 GMT  
		Size: 8.9 MB (8943865 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434603b3ca6afa0d98d156ce7cf27f62521deff77dc075bac65467dee40807b9`  
		Last Modified: Sat, 16 Jan 2021 00:49:07 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb1675c5009af9b5558be9335b86e1433036279d77f3f79aa779be5e223d4fa8`  
		Last Modified: Thu, 21 Jan 2021 19:54:14 GMT  
		Size: 4.7 MB (4713311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6876af6b6d1e9bd6757165c657e5263d44cc2150446e6e7c648e377a57365ec2`  
		Last Modified: Thu, 21 Jan 2021 19:54:13 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a26ba13be159c70fbe8330cb3a1d738b72656de52a648a59c40c7b577a984ae`  
		Last Modified: Thu, 21 Jan 2021 19:54:13 GMT  
		Size: 1.2 MB (1206113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9dec9ff6c3ee7224d83521a6a3021a96f569ded37f55ec70f606f96e52eef80`  
		Last Modified: Thu, 21 Jan 2021 19:54:13 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4-php7.4` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:4ba948e0e7af1e3298ff3a23ad8d899bcf462b51d83887ba7d3da9463269adb0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.4 MB (41371788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ff3c7ed8d9f5c812d2cf91a261cf69e7366e52fd75306a0afe6b273ca4017154`
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
# Fri, 15 Jan 2021 23:12:59 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 15 Jan 2021 23:12:59 GMT
ENV PHP_VERSION=7.4.14
# Fri, 15 Jan 2021 23:13:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 15 Jan 2021 23:13:01 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 15 Jan 2021 23:13:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:13:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:16:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:12:21 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:12:25 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:12:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:12:28 GMT
CMD ["php" "-a"]
# Thu, 21 Jan 2021 20:25:18 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 21 Jan 2021 20:25:20 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 21 Jan 2021 20:25:21 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 20:26:47 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Jan 2021 20:26:53 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 21 Jan 2021 20:26:54 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 21 Jan 2021 20:26:55 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 21 Jan 2021 20:26:56 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 21 Jan 2021 20:27:04 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 21 Jan 2021 20:27:05 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 20:27:06 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 21 Jan 2021 20:27:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 20:27:07 GMT
USER www-data
# Thu, 21 Jan 2021 20:27:08 GMT
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
	-	`sha256:6d411a9897320524d0ec6b6ab3882131b4287b10b7e05035a73738f6903334f9`  
		Last Modified: Fri, 15 Jan 2021 23:44:15 GMT  
		Size: 10.3 MB (10346239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c5163521f805487ee4604684f41ca45bf7f75e37a6a61eb36be0e4b31219898`  
		Last Modified: Fri, 15 Jan 2021 23:44:14 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2dd1ea7aef93b42d2986a2cb55904f342b81e0a20a471c198ebdc84e381615`  
		Last Modified: Fri, 15 Jan 2021 23:44:16 GMT  
		Size: 12.8 MB (12752311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea1be7eb284f2d0cc98958e23ca92cd4d5975ba78d563e585d99b754c8badd6e`  
		Last Modified: Thu, 21 Jan 2021 19:27:05 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:214764e190a9c46d024818c9b3ceaa39a4ee2eb4a9719ca166e9775dd9492a6c`  
		Last Modified: Thu, 21 Jan 2021 19:27:06 GMT  
		Size: 17.5 KB (17537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137131e6b6195081fe045be39092e2e482650f97d0fd6cefe78c6f101704984f`  
		Last Modified: Thu, 21 Jan 2021 20:40:32 GMT  
		Size: 8.7 MB (8661188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a8be4b42e28aa767ef216aad19068414e69be5d0726885995d16e88607c1519`  
		Last Modified: Sat, 16 Jan 2021 01:06:49 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938c2c0eb76d6dfb784aeaf3f0ae92ed801fbca214cec485948ae892f1705a4c`  
		Last Modified: Thu, 21 Jan 2021 20:40:31 GMT  
		Size: 4.4 MB (4405314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:422f29aeb0eadf632fb98390a06dae58e2e4860f7e68d97ec2f27da3f4846b12`  
		Last Modified: Thu, 21 Jan 2021 20:40:28 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06e3ca92003a4fce1b8f341380668dabaab63dfa0a89243ab8fe01b62dd5adb`  
		Last Modified: Thu, 21 Jan 2021 20:40:28 GMT  
		Size: 1.2 MB (1206089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d53b6cf1e04ef42617addee0ac02d69b979a5d970f21fd1f99edea826035423`  
		Last Modified: Thu, 21 Jan 2021 20:40:27 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4-php7.4` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:bda7e5ff8aba6520685548e9d453a65b04ac98182d77e2e7cc738fbb70bd129b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44522373 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fc2a14aa962ebe3fd2074651f2b5064fb0e65a7c9b3e8681b63f16e1de890fd`
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
# Fri, 15 Jan 2021 23:15:53 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 15 Jan 2021 23:15:53 GMT
ENV PHP_VERSION=7.4.14
# Fri, 15 Jan 2021 23:15:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 15 Jan 2021 23:15:56 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 15 Jan 2021 23:16:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:16:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:20:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:54:02 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:54:06 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:54:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:54:08 GMT
CMD ["php" "-a"]
# Thu, 21 Jan 2021 21:12:46 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 21 Jan 2021 21:12:49 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 21 Jan 2021 21:12:49 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 21:14:10 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Jan 2021 21:14:14 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 21 Jan 2021 21:14:15 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 21 Jan 2021 21:14:15 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 21 Jan 2021 21:14:17 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 21 Jan 2021 21:14:24 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 21 Jan 2021 21:14:25 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 21:14:26 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 21 Jan 2021 21:14:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 21:14:28 GMT
USER www-data
# Thu, 21 Jan 2021 21:14:28 GMT
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
	-	`sha256:cbfb39756d597307a803dfcdef775730ead6e04a48d6295f2b323c75c1a3270e`  
		Last Modified: Fri, 15 Jan 2021 23:51:26 GMT  
		Size: 10.3 MB (10346266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d903a2b9ea57349eb2a82373140934fe19f981b950ba4a9e2e5978f1c0c4aa25`  
		Last Modified: Fri, 15 Jan 2021 23:51:25 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ffa509145ddd0a07bd759158d4b73e8595b0ce6641957e19bea1284a526e422`  
		Last Modified: Fri, 15 Jan 2021 23:51:28 GMT  
		Size: 14.4 MB (14419780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a49ed284157cee3540d1a1f370478f74184670765adc9944241399fec321575`  
		Last Modified: Thu, 21 Jan 2021 20:08:28 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c332bf466fd90957eeadb28703a02b621161c74bbfb44111dc281bfc51266771`  
		Last Modified: Thu, 21 Jan 2021 20:08:28 GMT  
		Size: 17.6 KB (17550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0417b7ab00936a68712915933c3ce816f6275dd7c678c957fca55498c9094e23`  
		Last Modified: Thu, 21 Jan 2021 21:27:54 GMT  
		Size: 9.4 MB (9403052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53103071e50e1556b0cf07d79b8c28f48d04248cec6ca1b0d6ade114fc82a836`  
		Last Modified: Sat, 16 Jan 2021 01:56:20 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2aea5e6b2d3efdb68f600ce53ddd52805ac63bcbdf64c84873f308cda08fc1d`  
		Last Modified: Thu, 21 Jan 2021 21:27:54 GMT  
		Size: 4.7 MB (4718903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beead6cc1998bbffcff685045314d1bb0e83eb7ef40a17ff242d04da90877295`  
		Last Modified: Thu, 21 Jan 2021 21:27:51 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20545d27261cc735ca02055b5c55c236f30d8c40db6dfb7a15e33b206e23ef85`  
		Last Modified: Thu, 21 Jan 2021 21:27:52 GMT  
		Size: 1.2 MB (1206106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd3b9e77779763ca2250f01ac118cb9d158620ca148fd1a3466ce063aa361dc2`  
		Last Modified: Thu, 21 Jan 2021 21:27:54 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4-php7.4` - linux; 386

```console
$ docker pull wordpress@sha256:701bb2110931778ff0bc09a6099995d6fe9c6b8430c7afb1960382ab9ebda15b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45731351 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:444ae5dac582bfbdca4905f714a79990fdb6aa9fc41df7ed510548f4cf041e7f`
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
# Fri, 15 Jan 2021 22:57:43 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 15 Jan 2021 22:57:43 GMT
ENV PHP_VERSION=7.4.14
# Fri, 15 Jan 2021 22:57:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 15 Jan 2021 22:57:44 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 15 Jan 2021 22:57:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 22:57:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:04:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:46:36 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:46:38 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:46:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:46:39 GMT
CMD ["php" "-a"]
# Thu, 21 Jan 2021 21:06:43 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 21 Jan 2021 21:06:44 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 21 Jan 2021 21:06:45 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 21:07:45 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Jan 2021 21:07:47 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 21 Jan 2021 21:07:47 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 21 Jan 2021 21:07:48 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 21 Jan 2021 21:07:48 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 21 Jan 2021 21:07:50 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 21 Jan 2021 21:07:51 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 21:07:51 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 21 Jan 2021 21:07:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 21:07:51 GMT
USER www-data
# Thu, 21 Jan 2021 21:07:52 GMT
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
	-	`sha256:84ab03194916cfd454c1b5a9289f46465567e195b6c886cd7d1010d666a3e4a4`  
		Last Modified: Fri, 15 Jan 2021 23:52:12 GMT  
		Size: 10.3 MB (10346204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3cd8a4806d551549a931531a419b3afd220efff12cfc5b88e732f29dca4d20a`  
		Last Modified: Fri, 15 Jan 2021 23:52:11 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee3cdd6d961e6bbf5c1f8e05a216998e3f29c3c6c072841050cd9b40b7ef7390`  
		Last Modified: Fri, 15 Jan 2021 23:52:16 GMT  
		Size: 15.0 MB (14994961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:993c1d208c33643a14b69a2710100992852eb36a926e397383c9e8b743193c31`  
		Last Modified: Thu, 21 Jan 2021 19:58:27 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9cef334c12ce1fb415168b349f992777231f74ca501f163ed98ded15bce10`  
		Last Modified: Thu, 21 Jan 2021 19:58:28 GMT  
		Size: 17.5 KB (17523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f1f98b7e6f5ac15ab702b5cfea5436d616e464f6715b5953a1c655f29a4509`  
		Last Modified: Thu, 21 Jan 2021 21:17:37 GMT  
		Size: 9.5 MB (9498431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13da9b6c372c9cd37b469a6b5e799a5b03e8fb06a1b2a8a6d9c8836ed95d8294`  
		Last Modified: Sat, 16 Jan 2021 01:41:46 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34288e84d6e07a55129c2b2b58c336819d7f757025c1d48a847f391fa865b826`  
		Last Modified: Thu, 21 Jan 2021 21:17:36 GMT  
		Size: 5.1 MB (5052349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:121343ee3124851393a614b966042dd862609494621ea74774fdac39a553a5a6`  
		Last Modified: Thu, 21 Jan 2021 21:17:35 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1950d13067a8cff806bad189a43bb2990adf01d0a7819044b7b039402290f1a7`  
		Last Modified: Thu, 21 Jan 2021 21:17:36 GMT  
		Size: 1.2 MB (1206073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdede81af431a8edfc9b9884b0f39a06cef47fc2643f8b8a0960ca4dbc9510cc`  
		Last Modified: Thu, 21 Jan 2021 21:17:37 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4-php7.4` - linux; ppc64le

```console
$ docker pull wordpress@sha256:a7c2576d52f159415991eec0ade88fee1f7bd5e3c77ddc6dded4030c6e8050c7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46310320 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5db23b06ccaf6849e949a0f999deffd07dd6b11284012dac4d30abda5935668`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Fri, 15 Jan 2021 02:41:43 GMT
ADD file:137e8f98476d5dceaeb2e8359f50eb818dee4c327e4492d16e87fb27d40aa891 in / 
# Fri, 15 Jan 2021 02:41:46 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 23:17:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 23:17:44 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 23:17:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 23:18:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 23:18:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 23:18:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:18:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:18:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 23:33:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 15 Jan 2021 23:33:54 GMT
ENV PHP_VERSION=7.4.14
# Fri, 15 Jan 2021 23:33:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 15 Jan 2021 23:34:02 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 15 Jan 2021 23:34:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:34:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:39:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 15 Jan 2021 23:39:11 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:39:19 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 Jan 2021 23:39:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 Jan 2021 23:39:25 GMT
CMD ["php" "-a"]
# Sat, 16 Jan 2021 02:03:57 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Sat, 16 Jan 2021 02:04:10 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Sat, 16 Jan 2021 02:04:14 GMT
WORKDIR /var/www/html
# Sat, 16 Jan 2021 02:05:22 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 16 Jan 2021 02:05:33 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 16 Jan 2021 02:05:38 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Sat, 16 Jan 2021 02:05:43 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Sat, 16 Jan 2021 02:05:48 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Sat, 16 Jan 2021 02:06:03 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Sat, 16 Jan 2021 02:06:10 GMT
VOLUME [/var/www/html]
# Sat, 16 Jan 2021 02:06:11 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Sat, 16 Jan 2021 02:06:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 16 Jan 2021 02:06:19 GMT
USER www-data
# Sat, 16 Jan 2021 02:06:28 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:cb0f06c26ffdc2117b9a3467f79e69cdf8d9c677a3c0bacabc8a694a9fe303a8`  
		Last Modified: Fri, 15 Jan 2021 02:42:19 GMT  
		Size: 2.8 MB (2812389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9a7aad5bd113c5dca33b681663b0c58f66e510017e693801a6688a9c4bab60`  
		Last Modified: Sat, 16 Jan 2021 00:14:01 GMT  
		Size: 1.7 MB (1741834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ce1d80ff72759b98cf2f5ad1efa6dd181e5f4343bb0e25cbb4ec9d5d3847f4`  
		Last Modified: Sat, 16 Jan 2021 00:14:01 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48055526d8202af50f6248db9b3cb8938cab9cfec15a1312b4c1e3782f3307c4`  
		Last Modified: Sat, 16 Jan 2021 00:14:02 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36406d6bda8ae108b8ce9b7caaac7e99032ed25534334455208005eb42bedfe4`  
		Last Modified: Sat, 16 Jan 2021 00:15:57 GMT  
		Size: 10.3 MB (10346249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddd49420b8de2770a516bec72c6067487b5cb098f90b35e87c52e937e49f7822`  
		Last Modified: Sat, 16 Jan 2021 00:15:56 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99bf0f30c21cf49de5dbc892b21887a6d900bbd4641c3b0ad52876df494a09d`  
		Last Modified: Sat, 16 Jan 2021 00:15:59 GMT  
		Size: 15.7 MB (15663445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0c6476a59d97c1b984797c05969c3982e999f3626139df9a51cc01d60f7fb83`  
		Last Modified: Sat, 16 Jan 2021 00:15:55 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69bcff97f817a7777ddcf6ac4a78a81972570c084c6bc054403d2b5924944066`  
		Last Modified: Sat, 16 Jan 2021 00:15:57 GMT  
		Size: 17.5 KB (17525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03575ab564b6d9865274eef873fa95bcfc213146679bf456cdd93b8dc536e289`  
		Last Modified: Sat, 16 Jan 2021 02:14:19 GMT  
		Size: 9.5 MB (9530709 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a188d7b14935a2e42e379349727abbe882cbce92776039960f680f3c44ba0ec8`  
		Last Modified: Sat, 16 Jan 2021 02:14:14 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91c96b3be58a2fd7528a84cbb60633c7cd3ff93df2ea025f4088d9106af40e52`  
		Last Modified: Sat, 16 Jan 2021 02:14:16 GMT  
		Size: 5.0 MB (4986868 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc95cc8e4fe082e450b5a88935017d88ba9e33a25f89ae8e1a3b830ae7d6d479`  
		Last Modified: Sat, 16 Jan 2021 02:14:14 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f5591e7e6c7de16b809652844547d81862f1318184b1c80193b7bef71949c32`  
		Last Modified: Sat, 16 Jan 2021 02:14:14 GMT  
		Size: 1.2 MB (1206076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0923b3d36333b6fd2d0501f81d1816468ce79cc4cadd91c9b52d8205a6b239d`  
		Last Modified: Sat, 16 Jan 2021 02:14:14 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4-php7.4` - linux; s390x

```console
$ docker pull wordpress@sha256:6287fe0d35accc6f83f11947d2494c8cb07ae12d88ef7ddf0f08317f13943a07
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44633641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c86489eeac953ddf152c389ab937c21839d1edd9fc0b63b12f91d39c3311d10d`
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
# Fri, 15 Jan 2021 23:08:13 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 15 Jan 2021 23:08:13 GMT
ENV PHP_VERSION=7.4.14
# Fri, 15 Jan 2021 23:08:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 15 Jan 2021 23:08:14 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 15 Jan 2021 23:08:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:08:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:11:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:55:46 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:55:48 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:55:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:55:49 GMT
CMD ["php" "-a"]
# Thu, 21 Jan 2021 21:11:54 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 21 Jan 2021 21:11:58 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 21 Jan 2021 21:11:58 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 21:13:15 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 21 Jan 2021 21:13:17 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 21 Jan 2021 21:13:18 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 21 Jan 2021 21:13:19 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 21 Jan 2021 21:13:19 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 21 Jan 2021 21:13:23 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 21 Jan 2021 21:13:24 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 21:13:25 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 21 Jan 2021 21:13:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 21 Jan 2021 21:13:26 GMT
USER www-data
# Thu, 21 Jan 2021 21:13:27 GMT
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
	-	`sha256:c6101217d012d38a66e76c4357337b802741885df369dc9d35f470d48982bda7`  
		Last Modified: Fri, 15 Jan 2021 23:45:13 GMT  
		Size: 10.3 MB (10346238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2728adb88ef376f1ae2c3a7cba2e7d9f3dd8265662c927ab21799d8b36171a`  
		Last Modified: Fri, 15 Jan 2021 23:45:11 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30999da95da14fc976f0705aabb31ad35bab96ca0904a458cf362038b4c09ec`  
		Last Modified: Fri, 15 Jan 2021 23:45:13 GMT  
		Size: 14.0 MB (14004239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8264743229e7f5caa3e17bf1a58333d4096541ac5a544a8512bb57a9778071d`  
		Last Modified: Thu, 21 Jan 2021 20:09:07 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f871637bb4d7105582bd9d776d0d7fd4200c1b0d812f66e97acc70ff0688b3`  
		Last Modified: Thu, 21 Jan 2021 20:09:07 GMT  
		Size: 17.5 KB (17538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db62d78ef232cea495ae2d3b09c14c3de657983c84c4fd26ee92f791842b704b`  
		Last Modified: Thu, 21 Jan 2021 21:26:48 GMT  
		Size: 9.8 MB (9830182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca1b5d57ef3148f23d0f37446e7e3d9b6442245cef84ef4c6447fcb7eecfa76e`  
		Last Modified: Sat, 16 Jan 2021 01:06:25 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e37ffaf6cc3c8c06748c74c508bacb943f3470fd8a42d6f9c8b6c760cc12f531`  
		Last Modified: Thu, 21 Jan 2021 21:26:45 GMT  
		Size: 4.9 MB (4866063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9b9ef01eb0e9acd39cd0e29eebc32844c4e44e93fd6a03acda38f17269cbb5`  
		Last Modified: Thu, 21 Jan 2021 21:26:44 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:487dd3d33b64d7ff9ede0b14a3a1adbc987d86f7b7f0f83e5f06de3973dd8d87`  
		Last Modified: Thu, 21 Jan 2021 21:26:44 GMT  
		Size: 1.2 MB (1206080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b1e3baa6f00cac1c73fdde76026e68353eeceeeff06b822b0e55d4bab00651`  
		Last Modified: Thu, 21 Jan 2021 21:26:44 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
