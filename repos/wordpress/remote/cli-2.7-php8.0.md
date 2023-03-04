## `wordpress:cli-2.7-php8.0`

```console
$ docker pull wordpress@sha256:d55e7f92049ea2ae6ddbf564db10b26308bd419ecfc986161c99a437af9d36d3
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

### `wordpress:cli-2.7-php8.0` - linux; amd64

```console
$ docker pull wordpress@sha256:be0be498363a8c9b024e2465e1d2b07e77ed502e1b20f1f2562de8b28abf42e6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.4 MB (50420930 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40cc2112251173e88e0f27360ce2cd5393ff55a82c38b4565d746d4e851b8f8b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 10:28:32 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 10:28:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 10:28:34 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 10:28:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 11 Feb 2023 10:28:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 11 Feb 2023 10:28:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 10:28:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 10:28:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 11 Feb 2023 11:05:05 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 14 Feb 2023 22:25:34 GMT
ENV PHP_VERSION=8.0.28
# Tue, 14 Feb 2023 22:25:34 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Tue, 14 Feb 2023 22:25:35 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Tue, 14 Feb 2023 22:25:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 14 Feb 2023 22:25:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:29:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 14 Feb 2023 22:29:26 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:29:28 GMT
RUN docker-php-ext-enable sodium
# Tue, 14 Feb 2023 22:29:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 14 Feb 2023 22:29:28 GMT
CMD ["php" "-a"]
# Wed, 15 Feb 2023 01:13:00 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Wed, 15 Feb 2023 01:13:00 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Wed, 15 Feb 2023 01:13:00 GMT
WORKDIR /var/www/html
# Wed, 15 Feb 2023 01:13:52 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 15 Feb 2023 01:13:53 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 15 Feb 2023 01:13:53 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Wed, 15 Feb 2023 01:13:53 GMT
ENV WORDPRESS_CLI_VERSION=2.7.1
# Wed, 15 Feb 2023 01:13:53 GMT
ENV WORDPRESS_CLI_SHA512=956b5e3e1a076bd5441c082ee754e3ff4517ec965b93c621f455c2bf5719358c36e67d52f676492700b59d42cacb34a50d382535c035f19da7a0b98bc41860de
# Wed, 15 Feb 2023 01:13:57 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Wed, 15 Feb 2023 01:13:57 GMT
VOLUME [/var/www/html]
# Wed, 15 Feb 2023 01:13:57 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Wed, 15 Feb 2023 01:13:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Feb 2023 01:13:57 GMT
USER www-data
# Wed, 15 Feb 2023 01:13:57 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd032c1d9bc64fb28abb14a4f1f7ba3b82f201fe308eb5cb5f9a25ef1c0b524`  
		Last Modified: Sat, 11 Feb 2023 11:21:33 GMT  
		Size: 1.7 MB (1721195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be86720d648286af3b185a53ce7968d957f0370224f1ecbfbe38dc2ab06c6647`  
		Last Modified: Sat, 11 Feb 2023 11:21:33 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03010434aa246ad0ecbd25429ffe16a52c424f962893504bc1303a6e13f33cf8`  
		Last Modified: Sat, 11 Feb 2023 11:21:32 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7135a4d741b88c4c2fc57f4ea06a9252143b246c13ee3b572b33d0076b32b4d3`  
		Last Modified: Tue, 14 Feb 2023 22:52:49 GMT  
		Size: 10.8 MB (10821694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab8de11e4dc2c7b78ca270224de83c9cd0dfc3e153bc8db80f192c375428b86`  
		Last Modified: Tue, 14 Feb 2023 22:52:48 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ced9817301a9b38966a8d6a8c80df8fa529923bc6bf4f535e29c0da7cc54029`  
		Last Modified: Tue, 14 Feb 2023 22:52:51 GMT  
		Size: 15.8 MB (15786322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186736c2ddd80ce8503bd46b2201495ce9ad37a91f9febe27a6924d484b8c347`  
		Last Modified: Tue, 14 Feb 2023 22:52:48 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73966b113bec5feb617122324f288704b327f4ea484175d0f32bff11ebab5428`  
		Last Modified: Tue, 14 Feb 2023 22:52:48 GMT  
		Size: 18.7 KB (18673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce99b761e4a910368e37f0570c38bb1b1d7e5d67eeeffca1639769bfbcb6f3da`  
		Last Modified: Wed, 15 Feb 2023 01:24:28 GMT  
		Size: 9.4 MB (9414835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee04395ca7c71b2d9e568621eaeb36335df3f55a9d2e84768b2a93ed63cf2fe8`  
		Last Modified: Wed, 15 Feb 2023 01:24:25 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77342b375820d8a49306991b1944a2b2b96d71aa617205938dea7039e6ad00d`  
		Last Modified: Wed, 15 Feb 2023 01:24:27 GMT  
		Size: 8.4 MB (8409911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7fd88f4edd19c417116820368504051a82da7f3a121912531a1e97d7b38faec`  
		Last Modified: Wed, 15 Feb 2023 01:24:25 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4debb0157f92d04a2d679acb952a4b300fc0e1cdfde7c400314c43ee59f41a60`  
		Last Modified: Wed, 15 Feb 2023 01:24:25 GMT  
		Size: 1.4 MB (1435122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:263ab354680ba00daf1c9fd800e068156867198df05a062d076ecd881bffcf6c`  
		Last Modified: Wed, 15 Feb 2023 01:24:25 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.7-php8.0` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:eee92fd3d610d2247c1d44da80080de4c27c05c48481126bbb6a6a91825448a8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (47984001 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4429dd46baf4763104a083c88b8c0c258e5267a20da7977ad7ceebd4cff73d65`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:32 GMT
ADD file:be37ec4af7b6db1fa6f84ab2c33fc04aaba5914eb2ac433a417e619fed27c5b4 in / 
# Fri, 10 Feb 2023 20:49:32 GMT
CMD ["/bin/sh"]
# Sat, 04 Mar 2023 00:12:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 04 Mar 2023 00:12:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 04 Mar 2023 00:12:35 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 04 Mar 2023 00:12:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 04 Mar 2023 00:12:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 04 Mar 2023 00:12:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Mar 2023 00:12:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 04 Mar 2023 00:12:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 04 Mar 2023 01:26:53 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Sat, 04 Mar 2023 01:26:53 GMT
ENV PHP_VERSION=8.0.28
# Sat, 04 Mar 2023 01:26:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Sat, 04 Mar 2023 01:26:54 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Sat, 04 Mar 2023 01:27:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 04 Mar 2023 01:27:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 04 Mar 2023 01:30:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 04 Mar 2023 01:30:11 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Sat, 04 Mar 2023 01:30:12 GMT
RUN docker-php-ext-enable sodium
# Sat, 04 Mar 2023 01:30:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 04 Mar 2023 01:30:12 GMT
CMD ["php" "-a"]
# Sat, 04 Mar 2023 02:57:24 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Sat, 04 Mar 2023 02:57:25 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Sat, 04 Mar 2023 02:57:25 GMT
WORKDIR /var/www/html
# Sat, 04 Mar 2023 02:58:14 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Sat, 04 Mar 2023 02:58:15 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 04 Mar 2023 02:58:15 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Sat, 04 Mar 2023 02:58:15 GMT
ENV WORDPRESS_CLI_VERSION=2.7.1
# Sat, 04 Mar 2023 02:58:15 GMT
ENV WORDPRESS_CLI_SHA512=956b5e3e1a076bd5441c082ee754e3ff4517ec965b93c621f455c2bf5719358c36e67d52f676492700b59d42cacb34a50d382535c035f19da7a0b98bc41860de
# Sat, 04 Mar 2023 02:58:19 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Sat, 04 Mar 2023 02:58:19 GMT
VOLUME [/var/www/html]
# Sat, 04 Mar 2023 02:58:19 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Sat, 04 Mar 2023 02:58:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 04 Mar 2023 02:58:19 GMT
USER www-data
# Sat, 04 Mar 2023 02:58:19 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:c35ac6bda1fd9456dc61d44052491ecd935dcde4eb6088d66765ca8c6b57cb7d`  
		Last Modified: Fri, 10 Feb 2023 20:50:40 GMT  
		Size: 2.6 MB (2616778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709cd8d5fc8b0e3f6cda6fbb8a3b78c3da3fdc05b73ca1ad6bccaca580064853`  
		Last Modified: Sat, 04 Mar 2023 01:44:20 GMT  
		Size: 1.7 MB (1708422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2582bf09384cea545ff55bee287aa129feb9889f6046a94fbe310ae4953b6f20`  
		Last Modified: Sat, 04 Mar 2023 01:44:19 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2c7a68e83ffcfbcce51b3b9571c3a768468d98eceb56d6113fc26cd1f46574b`  
		Last Modified: Sat, 04 Mar 2023 01:44:19 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77ae6ee338dafb765d835616c849cdf5e6a9a8286f489b82d67eb228566f08d0`  
		Last Modified: Sat, 04 Mar 2023 01:52:21 GMT  
		Size: 10.8 MB (10821696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43b94ad300c451316bf8ead22217229b84a50c1e62a94295fc7faf687a4e8044`  
		Last Modified: Sat, 04 Mar 2023 01:52:20 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90bf58170ceaf417254277a6b2ff2b4e5837e3ff8ea78857803868194b8736bb`  
		Last Modified: Sat, 04 Mar 2023 01:52:24 GMT  
		Size: 14.4 MB (14399980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3106d06addfa688ebe301b33fa351a8218ccc171b81282a6b76f7c250b360cd1`  
		Last Modified: Sat, 04 Mar 2023 01:52:20 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a8dc4151b76a50056bdebf34bb9da8584c345c8e22603c563a550d7954544c0`  
		Last Modified: Sat, 04 Mar 2023 01:52:20 GMT  
		Size: 18.7 KB (18668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0285caf1e6f02ca438f3732923e3f6b015e9a0f688ebfa2219b8801a898c9373`  
		Last Modified: Sat, 04 Mar 2023 03:04:51 GMT  
		Size: 9.0 MB (8988949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8741ac1f4014ad0477fa131e1595340ccce785ef4789bacbe80019c4182e1be9`  
		Last Modified: Sat, 04 Mar 2023 03:04:47 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef100ed151fabce0c7acfd2fff782aeb1f3df89f88da956e9e70e3d69580ad46`  
		Last Modified: Sat, 04 Mar 2023 03:04:48 GMT  
		Size: 8.0 MB (7988950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54cb726a494b6c724630f131b67756242a40df4efe6a568a8078dfa2dceee72e`  
		Last Modified: Sat, 04 Mar 2023 03:04:47 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9877452311f3ad4109f90f5aaefbdb1038468268b02f4a0d2e5d18c184bd262`  
		Last Modified: Sat, 04 Mar 2023 03:04:47 GMT  
		Size: 1.4 MB (1435142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85352dd3111ec447fc84dd2ec68541ff1bceaff7f5e947f7b5da13d1dfb464ba`  
		Last Modified: Sat, 04 Mar 2023 03:04:47 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.7-php8.0` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:c9720a6776603d465390768f8b248a67f6603c16b64c5a333c70e7d1ffb37d31
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45987365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13659f02e36f8d190cc806b13e1673959836c041e056027492ecf3a6493a07ca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:37 GMT
ADD file:193f48d48ed2e90a0e81663757e372f59806151c17e82113f03443db0ef723c3 in / 
# Fri, 10 Feb 2023 21:51:37 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 21:45:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 01 Mar 2023 21:45:06 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 01 Mar 2023 21:45:06 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Mar 2023 21:45:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Mar 2023 21:45:07 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Mar 2023 21:45:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 21:45:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 21:45:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Mar 2023 22:47:43 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 01 Mar 2023 22:47:43 GMT
ENV PHP_VERSION=8.0.28
# Wed, 01 Mar 2023 22:47:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 01 Mar 2023 22:47:43 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 01 Mar 2023 22:47:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 01 Mar 2023 22:47:50 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Mar 2023 22:50:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Mar 2023 22:50:27 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Wed, 01 Mar 2023 22:50:28 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Mar 2023 22:50:28 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Mar 2023 22:50:28 GMT
CMD ["php" "-a"]
# Thu, 02 Mar 2023 10:04:54 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 02 Mar 2023 10:04:55 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 02 Mar 2023 10:04:55 GMT
WORKDIR /var/www/html
# Thu, 02 Mar 2023 10:05:45 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 02 Mar 2023 10:05:45 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 02 Mar 2023 10:05:45 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 02 Mar 2023 10:05:45 GMT
ENV WORDPRESS_CLI_VERSION=2.7.1
# Thu, 02 Mar 2023 10:05:45 GMT
ENV WORDPRESS_CLI_SHA512=956b5e3e1a076bd5441c082ee754e3ff4517ec965b93c621f455c2bf5719358c36e67d52f676492700b59d42cacb34a50d382535c035f19da7a0b98bc41860de
# Thu, 02 Mar 2023 10:05:48 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 02 Mar 2023 10:05:48 GMT
VOLUME [/var/www/html]
# Thu, 02 Mar 2023 10:05:48 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 02 Mar 2023 10:05:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 10:05:49 GMT
USER www-data
# Thu, 02 Mar 2023 10:05:49 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:beefe5ad637c7db32e6afc68103fc4e779630219979216a625338ab55f7d191c`  
		Last Modified: Fri, 10 Feb 2023 21:52:51 GMT  
		Size: 2.4 MB (2420494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5eaea2941b2a8a3333b438141aaaa54ac5708580161e12c4966caadc4bc1f0a`  
		Last Modified: Wed, 01 Mar 2023 23:10:08 GMT  
		Size: 1.6 MB (1575752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:850c399b4149e76aca896d6ba3a512e86576b1321bc1c4ade91ff4dd4f7d976b`  
		Last Modified: Wed, 01 Mar 2023 23:10:08 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f370270b11e8101c385b8e4b819118371407c42b1cb37c63d942677c5b1059b6`  
		Last Modified: Wed, 01 Mar 2023 23:10:08 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f86429e3eee2d8f5925f294612c3d383ff3a02b76e74ef0a7c5f5a9897c996b`  
		Last Modified: Wed, 01 Mar 2023 23:18:27 GMT  
		Size: 10.8 MB (10821690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58cd0b45814565f323156e75c0ab7e0ad0101e3aa622415c1c88e71112240edb`  
		Last Modified: Wed, 01 Mar 2023 23:18:26 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95de3905843e26b99a1b5bfd1deafade2579d875f2b2785cfb78627823bb3c85`  
		Last Modified: Wed, 01 Mar 2023 23:18:28 GMT  
		Size: 13.5 MB (13524980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a92a88263e34e34e0c05ed7141af2afeef03839878ef345c80fba8d6fd57467`  
		Last Modified: Wed, 01 Mar 2023 23:18:26 GMT  
		Size: 2.4 KB (2445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a46011fbfdd558761da0e747515b585fea62678b5aac49757034081ce083fb3`  
		Last Modified: Wed, 01 Mar 2023 23:18:26 GMT  
		Size: 18.6 KB (18641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb91234ebf26f30c5b3a52e037ce358b2c108b0c7b6fc91573a98a04f36b2b28`  
		Last Modified: Thu, 02 Mar 2023 10:20:41 GMT  
		Size: 8.7 MB (8702821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735d9fa31e12f4e16d6f8fb94b82857fd8fe21674612be122d84598466cd7c9b`  
		Last Modified: Thu, 02 Mar 2023 10:20:37 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75c493cc5fb3d95276739f05ff8d1fd23842c7ea95100fde67f6c89e0f1b6dd`  
		Last Modified: Thu, 02 Mar 2023 10:20:39 GMT  
		Size: 7.5 MB (7482464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb162562fa43415d0617cb8cd2d4a9d86a8c15c309623c261e13cf928b7dea5`  
		Last Modified: Thu, 02 Mar 2023 10:20:37 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9b0609276dd18aed7f1193a5842e4623761c707e4062c8cdb4ea5084b10fb44`  
		Last Modified: Thu, 02 Mar 2023 10:20:38 GMT  
		Size: 1.4 MB (1435106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e026595ba810047b40d69cfc0fc576e920f73c34b4fa3a83724fe60e48559109`  
		Last Modified: Thu, 02 Mar 2023 10:20:37 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.7-php8.0` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:974e7d2bffb1e4f0590c0b1928756fbfe526ae31b94b65d211b6d2ba1e50c5cf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.6 MB (49582389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8d687d419381ceb76630e9ac5d83f485b83a246cdac4895bee6609187f2214e6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:13 GMT
ADD file:738e640812bf6089767190a2976ceffc11f3e809be3e2b1ebb43c85ad3199fba in / 
# Fri, 10 Feb 2023 21:24:13 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 02:14:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 02:14:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 02:14:05 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 02:14:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 11 Feb 2023 02:14:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 11 Feb 2023 02:14:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 02:14:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 02:14:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 11 Feb 2023 02:50:28 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 14 Feb 2023 22:40:04 GMT
ENV PHP_VERSION=8.0.28
# Tue, 14 Feb 2023 22:40:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Tue, 14 Feb 2023 22:40:04 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Tue, 14 Feb 2023 22:40:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 14 Feb 2023 22:40:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:42:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 14 Feb 2023 22:42:44 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:42:45 GMT
RUN docker-php-ext-enable sodium
# Tue, 14 Feb 2023 22:42:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 14 Feb 2023 22:42:45 GMT
CMD ["php" "-a"]
# Wed, 15 Feb 2023 01:57:27 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Wed, 15 Feb 2023 01:57:28 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Wed, 15 Feb 2023 01:57:28 GMT
WORKDIR /var/www/html
# Wed, 15 Feb 2023 01:58:11 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 15 Feb 2023 01:58:12 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 15 Feb 2023 01:58:12 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Wed, 15 Feb 2023 01:58:12 GMT
ENV WORDPRESS_CLI_VERSION=2.7.1
# Wed, 15 Feb 2023 01:58:12 GMT
ENV WORDPRESS_CLI_SHA512=956b5e3e1a076bd5441c082ee754e3ff4517ec965b93c621f455c2bf5719358c36e67d52f676492700b59d42cacb34a50d382535c035f19da7a0b98bc41860de
# Wed, 15 Feb 2023 01:58:16 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Wed, 15 Feb 2023 01:58:16 GMT
VOLUME [/var/www/html]
# Wed, 15 Feb 2023 01:58:16 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Wed, 15 Feb 2023 01:58:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Feb 2023 01:58:16 GMT
USER www-data
# Wed, 15 Feb 2023 01:58:16 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:3760b48202b3e349986edb6fe5dd93cd003726b7c345d51f6fc4ace1b46fc2ba`  
		Last Modified: Fri, 10 Feb 2023 21:24:52 GMT  
		Size: 2.7 MB (2709502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24945052da1277802c9acdaf867899c620d73633d9ffdb9141894016d23502a8`  
		Last Modified: Sat, 11 Feb 2023 03:03:59 GMT  
		Size: 1.7 MB (1715610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aab80b0b76f2ca115ba0bf03f9e94151c3b730634d2d9e928f9cda792e65966`  
		Last Modified: Sat, 11 Feb 2023 03:03:58 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3b2459980e300f1a871481cd0f9ef1a474248c2a36c1a7cad8928a45283a0fa`  
		Last Modified: Sat, 11 Feb 2023 03:03:58 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca888fb20293743bd6573d01157168178e00266ddfc290f75bde10fb51b88d4`  
		Last Modified: Tue, 14 Feb 2023 23:04:01 GMT  
		Size: 10.8 MB (10821700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ae4ff473722ad7294c6207299979a30850536e19d951c080b20f9bdc8742d56`  
		Last Modified: Tue, 14 Feb 2023 23:04:00 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971e9f5739b4c484bdcc4adf33bef1a60446cd9278f82f023c3f2322185e2cb7`  
		Last Modified: Tue, 14 Feb 2023 23:04:02 GMT  
		Size: 15.2 MB (15200341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7c1a501e6f856fbf42c3d7d7a5da0f00e79d4e2fbecf84584127d5bee78fbf`  
		Last Modified: Tue, 14 Feb 2023 23:04:00 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83790f20155f94e4823eebd8f48ae616db3ad7034327bb7df9b62b61509a0a96`  
		Last Modified: Tue, 14 Feb 2023 23:04:00 GMT  
		Size: 18.7 KB (18677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd36ced259505fee2300aaa1db0df4e638f1bbd7e47e25b3b1cc877758b8cc8`  
		Last Modified: Wed, 15 Feb 2023 02:07:55 GMT  
		Size: 9.5 MB (9462550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8afccc72444fe42c8446cb22c31f0b946be243037d4f06203ed82d9d0810c8d`  
		Last Modified: Wed, 15 Feb 2023 02:07:52 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb84aee5844f42e1a402cbd5f56ef53b8d5d9cb5dddf0be4df3660cac5afcf8`  
		Last Modified: Wed, 15 Feb 2023 02:07:53 GMT  
		Size: 8.2 MB (8213467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698a72cd09c2927428cf8e4a0dc643424e0a68b56652f359ec3a4fc5188279e6`  
		Last Modified: Wed, 15 Feb 2023 02:07:52 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9b7c0799b7d576fc6bfe9208271a57bd439584fe66db581b1ec2295567530b6`  
		Last Modified: Wed, 15 Feb 2023 02:07:52 GMT  
		Size: 1.4 MB (1435129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfb2651fc5d60ea69f02654ec80efb5145e03d7c0cf9f51d87ab0ace4b05166`  
		Last Modified: Wed, 15 Feb 2023 02:07:52 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.7-php8.0` - linux; 386

```console
$ docker pull wordpress@sha256:771fe4e638a622f4a01bce37f2cafb011039b4d65388e9286308240ac41b70c6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51407235 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea2f0bebdd4b3f224a402061f97fc8f3ca8d750fe8244510a01a8e2341d73cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:29 GMT
ADD file:59ac1f8f33f9b9727892b7e45b33f54ef3c20d9d876c49d6a4c057641821d68f in / 
# Fri, 10 Feb 2023 21:24:29 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 15:26:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 01 Mar 2023 15:26:56 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 01 Mar 2023 15:26:56 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Mar 2023 15:26:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Mar 2023 15:26:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Mar 2023 15:26:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 15:26:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 15:26:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Mar 2023 17:50:31 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Wed, 01 Mar 2023 17:50:31 GMT
ENV PHP_VERSION=8.0.28
# Wed, 01 Mar 2023 17:50:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Wed, 01 Mar 2023 17:50:31 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Wed, 01 Mar 2023 17:50:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 01 Mar 2023 17:50:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:57:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Mar 2023 17:57:38 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Wed, 01 Mar 2023 17:57:39 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Mar 2023 17:57:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Mar 2023 17:57:39 GMT
CMD ["php" "-a"]
# Thu, 02 Mar 2023 10:22:12 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 02 Mar 2023 10:22:12 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 02 Mar 2023 10:22:13 GMT
WORKDIR /var/www/html
# Thu, 02 Mar 2023 10:23:24 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 02 Mar 2023 10:23:24 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 02 Mar 2023 10:23:24 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 02 Mar 2023 10:23:24 GMT
ENV WORDPRESS_CLI_VERSION=2.7.1
# Thu, 02 Mar 2023 10:23:24 GMT
ENV WORDPRESS_CLI_SHA512=956b5e3e1a076bd5441c082ee754e3ff4517ec965b93c621f455c2bf5719358c36e67d52f676492700b59d42cacb34a50d382535c035f19da7a0b98bc41860de
# Thu, 02 Mar 2023 10:23:28 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 02 Mar 2023 10:23:28 GMT
VOLUME [/var/www/html]
# Thu, 02 Mar 2023 10:23:28 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 02 Mar 2023 10:23:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 02 Mar 2023 10:23:29 GMT
USER www-data
# Thu, 02 Mar 2023 10:23:29 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:0987f51cd58a7d03bc7d6ff0a3a0a843c1a3fefcd41e3c8adc3999ddde7441e8`  
		Last Modified: Fri, 10 Feb 2023 21:25:30 GMT  
		Size: 2.8 MB (2810653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d091c6f48c68be93c6f41db2e3cb3a38d8c2214d2031a89c8b67337b835250c`  
		Last Modified: Wed, 01 Mar 2023 18:25:52 GMT  
		Size: 1.8 MB (1821075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40bfd5d06495a38237df65a5c02bf7cc672f7809651927ec9917e2e6b4b496ec`  
		Last Modified: Wed, 01 Mar 2023 18:25:51 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df8abb5e986c8eae8689259431d8cfd9e1a5c97436d86e75a2b3f6c1ba021c8`  
		Last Modified: Wed, 01 Mar 2023 18:25:51 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3d707ecb1738fe7e5969527bf044a2dc5a9d88d5ee9096ea97f4ba1645fcd2`  
		Last Modified: Wed, 01 Mar 2023 18:34:40 GMT  
		Size: 10.8 MB (10821689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91961c4330a6a193668dc96096990f99d85df6914dece8c58ecad3f0cd59d354`  
		Last Modified: Wed, 01 Mar 2023 18:34:38 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003c01338339fe5bb05eee1efb54daeeb8173369c374906f7a8ad9762d881522`  
		Last Modified: Wed, 01 Mar 2023 18:34:42 GMT  
		Size: 16.1 MB (16139849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381ae5ba1aafc53a71086d328a597bb5e6f0fe0bdb912692f12e5d19be13c5ff`  
		Last Modified: Wed, 01 Mar 2023 18:34:38 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c47b32bf9f6a3792d7da3ca56895d9ff0c5bbabb56758549b528ced4f9d08037`  
		Last Modified: Wed, 01 Mar 2023 18:34:38 GMT  
		Size: 18.6 KB (18650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0f9d19b2b9dc13040b0f127ac88894df6f7a513bc4471e861dc5c9c5c3b6f1`  
		Last Modified: Thu, 02 Mar 2023 10:38:15 GMT  
		Size: 9.6 MB (9573462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8133c4e647dbe02d5c2e0ea0a60ec6aef0c47de0f64a9d7f7d0026adc4af3108`  
		Last Modified: Thu, 02 Mar 2023 10:38:11 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98cf809e4a4c2e03200df017f677f7cfe25e13ebe2b7e76bf39032973782295b`  
		Last Modified: Thu, 02 Mar 2023 10:38:12 GMT  
		Size: 8.8 MB (8781318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d41d8b701fdf3487f821330f7ea43ae0233ee99442fe55d1a7c88b678a5e8a7`  
		Last Modified: Thu, 02 Mar 2023 10:38:10 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073a4140c42644d618057ba0a7e411bf7b497c303b1ceff928672c1ffcdef0ea`  
		Last Modified: Thu, 02 Mar 2023 10:38:11 GMT  
		Size: 1.4 MB (1435125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1ed5d30c88838dd03f1fbff31c837071d56af8e12411f9e8306fbc9d657d408`  
		Last Modified: Thu, 02 Mar 2023 10:38:10 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.7-php8.0` - linux; ppc64le

```console
$ docker pull wordpress@sha256:61b7cc33a54f30488f7ea42ff4d14d7e42736354eb556641e1abb6a9dbbb4530
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51681573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44fa8e73f1b7f239237d32f6e4249fd2b5d3719f647ef1f97f776878c0501996`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:44 GMT
ADD file:d9267e5b7618ca1c5ac918cde29e6967fae2132ab0672112ee2c6604e96a0b66 in / 
# Fri, 10 Feb 2023 21:20:45 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 23:21:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 10 Feb 2023 23:21:16 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 10 Feb 2023 23:21:18 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 10 Feb 2023 23:21:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 10 Feb 2023 23:21:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 10 Feb 2023 23:21:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 10 Feb 2023 23:21:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 10 Feb 2023 23:21:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 11 Feb 2023 00:06:13 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 14 Feb 2023 22:07:47 GMT
ENV PHP_VERSION=8.0.28
# Tue, 14 Feb 2023 22:07:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Tue, 14 Feb 2023 22:07:48 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Tue, 14 Feb 2023 22:07:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 14 Feb 2023 22:07:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:12:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 14 Feb 2023 22:12:51 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:12:53 GMT
RUN docker-php-ext-enable sodium
# Tue, 14 Feb 2023 22:12:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 14 Feb 2023 22:12:54 GMT
CMD ["php" "-a"]
# Wed, 15 Feb 2023 04:01:36 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Wed, 15 Feb 2023 04:01:37 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Wed, 15 Feb 2023 04:01:38 GMT
WORKDIR /var/www/html
# Wed, 15 Feb 2023 04:03:10 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 15 Feb 2023 04:03:12 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 15 Feb 2023 04:03:13 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Wed, 15 Feb 2023 04:03:14 GMT
ENV WORDPRESS_CLI_VERSION=2.7.1
# Wed, 15 Feb 2023 04:03:15 GMT
ENV WORDPRESS_CLI_SHA512=956b5e3e1a076bd5441c082ee754e3ff4517ec965b93c621f455c2bf5719358c36e67d52f676492700b59d42cacb34a50d382535c035f19da7a0b98bc41860de
# Wed, 15 Feb 2023 04:03:19 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Wed, 15 Feb 2023 04:03:20 GMT
VOLUME [/var/www/html]
# Wed, 15 Feb 2023 04:03:21 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Wed, 15 Feb 2023 04:03:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Feb 2023 04:03:22 GMT
USER www-data
# Wed, 15 Feb 2023 04:03:22 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:e3b9153081a195877a8587137034c9b223749c582ea32371419055f7d77c97ba`  
		Last Modified: Fri, 10 Feb 2023 21:21:53 GMT  
		Size: 2.8 MB (2804628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77483b79fe489e3d1e457273e36c12fdbbfda2b9134aa1ed6c809edb4bc207c9`  
		Last Modified: Sat, 11 Feb 2023 00:30:19 GMT  
		Size: 1.8 MB (1772435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa4d9c93206a48a73541502538d2448b50970846318272100e6410859ee40e1`  
		Last Modified: Sat, 11 Feb 2023 00:30:19 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44eb343fe0eefc0c427b565973e982dbcf3c0991674564b7317125e6dbcaf69e`  
		Last Modified: Sat, 11 Feb 2023 00:30:19 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f681a6d5ac50e39a6bd72ca6bd10841dbd5c33073cda6a9c4bdb8f8b76c6d39`  
		Last Modified: Tue, 14 Feb 2023 22:41:50 GMT  
		Size: 10.8 MB (10821698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f11dabf855e505caf6b2af3d7e8525161a536df63ca4d1949eda3c58fa9b23d`  
		Last Modified: Tue, 14 Feb 2023 22:41:48 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285865f64b57f87449bb3ef45877d9695a6af08beae977e864544d870b30346e`  
		Last Modified: Tue, 14 Feb 2023 22:41:53 GMT  
		Size: 16.6 MB (16587533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86e27822668b3bf4fe0f8a4fee7de83052d900af4b96bd3c2d8432ece2ead8db`  
		Last Modified: Tue, 14 Feb 2023 22:41:48 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c96c419526537de24e6de90f5e82321099704c0717994251419afe6e10c0e41f`  
		Last Modified: Tue, 14 Feb 2023 22:41:48 GMT  
		Size: 18.7 KB (18660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f07d89f6f0262236cb4de60f0d1e6d0bb13cecd534207ad1c6e2f2bb8c7be3`  
		Last Modified: Wed, 15 Feb 2023 04:21:48 GMT  
		Size: 9.6 MB (9597261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd17a16a1a8272ef4e2bafefa0b5a7f9c84ade6a9f4527f5e58f0a91619d1da9`  
		Last Modified: Wed, 15 Feb 2023 04:21:43 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f1c1087183fb37c53863ce95ccf4830367c69b02c54393f19bf39d402fcde0e`  
		Last Modified: Wed, 15 Feb 2023 04:21:46 GMT  
		Size: 8.6 MB (8638801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30afc9a5895d912fecedbf045efbb7633f730ab0360b272a71c175afa8c1b1ad`  
		Last Modified: Wed, 15 Feb 2023 04:21:43 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23950befea3dd644235865ff730bed18f536af13855798287f50870da3d301df`  
		Last Modified: Wed, 15 Feb 2023 04:21:44 GMT  
		Size: 1.4 MB (1435137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a466a15babab2d39216b10f5c85d7f6259891932b362859b1a90d331416991`  
		Last Modified: Wed, 15 Feb 2023 04:21:43 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.7-php8.0` - linux; s390x

```console
$ docker pull wordpress@sha256:6c2534347133619606d25fd6ce1c761262c90f554a15918b091b3dcaa4443871
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.8 MB (49806725 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d135f3be233d27aa92591144a65b5a8a336ab999d85b595315c1fc0eab1ae565`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:31 GMT
ADD file:17af250b49631cf2acf655c85df90977eddab4c9afd67bda3c577db5200364f1 in / 
# Fri, 10 Feb 2023 21:41:32 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:49:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 11 Feb 2023 03:49:57 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 11 Feb 2023 03:49:57 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 03:49:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 11 Feb 2023 03:49:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 11 Feb 2023 03:49:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 03:49:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 11 Feb 2023 03:49:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 11 Feb 2023 04:20:16 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F 2C16C765DBE54A088130F1BC4B9B5F600B55F3B4
# Tue, 14 Feb 2023 22:01:44 GMT
ENV PHP_VERSION=8.0.28
# Tue, 14 Feb 2023 22:01:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.28.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.28.tar.xz.asc
# Tue, 14 Feb 2023 22:01:44 GMT
ENV PHP_SHA256=5e07278a1f315a67d36a676c01343ca2d4da5ec5bdb15d018e4248b3012bc0cd
# Tue, 14 Feb 2023 22:01:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 14 Feb 2023 22:01:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:04:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 14 Feb 2023 22:04:45 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Tue, 14 Feb 2023 22:04:46 GMT
RUN docker-php-ext-enable sodium
# Tue, 14 Feb 2023 22:04:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 14 Feb 2023 22:04:47 GMT
CMD ["php" "-a"]
# Wed, 15 Feb 2023 00:50:02 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Wed, 15 Feb 2023 00:50:03 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Wed, 15 Feb 2023 00:50:03 GMT
WORKDIR /var/www/html
# Wed, 15 Feb 2023 00:50:43 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 15 Feb 2023 00:50:44 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 15 Feb 2023 00:50:44 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Wed, 15 Feb 2023 00:50:44 GMT
ENV WORDPRESS_CLI_VERSION=2.7.1
# Wed, 15 Feb 2023 00:50:45 GMT
ENV WORDPRESS_CLI_SHA512=956b5e3e1a076bd5441c082ee754e3ff4517ec965b93c621f455c2bf5719358c36e67d52f676492700b59d42cacb34a50d382535c035f19da7a0b98bc41860de
# Wed, 15 Feb 2023 00:50:47 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Wed, 15 Feb 2023 00:50:47 GMT
VOLUME [/var/www/html]
# Wed, 15 Feb 2023 00:50:47 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Wed, 15 Feb 2023 00:50:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 15 Feb 2023 00:50:47 GMT
USER www-data
# Wed, 15 Feb 2023 00:50:47 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:667d93a24f321610e24486f3148545191f113ab9ab2444804087dd65ebbda9ed`  
		Last Modified: Fri, 10 Feb 2023 21:42:26 GMT  
		Size: 2.6 MB (2593581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:476a3a3fc00d505f146f9062bf162efa67799d1f39390acbac0a7a316be08a7c`  
		Last Modified: Sat, 11 Feb 2023 04:36:27 GMT  
		Size: 1.8 MB (1776052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:548ad0a6b1dee36843d375e2a426690db3337e78377cb2d8863a1848f9439897`  
		Last Modified: Sat, 11 Feb 2023 04:36:27 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdded828c248ae0d95503cd8211f9017f84d334e34aae9ecc47b64fbb554eacb`  
		Last Modified: Sat, 11 Feb 2023 04:36:27 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fa85a3a0f28ab377d9eed561422b2c4da584ff3ed45bd9ef0c796e9c3fcb36`  
		Last Modified: Tue, 14 Feb 2023 22:23:44 GMT  
		Size: 10.8 MB (10821697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70d9e6ed01ef59b2337d201dd18a0a37f43e6d17489ec8ef82e2be1e35f7ac7c`  
		Last Modified: Tue, 14 Feb 2023 22:23:44 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f978a95a2e3662f15cc14b8ba5ef01f6817f8a1055abac7012332d0401a80a46`  
		Last Modified: Tue, 14 Feb 2023 22:23:46 GMT  
		Size: 14.8 MB (14805461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:103bf2727296c29a37217ee85c4d2c0f773ad8e3480bc80804d347473711d53b`  
		Last Modified: Tue, 14 Feb 2023 22:23:44 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84b699229e10367224db7301ed27c9120db816b829c18043b5821c868051b605`  
		Last Modified: Tue, 14 Feb 2023 22:23:44 GMT  
		Size: 18.7 KB (18665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f46606604e4ef1cb1c3d8ace02497c5105357a4ab46c2a1f7a395652a52fdb2`  
		Last Modified: Wed, 15 Feb 2023 01:02:27 GMT  
		Size: 9.9 MB (9912989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa92d5f26a61b4631a86c8befabb902391b99311d28579b0543f5eec2c00280`  
		Last Modified: Wed, 15 Feb 2023 01:02:25 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad4d133687b28e0dd3212fe3d9aa24bbce7a02418b89ca8729a341f749b195b`  
		Last Modified: Wed, 15 Feb 2023 01:02:26 GMT  
		Size: 8.4 MB (8437739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04bcecfb2f0f361d3ac0d6baca40ff7d86b229cb85ded87791ba1184055cc7a7`  
		Last Modified: Wed, 15 Feb 2023 01:02:25 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d67a68eb084273acb47de7965009d9145f7d41aa6d80e8acf56f63e00e3f0e47`  
		Last Modified: Wed, 15 Feb 2023 01:02:25 GMT  
		Size: 1.4 MB (1435123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e7799a515be4a432bfb51b25f1c2b5f7750a7004e00af80c55c796666a14ed1`  
		Last Modified: Wed, 15 Feb 2023 01:02:25 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
