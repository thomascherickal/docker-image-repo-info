## `wordpress:cli-2.6.0-php8.1`

```console
$ docker pull wordpress@sha256:56c79913796064be9a28192808c53342188e4b30c7a92fd8cbe29c76f588c72b
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

### `wordpress:cli-2.6.0-php8.1` - linux; amd64

```console
$ docker pull wordpress@sha256:8b9445160e40b6fe97301fc5e18e803cf9d066b6a5e7dedc5e80b95c2d7e58bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (51992587 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b76b2163c576ef1d98ecc557bec5727287364cf5b578820fb7bb749ad6864d33`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 21:20:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 09 Aug 2022 21:20:18 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 09 Aug 2022 21:20:18 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 09 Aug 2022 21:20:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Aug 2022 21:20:19 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Aug 2022 21:20:19 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 21:20:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 21:20:19 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Aug 2022 21:45:12 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 01 Sep 2022 21:36:56 GMT
ENV PHP_VERSION=8.1.10
# Thu, 01 Sep 2022 21:36:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.10.tar.xz.asc
# Thu, 01 Sep 2022 21:36:56 GMT
ENV PHP_SHA256=90e7120c77ee83630e6ac928d23bc6396603d62d83a3cf5df8a450d2e3070162
# Thu, 01 Sep 2022 21:37:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Sep 2022 21:37:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Sep 2022 21:40:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Sep 2022 21:40:58 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 01 Sep 2022 21:40:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Sep 2022 21:40:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Sep 2022 21:41:00 GMT
CMD ["php" "-a"]
# Fri, 02 Sep 2022 01:01:16 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 02 Sep 2022 01:01:17 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 02 Sep 2022 01:01:17 GMT
WORKDIR /var/www/html
# Fri, 02 Sep 2022 01:02:12 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 02 Sep 2022 01:02:13 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 02 Sep 2022 01:02:13 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 02 Sep 2022 01:02:13 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Fri, 02 Sep 2022 01:02:13 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Fri, 02 Sep 2022 01:02:16 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 02 Sep 2022 01:02:16 GMT
VOLUME [/var/www/html]
# Fri, 02 Sep 2022 01:02:16 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 02 Sep 2022 01:02:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 01:02:16 GMT
USER www-data
# Fri, 02 Sep 2022 01:02:16 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a600fdbc30cc6501babd12a4b22d75316d5ae384a68b9b4c588bfba33109bbc0`  
		Last Modified: Tue, 09 Aug 2022 23:00:27 GMT  
		Size: 1.7 MB (1720948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cdd6cb15c0d57bb696f4a1a47b41374e78a6a5f1cdd24c45d8b9655b52caa40`  
		Last Modified: Tue, 09 Aug 2022 23:00:26 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c40d8aee7b41f415744811ec585376e2f7798b79ac68e04b7127fb847d566`  
		Last Modified: Tue, 09 Aug 2022 23:00:26 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5febe94aae23128deeea3264b57631dee36170e7306e78b31fe5b108ec91441`  
		Last Modified: Thu, 01 Sep 2022 23:02:35 GMT  
		Size: 11.8 MB (11756460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1451319437ef5a71008abe5fe027beb5da19b24c450c13278c9a6186c01f376`  
		Last Modified: Thu, 01 Sep 2022 23:02:34 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebbdb48e518042c94cd1c3b63e428323cdbf8a110b7c4f29c9f0689088757792`  
		Last Modified: Thu, 01 Sep 2022 23:02:37 GMT  
		Size: 16.5 MB (16509882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93507073674d41bec3607cf4a7f5b3a5e5f570795407ebdba8589a492d91acf4`  
		Last Modified: Thu, 01 Sep 2022 23:02:34 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba004a55078fd14193da3f396f2b873e66f58ebe3b19ee79b16d3f5c1235fcb7`  
		Last Modified: Thu, 01 Sep 2022 23:02:34 GMT  
		Size: 18.9 KB (18888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8a14fa632b02bc31767089b47957eee03e6b51ee8851387186c091fee1f6a0`  
		Last Modified: Fri, 02 Sep 2022 01:07:09 GMT  
		Size: 9.4 MB (9372753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b148a163fab9762b24899e84e85220fd8ccb15f678cb3e0839dd2697f111164`  
		Last Modified: Fri, 02 Sep 2022 01:07:05 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa7afa54a4d443564344b6dc398ef332a7b3d03ab64c4f192e9258f884ba982`  
		Last Modified: Fri, 02 Sep 2022 01:07:06 GMT  
		Size: 8.4 MB (8418459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:732eb6c1b2f40c65655d12cb61052749bf47f813b994dc9de3e4251236e5f125`  
		Last Modified: Fri, 02 Sep 2022 01:07:05 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6203d1e67d0eb31014285b95851ebdeb1f768c9ab88545a70274bfab973c7d73`  
		Last Modified: Fri, 02 Sep 2022 01:07:05 GMT  
		Size: 1.4 MB (1383726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bdc968506786d31875e510d2ea49c6bd3b2239ddd4910e7115e1887dc4bfc13`  
		Last Modified: Fri, 02 Sep 2022 01:07:05 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.6.0-php8.1` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:842ba913c665544a7350193720ce02fd8cd1308974b8b335d4de8abc25bdee40
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49323277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f308e7e1c9897ce7948fe4adfda2d7b7e361ef6c1a37ec0cac68fd624cb6cc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 11:16:54 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 10 Aug 2022 11:16:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 10 Aug 2022 11:16:56 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 10 Aug 2022 11:16:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 10 Aug 2022 11:16:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 10 Aug 2022 11:16:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 11:16:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 11:16:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 10 Aug 2022 12:37:11 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 10 Aug 2022 12:37:11 GMT
ENV PHP_VERSION=8.1.9
# Wed, 10 Aug 2022 12:37:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.9.tar.xz.asc
# Wed, 10 Aug 2022 12:37:11 GMT
ENV PHP_SHA256=53477e73e6254dc942b68913a58d815ffdbf6946baf61a1f8ef854de524c27bf
# Wed, 10 Aug 2022 12:37:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 10 Aug 2022 12:37:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 10 Aug 2022 12:50:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 10 Aug 2022 12:50:46 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Wed, 10 Aug 2022 12:50:47 GMT
RUN docker-php-ext-enable sodium
# Wed, 10 Aug 2022 12:50:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 10 Aug 2022 12:50:48 GMT
CMD ["php" "-a"]
# Thu, 11 Aug 2022 02:54:07 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 11 Aug 2022 02:54:08 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 11 Aug 2022 02:54:08 GMT
WORKDIR /var/www/html
# Thu, 11 Aug 2022 02:56:02 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 11 Aug 2022 02:56:03 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 11 Aug 2022 02:56:03 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 11 Aug 2022 02:56:03 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Thu, 11 Aug 2022 02:56:03 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Thu, 11 Aug 2022 02:56:07 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 11 Aug 2022 02:56:07 GMT
VOLUME [/var/www/html]
# Thu, 11 Aug 2022 02:56:07 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 11 Aug 2022 02:56:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 02:56:07 GMT
USER www-data
# Thu, 11 Aug 2022 02:56:07 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b6fa03280302058f33539e036c049c26e6b1f95d1306b571a247717725212b5`  
		Last Modified: Wed, 10 Aug 2022 16:20:51 GMT  
		Size: 1.7 MB (1707962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91a0a3e2190be4d464337d2b34ae250925d898b9100464d1528683a35ea7b54d`  
		Last Modified: Wed, 10 Aug 2022 16:20:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1efb22106c208d7e172696b03b8551465117d04b728caffe704132bdf3246185`  
		Last Modified: Wed, 10 Aug 2022 16:20:50 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c9320e3c0294df7ba17e8f824566691137433187d374a9cd83068c0a34fe3b`  
		Last Modified: Wed, 10 Aug 2022 16:23:12 GMT  
		Size: 11.8 MB (11808421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50718650792e4eb3fa17bdb3b1dbbe9f7ac0e4fa29d2f8dc699626b8ecf17a29`  
		Last Modified: Wed, 10 Aug 2022 16:23:11 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e7777cbf9e275a60219c30bcd59e8b02d77f00b5d230810e7c54b38610e9ef`  
		Last Modified: Wed, 10 Aug 2022 16:23:15 GMT  
		Size: 14.8 MB (14819532 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea2b2f2adcbc9e94638640d63b5f8642cfc02c9970380a7c09adca5171d92d8`  
		Last Modified: Wed, 10 Aug 2022 16:23:10 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e25fa814c75b62dc054d0d3e277933f3bfa403efe24aa8a5b3ef597dcab38488`  
		Last Modified: Wed, 10 Aug 2022 16:23:10 GMT  
		Size: 18.6 KB (18626 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e32de9856240d3e1df2cc8c091ac843fc3e3bb1a16bd5caf15225be9b292f921`  
		Last Modified: Thu, 11 Aug 2022 03:01:02 GMT  
		Size: 9.0 MB (8973935 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64c56349c8ef1e2d4846965585034e1f9a3c9536dc9871a811f8a4f7fd96532`  
		Last Modified: Thu, 11 Aug 2022 03:00:57 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f188d016dcc3731d99671b5225448083f97e8c3916213b503daa92e704988d97`  
		Last Modified: Thu, 11 Aug 2022 03:01:00 GMT  
		Size: 8.0 MB (7991759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cddb0bf965cce9d0e13d0910c1ad60689a5239d117ee80542fc00473a07bf49`  
		Last Modified: Thu, 11 Aug 2022 03:00:57 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b596fbe29a155e3fdff496a4412988b01b28905e071e0cb8971937d0c15a9eea`  
		Last Modified: Thu, 11 Aug 2022 03:00:58 GMT  
		Size: 1.4 MB (1383665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aace507282a4f9b173e7f370c6168ef7f7eca98b8df5865278aacb61483f8cbc`  
		Last Modified: Thu, 11 Aug 2022 03:00:57 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.6.0-php8.1` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:9db76d71966a385ead1221dc6dca33da5961cdfa407030866fb24f2d29f4bbe6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.3 MB (47261532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce06803db5abd7159efe66a515b5a9f19606f29ba29822e0dbd62180ea3e1b51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 14:13:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 10 Aug 2022 14:13:14 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 10 Aug 2022 14:13:15 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 10 Aug 2022 14:13:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 10 Aug 2022 14:13:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 10 Aug 2022 14:13:16 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 14:13:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 14:13:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 10 Aug 2022 15:33:03 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 10 Aug 2022 15:33:04 GMT
ENV PHP_VERSION=8.1.9
# Wed, 10 Aug 2022 15:33:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.9.tar.xz.asc
# Wed, 10 Aug 2022 15:33:04 GMT
ENV PHP_SHA256=53477e73e6254dc942b68913a58d815ffdbf6946baf61a1f8ef854de524c27bf
# Wed, 10 Aug 2022 15:33:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 10 Aug 2022 15:33:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 10 Aug 2022 15:45:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 10 Aug 2022 15:45:58 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Wed, 10 Aug 2022 15:45:59 GMT
RUN docker-php-ext-enable sodium
# Wed, 10 Aug 2022 15:45:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 10 Aug 2022 15:45:59 GMT
CMD ["php" "-a"]
# Thu, 11 Aug 2022 06:40:26 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 11 Aug 2022 06:40:26 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 11 Aug 2022 06:40:26 GMT
WORKDIR /var/www/html
# Thu, 11 Aug 2022 06:41:36 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 11 Aug 2022 06:41:36 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 11 Aug 2022 06:41:36 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 11 Aug 2022 06:41:36 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Thu, 11 Aug 2022 06:41:36 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Thu, 11 Aug 2022 06:41:39 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 11 Aug 2022 06:41:39 GMT
VOLUME [/var/www/html]
# Thu, 11 Aug 2022 06:41:39 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 11 Aug 2022 06:41:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 11 Aug 2022 06:41:39 GMT
USER www-data
# Thu, 11 Aug 2022 06:41:39 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533661cc695e850f2ce9a61f8d6bcabf20631bc4be493498e7c06a85445a834d`  
		Last Modified: Wed, 10 Aug 2022 19:17:39 GMT  
		Size: 1.6 MB (1575470 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83ea8309925b47b4d8ed5708b410d6856267d8d8dea3544802ae2a6d8e16e2a5`  
		Last Modified: Wed, 10 Aug 2022 19:17:38 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a23ce236c2c67c8bab1a6d9e5111a49299c4b7a07b9914b84c845eb1ff3c3ab`  
		Last Modified: Wed, 10 Aug 2022 19:17:38 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e88debab293da40fab9f56bfa8bf80658cd4ed36a849f654206d4747e7b3196c`  
		Last Modified: Wed, 10 Aug 2022 19:20:48 GMT  
		Size: 11.8 MB (11808410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa74bbff85b060c5693d688a59be345ec72a9f62a43ab9ff210e4ceda3f5a96`  
		Last Modified: Wed, 10 Aug 2022 19:20:47 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e39d65bf3058634db2875014dab9687caae7942aa141c506ee063d98a222a98`  
		Last Modified: Wed, 10 Aug 2022 19:20:51 GMT  
		Size: 13.9 MB (13888902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d13833d9435e8524ea8db27296de79bc37cbc154a02d2bb2d27ae5b9bd93bede`  
		Last Modified: Wed, 10 Aug 2022 19:20:46 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0642507a46f8f3ca3b3884f6eb775becef39aa7ef03ec61482ec40cef8b6806f`  
		Last Modified: Wed, 10 Aug 2022 19:20:46 GMT  
		Size: 18.6 KB (18604 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a339dacb948065c8852f2cc7ebf325f1fee4432fbfb1e1607cf62e0f7a57c2c`  
		Last Modified: Thu, 11 Aug 2022 06:48:25 GMT  
		Size: 8.7 MB (8677827 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6254327da3c1cf2df9ac82a766d2ab86c277767d53dfcef6e084add4f8aee8`  
		Last Modified: Thu, 11 Aug 2022 06:48:21 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecf65f5ad6fba2eb0b4fdf2c82b69df0619e308e8a1c9eeed4ea2437eb931bda`  
		Last Modified: Thu, 11 Aug 2022 06:48:22 GMT  
		Size: 7.5 MB (7486186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f795c2abaedfcdc5137353f5f7504c144da52986766636ee0633d239a7e921`  
		Last Modified: Thu, 11 Aug 2022 06:48:21 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91243f438b67d536887f897d42cc18f660a7fed5d035288a923f337e667861a6`  
		Last Modified: Thu, 11 Aug 2022 06:48:21 GMT  
		Size: 1.4 MB (1383648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:791b0a4321c44afe8f108c6ae7e5658d3bfe9d35a37bcd448be7bc44a28e96ec`  
		Last Modified: Thu, 11 Aug 2022 06:48:21 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.6.0-php8.1` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:17c4af9d9d20d1ff4e66f1810bee6be4e6eff02089ce24ad377fdd6286b7f122
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51533567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc429221e15be5d94c5fb94be6c6c70c1eb2c3f3f06ec63008291455de7433ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Wed, 10 Aug 2022 00:03:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 10 Aug 2022 00:03:59 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 10 Aug 2022 00:04:00 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 10 Aug 2022 00:04:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 10 Aug 2022 00:04:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 10 Aug 2022 00:04:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 00:04:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 10 Aug 2022 00:04:05 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 10 Aug 2022 00:40:57 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 10 Aug 2022 00:40:58 GMT
ENV PHP_VERSION=8.1.9
# Wed, 10 Aug 2022 00:40:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.9.tar.xz.asc
# Wed, 10 Aug 2022 00:41:00 GMT
ENV PHP_SHA256=53477e73e6254dc942b68913a58d815ffdbf6946baf61a1f8ef854de524c27bf
# Wed, 10 Aug 2022 00:41:06 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 10 Aug 2022 00:41:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 10 Aug 2022 00:46:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 10 Aug 2022 00:46:57 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Wed, 10 Aug 2022 00:46:58 GMT
RUN docker-php-ext-enable sodium
# Wed, 10 Aug 2022 00:46:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 10 Aug 2022 00:47:00 GMT
CMD ["php" "-a"]
# Wed, 10 Aug 2022 08:51:37 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Wed, 10 Aug 2022 08:51:38 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Wed, 10 Aug 2022 08:51:39 GMT
WORKDIR /var/www/html
# Wed, 10 Aug 2022 08:52:39 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 10 Aug 2022 08:52:39 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 10 Aug 2022 08:52:40 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Wed, 10 Aug 2022 08:52:41 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Wed, 10 Aug 2022 08:52:42 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Wed, 10 Aug 2022 08:52:45 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Wed, 10 Aug 2022 08:52:46 GMT
VOLUME [/var/www/html]
# Wed, 10 Aug 2022 08:52:48 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Wed, 10 Aug 2022 08:52:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 10 Aug 2022 08:52:49 GMT
USER www-data
# Wed, 10 Aug 2022 08:52:50 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2451bb80cc25fd19497adebf3450060e0befb8338668e6f8f8997c1cdbfa8449`  
		Last Modified: Wed, 10 Aug 2022 02:14:32 GMT  
		Size: 1.7 MB (1715287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8596f4ed07f5a52b53624b796113b36143107921db4f999141aeaf08e9726c`  
		Last Modified: Wed, 10 Aug 2022 02:14:32 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:753cf0136f4270e91e1fcba1ad4b3a086700d0092f3fd518f573ee69444de99d`  
		Last Modified: Wed, 10 Aug 2022 02:14:32 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90f2f867414db8448db21467c96957c89da1f3cc0e70d78d901e0209ba824bc`  
		Last Modified: Wed, 10 Aug 2022 02:17:09 GMT  
		Size: 11.8 MB (11808189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4895f3961c0f3c07c21e0e9309f9c634ec6caaf38c89824c5aa8189b9798ad8`  
		Last Modified: Wed, 10 Aug 2022 02:17:08 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:660af490c100fe66c521494ca22b1b0a261baf582afd1c4c5f96ac7df5dd439b`  
		Last Modified: Wed, 10 Aug 2022 02:17:11 GMT  
		Size: 16.2 MB (16233732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffefe6567dfdccb1792dab6cfae072ea4618395f882541a66c66e9ec4c0a31d`  
		Last Modified: Wed, 10 Aug 2022 02:17:08 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc16c6dfeef0043a1e92dbfb3f9bbf19bc9e5f84a30bd6c89e94dc8507687e81`  
		Last Modified: Wed, 10 Aug 2022 02:17:08 GMT  
		Size: 18.5 KB (18544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a95e7256dd9e9dd0f93df1259a529e091c47b94fe199493ca3076fc5e659c3c7`  
		Last Modified: Wed, 10 Aug 2022 08:58:26 GMT  
		Size: 9.4 MB (9441972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84329100fa7f15626139958861ae9bf00e421ac12a8a5b4ef7dfa716c68d22b0`  
		Last Modified: Wed, 10 Aug 2022 08:58:26 GMT  
		Size: 8.2 MB (8219547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a3023f79588d4daa6f62a3637ea1a3a820c00bea22289a8ae725d5e6db881e9`  
		Last Modified: Wed, 10 Aug 2022 08:58:25 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907ec93c874384723dd0de6f754589114bcc99c69007b71cd5aeb8f721ba2b49`  
		Last Modified: Wed, 10 Aug 2022 08:58:25 GMT  
		Size: 1.4 MB (1383436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f50e3029ca50b4aa2cfaeb9df7bf50d9c9f86cde6225528c464d2ec1d4e9364b`  
		Last Modified: Wed, 10 Aug 2022 08:58:24 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.6.0-php8.1` - linux; 386

```console
$ docker pull wordpress@sha256:1ea28e96bb2a8608cb7da2a252146549b106753656c2da5309bf59b6c83eca30
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53024331 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d245e0c30b19d232a29d63bf8275445400727ddf5ebbe247ba3abadc89631bc6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 18:56:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 09 Aug 2022 18:56:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 09 Aug 2022 18:56:28 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 09 Aug 2022 18:56:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Aug 2022 18:56:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Aug 2022 18:56:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 18:56:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 18:56:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Aug 2022 19:21:40 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 01 Sep 2022 21:52:47 GMT
ENV PHP_VERSION=8.1.10
# Thu, 01 Sep 2022 21:52:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.10.tar.xz.asc
# Thu, 01 Sep 2022 21:52:49 GMT
ENV PHP_SHA256=90e7120c77ee83630e6ac928d23bc6396603d62d83a3cf5df8a450d2e3070162
# Thu, 01 Sep 2022 21:52:56 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Sep 2022 21:52:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Sep 2022 21:56:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Sep 2022 21:56:52 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 01 Sep 2022 21:56:52 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Sep 2022 21:56:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Sep 2022 21:56:54 GMT
CMD ["php" "-a"]
# Fri, 02 Sep 2022 02:16:02 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 02 Sep 2022 02:16:02 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 02 Sep 2022 02:16:03 GMT
WORKDIR /var/www/html
# Fri, 02 Sep 2022 02:16:57 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 02 Sep 2022 02:16:58 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 02 Sep 2022 02:16:59 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 02 Sep 2022 02:17:00 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Fri, 02 Sep 2022 02:17:01 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Fri, 02 Sep 2022 02:17:04 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 02 Sep 2022 02:17:05 GMT
VOLUME [/var/www/html]
# Fri, 02 Sep 2022 02:17:07 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:17:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:17:08 GMT
USER www-data
# Fri, 02 Sep 2022 02:17:09 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458a15900474f3d2d2c9944341ff070dc1daf50815820580bd21463737a6c55a`  
		Last Modified: Tue, 09 Aug 2022 20:41:11 GMT  
		Size: 1.8 MB (1820367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40080bc9e2b22eebc8070ba53b95939ccd7e292319817fbcd98639a046e4da31`  
		Last Modified: Tue, 09 Aug 2022 20:41:11 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51e6830783d889ccc83e35eab559566fe80ed99bf0d67035474ed38e5ddc7b02`  
		Last Modified: Tue, 09 Aug 2022 20:41:10 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91e71f8aec85890ea2fbca71b07a124625fee18f6a92d9f765686d5aa71ef791`  
		Last Modified: Thu, 01 Sep 2022 23:23:34 GMT  
		Size: 11.8 MB (11756217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e9b262f52d4751c7b54d10e3502791fc8f44c2f353fbc2ac19e1359bf3acc2`  
		Last Modified: Thu, 01 Sep 2022 23:23:32 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa4536e1bd9646ec1f179d2e82171b9f90adac6dc0919ffa85304f9054f6f4a2`  
		Last Modified: Thu, 01 Sep 2022 23:23:35 GMT  
		Size: 16.9 MB (16923678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc41653e868a4732d428b96975b93a6d5b4a465c9995b60e2f014ce5c34ea4d3`  
		Last Modified: Thu, 01 Sep 2022 23:23:32 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f1967e9d39c7e2c9dd0ba3077b13fa2626aa88a150a696bff4ba509321687b`  
		Last Modified: Thu, 01 Sep 2022 23:23:33 GMT  
		Size: 18.8 KB (18781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1865674385e812d979e826e25160d168ded0e7c7672bcb0de75d22404ddba019`  
		Last Modified: Fri, 02 Sep 2022 02:24:12 GMT  
		Size: 9.5 MB (9519615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15deea5827cb7d7676a7f285432f5ce330ed6af8a3bc2335fd3554b8caff56f3`  
		Last Modified: Fri, 02 Sep 2022 02:24:12 GMT  
		Size: 8.8 MB (8789882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04dc57c7663f2e80b366759e28630d8b4aeb1f40e649c0bb937ba6b4e9c9a745`  
		Last Modified: Fri, 02 Sep 2022 02:24:10 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:336a0c54d21ac644b4c0bd24887da96903d991c9fb7cce6aa8a1b906013bfefd`  
		Last Modified: Fri, 02 Sep 2022 02:24:11 GMT  
		Size: 1.4 MB (1383468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4c3f50f3cfc103a68f1a35ef2511300079e9ef72b9fbe91d692f7eecb34119`  
		Last Modified: Fri, 02 Sep 2022 02:24:11 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.6.0-php8.1` - linux; ppc64le

```console
$ docker pull wordpress@sha256:15aa018e48976e5e7e2a3ea9d024774a3236f94e20285288dfdfa51b2ec9a95f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (53025830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4644d8de85715cf034d155ce273f2ff8e413d293f44a3cdfaa86dd13a8e86659`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 19:38:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 09 Aug 2022 19:38:12 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 09 Aug 2022 19:38:13 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 09 Aug 2022 19:38:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Aug 2022 19:38:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Aug 2022 19:38:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 19:38:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 19:38:16 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Aug 2022 20:12:55 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 01 Sep 2022 21:22:42 GMT
ENV PHP_VERSION=8.1.10
# Thu, 01 Sep 2022 21:22:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.10.tar.xz.asc
# Thu, 01 Sep 2022 21:22:43 GMT
ENV PHP_SHA256=90e7120c77ee83630e6ac928d23bc6396603d62d83a3cf5df8a450d2e3070162
# Thu, 01 Sep 2022 21:22:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Sep 2022 21:22:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Sep 2022 21:27:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Sep 2022 21:27:44 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 01 Sep 2022 21:27:46 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Sep 2022 21:27:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Sep 2022 21:27:46 GMT
CMD ["php" "-a"]
# Fri, 02 Sep 2022 02:51:55 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 02 Sep 2022 02:51:57 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 02 Sep 2022 02:51:57 GMT
WORKDIR /var/www/html
# Fri, 02 Sep 2022 02:53:30 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 02 Sep 2022 02:53:32 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 02 Sep 2022 02:53:32 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 02 Sep 2022 02:53:33 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Fri, 02 Sep 2022 02:53:33 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Fri, 02 Sep 2022 02:53:37 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 02 Sep 2022 02:53:37 GMT
VOLUME [/var/www/html]
# Fri, 02 Sep 2022 02:53:38 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 02 Sep 2022 02:53:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 02:53:38 GMT
USER www-data
# Fri, 02 Sep 2022 02:53:39 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b19bea03a0d19d92d9affb999a9d6e5bddf7ccb99ced434a118735e98eda42`  
		Last Modified: Tue, 09 Aug 2022 21:56:16 GMT  
		Size: 1.8 MB (1772201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f9859feb1e3bcc24ef58fc12055cdbc53accb9d3c77721c61161ec83fd7cfb6`  
		Last Modified: Tue, 09 Aug 2022 21:56:15 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c00a2acb11c8adb08413d315161b5e31709b25d4a157a151371861eaca20fd9`  
		Last Modified: Tue, 09 Aug 2022 21:56:15 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786985e6455c288dc0b76ed3a604e41d5e42005329c3e79cdd22c88392d2767b`  
		Last Modified: Thu, 01 Sep 2022 22:56:51 GMT  
		Size: 11.8 MB (11756462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc8de333e3faff4a5ebfe5e379340ebaa839090dbe6981096dede5bfa268c712`  
		Last Modified: Thu, 01 Sep 2022 22:56:50 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4948c3aa1be8ffb39d1e4711c3a3b560eca9085ef3d5a6a25cfb0f16f457e75`  
		Last Modified: Thu, 01 Sep 2022 22:56:55 GMT  
		Size: 17.1 MB (17060357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179923961aa150c3512b0fb93fdfa468e1c65d8df77527c1ef9263b86c356f3f`  
		Last Modified: Thu, 01 Sep 2022 22:56:50 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc9c499a598999944a4aeb8011abd5c5d4f278db87e315ff54c215a97939de1a`  
		Last Modified: Thu, 01 Sep 2022 22:56:50 GMT  
		Size: 18.6 KB (18629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e647e6d6af56137f361a68469798acabecdaa7eb40626c84068f29a71cb32a89`  
		Last Modified: Fri, 02 Sep 2022 03:01:28 GMT  
		Size: 9.6 MB (9577815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ce29c86017c1472ef3a7d204d1ecaf64b3940750026b2bc181c4a33aaa4b68`  
		Last Modified: Fri, 02 Sep 2022 03:01:22 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c893fd8be13a14eb3e14ae81e06fa846567f61c343c0ab6d55cfec113154ea74`  
		Last Modified: Fri, 02 Sep 2022 03:01:25 GMT  
		Size: 8.6 MB (8647941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c3c43ed9a2a919688e77d339b8015d1174bb661c08cd88353b16004b32a8365`  
		Last Modified: Fri, 02 Sep 2022 03:01:22 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a53272e2f17e2effe9ed355ce82f39d825dda2462a5e6c68aa47f9745af14709`  
		Last Modified: Fri, 02 Sep 2022 03:01:23 GMT  
		Size: 1.4 MB (1383676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:921d09abac098f7f12f094bf0ad2efc30f9ff7ef7eeb43e11d5f664e31d2a723`  
		Last Modified: Fri, 02 Sep 2022 03:01:22 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.6.0-php8.1` - linux; s390x

```console
$ docker pull wordpress@sha256:6e2bb58b6bb0430e7de5b529c29362aa17b56722ba002ac873f7778c1f4e8032
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.4 MB (51359240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32a61d14a31efaddf0004fd11e8bca5918237d6501ef975b3a5269ad1f54ccf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 23:13:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 09 Aug 2022 23:13:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 09 Aug 2022 23:13:52 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 09 Aug 2022 23:13:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 09 Aug 2022 23:13:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 09 Aug 2022 23:13:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 23:13:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 09 Aug 2022 23:13:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 09 Aug 2022 23:51:00 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 01 Sep 2022 21:30:50 GMT
ENV PHP_VERSION=8.1.10
# Thu, 01 Sep 2022 21:30:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.10.tar.xz.asc
# Thu, 01 Sep 2022 21:30:51 GMT
ENV PHP_SHA256=90e7120c77ee83630e6ac928d23bc6396603d62d83a3cf5df8a450d2e3070162
# Thu, 01 Sep 2022 21:30:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Sep 2022 21:30:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Sep 2022 21:34:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Sep 2022 21:34:10 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 01 Sep 2022 21:34:11 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Sep 2022 21:34:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Sep 2022 21:34:11 GMT
CMD ["php" "-a"]
# Fri, 02 Sep 2022 00:35:24 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 02 Sep 2022 00:35:25 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 02 Sep 2022 00:35:25 GMT
WORKDIR /var/www/html
# Fri, 02 Sep 2022 00:36:13 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 02 Sep 2022 00:36:14 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 02 Sep 2022 00:36:14 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 02 Sep 2022 00:36:15 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Fri, 02 Sep 2022 00:36:15 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Fri, 02 Sep 2022 00:36:17 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 02 Sep 2022 00:36:18 GMT
VOLUME [/var/www/html]
# Fri, 02 Sep 2022 00:36:18 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 02 Sep 2022 00:36:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 02 Sep 2022 00:36:18 GMT
USER www-data
# Fri, 02 Sep 2022 00:36:18 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7c93f21d9f546f68476c05adafca1709482765850b132881bc932f21c2c4a22`  
		Last Modified: Wed, 10 Aug 2022 01:11:20 GMT  
		Size: 1.8 MB (1775799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3435c93d9a06d643ccde0e4d6a2f2e1352451f34309ec4c24470974d6ed10d7`  
		Last Modified: Wed, 10 Aug 2022 01:11:20 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe8bd3886087a99fec0c70835271597facb70fc1e142318fef69263a4b277d4`  
		Last Modified: Wed, 10 Aug 2022 01:11:20 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e6ba3225f0df7df1f424c5d2034376ca7e0f7673acf1ed3ee3bcfcbf68d1d7d`  
		Last Modified: Thu, 01 Sep 2022 22:37:29 GMT  
		Size: 11.8 MB (11756472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75592979d90ee95101846c9d31e0ccfaf16bfda3a3c2b6022e586735b7dea89a`  
		Last Modified: Thu, 01 Sep 2022 22:37:29 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c64440f756f18fb890b0d4748d7c781a4e7f9fca5747d8adec450e698bbddf5`  
		Last Modified: Thu, 01 Sep 2022 22:37:32 GMT  
		Size: 15.5 MB (15474578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad54176f717c0b3d96d413f06e3f75f298dbf165094286ded3b70b40c5273c9d`  
		Last Modified: Thu, 01 Sep 2022 22:37:29 GMT  
		Size: 2.4 KB (2445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a7bedc5106468eeda7e018afb0c45f9524a13c2f7b986c976a4953efe867ea9`  
		Last Modified: Thu, 01 Sep 2022 22:37:29 GMT  
		Size: 18.7 KB (18688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81cbae3bb86f497e65fa551ff59e3db65fd0469012938997bbac0de9a9c05aad`  
		Last Modified: Fri, 02 Sep 2022 00:41:39 GMT  
		Size: 9.9 MB (9913459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733b47c8ecf31b255d5f55bc3f69a400de3962b8813579fcd10040b84650cc76`  
		Last Modified: Fri, 02 Sep 2022 00:41:36 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c730b27f2ac8dbc857160725f9a31227c412af75e6e9e8667c9ca22769cd6bbf`  
		Last Modified: Fri, 02 Sep 2022 00:41:38 GMT  
		Size: 8.4 MB (8440504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb22f52a8d359ecc89db3f977fc0f90b18838807c21f5f9da0ed1704789ee382`  
		Last Modified: Fri, 02 Sep 2022 00:41:36 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9087ac546bda098beb2b5c09cf75f2d932bd826808a9ad0deb5519eb8829d71`  
		Last Modified: Fri, 02 Sep 2022 00:41:36 GMT  
		Size: 1.4 MB (1383724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffabb7f31b1a87d161e271f48bc76c7dc4eae4fc4f77d811b267fe002c277249`  
		Last Modified: Fri, 02 Sep 2022 00:41:36 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
