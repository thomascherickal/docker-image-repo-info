## `wordpress:cli-2-php8.1`

```console
$ docker pull wordpress@sha256:b2359b4f6d6a5136260290fc1df8176f112974cab7975ed2c26e3adc505f9173
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

### `wordpress:cli-2-php8.1` - linux; amd64

```console
$ docker pull wordpress@sha256:e21b1cb0f19591ed135664867fd34bc8932c12a269280caf22433a2968e5df0c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51747394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94d4a97a339c96fbb292cb8e0f399d322f2fd13b90e032a8675e12938afcee16`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 00:27:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 19 Jul 2022 00:27:06 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 19 Jul 2022 00:27:06 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 19 Jul 2022 00:27:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 19 Jul 2022 00:27:07 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 19 Jul 2022 00:27:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 19 Jul 2022 00:27:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 19 Jul 2022 00:27:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 19 Jul 2022 00:41:27 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 04 Aug 2022 21:27:53 GMT
ENV PHP_VERSION=8.1.9
# Thu, 04 Aug 2022 21:27:53 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.9.tar.xz.asc
# Thu, 04 Aug 2022 21:27:53 GMT
ENV PHP_SHA256=53477e73e6254dc942b68913a58d815ffdbf6946baf61a1f8ef854de524c27bf
# Thu, 04 Aug 2022 21:28:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 04 Aug 2022 21:28:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:32:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Aug 2022 21:32:05 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:32:06 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Aug 2022 21:32:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Aug 2022 21:32:06 GMT
CMD ["php" "-a"]
# Fri, 05 Aug 2022 01:56:38 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 05 Aug 2022 01:56:39 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 05 Aug 2022 01:56:39 GMT
WORKDIR /var/www/html
# Fri, 05 Aug 2022 01:57:35 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 05 Aug 2022 01:57:35 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 05 Aug 2022 01:57:35 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 05 Aug 2022 01:57:36 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Fri, 05 Aug 2022 01:57:36 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Fri, 05 Aug 2022 01:57:38 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 05 Aug 2022 01:57:38 GMT
VOLUME [/var/www/html]
# Fri, 05 Aug 2022 01:57:38 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 05 Aug 2022 01:57:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Aug 2022 01:57:39 GMT
USER www-data
# Fri, 05 Aug 2022 01:57:39 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cfb8455962e8dee2ec89d1aca6167797ee8fb124669b4f37e54aa82accbd11`  
		Last Modified: Tue, 19 Jul 2022 01:26:20 GMT  
		Size: 1.7 MB (1705561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72bc08afeabf24400f8800b72194e328506b82a27cefb34b8b9f573393b8bc2`  
		Last Modified: Tue, 19 Jul 2022 01:26:19 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb7a732550aeef70ff8ae6f2fdc1f988da20f7adbd4fa74770ad6e4f15be150`  
		Last Modified: Tue, 19 Jul 2022 01:26:20 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42fa8815d7481479d2139a7775c2e32c15ad1d8c114d74047dfc64223c4a9dbd`  
		Last Modified: Thu, 04 Aug 2022 22:56:16 GMT  
		Size: 11.8 MB (11808237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7bffe2121e9a86a4a4fedebac9daf544451bf86a3853a54d8109074f1409d4`  
		Last Modified: Thu, 04 Aug 2022 22:56:15 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7abc157d5cebc11d64341f89485cc221cbbbf10d09bb24704fb15b1c5c2bb783`  
		Last Modified: Thu, 04 Aug 2022 22:56:18 GMT  
		Size: 16.3 MB (16255226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68fbd7c363fda09cb85d86470aeaf7b65e7cb72e8695e3615ba1af6f474d2b52`  
		Last Modified: Thu, 04 Aug 2022 22:56:15 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee61ef7c349ca04029434a6c62cd0bc7c52f0194877d54033c987069bf88361d`  
		Last Modified: Thu, 04 Aug 2022 22:56:15 GMT  
		Size: 18.6 KB (18553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef249b8417f024a93f4559d76e1678e95e57dc354bb3e5ad613c5ce970fa40e`  
		Last Modified: Fri, 05 Aug 2022 01:59:06 GMT  
		Size: 9.4 MB (9353971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa1a4e0e708ff49df1f6e809563a7a348e43c4d1585a0410aab9efe847a1f639`  
		Last Modified: Fri, 05 Aug 2022 01:59:02 GMT  
		Size: 148.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf628660f5dfa9fef8f3c3c06358331b2f56851069df50b0a3f0728550424bc7`  
		Last Modified: Fri, 05 Aug 2022 01:59:04 GMT  
		Size: 8.4 MB (8418316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08f4912428030adeaa12577181b2541c1462a474c547702efac9aa8a80fe5dfd`  
		Last Modified: Fri, 05 Aug 2022 01:59:02 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2287f4b388ad6e3b1a1b61baf00ff361c1533ff8c94135f084b1e01946a88668`  
		Last Modified: Fri, 05 Aug 2022 01:59:03 GMT  
		Size: 1.4 MB (1383299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:048c388055ac17b836fb1e8609603c5fbdbf2abcd02e1c75a8e8ca428045757d`  
		Last Modified: Fri, 05 Aug 2022 01:59:02 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php8.1` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:07b40e65944343a5159768d22fa408374c9c9e80246315a10d3e5a3df9384ed9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.2 MB (49234154 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a3195fcead778721928cce4bb5611d2225cb330aab02b65206c5eeadfad3455`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 02:54:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 19 Jul 2022 02:54:49 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 19 Jul 2022 02:54:51 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 19 Jul 2022 02:54:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 19 Jul 2022 02:54:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 19 Jul 2022 02:54:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 19 Jul 2022 02:54:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 19 Jul 2022 02:54:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 19 Jul 2022 03:11:25 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 19 Jul 2022 03:11:25 GMT
ENV PHP_VERSION=8.1.8
# Tue, 19 Jul 2022 03:11:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Tue, 19 Jul 2022 03:11:26 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Tue, 19 Jul 2022 03:11:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 19 Jul 2022 03:11:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Jul 2022 03:16:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Jul 2022 03:16:21 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Tue, 19 Jul 2022 03:16:24 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Jul 2022 03:16:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Jul 2022 03:16:25 GMT
CMD ["php" "-a"]
# Tue, 19 Jul 2022 06:49:54 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Tue, 19 Jul 2022 06:49:56 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Tue, 19 Jul 2022 06:49:56 GMT
WORKDIR /var/www/html
# Tue, 19 Jul 2022 06:52:23 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 19 Jul 2022 06:52:24 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 19 Jul 2022 06:52:25 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Tue, 19 Jul 2022 06:52:25 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Tue, 19 Jul 2022 06:52:26 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Tue, 19 Jul 2022 06:52:30 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Tue, 19 Jul 2022 06:52:31 GMT
VOLUME [/var/www/html]
# Tue, 19 Jul 2022 06:52:31 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Tue, 19 Jul 2022 06:52:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 06:52:32 GMT
USER www-data
# Tue, 19 Jul 2022 06:52:32 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3a20f98c3862e8b151953d654ed54191d3b27050e2581dffbfb6e8c9137978`  
		Last Modified: Tue, 19 Jul 2022 04:19:22 GMT  
		Size: 1.7 MB (1693959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2b70338f2368181e0f61f4907a974178bd8b93cdf93d44a432380e99c5d154`  
		Last Modified: Tue, 19 Jul 2022 04:19:21 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0a1e200dbbea4736643651e71bfdcf1414cc80f1047b39f7d6732be05ff46a`  
		Last Modified: Tue, 19 Jul 2022 04:19:21 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c86a4b66324dd8a8d3189a079ce234e0540689c04c6a406ac2800d4560f55e8`  
		Last Modified: Tue, 19 Jul 2022 04:21:13 GMT  
		Size: 11.7 MB (11742265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e850c19bf4b40f8278561c327494f60fd56758f3fbaa73866741cedf8c89eb91`  
		Last Modified: Tue, 19 Jul 2022 04:21:10 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b1c8b5f65e3ed16f1f74a3c9e56bd380d99ee4ea96612078608721c978f4a9`  
		Last Modified: Tue, 19 Jul 2022 04:21:21 GMT  
		Size: 14.8 MB (14818867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f078a5150b01d21e978cc3bd0d8cc4c156b95431e5f461e062126ac618100c5`  
		Last Modified: Tue, 19 Jul 2022 04:21:10 GMT  
		Size: 2.4 KB (2445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ea50ef2de5cad8530da8107b3b66f01a65bfddc1bec462bfe9dad88221a3f9`  
		Last Modified: Tue, 19 Jul 2022 04:21:10 GMT  
		Size: 18.4 KB (18376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2a6967b7ffb4b4cc7ba6ef29161824f455a2ccb7d1a48f5eae326c82b4d1df`  
		Last Modified: Tue, 19 Jul 2022 06:59:06 GMT  
		Size: 9.0 MB (8974019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb82f32f8725d7d31f82e5aa3d216eeef4d2cfd099eb65bd2022a78d5d9886c0`  
		Last Modified: Tue, 19 Jul 2022 06:58:58 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03abd6d3b523bdcf1970dce0619c841abe77df03b10894765c2888d6cf1ab769`  
		Last Modified: Tue, 19 Jul 2022 06:59:03 GMT  
		Size: 8.0 MB (7991519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53af236efc3fb62229814a1ff27b739a354ceac8a9f3accaf41a1ba78029ad90`  
		Last Modified: Tue, 19 Jul 2022 06:58:58 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59ca2d0a9273f7dae552e5aa5ae71afb71dab0e844d9e21b73aeb577f97d1601`  
		Last Modified: Tue, 19 Jul 2022 06:58:59 GMT  
		Size: 1.4 MB (1383310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb86341f2d003e1c4b28934ddee1b76eb968ca1879a24169c83f622dbf20e3d`  
		Last Modified: Tue, 19 Jul 2022 06:58:58 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php8.1` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:83584440c058e99e37c07a07b339a40396862b9dca8a16cf098325b4b8252920
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.2 MB (47190588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64c4cff0b480d94f0c966074c97adff715881a3a5cae28ce427d24f253b5f181`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Mon, 18 Jul 2022 21:24:47 GMT
ADD file:68590e866bc6db27ad54d23de7dd275d0389cb86e4e6291a1243fcc234f2f7a1 in / 
# Mon, 18 Jul 2022 21:24:47 GMT
CMD ["/bin/sh"]
# Tue, 02 Aug 2022 11:00:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 02 Aug 2022 11:00:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 02 Aug 2022 11:00:51 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 02 Aug 2022 11:00:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 11:00:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 11:00:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 11:00:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 11:00:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 13:31:26 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 02 Aug 2022 15:59:13 GMT
ENV PHP_VERSION=8.1.8
# Tue, 02 Aug 2022 15:59:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.8.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.8.tar.xz.asc
# Tue, 02 Aug 2022 15:59:13 GMT
ENV PHP_SHA256=04c065515bc347bc68e0bb1ac7182669a98a731e4a17727e5731650ad3d8de4c
# Tue, 02 Aug 2022 15:59:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 02 Aug 2022 15:59:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 02 Aug 2022 16:12:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 02 Aug 2022 16:12:05 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Tue, 02 Aug 2022 16:12:06 GMT
RUN docker-php-ext-enable sodium
# Tue, 02 Aug 2022 16:12:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 02 Aug 2022 16:12:07 GMT
CMD ["php" "-a"]
# Thu, 04 Aug 2022 12:35:59 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 04 Aug 2022 12:35:59 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 04 Aug 2022 12:35:59 GMT
WORKDIR /var/www/html
# Thu, 04 Aug 2022 12:37:11 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 04 Aug 2022 12:37:11 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 04 Aug 2022 12:37:11 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 04 Aug 2022 12:37:11 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Thu, 04 Aug 2022 12:37:11 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Thu, 04 Aug 2022 12:37:14 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 04 Aug 2022 12:37:14 GMT
VOLUME [/var/www/html]
# Thu, 04 Aug 2022 12:37:14 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 04 Aug 2022 12:37:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Aug 2022 12:37:14 GMT
USER www-data
# Thu, 04 Aug 2022 12:37:14 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:a6b45ace95f42a930d15c33679ab9c85d46019b7e73954cadc73bb9ba176509b`  
		Last Modified: Mon, 18 Jul 2022 19:08:56 GMT  
		Size: 2.4 MB (2412307 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee58ddb705eb7b64c145780f43f5387b1fbaab55cb4343097283ab20f962569`  
		Last Modified: Wed, 03 Aug 2022 00:59:41 GMT  
		Size: 1.6 MB (1575500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44b44fb7e50395cddc49eb6beec73d881ed98348d72f0ed16650e437cb540b1`  
		Last Modified: Wed, 03 Aug 2022 00:59:40 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22ab5841dbdd1657506e0d13fcede092739bfe1cd0a1ac1fb8dbe847475354b7`  
		Last Modified: Wed, 03 Aug 2022 00:59:40 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bd5344541cebcb5f59e7bb10d3f13ddba552602450871dd13fce7b6710dd8b3`  
		Last Modified: Wed, 03 Aug 2022 01:13:01 GMT  
		Size: 11.7 MB (11742467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b911375076faace847399b8350bbc1d076bfff1b5db4256b293b183f247676`  
		Last Modified: Wed, 03 Aug 2022 01:12:59 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4467b0035adaf5ee9c3bad507fe611a07d35097f3ba85e7f191a0148595ebd52`  
		Last Modified: Wed, 03 Aug 2022 01:13:03 GMT  
		Size: 13.9 MB (13888288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f4e202f28692b9c22f1757f1441c85325967138a4d98a6d8dd3e8efd9cf880`  
		Last Modified: Wed, 03 Aug 2022 01:12:59 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4f3115f7515d145c9e28ca7110343533f44a81a81c46cb0c3fd75aeb244e4e`  
		Last Modified: Wed, 03 Aug 2022 01:12:59 GMT  
		Size: 18.6 KB (18642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:226a584a562b6dca892e6200c1ea2ae42aeab05b8e5460e662e08b675938d9b4`  
		Last Modified: Thu, 04 Aug 2022 12:47:53 GMT  
		Size: 8.7 MB (8677809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35e25d78be543d0b4b6925859012082e4653d923ae6f99fef2bc2436ab1301b`  
		Last Modified: Thu, 04 Aug 2022 12:47:49 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3cbb3fc25fa918a0e7e6c2639941bccfc6884821d0c1c79b0540ce3b00bead`  
		Last Modified: Thu, 04 Aug 2022 12:47:51 GMT  
		Size: 7.5 MB (7486422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b3eadb04d60fb8e96b900b23c1393d0845b8eac00f7b9cb600a9362e81c992`  
		Last Modified: Thu, 04 Aug 2022 12:47:49 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a42cc0db67ac289649e5077e8289dd9aadbdb64b5c011e0fca123c04e474b4`  
		Last Modified: Thu, 04 Aug 2022 12:47:50 GMT  
		Size: 1.4 MB (1383735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0952d8ce997f8ac0c48e86b98d74dd966ca03e5af4c222c161bc385735305156`  
		Last Modified: Thu, 04 Aug 2022 12:47:49 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php8.1` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:302302664dc06304ae585aa92babe2e34e2f60e6903708fa028986b6dd005d35
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.5 MB (51508083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d3b75ef7108849af68a92e8a361ba105f8d6197932ede6e1e0f6c590061cf329`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 03:14:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 19 Jul 2022 03:14:57 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 19 Jul 2022 03:14:58 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 19 Jul 2022 03:14:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 19 Jul 2022 03:15:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 19 Jul 2022 03:15:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 19 Jul 2022 03:15:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 19 Jul 2022 03:15:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 19 Jul 2022 03:33:54 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 04 Aug 2022 22:25:10 GMT
ENV PHP_VERSION=8.1.9
# Thu, 04 Aug 2022 22:25:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.9.tar.xz.asc
# Thu, 04 Aug 2022 22:25:12 GMT
ENV PHP_SHA256=53477e73e6254dc942b68913a58d815ffdbf6946baf61a1f8ef854de524c27bf
# Thu, 04 Aug 2022 22:25:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 04 Aug 2022 22:25:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Aug 2022 22:31:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Aug 2022 22:31:06 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 04 Aug 2022 22:31:07 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Aug 2022 22:31:08 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Aug 2022 22:31:09 GMT
CMD ["php" "-a"]
# Fri, 05 Aug 2022 03:16:02 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 05 Aug 2022 03:16:02 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 05 Aug 2022 03:16:03 GMT
WORKDIR /var/www/html
# Fri, 05 Aug 2022 03:17:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 05 Aug 2022 03:17:06 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 05 Aug 2022 03:17:07 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 05 Aug 2022 03:17:08 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Fri, 05 Aug 2022 03:17:09 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Fri, 05 Aug 2022 03:17:12 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 05 Aug 2022 03:17:13 GMT
VOLUME [/var/www/html]
# Fri, 05 Aug 2022 03:17:15 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 05 Aug 2022 03:17:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Aug 2022 03:17:16 GMT
USER www-data
# Fri, 05 Aug 2022 03:17:17 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e5d6c316a066af896390af8c46674b59f76a8a7944d745d97f07baa51331e9`  
		Last Modified: Tue, 19 Jul 2022 04:26:56 GMT  
		Size: 1.7 MB (1704103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91bb00cf3b67a671a451b05b313e1cdf88da5050cc552ebd31cac2cf9ee7fb6`  
		Last Modified: Tue, 19 Jul 2022 04:26:55 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d399c457bfcaf74cbdbcb45d847f80dab959ac4d6106cf448656b5a4d0ee09`  
		Last Modified: Tue, 19 Jul 2022 04:26:55 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00fa1f5d561656f9a47a06e09c4a6416ace40cecb12d88360e1c79de5d90981a`  
		Last Modified: Fri, 05 Aug 2022 00:06:25 GMT  
		Size: 11.8 MB (11808013 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b3639f8b881849bf0e06f537b3570a2fe96099154b09b1c4e37de850f220ab5`  
		Last Modified: Fri, 05 Aug 2022 00:06:24 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:470d809881a9c14738990b978eff34ca9b6e69e09ed7799188ed8397b9650915`  
		Last Modified: Fri, 05 Aug 2022 00:06:27 GMT  
		Size: 16.2 MB (16233397 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93ca97475e98ef5c68fc648a01a3b53ab9e9890dddbbd4a256bad1098a833082`  
		Last Modified: Fri, 05 Aug 2022 00:06:24 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0fda6783cb072ae7cb354852706102324897932adaac3c446beff70a036b00`  
		Last Modified: Fri, 05 Aug 2022 00:06:24 GMT  
		Size: 18.3 KB (18289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:910c2faf7c3fb5cfc645a4866367667d8f92dd1688679d2366e25cfe6cae7108`  
		Last Modified: Fri, 05 Aug 2022 03:24:14 GMT  
		Size: 9.4 MB (9441895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f6369a814eaf946414ac0810f7b97876441453ff7a5fcdf9fc308bb3d5483f3`  
		Last Modified: Fri, 05 Aug 2022 03:24:14 GMT  
		Size: 8.2 MB (8219389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fe80d83e35d6861fb95758067b7a886231424acd442f70556b7935d9f998198`  
		Last Modified: Fri, 05 Aug 2022 03:24:14 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7233abfe664d6a3832de40cf9a3434094e376255bf41ce3861492de6bb865be5`  
		Last Modified: Fri, 05 Aug 2022 03:24:13 GMT  
		Size: 1.4 MB (1383077 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1128ca4352cb770254040d0765c2bbeaa360e686f107bebf8dc00ef0cbf950c6`  
		Last Modified: Fri, 05 Aug 2022 03:24:13 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php8.1` - linux; 386

```console
$ docker pull wordpress@sha256:a316e80daa36e7963a302bd1a8b20382347e25ca39f5cffe6e0256663544460f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.7 MB (52742265 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b69153269ab3afe425bee063bd10896260c5dd5772f2ea84c13151332403f46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 21:41:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 18 Jul 2022 21:41:31 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 18 Jul 2022 21:41:32 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 18 Jul 2022 21:41:33 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 18 Jul 2022 21:41:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 18 Jul 2022 21:41:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 Jul 2022 21:41:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 Jul 2022 21:41:37 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 18 Jul 2022 21:55:28 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 04 Aug 2022 21:50:26 GMT
ENV PHP_VERSION=8.1.9
# Thu, 04 Aug 2022 21:50:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.9.tar.xz.asc
# Thu, 04 Aug 2022 21:50:28 GMT
ENV PHP_SHA256=53477e73e6254dc942b68913a58d815ffdbf6946baf61a1f8ef854de524c27bf
# Thu, 04 Aug 2022 21:50:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 04 Aug 2022 21:50:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:54:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Aug 2022 21:54:32 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:54:32 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Aug 2022 21:54:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Aug 2022 21:54:34 GMT
CMD ["php" "-a"]
# Fri, 05 Aug 2022 02:23:52 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 05 Aug 2022 02:23:52 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 05 Aug 2022 02:23:53 GMT
WORKDIR /var/www/html
# Fri, 05 Aug 2022 02:24:49 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 05 Aug 2022 02:24:49 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 05 Aug 2022 02:24:50 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 05 Aug 2022 02:24:51 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Fri, 05 Aug 2022 02:24:52 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Fri, 05 Aug 2022 02:24:55 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 05 Aug 2022 02:24:56 GMT
VOLUME [/var/www/html]
# Fri, 05 Aug 2022 02:24:58 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 05 Aug 2022 02:24:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Aug 2022 02:24:59 GMT
USER www-data
# Fri, 05 Aug 2022 02:25:00 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b497c2c5ebbc20f14d6736375ca0223ad07215dcc8af96c5bbce7c290f69ea2a`  
		Last Modified: Mon, 18 Jul 2022 22:43:39 GMT  
		Size: 1.8 MB (1808030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cce9082517109c8caf9a17724781a05e7c300af26cb96f1a17a34b407ec5354`  
		Last Modified: Mon, 18 Jul 2022 22:43:38 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11354c8cb04ba6f087c3a31b39b85cfce6d35433d6481e761df799bbbefae5a7`  
		Last Modified: Mon, 18 Jul 2022 22:43:38 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b21f38056c3c41f8a8581d608daddd42bbd1da4b3dc40eeca28e00dd8398bc80`  
		Last Modified: Thu, 04 Aug 2022 23:21:49 GMT  
		Size: 11.8 MB (11807988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5bedf9de7437fbd184fe266f68fc7c32a526493abcc37f72ea53700d34c5654`  
		Last Modified: Thu, 04 Aug 2022 23:21:46 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f524e764b89581b621dd2d9846ee34cedb2d50ab730f26372ff5f0714113c73`  
		Last Modified: Thu, 04 Aug 2022 23:21:50 GMT  
		Size: 16.6 MB (16634705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9aa5b7eb199b52827edafa6a8060bbb3c05593df8ac00b5d26ffcef81a44fef`  
		Last Modified: Thu, 04 Aug 2022 23:21:46 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6573876b73c1b7f761ad37e0a94dd91f4aec1b54a3fc5cff75ac5880e309d580`  
		Last Modified: Thu, 04 Aug 2022 23:21:46 GMT  
		Size: 18.5 KB (18454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c6b63bd1fa2d193f23ba778d523d67fbb312fcd8205c3795747d127e2f9443`  
		Last Modified: Fri, 05 Aug 2022 02:27:43 GMT  
		Size: 9.5 MB (9492231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab433ce8ec6035910ae77100b22ce56be90ac71c561126398487d4c48052ce35`  
		Last Modified: Fri, 05 Aug 2022 02:27:43 GMT  
		Size: 8.8 MB (8790262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd1a6705b37bdb77b6e1d834133faf66a8bb2725cbbe0928cfbb4541ca88bfc`  
		Last Modified: Fri, 05 Aug 2022 02:27:41 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97f577da28bc608e99ec52ef99cf679a8dc482a1240be2038a18969c118ae4ee`  
		Last Modified: Fri, 05 Aug 2022 02:27:42 GMT  
		Size: 1.4 MB (1383064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b4f363b20b8b9b6b05cc04b7821c4cb2e973ca7194ca1b124f6db4d5ff3832`  
		Last Modified: Fri, 05 Aug 2022 02:27:41 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php8.1` - linux; ppc64le

```console
$ docker pull wordpress@sha256:95faa277e86651fab69a13ef0b2d6d9790d52e4804344dbe21801d4ea51059e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53062551 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:562d73297b2f5f6ee378459749e4a50ba62f7d909a52b0a57fb9fa11b9280064`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Tue, 02 Aug 2022 08:43:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 02 Aug 2022 08:44:00 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 02 Aug 2022 08:44:01 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 02 Aug 2022 08:44:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 02 Aug 2022 08:44:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 02 Aug 2022 08:44:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 08:44:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 02 Aug 2022 08:44:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 02 Aug 2022 09:48:46 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 04 Aug 2022 21:51:12 GMT
ENV PHP_VERSION=8.1.9
# Thu, 04 Aug 2022 21:51:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.9.tar.xz.asc
# Thu, 04 Aug 2022 21:51:13 GMT
ENV PHP_SHA256=53477e73e6254dc942b68913a58d815ffdbf6946baf61a1f8ef854de524c27bf
# Thu, 04 Aug 2022 21:51:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 04 Aug 2022 21:51:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:56:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Aug 2022 21:56:17 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:56:19 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Aug 2022 21:56:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Aug 2022 21:56:20 GMT
CMD ["php" "-a"]
# Fri, 05 Aug 2022 03:22:29 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 05 Aug 2022 03:22:30 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 05 Aug 2022 03:22:31 GMT
WORKDIR /var/www/html
# Fri, 05 Aug 2022 03:24:02 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 05 Aug 2022 03:24:04 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 05 Aug 2022 03:24:05 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 05 Aug 2022 03:24:05 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Fri, 05 Aug 2022 03:24:05 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Fri, 05 Aug 2022 03:24:09 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 05 Aug 2022 03:24:10 GMT
VOLUME [/var/www/html]
# Fri, 05 Aug 2022 03:24:10 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 05 Aug 2022 03:24:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Aug 2022 03:24:11 GMT
USER www-data
# Fri, 05 Aug 2022 03:24:11 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e8cea93b5fef5fa8a1b6bd028c2b234f9d6a13eafbc7c56233a28d563e945d7`  
		Last Modified: Tue, 02 Aug 2022 14:39:56 GMT  
		Size: 1.8 MB (1772220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce77ca517c72afe49e0051e297b275de36878e5854404f8e58e392b245409fa9`  
		Last Modified: Tue, 02 Aug 2022 14:39:55 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e24f93cc16e56ba64a8de358b070286c71d51687f89649357febe021d2c189a`  
		Last Modified: Tue, 02 Aug 2022 14:39:55 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4347af31fb91c32a917ea69143f45cb18af2df1aa122272b553bb81d782cbb3a`  
		Last Modified: Thu, 04 Aug 2022 23:29:48 GMT  
		Size: 11.8 MB (11808463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbaeef40dba26fa4e570397069754e5510acd8d151be9af055809c54000020dc`  
		Last Modified: Thu, 04 Aug 2022 23:29:47 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69c5c559e84693eea087c833de03f4c7f3dbc212d4d2926617d8a095279061ee`  
		Last Modified: Thu, 04 Aug 2022 23:29:52 GMT  
		Size: 17.1 MB (17058368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ea2943c026bc91046d67462fcb073ae39a47ee46f338b129e061c9a66f5a3a`  
		Last Modified: Thu, 04 Aug 2022 23:29:48 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:058005b44eef28ddaa4a01e39cbea1dce0da7ce2a2b3602ceb6f91b375ce9bfb`  
		Last Modified: Thu, 04 Aug 2022 23:29:47 GMT  
		Size: 18.7 KB (18659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a362f5f34cf535f9752576a128b2ce473819ff3566f22d0814d80b3a969cefb9`  
		Last Modified: Fri, 05 Aug 2022 03:32:04 GMT  
		Size: 9.6 MB (9577913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97cf19e5009228898cb1f0d8d1192866d0287c49e259c9473c281719470b28b5`  
		Last Modified: Fri, 05 Aug 2022 03:31:58 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343e0b709a137845c70c515320b1ab4be295a87fa8d5efa1cb3baac8f3ca37e4`  
		Last Modified: Fri, 05 Aug 2022 03:32:00 GMT  
		Size: 8.6 MB (8647841 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:675d3983fb2b4db929d40f94cde7211b8d4ade2cc409b721752025b0fa79bd9f`  
		Last Modified: Fri, 05 Aug 2022 03:31:58 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c228a014d73ef6b0d94fdc485ebe4bf1d9cadf9b1f5c496ab8932caa6cbdff`  
		Last Modified: Fri, 05 Aug 2022 03:31:59 GMT  
		Size: 1.4 MB (1383736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c252c18f49b645c57cf705abc449320c3fc4aaff3ae845a647af1d319599368`  
		Last Modified: Fri, 05 Aug 2022 03:31:58 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php8.1` - linux; s390x

```console
$ docker pull wordpress@sha256:2b05a06c34d9f18189b137d49499f887e0473faf7123ffa6ee1187cdf25abea7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.1 MB (51103800 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25f4a28ca591e5942b14fc2de274444c241c03a9e500e653c479977cab867551`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 02:11:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 19 Jul 2022 02:11:25 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 19 Jul 2022 02:11:27 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 19 Jul 2022 02:11:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 19 Jul 2022 02:11:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 19 Jul 2022 02:11:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 19 Jul 2022 02:11:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 19 Jul 2022 02:11:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 19 Jul 2022 02:28:55 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Thu, 04 Aug 2022 21:17:17 GMT
ENV PHP_VERSION=8.1.9
# Thu, 04 Aug 2022 21:17:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.9.tar.xz.asc
# Thu, 04 Aug 2022 21:17:17 GMT
ENV PHP_SHA256=53477e73e6254dc942b68913a58d815ffdbf6946baf61a1f8ef854de524c27bf
# Thu, 04 Aug 2022 21:17:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 04 Aug 2022 21:17:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:20:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Aug 2022 21:20:12 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 04 Aug 2022 21:20:13 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Aug 2022 21:20:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Aug 2022 21:20:13 GMT
CMD ["php" "-a"]
# Fri, 05 Aug 2022 01:35:13 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 05 Aug 2022 01:35:14 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 05 Aug 2022 01:35:14 GMT
WORKDIR /var/www/html
# Fri, 05 Aug 2022 01:35:54 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 05 Aug 2022 01:35:55 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 05 Aug 2022 01:35:55 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 05 Aug 2022 01:35:55 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Fri, 05 Aug 2022 01:35:56 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Fri, 05 Aug 2022 01:35:57 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 05 Aug 2022 01:35:58 GMT
VOLUME [/var/www/html]
# Fri, 05 Aug 2022 01:35:58 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 05 Aug 2022 01:35:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Aug 2022 01:35:58 GMT
USER www-data
# Fri, 05 Aug 2022 01:35:58 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9842ade5e34b07c420965519970b802ea9e999bc04dc2757c682c4fcdb9a105`  
		Last Modified: Tue, 19 Jul 2022 03:30:23 GMT  
		Size: 1.8 MB (1766739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11189b7b565fb9039d6d93c6badbfaf6890f39532261d177b5352414b76fea65`  
		Last Modified: Tue, 19 Jul 2022 03:30:23 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36504c72275c98013fb2457e15e8efe23a0692912549611f4b044d0fcd9aec06`  
		Last Modified: Tue, 19 Jul 2022 03:30:23 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0c7d3dcfdb4c3dc2028bf0cb5b6dca91eb7c5b6977216e6b86df5a44ba8772`  
		Last Modified: Thu, 04 Aug 2022 22:20:07 GMT  
		Size: 11.8 MB (11808248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f643a19583281d8a87f45fff1f764f8e28fa4bada1aa9c614b4b38fb4ca0d72a`  
		Last Modified: Thu, 04 Aug 2022 22:20:02 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c33564ca26b12d3fc118634f6a8a9860c9eea2416e0be1fff970822b2baf16bd`  
		Last Modified: Thu, 04 Aug 2022 22:20:05 GMT  
		Size: 15.2 MB (15210207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52532737d37eb27c1afa9e6936ddc0607b67132264f84994707c21bd106f5595`  
		Last Modified: Thu, 04 Aug 2022 22:20:02 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2cdf38c26e6dfe60ccfd841881baeb030ec80a5b81e01eccc24b720768502a4`  
		Last Modified: Thu, 04 Aug 2022 22:20:02 GMT  
		Size: 18.4 KB (18396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512b576e4b6bb764ddf04741f33b055e4c117a4e37f0b668f2885352cf5c2e00`  
		Last Modified: Fri, 05 Aug 2022 01:38:21 GMT  
		Size: 9.9 MB (9891823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bc1d51a4ab7ffbb15a7feed463fae74d97346e8f4243fdb63faa1b7c9c1cac`  
		Last Modified: Fri, 05 Aug 2022 01:38:18 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82dcc1a2e7e34c4079222dc7f65f2205cbaa2a599b9360683ca6d96a1d015c14`  
		Last Modified: Fri, 05 Aug 2022 01:38:19 GMT  
		Size: 8.4 MB (8438844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17d01e14f45c7021246688026136691f590abedd9a32a8879c3406ba1125c926`  
		Last Modified: Fri, 05 Aug 2022 01:38:18 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df937ccf5e2de71d9a7bb90a7a3637417519c681089e5284f94982c85110e09b`  
		Last Modified: Fri, 05 Aug 2022 01:38:18 GMT  
		Size: 1.4 MB (1383327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19555abb16d5f15fd652adf5cd0f95ec868ead14cf4bba2e08df6668a6f9ad9e`  
		Last Modified: Fri, 05 Aug 2022 01:38:18 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
