## `wordpress:cli-2-php7.4`

```console
$ docker pull wordpress@sha256:98b406766cea295d831e0fe3b4cb943efea5bae1835e42f450fde8baf8caea1b
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

### `wordpress:cli-2-php7.4` - linux; amd64

```console
$ docker pull wordpress@sha256:7bfd80afb87c0cc8239b3457e81c44614047a578d6a59ea14eb29c25f00b9802
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46213823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d7224ce6eaca9a12cfdbd09e659d459b4bc7347984b981b83692b78fe4817f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Thu, 17 Dec 2020 00:19:41 GMT
ADD file:ec475c2abb2d46435286b5ae5efacf5b50b1a9e3b6293b69db3c0172b5b9658b in / 
# Thu, 17 Dec 2020 00:19:42 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 08:41:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 08:41:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 08:41:55 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 08:41:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 08:41:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 08:41:57 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 08:41:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 08:41:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 08:57:27 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Dec 2020 08:57:28 GMT
ENV PHP_VERSION=7.4.13
# Thu, 17 Dec 2020 08:57:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.13.tar.xz.asc
# Thu, 17 Dec 2020 08:57:28 GMT
ENV PHP_SHA256=aead303e3abac23106529560547baebbedba0bb2943b91d5aa08fff1f41680f4
# Thu, 17 Dec 2020 08:57:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 08:57:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 09:03:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 09:03:45 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 17 Dec 2020 09:03:47 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 09:03:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 09:03:47 GMT
CMD ["php" "-a"]
# Thu, 17 Dec 2020 18:48:43 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 17 Dec 2020 18:48:44 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 17 Dec 2020 18:48:46 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 17 Dec 2020 18:48:47 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 17 Dec 2020 18:48:47 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 18:48:47 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 17 Dec 2020 18:48:48 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 17 Dec 2020 18:48:48 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 17 Dec 2020 18:48:50 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Thu, 17 Dec 2020 18:48:50 GMT
VOLUME [/var/www/html]
# Thu, 17 Dec 2020 18:48:50 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 17 Dec 2020 18:48:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 18:48:51 GMT
USER www-data
# Thu, 17 Dec 2020 18:48:51 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:801bfaa63ef2094d770c809815b9e2b9c1194728e5e754ef7bc764030e140cea`  
		Last Modified: Wed, 16 Dec 2020 19:34:50 GMT  
		Size: 2.8 MB (2799066 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30e2096094279456885c5847855bddf4d9ac3b5c4f7f0ff73ef92fa69821ff86`  
		Last Modified: Thu, 17 Dec 2020 11:05:30 GMT  
		Size: 1.3 MB (1340903 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320f26ee9b1c7b4c2ce0b67550a066ea859fb8796c0ff8de576f7e1b330342da`  
		Last Modified: Thu, 17 Dec 2020 11:05:30 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4612e05a72cfb0fde0de7565baa2660900747122288141d8dba25482f4983fe0`  
		Last Modified: Thu, 17 Dec 2020 11:05:30 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d577b440bd5a08cde8b9fd1f211b90b557a8f5ab7e1e9cc3c122710e3133a7`  
		Last Modified: Thu, 17 Dec 2020 11:06:44 GMT  
		Size: 10.3 MB (10338560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f67ee0e7b40ae31d5bc49ceac18216bb11532d707592c64f1b56afd24c02a24`  
		Last Modified: Thu, 17 Dec 2020 11:06:41 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c84ce97d3b3d04f7b67f67266bb46f4eb5fc61913059dcaefaf1c9bc508a15`  
		Last Modified: Thu, 17 Dec 2020 11:06:46 GMT  
		Size: 14.2 MB (14184174 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e1a66d6657a468dac5474d11e3de5c26410f685e259c68d1c29e8603dce4a6c`  
		Last Modified: Thu, 17 Dec 2020 11:06:41 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea3ec22f9c6fb56eb3e791a45139f1195df00a45a3d2487a61a537653f4f1825`  
		Last Modified: Thu, 17 Dec 2020 11:06:41 GMT  
		Size: 16.9 KB (16876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a24756e21fb4b0efbd6281fc221b3b3350031fee3318206e28438438c9c75a0`  
		Last Modified: Thu, 17 Dec 2020 18:52:01 GMT  
		Size: 7.0 MB (7042851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5259eaaf873fefc0399de7f569f68a518942f570c815c9e8118d8b1755c491b`  
		Last Modified: Thu, 17 Dec 2020 18:51:58 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:983196ae5d88c7ee3b575b946411127828dd2b4b5837ac00c7a3c6c4fb284482`  
		Last Modified: Thu, 17 Dec 2020 18:52:00 GMT  
		Size: 9.3 MB (9280892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0407485a5373c9f56037e2af580190777b0a9aa8bdbf721ea2d0723d211a13a3`  
		Last Modified: Thu, 17 Dec 2020 18:51:58 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edd85bec5c080d4560d3fc11a57dcab08d923b68fc1844a753d0ed79e1065e47`  
		Last Modified: Thu, 17 Dec 2020 18:51:59 GMT  
		Size: 1.2 MB (1205353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15f807ce124e082bf4be5daa444c6a1e305e27cee9cb8ae0a4b5523f4aa5a47`  
		Last Modified: Thu, 17 Dec 2020 18:51:58 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.4` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:455d222a776cce75239d7bdeb0581638e3c25156048c18470c6c774d70485dd0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44231893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d36e95572c4e7d4b381e3b9c465b28ae6ff60de1abf42c26ec4f547031d5faff`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Wed, 16 Dec 2020 23:49:43 GMT
ADD file:0a16715e2d0e5811c3c578945d618db0e269847a799340248f9ba8d393c9eec2 in / 
# Wed, 16 Dec 2020 23:49:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 04:02:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 04:02:22 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 04:02:27 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 04:02:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 04:02:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 04:02:34 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 04:02:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 04:02:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 04:12:25 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 07 Jan 2021 17:53:27 GMT
ENV PHP_VERSION=7.4.14
# Thu, 07 Jan 2021 17:53:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Thu, 07 Jan 2021 17:53:29 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Thu, 07 Jan 2021 17:53:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jan 2021 17:53:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:57:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jan 2021 17:57:31 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 07 Jan 2021 17:57:35 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jan 2021 17:57:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jan 2021 17:57:38 GMT
CMD ["php" "-a"]
# Thu, 07 Jan 2021 20:21:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 07 Jan 2021 20:21:08 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Jan 2021 20:21:12 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 07 Jan 2021 20:21:14 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 07 Jan 2021 20:21:15 GMT
WORKDIR /var/www/html
# Thu, 07 Jan 2021 20:21:16 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 07 Jan 2021 20:21:16 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 07 Jan 2021 20:21:17 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 07 Jan 2021 20:21:21 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Thu, 07 Jan 2021 20:21:22 GMT
VOLUME [/var/www/html]
# Thu, 07 Jan 2021 20:21:23 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 07 Jan 2021 20:21:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Jan 2021 20:21:25 GMT
USER www-data
# Thu, 07 Jan 2021 20:21:25 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:93247449aef3c56eb4f7ab7b3fed95743c974b823def6dd86ec84008126e7903`  
		Last Modified: Wed, 16 Dec 2020 23:50:24 GMT  
		Size: 2.6 MB (2604163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16035da780bb4f74637b8f27602f05d4a81886aeea06f603ea7e46dd84d57b6d`  
		Last Modified: Thu, 17 Dec 2020 05:38:57 GMT  
		Size: 1.3 MB (1310288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdfae7d4501031aa09e0c64be274eb95df5740b32cde16be0182bcea9d8a4845`  
		Last Modified: Thu, 17 Dec 2020 05:38:57 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6384065388d88752c6562c2bb76398ecc59f1a03a1c5e4601dc75d768117919`  
		Last Modified: Thu, 17 Dec 2020 05:38:56 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:870eab60d059d25070e9f31293932a1eef060806b2a641cb236b7a5ddb8b5c66`  
		Last Modified: Thu, 07 Jan 2021 18:48:27 GMT  
		Size: 10.3 MB (10345693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6895d0a2ebc13a830252d44c71154d8089a5a854a5b95a7d193be1fdce4e05bc`  
		Last Modified: Thu, 07 Jan 2021 18:48:26 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da6415a6364bd6d860ea84f27cded09bdc386d1869e10fe570eceec2822810e`  
		Last Modified: Thu, 07 Jan 2021 18:48:29 GMT  
		Size: 13.2 MB (13201877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fea093ad63bd2cc3ac791ee09072420214a9098effea320b3c3451cae003133`  
		Last Modified: Thu, 07 Jan 2021 18:48:25 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030d3de27a8614e87621ea74772e56201c07b2cb10684b3bba8c5c8cf79f03cd`  
		Last Modified: Thu, 07 Jan 2021 18:48:25 GMT  
		Size: 16.9 KB (16882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e604e11baecaab32790471c02181a347b5871f4462866df6cf44a07d97932898`  
		Last Modified: Thu, 07 Jan 2021 20:23:29 GMT  
		Size: 6.7 MB (6669027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf632ff58c1d72a2aa1033282c2ff2bdf14456ef65bffa5199540f3f46cd7b8a`  
		Last Modified: Thu, 07 Jan 2021 20:23:23 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:402d4c07d137337fde18236b31165246bf196fbd4f529147ecc278cec429dcf7`  
		Last Modified: Thu, 07 Jan 2021 20:23:27 GMT  
		Size: 8.9 MB (8873285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905b6c9ec1ce466ca4b5ededb81f7a70ac50073f7d26ebe7d70b90fc2e033d69`  
		Last Modified: Thu, 07 Jan 2021 20:23:25 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459aff96526e381a48761ddfc1dcf7b80ab989b33a6a77282b7bdb1b121e07a9`  
		Last Modified: Thu, 07 Jan 2021 20:23:23 GMT  
		Size: 1.2 MB (1205451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13847907cc23e80ba2718faeb9d76298ed5955e7f71b71b728537c1365ef1d64`  
		Last Modified: Thu, 07 Jan 2021 20:23:23 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.4` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:0ac833dc58455431c004452d0ceb89fe36efe20fa08c922298c1165e7a25c64b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.6 MB (42643544 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c74cfd4d778e4c28e9c74f465ba2d90ba5356553bd2ea56ec56d59ad66ff1c49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Wed, 16 Dec 2020 23:58:14 GMT
ADD file:bd07f77a2b2741ca6bda80d9203be9c7274cf73145bff778cf000db0d8d4e903 in / 
# Wed, 16 Dec 2020 23:58:15 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 03:59:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 03:59:47 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 03:59:49 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 03:59:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 03:59:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 03:59:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 03:59:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 03:59:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 04:08:55 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Dec 2020 04:09:05 GMT
ENV PHP_VERSION=7.4.13
# Thu, 17 Dec 2020 04:09:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.13.tar.xz.asc
# Thu, 17 Dec 2020 04:09:10 GMT
ENV PHP_SHA256=aead303e3abac23106529560547baebbedba0bb2943b91d5aa08fff1f41680f4
# Thu, 17 Dec 2020 04:09:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 04:09:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:12:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 04:12:26 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:12:29 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 04:12:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 04:12:33 GMT
CMD ["php" "-a"]
# Thu, 17 Dec 2020 10:43:16 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 17 Dec 2020 10:43:18 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 17 Dec 2020 10:43:22 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 17 Dec 2020 10:43:24 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 17 Dec 2020 10:43:25 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 10:43:25 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 17 Dec 2020 10:43:26 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 17 Dec 2020 10:43:27 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 17 Dec 2020 10:43:30 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Thu, 17 Dec 2020 10:43:31 GMT
VOLUME [/var/www/html]
# Thu, 17 Dec 2020 10:43:32 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 17 Dec 2020 10:43:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 10:43:33 GMT
USER www-data
# Thu, 17 Dec 2020 10:43:34 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:c58e8a26a8407acc3ead776f6526efa889fda03270a8d05109208d9f59159420`  
		Last Modified: Wed, 16 Dec 2020 23:58:59 GMT  
		Size: 2.4 MB (2407555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb43bb12dd6693d888e6501fba59948c3e894b068d539fbf968aac1638f58847`  
		Last Modified: Thu, 17 Dec 2020 05:28:25 GMT  
		Size: 1.2 MB (1214517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52c593d596abc28364a253c99118c3080eec76e91bf5db463e2a66804da18dfa`  
		Last Modified: Thu, 17 Dec 2020 05:28:23 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:145a8f86ceab4a34dedf8d4173439cf517eec5c52b3074dea204dce67da7f3ad`  
		Last Modified: Thu, 17 Dec 2020 05:28:23 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:876182898cd45998c1b69cfdef1412be19b3aad5b8ef2c52aa614c942591cecc`  
		Last Modified: Thu, 17 Dec 2020 05:29:51 GMT  
		Size: 10.3 MB (10338570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:894aacf547d13df0dbde33a147528c9699fed1dc507481fea7d76ec8b9122e2e`  
		Last Modified: Thu, 17 Dec 2020 05:29:50 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a305b55eec78648f879ddcf4d0cec09b195486040d4f30e336f5d1684346f14e`  
		Last Modified: Thu, 17 Dec 2020 05:29:54 GMT  
		Size: 12.4 MB (12360629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4625c0d541238c7adacfe8d1bb33e8fb132291247f5576ae5950b5bc1a2b5db0`  
		Last Modified: Thu, 17 Dec 2020 05:29:50 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d925130e305bd441931f20f217b886fdfb03824f1321f4552e6015fe1e37c0f`  
		Last Modified: Thu, 17 Dec 2020 05:29:50 GMT  
		Size: 16.8 KB (16844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1498e4307cbabe826fa941b5637fb9ec9ac938ceb83c292dc1efc4254943fdf8`  
		Last Modified: Thu, 17 Dec 2020 10:47:19 GMT  
		Size: 6.5 MB (6485112 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2f4b9e146fb667b13e75fe6079e67aaaec86c3965c5d9d47381de9be416064`  
		Last Modified: Thu, 17 Dec 2020 10:47:03 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146eeb1db67d848ac5be06f6182c74f345dc65ba94088311eb3a570da0ce9371`  
		Last Modified: Thu, 17 Dec 2020 10:47:06 GMT  
		Size: 8.6 MB (8609681 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:495451e2b8e851f2a4b70aec8036d6170749a0a392558fb4622e1b32301433a0`  
		Last Modified: Thu, 17 Dec 2020 10:47:03 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff96c23c20b62dccabe9ca73380a34edb961812e09c5fc0bc0dd6f851a5830f`  
		Last Modified: Thu, 17 Dec 2020 10:47:04 GMT  
		Size: 1.2 MB (1205410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c04b1039b28215bff90659c0846bf3efaf2ca57fa5270bcffac418fd7d32271`  
		Last Modified: Thu, 17 Dec 2020 10:47:03 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.4` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:7dd7bca9dd8117fd18aae4f6321acc7d1c2aecdfe62895253768679834d8785b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.8 MB (45831116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30964057ddb54274ab98a87a7aaa659c6248da4f41fa1c4ac119da132ac70692`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Wed, 16 Dec 2020 23:40:26 GMT
ADD file:a4845c3840a3fd0e41e4635a179cce20c81afc6c02e34e3fd5bd2d535698918b in / 
# Wed, 16 Dec 2020 23:40:29 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 05:46:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 05:46:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 05:46:55 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 05:46:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 05:47:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 05:47:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 05:47:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 05:47:13 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 05:57:36 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Dec 2020 05:57:38 GMT
ENV PHP_VERSION=7.4.13
# Thu, 17 Dec 2020 05:57:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.13.tar.xz.asc
# Thu, 17 Dec 2020 05:57:42 GMT
ENV PHP_SHA256=aead303e3abac23106529560547baebbedba0bb2943b91d5aa08fff1f41680f4
# Thu, 17 Dec 2020 05:57:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 05:57:50 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 06:01:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 06:01:06 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 17 Dec 2020 06:01:09 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 06:01:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 06:01:11 GMT
CMD ["php" "-a"]
# Thu, 17 Dec 2020 12:40:09 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 17 Dec 2020 12:40:14 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 17 Dec 2020 12:40:17 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 17 Dec 2020 12:40:20 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 17 Dec 2020 12:40:21 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 12:40:21 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 17 Dec 2020 12:40:22 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 17 Dec 2020 12:40:23 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 17 Dec 2020 12:40:27 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Thu, 17 Dec 2020 12:40:29 GMT
VOLUME [/var/www/html]
# Thu, 17 Dec 2020 12:40:31 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 17 Dec 2020 12:40:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 12:40:33 GMT
USER www-data
# Thu, 17 Dec 2020 12:40:34 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:159e5727ea618dfe8b08811112e2c51f5bd2b9ae7db9eb214914a65249f70ca0`  
		Last Modified: Wed, 16 Dec 2020 23:41:08 GMT  
		Size: 2.7 MB (2709048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349511631cc12dc049249fd94f9012c505ccb000f16147091cb84874846fb9b1`  
		Last Modified: Thu, 17 Dec 2020 07:10:16 GMT  
		Size: 1.3 MB (1342931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:053bd098149c8419c2b9b5a2702c5d9c4e9de3b2131447e18aacde4047de2d88`  
		Last Modified: Thu, 17 Dec 2020 07:10:15 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00122640c7f935b33a14c9e88b946165e75935d6cd28f9b2d20d783d43c21423`  
		Last Modified: Thu, 17 Dec 2020 07:10:15 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:611f319a43952d0126ac7e7626706297457d7d936058deda6019329b80e20f5d`  
		Last Modified: Thu, 17 Dec 2020 07:11:21 GMT  
		Size: 10.3 MB (10338594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ad141be828b5644fe19583e0972e3067368f6923e9d9687af54c0f9a69c2d5`  
		Last Modified: Thu, 17 Dec 2020 07:11:19 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b3caff7e7a8666b6378fd9aa6d4431eaeff1683eb021f4e80af4c363077049`  
		Last Modified: Thu, 17 Dec 2020 07:11:24 GMT  
		Size: 14.0 MB (13997169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1ef935679835cdc407fad9aee6bd87dcdf4cdc10b292187138301df9d72de28`  
		Last Modified: Thu, 17 Dec 2020 07:11:20 GMT  
		Size: 2.3 KB (2257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18382b9c6b81b124ee9c9ab96384bc861d67cef3c16ff5492c0cf6e2f574b962`  
		Last Modified: Thu, 17 Dec 2020 07:11:20 GMT  
		Size: 16.9 KB (16893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87f2cf52886f60e30370b57bec4adea4913a8f7e8b62adea44c9a5a7fa1e0ccf`  
		Last Modified: Thu, 17 Dec 2020 12:44:05 GMT  
		Size: 6.9 MB (6875963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0469227209e2fa877ea1bbe5e850b5af23d832c423a64362cde319c0ae09ab2`  
		Last Modified: Thu, 17 Dec 2020 12:44:01 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338c916fc2b3af501eeb4876ffad597ba4db7db74b37c748a1bc831a592b56d8`  
		Last Modified: Thu, 17 Dec 2020 12:44:05 GMT  
		Size: 9.3 MB (9339887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6eef91c429317f6cf508fa5cafe42c0026679092386873108a4e68dc922fae`  
		Last Modified: Thu, 17 Dec 2020 12:44:01 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b16780b674aab0f216834bbc1576466b3c0caf68ee9414cc17e3f70dd7f2a895`  
		Last Modified: Thu, 17 Dec 2020 12:44:03 GMT  
		Size: 1.2 MB (1205406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7369fdba5b059377b703fcd62b778934458827c15030354c2c6fa1d13fd3926b`  
		Last Modified: Thu, 17 Dec 2020 12:44:01 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.4` - linux; 386

```console
$ docker pull wordpress@sha256:fee3b941c085f626b20b734036906bd6438bc49d0d4e1d084cf4c8e4c600a5c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.0 MB (46969872 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fd7f269eca95d8c4a8baaa8c81423de45a873f19db5da78d64cb6c29e239883`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Thu, 17 Dec 2020 00:38:32 GMT
ADD file:de33fda50a142403e842620d20bc4404e66fc4ace16edc6946c4539e8a797458 in / 
# Thu, 17 Dec 2020 00:38:32 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 03:34:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 03:34:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 03:34:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 03:34:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 03:34:07 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 03:34:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 03:34:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 03:34:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 03:46:45 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Dec 2020 03:46:46 GMT
ENV PHP_VERSION=7.4.13
# Thu, 17 Dec 2020 03:46:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.13.tar.xz.asc
# Thu, 17 Dec 2020 03:46:46 GMT
ENV PHP_SHA256=aead303e3abac23106529560547baebbedba0bb2943b91d5aa08fff1f41680f4
# Thu, 17 Dec 2020 03:46:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 03:46:50 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 03:52:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 03:52:25 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 17 Dec 2020 03:52:27 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 03:52:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 03:52:27 GMT
CMD ["php" "-a"]
# Thu, 17 Dec 2020 09:37:46 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 17 Dec 2020 09:37:47 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 17 Dec 2020 09:37:49 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 17 Dec 2020 09:37:50 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 17 Dec 2020 09:37:50 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 09:37:50 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 17 Dec 2020 09:37:51 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 17 Dec 2020 09:37:51 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 17 Dec 2020 09:37:53 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Thu, 17 Dec 2020 09:37:53 GMT
VOLUME [/var/www/html]
# Thu, 17 Dec 2020 09:37:53 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 17 Dec 2020 09:37:54 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 09:37:54 GMT
USER www-data
# Thu, 17 Dec 2020 09:37:54 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:455793c72b878001f0905634ed52a2524ba51796e7377bf00683a85123f7dce9`  
		Last Modified: Thu, 17 Dec 2020 00:39:18 GMT  
		Size: 2.8 MB (2794130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94d120997ac65664d4944fb3d9d4551e8e118f43c788aa67591c2cb54010aed`  
		Last Modified: Thu, 17 Dec 2020 05:43:55 GMT  
		Size: 1.4 MB (1439814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:657c96696eb3a101b3148ccc28a870e751ee94e39bb2f3cc1745bdec7655b033`  
		Last Modified: Thu, 17 Dec 2020 05:43:55 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25357089a74d7e4f4ee1bc77cd180c431537e393399785f113a7f2fe4ac7614`  
		Last Modified: Thu, 17 Dec 2020 05:43:52 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d4c7df9dd64c082a7a26e39228a73590a406d786f77f2b9a7349d2c64e9dade`  
		Last Modified: Thu, 17 Dec 2020 05:45:01 GMT  
		Size: 10.3 MB (10338554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d7ac467d981495ec16e131b58ee34c454db7f661981343b559ccf7000bb47ce`  
		Last Modified: Thu, 17 Dec 2020 05:44:50 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e2fa8f2a388b93b9e1ad517cd3496cfaf3666c8d4387979c9aa9586340e48fe`  
		Last Modified: Thu, 17 Dec 2020 05:44:54 GMT  
		Size: 14.6 MB (14568848 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ba068f9e7a5a1b64baa77bf997a4a05764a07f652ae6176edad0faae91aa7a6`  
		Last Modified: Thu, 17 Dec 2020 05:44:49 GMT  
		Size: 2.3 KB (2257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1976a5a6898495659e3d00920b73ccb64f462fc0c434024bf8bcd6b1057cc6`  
		Last Modified: Thu, 17 Dec 2020 05:44:50 GMT  
		Size: 16.9 KB (16872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2aa597f10365f81e677fdafeacde27a1ec360c353cf69c0257e0289afec28c`  
		Last Modified: Thu, 17 Dec 2020 09:41:55 GMT  
		Size: 7.2 MB (7166902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abd8e34f8531a2a39e3f33f039f394a0e30e631d7525f52042d68d7cb165498e`  
		Last Modified: Thu, 17 Dec 2020 09:41:48 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022f6f38f6e0657cb22aefb9b2a68622c2b6d8af1eab8123adefa51303ad1a84`  
		Last Modified: Thu, 17 Dec 2020 09:41:55 GMT  
		Size: 9.4 MB (9434271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1596f39670d5d694a5422ea9cb1fab69f232a97e9fea323959c7cfbfbd28c71`  
		Last Modified: Thu, 17 Dec 2020 09:41:48 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b10fcb332f4b1685d957b6a3f1677a0b41cff0feddf34f6d3079e2ac4b3bfe1`  
		Last Modified: Thu, 17 Dec 2020 09:41:49 GMT  
		Size: 1.2 MB (1205337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fe3c0979b5628ac52a4364dd0e377a604d98a7bdecbec5045cf5cdd95892d6a`  
		Last Modified: Thu, 17 Dec 2020 09:41:48 GMT  
		Size: 407.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.4` - linux; ppc64le

```console
$ docker pull wordpress@sha256:cd02574f59361054b88b263d4b8ad56d1b01c2e9264cd0ffc8475b487be16108
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.4 MB (47441065 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82bfa5b0375faf09a475e60d78388e6684bb54595fc47c0971357b723b91db7f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Thu, 17 Dec 2020 00:20:42 GMT
ADD file:0a38c9b4955f8faa79627c166fca80ef342e443a16ce2925a30eeae317bbd786 in / 
# Thu, 17 Dec 2020 00:20:48 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:02:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 06:02:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 06:03:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 06:03:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 06:03:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 06:03:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 06:04:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 06:04:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 06:16:31 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Dec 2020 06:16:37 GMT
ENV PHP_VERSION=7.4.13
# Thu, 17 Dec 2020 06:16:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.13.tar.xz.asc
# Thu, 17 Dec 2020 06:16:50 GMT
ENV PHP_SHA256=aead303e3abac23106529560547baebbedba0bb2943b91d5aa08fff1f41680f4
# Thu, 17 Dec 2020 06:17:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 06:17:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 06:21:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 06:21:07 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 17 Dec 2020 06:21:15 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 06:21:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 06:21:22 GMT
CMD ["php" "-a"]
# Thu, 17 Dec 2020 16:22:19 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 17 Dec 2020 16:22:34 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 17 Dec 2020 16:22:47 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 17 Dec 2020 16:22:59 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 17 Dec 2020 16:23:06 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 16:23:18 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 17 Dec 2020 16:23:27 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 17 Dec 2020 16:23:32 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 17 Dec 2020 16:23:49 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Thu, 17 Dec 2020 16:23:57 GMT
VOLUME [/var/www/html]
# Thu, 17 Dec 2020 16:24:00 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 17 Dec 2020 16:24:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 16:24:14 GMT
USER www-data
# Thu, 17 Dec 2020 16:24:22 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:a9d343b7bcc225fe7ac17d96a81329510ab7f31a50472311cafe7168d3107317`  
		Last Modified: Thu, 17 Dec 2020 00:21:33 GMT  
		Size: 2.8 MB (2805226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4878c44618050313be4a5ac046d572683a6e0d371586c31a768e1768423df9a3`  
		Last Modified: Thu, 17 Dec 2020 08:04:10 GMT  
		Size: 1.4 MB (1383302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577c712c96426aadbf75437b4aae5841ed84ba25ee142ec3aaaf86802464d6f9`  
		Last Modified: Thu, 17 Dec 2020 08:04:08 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a10ca736025b1646c79fbd378c22773ccb82df4aadc2cb960dea6eacb8bbb16`  
		Last Modified: Thu, 17 Dec 2020 08:04:08 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27683514f10362bb29882d29f8d06428b27be3bef6cbfd4d8685312864fc8187`  
		Last Modified: Thu, 17 Dec 2020 08:05:51 GMT  
		Size: 10.3 MB (10338596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b2fdb11e6d3ac89e642800bd2d45099d48f9017d546feee3cdf1c4906113b7`  
		Last Modified: Thu, 17 Dec 2020 08:05:50 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb83c724d8476df5ad788192e4ede4f91373fa78dd270ee20b61280a0e037b8`  
		Last Modified: Thu, 17 Dec 2020 08:05:54 GMT  
		Size: 15.2 MB (15158127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3071f95028d35529d7555f5e7c26a85aa730e02ffc31bdac99134cc018e18fb9`  
		Last Modified: Thu, 17 Dec 2020 08:05:51 GMT  
		Size: 2.3 KB (2256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc4ceb48cf2d01ed7d0f76be417aecde084565e23e9ab3f47582aa44a510865`  
		Last Modified: Thu, 17 Dec 2020 08:05:51 GMT  
		Size: 16.9 KB (16930 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b79c079449b0f24dbc6baa1b8b4098f53463c3381f6a8da8c90fc5a28ae6087`  
		Last Modified: Thu, 17 Dec 2020 16:28:51 GMT  
		Size: 7.1 MB (7060882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae671ea938cba04564107e8772bae470762b8af7baa19494b8902c5f99534c59`  
		Last Modified: Thu, 17 Dec 2020 16:28:47 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69a67f394b57ac9138ed67c8dd535985768d15ba0dac561cf50c97b7eeb8136d`  
		Last Modified: Thu, 17 Dec 2020 16:28:49 GMT  
		Size: 9.5 MB (9467355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:098792fe7b75c36f26371a199bea65c2d697172626d12cc8af8abbd0ffc56686`  
		Last Modified: Thu, 17 Dec 2020 16:28:47 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62d14bc88002be4b41e49bbe4c61a4570e46a2c059890b5a1697dbedd25e41e5`  
		Last Modified: Thu, 17 Dec 2020 16:28:47 GMT  
		Size: 1.2 MB (1205419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce759c7566464a399e9c507eb9927f66cee6f81dcd82c1461b225afb01aa8fa9`  
		Last Modified: Thu, 17 Dec 2020 16:28:46 GMT  
		Size: 413.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.4` - linux; s390x

```console
$ docker pull wordpress@sha256:72b994529bb95c0f4581b8a2f610a746205c4744e4256d496f10572983189cab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.6 MB (45551130 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db4612696dff57ff7cd6ed58f773e67f5949c6d03c48e6b8ed225bffaef37078`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Wed, 16 Dec 2020 23:41:37 GMT
ADD file:3ad3856d165e8760af85574a8ffa75ca44b7e1b97b64d1d6d4608445efa4b860 in / 
# Wed, 16 Dec 2020 23:41:37 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 06:11:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Dec 2020 06:11:31 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Dec 2020 06:11:33 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Dec 2020 06:11:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Dec 2020 06:11:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Dec 2020 06:11:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 06:11:37 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Dec 2020 06:11:38 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Dec 2020 06:23:07 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 17 Dec 2020 06:23:07 GMT
ENV PHP_VERSION=7.4.13
# Thu, 17 Dec 2020 06:23:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.13.tar.xz.asc
# Thu, 17 Dec 2020 06:23:09 GMT
ENV PHP_SHA256=aead303e3abac23106529560547baebbedba0bb2943b91d5aa08fff1f41680f4
# Thu, 17 Dec 2020 06:23:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 06:23:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 06:28:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 06:28:17 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 17 Dec 2020 06:28:19 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 06:28:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 06:28:20 GMT
CMD ["php" "-a"]
# Thu, 17 Dec 2020 13:14:34 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 17 Dec 2020 13:14:37 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 17 Dec 2020 13:14:42 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 17 Dec 2020 13:14:46 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 17 Dec 2020 13:14:46 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 13:14:47 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 17 Dec 2020 13:14:48 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 17 Dec 2020 13:14:49 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 17 Dec 2020 13:14:53 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Thu, 17 Dec 2020 13:14:54 GMT
VOLUME [/var/www/html]
# Thu, 17 Dec 2020 13:14:54 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 17 Dec 2020 13:14:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:14:56 GMT
USER www-data
# Thu, 17 Dec 2020 13:14:56 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:ee52640a49e15b8b7c8edb66c2d048b26abdee8d828d6e5ef4e10a28cb15a84f`  
		Last Modified: Wed, 16 Dec 2020 23:42:15 GMT  
		Size: 2.6 MB (2567018 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b33a1a773ad25f9d9c6930913defa3b9196c1fdcd8d5a2d592215cda11cf944`  
		Last Modified: Thu, 17 Dec 2020 08:07:32 GMT  
		Size: 1.4 MB (1382756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b4721c450aa935167d123ebc6322a5f753171e457cd26615b6c8cea6dcc8648`  
		Last Modified: Thu, 17 Dec 2020 08:07:31 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e17cb6f51130bdca075886a326b2ea4010f9a422c82d02cdb21ff7fb1bcd6936`  
		Last Modified: Thu, 17 Dec 2020 08:07:31 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9ebbc899c15e91c45de79b49bbd360e4ddbc63b7488baea1ffbab3aa911f17e`  
		Last Modified: Thu, 17 Dec 2020 08:08:40 GMT  
		Size: 10.3 MB (10338583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b387b41e50db947745ad4bfba4d52b4064a9ea14762e81a16cbf295225842a72`  
		Last Modified: Thu, 17 Dec 2020 08:08:40 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53b844c8450b2d4b65f03149fa5eade999f38a1775ec2b9248168a239acc715f`  
		Last Modified: Thu, 17 Dec 2020 08:08:43 GMT  
		Size: 13.5 MB (13485998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5654c83cd9d5e80c918dbcbf236dd6fdd53303fbfdfe371089df32794501da`  
		Last Modified: Thu, 17 Dec 2020 08:08:40 GMT  
		Size: 2.3 KB (2260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee910f80d5b1e3cef0b873a0c99d7a5cdaf0d73383c29d99fcc859738ed3493e`  
		Last Modified: Thu, 17 Dec 2020 08:08:40 GMT  
		Size: 16.9 KB (16884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c73364484e2729c5671fe5981b25576744a10c752e376f585d075cb5454add`  
		Last Modified: Thu, 17 Dec 2020 13:19:03 GMT  
		Size: 6.8 MB (6794179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3527db933427933f50c7797012cd694be035cd36ba58d985f1f9b32d7c23a8c`  
		Last Modified: Thu, 17 Dec 2020 13:19:00 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb75868c93c91913a9c814c99baf1e8366c5cee6f74bdddb8b7389d389defc0`  
		Last Modified: Thu, 17 Dec 2020 13:19:02 GMT  
		Size: 9.8 MB (9755087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0437bc1bfd0e7a72bc05eaa4a8b6f54a4bdffe370b46dccdaa3366211e58a69c`  
		Last Modified: Thu, 17 Dec 2020 13:19:00 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44823961c5568748c16b0f52a1cd3fb7182af371e52404df78c6effeb0f25bd4`  
		Last Modified: Thu, 17 Dec 2020 13:19:01 GMT  
		Size: 1.2 MB (1205395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dace9b3d07888067be39d8bd30fbe33824ef197a8e59c6e8cf8230dd349a7bdd`  
		Last Modified: Thu, 17 Dec 2020 13:19:00 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
