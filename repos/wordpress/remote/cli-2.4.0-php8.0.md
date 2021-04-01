## `wordpress:cli-2.4.0-php8.0`

```console
$ docker pull wordpress@sha256:1c66b6e56f1c4370571d473c7f940dbcea0805eb0ac03fa9236b0ec3db2335aa
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

### `wordpress:cli-2.4.0-php8.0` - linux; amd64

```console
$ docker pull wordpress@sha256:4062c4d9b04b41fc5870fd9a6da00a83ca73e6bacb869858a3ff0a75e0742c90
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.0 MB (41958389 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ac923e2c2f3f6f81295beeda1b8202c2620c5e87a1c8961f14850f6f9362745`
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
# Thu, 25 Mar 2021 22:52:05 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 25 Mar 2021 22:52:05 GMT
ENV PHP_VERSION=8.0.3
# Thu, 25 Mar 2021 22:52:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 25 Mar 2021 22:52:05 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 25 Mar 2021 22:52:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 25 Mar 2021 22:52:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 25 Mar 2021 22:58:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 25 Mar 2021 22:58:53 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 25 Mar 2021 22:58:54 GMT
RUN docker-php-ext-enable sodium
# Thu, 25 Mar 2021 22:58:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 25 Mar 2021 22:58:55 GMT
CMD ["php" "-a"]
# Fri, 26 Mar 2021 18:15:02 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 26 Mar 2021 18:15:03 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 26 Mar 2021 18:15:03 GMT
WORKDIR /var/www/html
# Fri, 26 Mar 2021 18:15:58 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 26 Mar 2021 18:15:59 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 26 Mar 2021 18:15:59 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 26 Mar 2021 18:15:59 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Fri, 26 Mar 2021 18:16:00 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Fri, 26 Mar 2021 18:16:03 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 26 Mar 2021 18:16:03 GMT
VOLUME [/var/www/html]
# Fri, 26 Mar 2021 18:16:03 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:16:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 18:16:04 GMT
USER www-data
# Fri, 26 Mar 2021 18:16:04 GMT
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
	-	`sha256:483f3f97a5bcb32f77f902da843392163e0b95ddf993c10a5b44aa7a63d2063b`  
		Last Modified: Fri, 26 Mar 2021 01:05:18 GMT  
		Size: 10.8 MB (10775190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e078e9d6b760b6690e02ae66107269a2d35faa80dacef6f2d00a7792f1bf7c7a`  
		Last Modified: Fri, 26 Mar 2021 01:05:16 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c134042be4098f28eae1d619deca5adb1f2c85babe782d8a89a0bcb1de65714`  
		Last Modified: Fri, 26 Mar 2021 01:05:21 GMT  
		Size: 15.0 MB (14950323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db5fecf1aa2d2da049d43e7b0095f0c7052ade3f0bf64963f296f314c51df53e`  
		Last Modified: Fri, 26 Mar 2021 01:05:17 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f28c38a75bec88d24962cb60dcd1e0c739d8bc930182f5c5b3ab05ba507b7214`  
		Last Modified: Fri, 26 Mar 2021 01:05:16 GMT  
		Size: 17.5 KB (17510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbb37515208982f502ca3a023edcaa9f3a7d9d6171b9c0fa1bc15f17fb767f37`  
		Last Modified: Fri, 26 Mar 2021 18:21:22 GMT  
		Size: 9.3 MB (9334503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:413ab16dc120864d229245ed1a5b36ef07879c6f958c23183fbb80ff5c95402d`  
		Last Modified: Fri, 26 Mar 2021 18:21:16 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d65bf877a50e998ad36f6d8dc22ae2eed82f7c41a6a57f279080a03e13af590`  
		Last Modified: Fri, 26 Mar 2021 18:21:18 GMT  
		Size: 1.2 MB (1172877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f45284cd17e87eba4b0a1023dab50e732dc78b3bb362966d52da2d72b918ba2`  
		Last Modified: Fri, 26 Mar 2021 18:21:16 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01072b9a3721d2f25ee48b4171e4944ab2fc4b4b634c7a56193636c5c6163d57`  
		Last Modified: Fri, 26 Mar 2021 18:21:17 GMT  
		Size: 1.2 MB (1196255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b11203c8e670fc070e73e6712071f68f4da86015bab75c1207b58aa1b4cdaa`  
		Last Modified: Fri, 26 Mar 2021 18:21:19 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4.0-php8.0` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:029a9159e55c9843b263c6e49c634c9b0833b8ce260d3d618c58d78ce074c27e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39893715 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa29ff1571babe55f27000965280ef35c0b160c401611193bf328856621e7fd5`
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
# Wed, 31 Mar 2021 22:37:21 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 31 Mar 2021 22:37:22 GMT
ENV PHP_VERSION=8.0.3
# Wed, 31 Mar 2021 22:37:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Wed, 31 Mar 2021 22:37:23 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Wed, 31 Mar 2021 22:37:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 31 Mar 2021 22:37:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 31 Mar 2021 22:42:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 31 Mar 2021 22:42:33 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Wed, 31 Mar 2021 22:42:40 GMT
RUN docker-php-ext-enable sodium
# Wed, 31 Mar 2021 22:42:42 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 31 Mar 2021 22:42:43 GMT
CMD ["php" "-a"]
# Thu, 01 Apr 2021 06:07:37 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 01 Apr 2021 06:07:41 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 01 Apr 2021 06:07:43 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 06:08:35 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 06:08:38 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 01 Apr 2021 06:08:39 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 01 Apr 2021 06:08:39 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 01 Apr 2021 06:08:40 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 01 Apr 2021 06:08:45 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 01 Apr 2021 06:08:45 GMT
VOLUME [/var/www/html]
# Thu, 01 Apr 2021 06:08:46 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 01 Apr 2021 06:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 06:08:48 GMT
USER www-data
# Thu, 01 Apr 2021 06:08:49 GMT
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
	-	`sha256:fbcda67aa7c1950b8e998569bde08b6c9081c09f7962e3c02686633b4e3bccf8`  
		Last Modified: Thu, 01 Apr 2021 00:01:46 GMT  
		Size: 10.8 MB (10775169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88cb83dcd27c456011988703627db7a36c7397dfe9559e04686cd241d702507a`  
		Last Modified: Thu, 01 Apr 2021 00:01:42 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b41fa81b4d70176dd27767491d052195000a01d0901383deac69f84d1c7baff`  
		Last Modified: Thu, 01 Apr 2021 00:01:51 GMT  
		Size: 13.6 MB (13585364 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38f25e307c7ea4dc9cab6903716513ff9ca4741403d6035f29a97a7d553ebbc9`  
		Last Modified: Thu, 01 Apr 2021 00:01:41 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de3ecec900ef5e9f4544e0dd136517037c9f0511817d133acf498156c0c9263`  
		Last Modified: Thu, 01 Apr 2021 00:01:40 GMT  
		Size: 17.5 KB (17509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7cd8184066b4f0d8972f060e901c92be24c54b115d58f90edab0a08da6eb039`  
		Last Modified: Thu, 01 Apr 2021 06:11:35 GMT  
		Size: 8.9 MB (8943830 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6bdf8cb60479489579f56a79e9c2cc842ece36a1d7e1147b57170a662208d53`  
		Last Modified: Thu, 01 Apr 2021 06:11:30 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7df329b5d26fdeaa158064b1abd61d3205934bcfbf2207b0854a85da41705e`  
		Last Modified: Thu, 01 Apr 2021 06:11:30 GMT  
		Size: 1.1 MB (1063549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e1d9646753e9cc7402f1f5419feea09100347216ee4c3505004550a423a2cc`  
		Last Modified: Thu, 01 Apr 2021 06:11:30 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90dc51395812ac3b2a5591a54636a448ed1b55b99b4623339cda0db1a21e1346`  
		Last Modified: Thu, 01 Apr 2021 06:11:30 GMT  
		Size: 1.2 MB (1196245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2a78d51eefd43276ae5c7e2345777e849c70561e70301048bd06890573c040`  
		Last Modified: Thu, 01 Apr 2021 06:11:30 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4.0-php8.0` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:7a29b8bf6ef456eec82cc8832c0858cb3178b0319936119d3185dbff7edd2094
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.3 MB (38335742 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63e043a68d9a980694652fe12091baac6b99d8a67436fc6e9c1db05a1494795f`
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
# Fri, 26 Mar 2021 06:57:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 26 Mar 2021 06:57:11 GMT
ENV PHP_VERSION=8.0.3
# Fri, 26 Mar 2021 06:57:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Fri, 26 Mar 2021 06:57:13 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Fri, 26 Mar 2021 06:57:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 26 Mar 2021 06:57:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:00:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 26 Mar 2021 07:00:24 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 26 Mar 2021 07:00:29 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Mar 2021 07:00:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Mar 2021 07:00:31 GMT
CMD ["php" "-a"]
# Fri, 26 Mar 2021 11:56:41 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 26 Mar 2021 11:56:44 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 26 Mar 2021 11:56:46 GMT
WORKDIR /var/www/html
# Fri, 26 Mar 2021 11:57:35 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 26 Mar 2021 11:57:38 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 26 Mar 2021 11:57:39 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 26 Mar 2021 11:57:39 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Fri, 26 Mar 2021 11:57:40 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Fri, 26 Mar 2021 11:57:46 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 26 Mar 2021 11:57:47 GMT
VOLUME [/var/www/html]
# Fri, 26 Mar 2021 11:57:48 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 26 Mar 2021 11:57:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 11:57:49 GMT
USER www-data
# Fri, 26 Mar 2021 11:57:50 GMT
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
	-	`sha256:15dcd8a2af36e527243e6357083f4e15c8c480c0ab8e3bfdd9ea6a9e8bdc1c9a`  
		Last Modified: Fri, 26 Mar 2021 07:56:01 GMT  
		Size: 10.8 MB (10775170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66328c63f9613b64c5a51ac9105551351b5acd84e166c0e1470a026638412d59`  
		Last Modified: Fri, 26 Mar 2021 07:56:00 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:854233c883fb0f54ae096072430bc6a7295b3623d6467cbf436f277cdcb456b3`  
		Last Modified: Fri, 26 Mar 2021 07:56:04 GMT  
		Size: 12.7 MB (12732753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3008ba97dacdfbdf8ad932dc6f8df69ea3613ec4ef6c7e661aff5b3140a1d337`  
		Last Modified: Fri, 26 Mar 2021 07:56:00 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85000bd3ddfb263aa452b8e550e0fea4b53975629b7e01bc27f4b0137e664d7d`  
		Last Modified: Fri, 26 Mar 2021 07:56:00 GMT  
		Size: 17.5 KB (17512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d61b2650aad9639b37148fe4035a6913859b8f327d00ff642e3e4aaa4fda06`  
		Last Modified: Fri, 26 Mar 2021 12:01:31 GMT  
		Size: 8.7 MB (8661142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94216e8313aea1eafe92b5439fc4f0883432a7597eaada0c274b63307baf0114`  
		Last Modified: Fri, 26 Mar 2021 12:01:27 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a50765b9bfdb7e0a60eb8d4964d0d62991a0c8f78d8b1a05b4f4c8cb09c1351`  
		Last Modified: Fri, 26 Mar 2021 12:01:27 GMT  
		Size: 968.6 KB (968564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5a8dd4a563f7904802a5cf711e881da56c567537e108835148907569b8431ab`  
		Last Modified: Fri, 26 Mar 2021 12:01:26 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b146c3259d5dda2b9a4135cdc1b6d294d680248d13a2f6da5543be33428e5ccd`  
		Last Modified: Fri, 26 Mar 2021 12:01:27 GMT  
		Size: 1.2 MB (1196241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd8e98cd0ee4e0389e18a09045b07536c2557622dc5d1e151a6acf4832e4e6c`  
		Last Modified: Fri, 26 Mar 2021 12:01:27 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4.0-php8.0` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:df0f2bafdf83a4e8af0c28d8ee188a849b9933b3e5e62882ec91dc689ba865cb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41328888 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db1f77276d7616f406e7eb1da47cb19289f1784730e22b3033af3b7e98161478`
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
# Fri, 26 Mar 2021 03:48:09 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 26 Mar 2021 03:48:10 GMT
ENV PHP_VERSION=8.0.3
# Fri, 26 Mar 2021 03:48:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Fri, 26 Mar 2021 03:48:11 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Fri, 26 Mar 2021 03:48:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 26 Mar 2021 03:48:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Mar 2021 03:52:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 26 Mar 2021 03:52:18 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 26 Mar 2021 03:52:23 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Mar 2021 03:52:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Mar 2021 03:52:25 GMT
CMD ["php" "-a"]
# Fri, 26 Mar 2021 18:08:05 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 26 Mar 2021 18:08:08 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 26 Mar 2021 18:08:09 GMT
WORKDIR /var/www/html
# Fri, 26 Mar 2021 18:09:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 26 Mar 2021 18:09:08 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 26 Mar 2021 18:09:09 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 26 Mar 2021 18:09:10 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Fri, 26 Mar 2021 18:09:11 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Fri, 26 Mar 2021 18:09:17 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 26 Mar 2021 18:09:19 GMT
VOLUME [/var/www/html]
# Fri, 26 Mar 2021 18:09:20 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 26 Mar 2021 18:09:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 26 Mar 2021 18:09:23 GMT
USER www-data
# Fri, 26 Mar 2021 18:09:25 GMT
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
	-	`sha256:dd668848e734b4818f94d3ce37a652e08b53a42d01ee40449d9f356e82bc3399`  
		Last Modified: Fri, 26 Mar 2021 05:10:48 GMT  
		Size: 10.8 MB (10775195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:591a8904db45f81525c8c9d9110e160786bd97b922996b99ecb1c86c9be9e9bb`  
		Last Modified: Fri, 26 Mar 2021 05:10:46 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3be55e0cbdd68084d435a1bd3bee6d9ad5f8e1ada318bef734aefaa69e472c8a`  
		Last Modified: Fri, 26 Mar 2021 05:10:52 GMT  
		Size: 14.4 MB (14377500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b35a9b824a1f9cdaa385503b216cc1211b8a7789e9be41552ed033507b41bd08`  
		Last Modified: Fri, 26 Mar 2021 05:10:46 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fca769742f8c46bf1bf5407c7a2affe8759582260b9a72156b597c688287bad5`  
		Last Modified: Fri, 26 Mar 2021 05:10:46 GMT  
		Size: 17.5 KB (17528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc1e778e78a87791a022637cc658862e8e4454e0080b57939599bb4b6c07c73`  
		Last Modified: Fri, 26 Mar 2021 18:13:17 GMT  
		Size: 9.4 MB (9403166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9964de58ec715b8f77be0bed8aaae9c601a1de19a20a4c943539941e6696687`  
		Last Modified: Fri, 26 Mar 2021 18:13:14 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b99d673db91781c60be153c5f6748a96b7e9544f9fa95d04d4bf95c327a32149`  
		Last Modified: Fri, 26 Mar 2021 18:13:13 GMT  
		Size: 1.1 MB (1147609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:444610d7d4474609f8e94c79ae39eda7b25640829a59e1079ae306476666ac58`  
		Last Modified: Fri, 26 Mar 2021 18:13:13 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c60363a9bb0c16537806142be5f3776776f5fdd9114423f4421bfb42d2e138f`  
		Last Modified: Fri, 26 Mar 2021 18:13:13 GMT  
		Size: 1.2 MB (1196249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03eb1fb5700f08e40a9a745bf429b48d97199533cfb52a645a588e500e43f97`  
		Last Modified: Fri, 26 Mar 2021 18:13:13 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4.0-php8.0` - linux; 386

```console
$ docker pull wordpress@sha256:4079ea4c28081204a434c9719354cf569959a8d6b578bccb8eed4ece5bdf5f34
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.3 MB (42317566 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6acc80a12e804b8e2dadd26ba45ab2c91f0b24f69681f1fc01183758f4ced22`
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
# Thu, 01 Apr 2021 02:49:05 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Apr 2021 02:49:05 GMT
ENV PHP_VERSION=8.0.3
# Thu, 01 Apr 2021 02:49:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 01 Apr 2021 02:49:06 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 01 Apr 2021 02:49:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 02:49:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 02:55:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 02:55:37 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 01 Apr 2021 02:55:39 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 02:55:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 02:55:39 GMT
CMD ["php" "-a"]
# Thu, 01 Apr 2021 10:39:07 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 01 Apr 2021 10:39:08 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 01 Apr 2021 10:39:08 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 10:39:41 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 10:39:42 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 01 Apr 2021 10:39:42 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 01 Apr 2021 10:39:42 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 01 Apr 2021 10:39:42 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 01 Apr 2021 10:39:45 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 01 Apr 2021 10:39:45 GMT
VOLUME [/var/www/html]
# Thu, 01 Apr 2021 10:39:46 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 01 Apr 2021 10:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 10:39:46 GMT
USER www-data
# Thu, 01 Apr 2021 10:39:46 GMT
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
	-	`sha256:481735f9f9641e0e6ad09dfebbe4b5a8f755d17622bba26fc9965a28f5f39722`  
		Last Modified: Thu, 01 Apr 2021 04:41:11 GMT  
		Size: 10.8 MB (10775157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7638dc8ae8cf3f6710b678fc1d9760d1d3dedc5a93a0f3ba36de8ac138c17c9`  
		Last Modified: Thu, 01 Apr 2021 04:41:09 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc1c7edadcf6c2620deef76b775c3539eb02def7a711af99d5b9fee4c0ab8704`  
		Last Modified: Thu, 01 Apr 2021 04:41:14 GMT  
		Size: 15.0 MB (14974526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d02c68d2aaa7ce235ac7964874a4b414e2baf705bb55d3c1ad9c69cdacd35124`  
		Last Modified: Thu, 01 Apr 2021 04:41:09 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6554c8a47e39798355b0118a124e05cbe8b355110a94e7322db96b1b43220741`  
		Last Modified: Thu, 01 Apr 2021 04:41:09 GMT  
		Size: 17.5 KB (17506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:584426d548ae69b1dc6fa1784bc1b25551dcc34b342ebcca4dee6b79f096a9be`  
		Last Modified: Thu, 01 Apr 2021 10:48:29 GMT  
		Size: 9.5 MB (9498568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94d469e4d27bf03a228dc834cd43e17550599605dd38e7234b7a35c8db90a7c7`  
		Last Modified: Thu, 01 Apr 2021 10:48:22 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2e67e6e4d2d2fce7d471d70d48b34f536a22c0bb3420dc30592c31324a2fe3`  
		Last Modified: Thu, 01 Apr 2021 10:48:23 GMT  
		Size: 1.2 MB (1237839 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84952b28e04a4bb40bf5375a35fe5bf383d80f2785631854522acdff9c05cbc9`  
		Last Modified: Thu, 01 Apr 2021 10:48:23 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a301c8baf970539ff452265b805ce9248ebd63715993c1d9a198149ebe170a`  
		Last Modified: Thu, 01 Apr 2021 10:48:23 GMT  
		Size: 1.2 MB (1196229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cfb1a2bdfd70a2ae3359c831633909110bede55bcd876f3e323fb7ca6af037`  
		Last Modified: Thu, 01 Apr 2021 10:48:22 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4.0-php8.0` - linux; ppc64le

```console
$ docker pull wordpress@sha256:986ac323bca498bbf999864423e2f57421ccbcb03c6f83720f5d06e2d29c9541
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43005546 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8496b09108c7fa50177e3989c7c8f9b446a28553590d16ed5a3af648b69326e3`
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
# Fri, 26 Mar 2021 12:18:05 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 26 Mar 2021 12:18:08 GMT
ENV PHP_VERSION=8.0.3
# Fri, 26 Mar 2021 12:18:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Fri, 26 Mar 2021 12:18:19 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Fri, 26 Mar 2021 12:18:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 26 Mar 2021 12:18:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:23:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 26 Mar 2021 12:23:58 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 26 Mar 2021 12:24:11 GMT
RUN docker-php-ext-enable sodium
# Fri, 26 Mar 2021 12:24:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 26 Mar 2021 12:24:21 GMT
CMD ["php" "-a"]
# Sat, 27 Mar 2021 04:36:45 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Sat, 27 Mar 2021 04:36:55 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Sat, 27 Mar 2021 04:36:57 GMT
WORKDIR /var/www/html
# Sat, 27 Mar 2021 04:37:56 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Sat, 27 Mar 2021 04:38:05 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 27 Mar 2021 04:38:08 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Sat, 27 Mar 2021 04:38:12 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Sat, 27 Mar 2021 04:38:19 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Sat, 27 Mar 2021 04:38:30 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Sat, 27 Mar 2021 04:38:33 GMT
VOLUME [/var/www/html]
# Sat, 27 Mar 2021 04:38:34 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Sat, 27 Mar 2021 04:38:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 27 Mar 2021 04:38:43 GMT
USER www-data
# Sat, 27 Mar 2021 04:38:47 GMT
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
	-	`sha256:2293416441f59c8bb82509f958f3a280c94d3239131fc89ed938cd14ec1d931d`  
		Last Modified: Fri, 26 Mar 2021 14:03:38 GMT  
		Size: 10.8 MB (10775165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c4d86ed3458f8d41c2cd92288a3ed989c0fedc4b04fbb2ca5eb805c265cdc7`  
		Last Modified: Fri, 26 Mar 2021 14:03:37 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b76633e521669ebaae1807e58e89b875101bf362b52165531dcb282e0ac194af`  
		Last Modified: Fri, 26 Mar 2021 14:03:41 GMT  
		Size: 15.7 MB (15673215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11e01ffa97b3d06a4c6c3b8043b8afa755315b5c440a2290e4a2ab71efa1776f`  
		Last Modified: Fri, 26 Mar 2021 14:03:37 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebead7c4e50805c386ab3d520ca1bae23d38cdbc7c80863eb6f6372286933c84`  
		Last Modified: Fri, 26 Mar 2021 14:03:37 GMT  
		Size: 17.5 KB (17521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df2256d44f01c2ca7c7996f91f5359a7aafc2555d25d04fdf4223ef18092928`  
		Last Modified: Sat, 27 Mar 2021 04:46:41 GMT  
		Size: 9.5 MB (9530671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010336d1e5fd04288eb40b23ef98b81ee307eaf3b9b182d22b31aab2b8f27089`  
		Last Modified: Sat, 27 Mar 2021 04:46:36 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffafd8327de71c4804ec1740dfb557d391bbda245a0ecbf7bae9d26615b23453`  
		Last Modified: Sat, 27 Mar 2021 04:46:36 GMT  
		Size: 1.3 MB (1252597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe7e38aae49242f5432e31801bb0ab9ef8849dd8dfe295584ed8fd7965d9b58`  
		Last Modified: Sat, 27 Mar 2021 04:46:36 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53029c7cea5d6db189a289c180e9112d6ee127d1753e5a24dcfbee9de42f8d14`  
		Last Modified: Sat, 27 Mar 2021 04:46:36 GMT  
		Size: 1.2 MB (1196270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3827babe1b1cddbdf22fff8b89e5f6033cebe9be4b8b763b99b95470e728a9f4`  
		Last Modified: Sat, 27 Mar 2021 04:46:36 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.4.0-php8.0` - linux; s390x

```console
$ docker pull wordpress@sha256:6c5785830cdfaf2b0d5db6bc04c2128bcb615c4b99be6d36a7e264f0920ba474
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.3 MB (41329835 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6efd2380555b4b3d25969f28ed2a46aba7a24f303c26a429bc0878fc42c12954`
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
# Thu, 01 Apr 2021 01:11:55 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Thu, 01 Apr 2021 01:11:55 GMT
ENV PHP_VERSION=8.0.3
# Thu, 01 Apr 2021 01:11:55 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.3.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.3.tar.xz.asc
# Thu, 01 Apr 2021 01:11:55 GMT
ENV PHP_SHA256=c9816aa9745a9695672951eaff3a35ca5eddcb9cacf87a4f04b9fb1169010251
# Thu, 01 Apr 2021 01:11:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Apr 2021 01:11:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Apr 2021 01:15:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Apr 2021 01:15:55 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 01 Apr 2021 01:15:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Apr 2021 01:15:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Apr 2021 01:15:57 GMT
CMD ["php" "-a"]
# Thu, 01 Apr 2021 05:20:39 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 01 Apr 2021 05:20:40 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 01 Apr 2021 05:20:40 GMT
WORKDIR /var/www/html
# Thu, 01 Apr 2021 05:21:03 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 01 Apr 2021 05:21:04 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 01 Apr 2021 05:21:04 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 01 Apr 2021 05:21:05 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 01 Apr 2021 05:21:05 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 01 Apr 2021 05:21:07 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 01 Apr 2021 05:21:07 GMT
VOLUME [/var/www/html]
# Thu, 01 Apr 2021 05:21:08 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 01 Apr 2021 05:21:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 05:21:08 GMT
USER www-data
# Thu, 01 Apr 2021 05:21:08 GMT
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
	-	`sha256:d45372af1406ab6210ec74f75f4086d2731db67b11627b59c63c1f96f0e728a9`  
		Last Modified: Thu, 01 Apr 2021 02:24:47 GMT  
		Size: 10.8 MB (10775166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07351f9d903b757a77cf6dcf850abfbb88076fb912520b8e0d4c05ade08102f1`  
		Last Modified: Thu, 01 Apr 2021 02:24:43 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17aaabcb4bdbdd84c449ab57394c6ceff9b031cf65f1f5886694c11426acdecc`  
		Last Modified: Thu, 01 Apr 2021 02:24:48 GMT  
		Size: 14.0 MB (13971990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171fab7f7616aa6ec989f6173cf12530484fab3622366d1a6a3ecfb01d3927ef`  
		Last Modified: Thu, 01 Apr 2021 02:24:43 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea321628f5a5287e2fcae37f5c7876352e07eea82f5f7f1ffc9d195c2bee2cb`  
		Last Modified: Thu, 01 Apr 2021 02:24:43 GMT  
		Size: 17.5 KB (17514 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9dad2a35c62c48204b063caa13e632ea124e3d12d3f50a83350fc0566b1f7b`  
		Last Modified: Thu, 01 Apr 2021 05:24:04 GMT  
		Size: 9.8 MB (9830212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c30e14b4a3efb556c6ad02083afebc44d0036b0cbc9bba26094de91ca8971b`  
		Last Modified: Thu, 01 Apr 2021 05:24:00 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca5e79becf2e4747797192f234c80f41049ef2f8f991a15615d0c9c28f9b155`  
		Last Modified: Thu, 01 Apr 2021 05:24:01 GMT  
		Size: 1.2 MB (1174402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35721f16af16ac03059c7e7e1e79a13604585742ac127979859cf22de27889eb`  
		Last Modified: Thu, 01 Apr 2021 05:24:01 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec4e292d219335e6e8dac37faca24991255044dec02f4b10fb2573dd60e901a`  
		Last Modified: Thu, 01 Apr 2021 05:24:01 GMT  
		Size: 1.2 MB (1196242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c1dbd5533d04fb8e3af44ced8adad619b0c57d2224fd17df8d8886731c4f284`  
		Last Modified: Thu, 01 Apr 2021 05:24:01 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
