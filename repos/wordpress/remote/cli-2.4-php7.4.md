## `wordpress:cli-2.4-php7.4`

```console
$ docker pull wordpress@sha256:d7a3024aa0c1776a48f71807a87c2efca106770c0e861b01ca8ac101b83a742a
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
$ docker pull wordpress@sha256:66cd2e3c7560b7923108547bcb0b315b5c33e08fdb970127593e4b708f8493e9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44312566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ebf7fca44cfcfca5692a7a456c5f56fa26f8eb19f9de6723c4c2f03dd734554`
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
# Thu, 25 Mar 2021 23:20:04 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 25 Mar 2021 23:20:05 GMT
ENV PHP_VERSION=7.4.16
# Thu, 25 Mar 2021 23:20:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Thu, 25 Mar 2021 23:20:05 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Thu, 25 Mar 2021 23:20:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 25 Mar 2021 23:20:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 25 Mar 2021 23:25:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 25 Mar 2021 23:25:57 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 25 Mar 2021 23:25:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 25 Mar 2021 23:25:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 25 Mar 2021 23:25:59 GMT
CMD ["php" "-a"]
# Fri, 26 Mar 2021 18:12:11 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 26 Mar 2021 18:12:13 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 26 Mar 2021 18:12:13 GMT
WORKDIR /var/www/html
# Sat, 27 Mar 2021 14:00:51 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 27 Mar 2021 14:00:52 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 27 Mar 2021 14:00:52 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Sat, 27 Mar 2021 14:00:53 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Sat, 27 Mar 2021 14:00:53 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Sat, 27 Mar 2021 14:00:55 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Sat, 27 Mar 2021 14:00:56 GMT
VOLUME [/var/www/html]
# Sat, 27 Mar 2021 14:00:56 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Sat, 27 Mar 2021 14:00:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 14:00:56 GMT
USER www-data
# Sat, 27 Mar 2021 14:00:56 GMT
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
	-	`sha256:f2ba0fadefcbafc405715685fb2e71bd05d198019f3ab4acb640552e35d58de0`  
		Last Modified: Fri, 26 Mar 2021 01:08:13 GMT  
		Size: 10.4 MB (10354094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:636a54b61db2d04da268472561ce8c4933a90cc59a9dd8011e397371f0c2b5eb`  
		Last Modified: Fri, 26 Mar 2021 01:08:12 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4910bcf8e655f6a6e44150b20e2a2cd6f03283b9d247b6e80c8ffaa8c4359b`  
		Last Modified: Fri, 26 Mar 2021 01:08:16 GMT  
		Size: 14.3 MB (14253523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:916259daac19a9deccfcff497c0ccb2e377296eed88caadd7cf7d65ec2b9274f`  
		Last Modified: Fri, 26 Mar 2021 01:08:12 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:964bb1b3446ab2806d02082165afa32cf432fe0102e477253a727d7d9da943a5`  
		Last Modified: Fri, 26 Mar 2021 01:08:12 GMT  
		Size: 17.5 KB (17513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66f0d4b7d9b774d180ce64bf3505c047bcf13488db99c71ebec68e0bafb5c168`  
		Last Modified: Fri, 26 Mar 2021 18:20:12 GMT  
		Size: 9.3 MB (9334505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97d703ade83d8b523dd11d1eae46a262dbe52e0b02d989d9223026e7d23329b5`  
		Last Modified: Fri, 26 Mar 2021 18:20:06 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f27e7237ff468171ad2c095b27e4375ada038314ad53eb28288326eca7743d6a`  
		Last Modified: Sat, 27 Mar 2021 14:08:47 GMT  
		Size: 4.6 MB (4635136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ec7b42fa36f76e4b39be1ffbd374fed4d4742d47a90db7263207c79c4344c11`  
		Last Modified: Sat, 27 Mar 2021 14:08:46 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e38cea2ee9bae3719a68d4116f8ba58fd2b196a8784c78e2f4779424efda6a7`  
		Last Modified: Sat, 27 Mar 2021 14:08:46 GMT  
		Size: 1.2 MB (1206061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bb923521bac7a010018bec1f1ce1d6520b5edf62c74fa45faad6d6db3bc99a7`  
		Last Modified: Sat, 27 Mar 2021 14:08:46 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4-php7.4` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:bff811ffc0f5cc9b7e35e376b08a1bf35d530ee2a3e6edccdc96aa9d1a31ebe9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42536511 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4139aa745ea36eb1c09cb9c8f590e8cfdc4f794db977ea2cb0da13c95d381ba`
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
# Wed, 31 Mar 2021 22:58:44 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Wed, 31 Mar 2021 22:58:45 GMT
ENV PHP_VERSION=7.4.16
# Wed, 31 Mar 2021 22:58:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Wed, 31 Mar 2021 22:58:47 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Wed, 31 Mar 2021 22:58:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 31 Mar 2021 22:58:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 23:04:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 23:04:30 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 31 Mar 2021 23:04:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 23:04:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 23:04:35 GMT
CMD ["php" "-a"]
# Thu, 01 Apr 2021 06:03:00 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 01 Apr 2021 06:03:03 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 01 Apr 2021 06:03:04 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 06:04:21 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 06:04:25 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 01 Apr 2021 06:04:27 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 01 Apr 2021 06:04:29 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 01 Apr 2021 06:04:30 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 01 Apr 2021 06:04:39 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 01 Apr 2021 06:04:44 GMT
VOLUME [/var/www/html]
# Thu, 01 Apr 2021 06:04:45 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 01 Apr 2021 06:04:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 06:04:48 GMT
USER www-data
# Thu, 01 Apr 2021 06:04:49 GMT
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
	-	`sha256:83f9adc6bded80e750a7e9ae68efeba5f28c85f9857bd88f38014e420f6aff60`  
		Last Modified: Thu, 01 Apr 2021 00:04:17 GMT  
		Size: 10.4 MB (10354070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a7f3446c2ed46218ba976971bcfa2b649685c0b0713c0ec94379eb188d4cc9a`  
		Last Modified: Thu, 01 Apr 2021 00:04:14 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473f7e3e57fb336fff28381d33fde6c1973e4c61c51f23cfe2d3ba9322da5ac4`  
		Last Modified: Thu, 01 Apr 2021 00:04:24 GMT  
		Size: 13.2 MB (13244278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6242e28c69b5e802b3e8cc5f12a2271b188fbe9519bc92f316cbd878dbaf5f`  
		Last Modified: Thu, 01 Apr 2021 00:04:14 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8cc46bec6d19cd67d87a9157cf8448b2ca30aabc5bda512720dfd52515f8c9f`  
		Last Modified: Thu, 01 Apr 2021 00:04:14 GMT  
		Size: 17.5 KB (17506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e355962249afe1fec54406a4a4b2a19bed3fb5b98c89763a4994c36acb5e3ee`  
		Last Modified: Thu, 01 Apr 2021 06:10:55 GMT  
		Size: 8.9 MB (8943838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb7ea36cd81e62446883b6aa230a842acb7f5847b1b2c3d93fd30e456044e01`  
		Last Modified: Thu, 01 Apr 2021 06:10:50 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ab2a8b4a8ef60162f5687887972b9dc7a5151886fcd84d7fc5821e2357ec45c`  
		Last Modified: Thu, 01 Apr 2021 06:10:52 GMT  
		Size: 4.5 MB (4458701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:175ff1d5504f66555958316a712a3eed14a4138dfabba3a1c166ab211d5b6be7`  
		Last Modified: Thu, 01 Apr 2021 06:10:50 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ceecb9277e177b5be6f03fec783b862b9d7f686a99a458c55c12ebd21cd143c`  
		Last Modified: Thu, 01 Apr 2021 06:10:51 GMT  
		Size: 1.2 MB (1206075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7deb1ad4a45ead66d2c47722ef35606020b0ae80363a171890da91eecffde310`  
		Last Modified: Thu, 01 Apr 2021 06:10:50 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4-php7.4` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:525aff59b5cf9f336a324d558750ed425e0eff2e1ab11ac850ed2f9f97ff0e2a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.8 MB (40783540 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31d9dc1a750f54e93bc45efeb982b7d3f01ea72c7a5702b120a80908012d56be`
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
# Fri, 26 Mar 2021 07:11:54 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 26 Mar 2021 07:11:54 GMT
ENV PHP_VERSION=7.4.16
# Fri, 26 Mar 2021 07:11:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Fri, 26 Mar 2021 07:11:56 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Fri, 26 Mar 2021 07:12:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 26 Mar 2021 07:12:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:15:06 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 26 Mar 2021 07:15:09 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:15:12 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Mar 2021 07:15:14 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Mar 2021 07:15:15 GMT
CMD ["php" "-a"]
# Fri, 26 Mar 2021 11:51:59 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 26 Mar 2021 11:52:01 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 26 Mar 2021 11:52:02 GMT
WORKDIR /var/www/html
# Sat, 27 Mar 2021 15:17:28 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 27 Mar 2021 15:17:31 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 27 Mar 2021 15:17:32 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Sat, 27 Mar 2021 15:17:34 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Sat, 27 Mar 2021 15:17:34 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Sat, 27 Mar 2021 15:17:39 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Sat, 27 Mar 2021 15:17:40 GMT
VOLUME [/var/www/html]
# Sat, 27 Mar 2021 15:17:41 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Sat, 27 Mar 2021 15:17:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 15:17:42 GMT
USER www-data
# Sat, 27 Mar 2021 15:17:43 GMT
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
	-	`sha256:41ec4d8944413145c1ebab07ad7654193dc4ca68b0791dbe277315ce3c5ca83e`  
		Last Modified: Fri, 26 Mar 2021 07:57:54 GMT  
		Size: 10.4 MB (10354080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b46d56b04bb557093fafb0d6d71ab394adabf086a42925e0ea4069a214355ec`  
		Last Modified: Fri, 26 Mar 2021 07:57:52 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82348165807b2693d9f8b864f0034e2bf16ef978e8ba06ad5502ab5cb0ba4e82`  
		Last Modified: Fri, 26 Mar 2021 07:57:56 GMT  
		Size: 12.4 MB (12406598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1759af3210519f0704e4c3571012a91052be85d2de692794309afe6bf06df9`  
		Last Modified: Fri, 26 Mar 2021 07:57:52 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:883a280418f5eaca79d94bc5112f0bfe1741e86410f72f1e79b2a45b03ce8106`  
		Last Modified: Fri, 26 Mar 2021 07:57:53 GMT  
		Size: 17.5 KB (17514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb6aff8ab9c599e0929a078b29ed24c72fccf6eefa0e058fe42f84f88a32a611`  
		Last Modified: Fri, 26 Mar 2021 12:00:51 GMT  
		Size: 8.7 MB (8661176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d68fa2154ed16db2591e638219cd15fd8fe30a23fa6aaeacbe5451a5275766b`  
		Last Modified: Fri, 26 Mar 2021 12:00:41 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75b884d993113635376f3582372bb91d6fdffc4880b2c4f1902b589846fa81c3`  
		Last Modified: Sat, 27 Mar 2021 15:24:13 GMT  
		Size: 4.2 MB (4153740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c9aef1a780a819bcb3f9c03f5725c87c83b02fa820adf543e0d81bef6482f5e`  
		Last Modified: Sat, 27 Mar 2021 15:24:11 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:062cf697f8c6d40a91db56d8a4b6f98363b78fe4ef20b3499f97e07220fe6781`  
		Last Modified: Sat, 27 Mar 2021 15:24:12 GMT  
		Size: 1.2 MB (1206061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa6d61b9ced830ee9aa4e3a091ee2510d99b049a00d1e8f54c0fcf5189d49417`  
		Last Modified: Sat, 27 Mar 2021 15:24:11 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4-php7.4` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:0f705342c3c35a5e44555947e3622a9b2cc4b2f0c099a3f4fa60e12fd057b680
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43882875 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab50845d013cbd2ea3edf92011986213baad6cc78efaead592dec94190347b3`
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
# Fri, 26 Mar 2021 04:05:34 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 26 Mar 2021 04:05:35 GMT
ENV PHP_VERSION=7.4.16
# Fri, 26 Mar 2021 04:05:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Fri, 26 Mar 2021 04:05:36 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Fri, 26 Mar 2021 04:05:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 26 Mar 2021 04:05:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:09:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 26 Mar 2021 04:09:40 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 26 Mar 2021 04:09:44 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Mar 2021 04:09:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Mar 2021 04:09:45 GMT
CMD ["php" "-a"]
# Fri, 26 Mar 2021 18:04:14 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 26 Mar 2021 18:04:20 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 26 Mar 2021 18:04:21 GMT
WORKDIR /var/www/html
# Sat, 27 Mar 2021 11:56:02 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 27 Mar 2021 11:56:05 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 27 Mar 2021 11:56:06 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Sat, 27 Mar 2021 11:56:07 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Sat, 27 Mar 2021 11:56:08 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Sat, 27 Mar 2021 11:56:13 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Sat, 27 Mar 2021 11:56:15 GMT
VOLUME [/var/www/html]
# Sat, 27 Mar 2021 11:56:16 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Sat, 27 Mar 2021 11:56:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 11:56:18 GMT
USER www-data
# Sat, 27 Mar 2021 11:56:19 GMT
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
	-	`sha256:6b489ea7fa61692e18cb5ad6027adb0eff01e8ab187e737f6f039bf10ca74d66`  
		Last Modified: Fri, 26 Mar 2021 05:12:49 GMT  
		Size: 10.4 MB (10354098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b24bc7dab07bac5fcd8739bec236a7fc9900ace7e6f1770e7d093e1bc0becc63`  
		Last Modified: Fri, 26 Mar 2021 05:12:48 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6bfa818cc4e3ce466e72a57e0ef01acd05068317ce8b28ddd6ba5d33db4aeb`  
		Last Modified: Fri, 26 Mar 2021 05:12:52 GMT  
		Size: 14.0 MB (14027217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d190148a9d1de133a3caa152f92acca1905c41fcc3d02ca84c8ffda87cc5255`  
		Last Modified: Fri, 26 Mar 2021 05:12:48 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aabeec78b08640d655304c6b4412835c24cd66167400cb174b7369ea6addbfa4`  
		Last Modified: Fri, 26 Mar 2021 05:12:48 GMT  
		Size: 17.5 KB (17530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8fe16aaf82d6504d9e63230304e8f853200932bdb9cd1fe9cb65627ceb8282`  
		Last Modified: Fri, 26 Mar 2021 18:12:40 GMT  
		Size: 9.4 MB (9403207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7d5b3f5f671a49744ee7ceb96696a1e2f849651d57de4b1bf6bd1ea29e10e96`  
		Last Modified: Fri, 26 Mar 2021 18:12:35 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:018d67564bc43dbc8445262b2b7596fcf5aa9aecdaba7ce8fea1660c6cacec73`  
		Last Modified: Sat, 27 Mar 2021 12:03:37 GMT  
		Size: 4.5 MB (4463111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b4d79b80a878c8afec4978f1fdbaa436fb442699d12e25d8be75d7a170063c9`  
		Last Modified: Sat, 27 Mar 2021 12:03:36 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc0bb6cf36ca914432cae3da2431d2f5b30f1605d4ca7927e36821888d5cc878`  
		Last Modified: Sat, 27 Mar 2021 12:03:36 GMT  
		Size: 1.2 MB (1206062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d2f429fb2b981e5b3d1750225f9ebfffa6f6841facc369a7bf59e9b04d95d7`  
		Last Modified: Sat, 27 Mar 2021 12:03:36 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4-php7.4` - linux; 386

```console
$ docker pull wordpress@sha256:c26880d8293396e2586960a5cd5012c78a454a19af558577c4e3e681eb3a40f0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.1 MB (45119094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5adeea501b16f810543cb71caeffb9460b3a1e4e192eb41d070ac2c8f13bb0d`
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
# Thu, 01 Apr 2021 03:15:31 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Apr 2021 03:15:31 GMT
ENV PHP_VERSION=7.4.16
# Thu, 01 Apr 2021 03:15:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Thu, 01 Apr 2021 03:15:32 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Thu, 01 Apr 2021 03:15:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 03:15:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:22:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 03:22:02 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 01 Apr 2021 03:22:04 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 03:22:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 03:22:05 GMT
CMD ["php" "-a"]
# Thu, 01 Apr 2021 10:36:27 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 01 Apr 2021 10:36:28 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 01 Apr 2021 10:36:28 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 10:37:21 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 10:37:21 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 01 Apr 2021 10:37:22 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 01 Apr 2021 10:37:22 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 01 Apr 2021 10:37:22 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 01 Apr 2021 10:37:37 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 01 Apr 2021 10:37:37 GMT
VOLUME [/var/www/html]
# Thu, 01 Apr 2021 10:37:37 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 01 Apr 2021 10:37:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 10:37:38 GMT
USER www-data
# Thu, 01 Apr 2021 10:37:38 GMT
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
	-	`sha256:66b36eb2a5730c967902742634417f87e6565eb6623b0f9d4ad6920f9a331be4`  
		Last Modified: Thu, 01 Apr 2021 04:44:34 GMT  
		Size: 10.4 MB (10354070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1866215f4e22f1c527eaa78b5048398800a7f6ae83761d678d2ac9d28594a73f`  
		Last Modified: Thu, 01 Apr 2021 04:44:32 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de52964447f5dee09ae162f698b8aec7cc24c128cc7192579f219d77b5b05e7b`  
		Last Modified: Thu, 01 Apr 2021 04:44:37 GMT  
		Size: 14.6 MB (14630258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d82dd6c8e9b5fa5096dbed5adb0ac5e72d7be8418d445d894fb93623216f6ee4`  
		Last Modified: Thu, 01 Apr 2021 04:44:33 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2631eea095f9a398e8e593976afffb3bd5b2d9531c4d77880a205cb7891e75`  
		Last Modified: Thu, 01 Apr 2021 04:44:33 GMT  
		Size: 17.5 KB (17508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a3e3926b875b9a50305aedc3f838c2582b53ce0609e215e54e8a0c56a5b677`  
		Last Modified: Thu, 01 Apr 2021 10:47:12 GMT  
		Size: 9.5 MB (9498620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2a8602247c952c389cfb136e5ad43cf0d6f59cd524ed5d5185fa3bff3ee89d0`  
		Last Modified: Thu, 01 Apr 2021 10:47:03 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81295844136c3cb531095ea6f80883bc432b45f17d61d87ffb4dcad63ae2bbc9`  
		Last Modified: Thu, 01 Apr 2021 10:47:06 GMT  
		Size: 4.8 MB (4794834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1ecab41b74f35fddcb0f71586112f70754786e0a93c0eb9786d0d0982edc262`  
		Last Modified: Thu, 01 Apr 2021 10:47:03 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ec21d9850405d261d677c797327ed64b7fb7b64ff9dd5c0024ea1ce3af24f53`  
		Last Modified: Thu, 01 Apr 2021 10:47:04 GMT  
		Size: 1.2 MB (1206063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174c40b0deda0db0a408a840a567fd903b2f639e790ba1b16f8de0f6fd4e17d6`  
		Last Modified: Thu, 01 Apr 2021 10:47:05 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4-php7.4` - linux; ppc64le

```console
$ docker pull wordpress@sha256:4191e4a29a3faf83285c9a07b64be02a2f087efd169cc655b4ebf7b6e4133477
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.7 MB (45673394 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d1734cbe204bb35a81eb760ed1eaccaaa13bf63c56ca9622d1954eadc5c0807`
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
# Fri, 26 Mar 2021 12:45:33 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 26 Mar 2021 12:45:38 GMT
ENV PHP_VERSION=7.4.16
# Fri, 26 Mar 2021 12:45:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Fri, 26 Mar 2021 12:45:51 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Fri, 26 Mar 2021 12:46:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 26 Mar 2021 12:46:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:51:21 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 26 Mar 2021 12:51:40 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:52:16 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Mar 2021 12:52:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Mar 2021 12:52:21 GMT
CMD ["php" "-a"]
# Sat, 27 Mar 2021 04:30:43 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Sat, 27 Mar 2021 04:30:59 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Sat, 27 Mar 2021 04:31:05 GMT
WORKDIR /var/www/html
# Sat, 27 Mar 2021 04:32:25 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 27 Mar 2021 04:32:32 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 27 Mar 2021 04:32:36 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Sat, 27 Mar 2021 04:32:39 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Sat, 27 Mar 2021 04:32:42 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Sat, 27 Mar 2021 04:32:56 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Sat, 27 Mar 2021 04:32:58 GMT
VOLUME [/var/www/html]
# Sat, 27 Mar 2021 04:33:00 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Sat, 27 Mar 2021 04:33:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 04:33:07 GMT
USER www-data
# Sat, 27 Mar 2021 04:33:11 GMT
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
	-	`sha256:3aacdb89ca82aa62fa0e33619332328e8f4631909ed6dd30dd76e52c1e589d50`  
		Last Modified: Fri, 26 Mar 2021 14:06:26 GMT  
		Size: 10.4 MB (10354079 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b33d859b946d78eac34f637f694e86386205b4b6640383bbbb9716f88c1117`  
		Last Modified: Fri, 26 Mar 2021 14:06:26 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98ed23ec5538344340107c55e798bcea7808960780845045fb527ad2f8c47c5d`  
		Last Modified: Fri, 26 Mar 2021 14:06:26 GMT  
		Size: 15.3 MB (15281497 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c295008d48fe6d51872d8d11a89468bad391e300bf0d6ee7d5cba91656482f5`  
		Last Modified: Fri, 26 Mar 2021 14:06:23 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b4e1972ce75552b8d64cc52238464f7803e652f1cd6dad3bbcb1e720eec4c3a`  
		Last Modified: Fri, 26 Mar 2021 14:06:23 GMT  
		Size: 17.5 KB (17525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2610e6ce50cf71773acc63c4ec83b86f330c23382a17d1e1ba3b7d9427198345`  
		Last Modified: Sat, 27 Mar 2021 04:45:43 GMT  
		Size: 9.5 MB (9530699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fd5b7600565afa2d5a7a53b5a14352b7749476337e634b68238472299f879f`  
		Last Modified: Sat, 27 Mar 2021 04:45:38 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d0130d6bd7f824f5f36257b8ed219d0062894b0c70e6ffab8412878f27c3978`  
		Last Modified: Sat, 27 Mar 2021 04:45:39 GMT  
		Size: 4.7 MB (4723401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8964ec641eb111c8278c5f90103f4bea4fc615bfce88bc3a37ab051de04345e5`  
		Last Modified: Sat, 27 Mar 2021 04:45:38 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c79536a01d623f38ae12fe9c78cc28daf29f178293756098787e0d0a682993`  
		Last Modified: Sat, 27 Mar 2021 04:45:38 GMT  
		Size: 1.2 MB (1206086 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf79ba2be1217fb5e9773a47d599987a5276761f89faf8614df371ed256991d0`  
		Last Modified: Sat, 27 Mar 2021 04:45:38 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4-php7.4` - linux; s390x

```console
$ docker pull wordpress@sha256:9590c24b289ffe4097d9c3ddc5e24df872ab881d4d085f93355fe03c4fe8a45a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.0 MB (43993250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b37c811ce2b78ba029d22a5bd9c5ca338063f4d93b12f20cefd94b8c6504c3`
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
# Thu, 01 Apr 2021 01:27:46 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Apr 2021 01:27:46 GMT
ENV PHP_VERSION=7.4.16
# Thu, 01 Apr 2021 01:27:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.16.tar.xz.asc
# Thu, 01 Apr 2021 01:27:46 GMT
ENV PHP_SHA256=1c16cefaf88ded4c92eed6a8a41eb682bb2ef42429deb55f1c4ba159053fb98b
# Thu, 01 Apr 2021 01:27:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 01:27:50 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 01:31:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 01:31:05 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 01 Apr 2021 01:31:06 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 01:31:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 01:31:06 GMT
CMD ["php" "-a"]
# Thu, 01 Apr 2021 05:19:02 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 01 Apr 2021 05:19:04 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 01 Apr 2021 05:19:05 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 05:19:38 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 05:19:40 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 01 Apr 2021 05:19:40 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 01 Apr 2021 05:19:40 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 01 Apr 2021 05:19:40 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 01 Apr 2021 05:19:42 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 01 Apr 2021 05:19:43 GMT
VOLUME [/var/www/html]
# Thu, 01 Apr 2021 05:19:43 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 01 Apr 2021 05:19:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 05:19:43 GMT
USER www-data
# Thu, 01 Apr 2021 05:19:43 GMT
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
	-	`sha256:e515f9f5249062a4fc8d6e07d019c560c99ae41742cf32c3c2519b5e0b26d626`  
		Last Modified: Thu, 01 Apr 2021 02:26:51 GMT  
		Size: 10.4 MB (10354073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1efb1722ee5c22acb127fe85a7f66e7e8c35e19e3390e271826a82157710d8`  
		Last Modified: Thu, 01 Apr 2021 02:26:51 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1df2f39a25175e1434592aa615bedee03b8b2fed57d8e6f040e471353f91084`  
		Last Modified: Thu, 01 Apr 2021 02:26:52 GMT  
		Size: 13.6 MB (13613285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20ecd4d9518eaeb834d279ec2b0f5bae47c80d24d0554ee70e40c34db1b94f88`  
		Last Modified: Thu, 01 Apr 2021 02:26:51 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7896c108a811ec59ae2d15cbf45b6c5882d6752043717e7dba6b3776dc035868`  
		Last Modified: Thu, 01 Apr 2021 02:26:50 GMT  
		Size: 17.5 KB (17511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30273a251f304f2b63ccbdf1787c863476f344a35ba6319b3fe5854e2633a37d`  
		Last Modified: Thu, 01 Apr 2021 05:23:36 GMT  
		Size: 9.8 MB (9830232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09b6e153ee115fa8b8d6b34da5e5852c3aee4008a7c688fd1cc2dd9fd3c08d75`  
		Last Modified: Thu, 01 Apr 2021 05:23:32 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2df078af79e2fe07ce22f3e9ab2094b9d4f9a19de60622ce4ec4ee85480d331`  
		Last Modified: Thu, 01 Apr 2021 05:23:33 GMT  
		Size: 4.6 MB (4607783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc910da5e56e7db705bf2646db942b7ff5279bb40c9db1fc83ea8cded0a5804b`  
		Last Modified: Thu, 01 Apr 2021 05:23:32 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6297861752365605ed07da6d97bd304fe48661dee4e083e0bc5b60242fa6d9`  
		Last Modified: Thu, 01 Apr 2021 05:23:33 GMT  
		Size: 1.2 MB (1206058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c29043fca7aed7e7314033118aaae99c442cf8e5e7152363a5df0c67a1447f1`  
		Last Modified: Thu, 01 Apr 2021 05:23:32 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
