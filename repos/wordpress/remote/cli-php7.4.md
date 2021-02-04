## `wordpress:cli-php7.4`

```console
$ docker pull wordpress@sha256:a6489b0345e273ba025a19913c7875d3e993ab267f5f5db3fa92cd46634a5cda
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

### `wordpress:cli-php7.4` - linux; amd64

```console
$ docker pull wordpress@sha256:afd1862bd0a68dd85537123892596d2f2d4c693a18ffa3689cf11909f1b4a300
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.5 MB (44544122 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:131c5696b018fa4f94cacff2251e6438aad99ea946886e1f93590e1c91d37f47`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Thu, 28 Jan 2021 23:19:38 GMT
ADD file:0e2d487cd80773e947c8aae6daad3d565b7bb019a954af2b8bff188681c00d81 in / 
# Thu, 28 Jan 2021 23:19:38 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 01:09:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Jan 2021 01:09:33 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Jan 2021 01:09:34 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Jan 2021 01:09:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Jan 2021 01:09:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 29 Jan 2021 01:09:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:09:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:09:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 01:32:50 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 29 Jan 2021 01:32:50 GMT
ENV PHP_VERSION=7.4.14
# Fri, 29 Jan 2021 01:32:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 29 Jan 2021 01:32:51 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 29 Jan 2021 01:32:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 29 Jan 2021 01:32:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:43:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 29 Jan 2021 01:43:57 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:44:00 GMT
RUN docker-php-ext-enable sodium
# Fri, 29 Jan 2021 01:44:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 29 Jan 2021 01:44:01 GMT
CMD ["php" "-a"]
# Fri, 29 Jan 2021 04:54:28 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 29 Jan 2021 04:54:29 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 29 Jan 2021 04:54:29 GMT
WORKDIR /var/www/html
# Fri, 29 Jan 2021 04:55:34 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 29 Jan 2021 04:55:35 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 29 Jan 2021 04:55:35 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 29 Jan 2021 04:55:36 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Fri, 29 Jan 2021 04:55:36 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Fri, 29 Jan 2021 04:55:38 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 29 Jan 2021 04:55:38 GMT
VOLUME [/var/www/html]
# Fri, 29 Jan 2021 04:55:39 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 29 Jan 2021 04:55:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 04:55:39 GMT
USER www-data
# Fri, 29 Jan 2021 04:55:39 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:4c0d98bf9879488e0407f897d9dd4bf758555a78e39675e72b5124ccf12c2580`  
		Last Modified: Thu, 28 Jan 2021 23:20:08 GMT  
		Size: 2.8 MB (2811321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed03eff2d6362e11708d8c6c19ad4c39f85830d917a40c5254ff7f589caa9982`  
		Last Modified: Fri, 29 Jan 2021 02:50:08 GMT  
		Size: 1.7 MB (1694844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa67667da1de1f032c9daa354a18c7525286103540b8f4a884606ccdef49006f`  
		Last Modified: Fri, 29 Jan 2021 02:50:07 GMT  
		Size: 1.2 KB (1229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6961b2fabe936ad3c26fc41f241379caba86b0d660acaf263f971d8d33e4219b`  
		Last Modified: Fri, 29 Jan 2021 02:50:07 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939a5b1ba662e3b1558bb95c4f29b5b584ab226a4b71b2e7243a6b53f9534b4e`  
		Last Modified: Fri, 29 Jan 2021 02:51:15 GMT  
		Size: 10.3 MB (10346235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f326b7215c3efcc128d39cff72062b50f218986d2d88812ede1ddaf70e987b74`  
		Last Modified: Fri, 29 Jan 2021 02:51:14 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8339edb3b7dbda6ac76f8dc58e36b8b3611d853377815aa20771523ae768850d`  
		Last Modified: Fri, 29 Jan 2021 02:51:18 GMT  
		Size: 14.2 MB (14235139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:771201734758660faf71b5108bd6610106fe0a974d43cdd5017963b4daf8f784`  
		Last Modified: Fri, 29 Jan 2021 02:51:14 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b747590f2e3ca452f56aee814ad471a40ed129d9ecacd853df3493991de7f64`  
		Last Modified: Fri, 29 Jan 2021 02:51:14 GMT  
		Size: 17.5 KB (17521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeb9d74256c5445a9c3d29d8e90d85079db6604d19fef479ad4c9be05786b397`  
		Last Modified: Fri, 29 Jan 2021 05:03:59 GMT  
		Size: 9.3 MB (9334546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e76e729301f010ad91cedb75a8b6cc665a0da4c9b21d49e65b6f390f0ef2018a`  
		Last Modified: Fri, 29 Jan 2021 05:03:56 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:338bf5a422321bb6a2075a968cbb0afa6e0fd473b7f0fa285ccf81a3a63bda5d`  
		Last Modified: Fri, 29 Jan 2021 05:03:57 GMT  
		Size: 4.9 MB (4893281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43f8677c4cf90c9c064fb977e5b5e01e30d7efb4ea530fc13bd8bfa2d45cb3de`  
		Last Modified: Fri, 29 Jan 2021 05:03:56 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15b2318245e02f8bbb2171962c56c6c1babe43c2e88a4439acf123fa6d78cd2`  
		Last Modified: Fri, 29 Jan 2021 05:03:57 GMT  
		Size: 1.2 MB (1206088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1657fc4c473d1962b18b4929ebd50d8837a90ac1227a9cad6bc07b121b452141`  
		Last Modified: Fri, 29 Jan 2021 05:03:56 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-php7.4` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:d56015779b4ee62ddb9f6c4853a1b84a3bfb6c3d1423bfadb8d6b52dd97df301
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.8 MB (42789102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b868a188216354fcf697e9573f5111ecc425a878b169c8439e1c55d0e14da87d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Thu, 28 Jan 2021 23:49:59 GMT
ADD file:c197324e4979e2a7b257ad683d20dd9cbdae525a076bd68fe6aa0e0b126875df in / 
# Thu, 28 Jan 2021 23:49:59 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 00:33:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Jan 2021 00:33:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Jan 2021 00:33:59 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Jan 2021 00:34:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Jan 2021 00:34:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 29 Jan 2021 00:34:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:34:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:34:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 00:41:40 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 04 Feb 2021 18:02:37 GMT
ENV PHP_VERSION=7.4.15
# Thu, 04 Feb 2021 18:02:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Thu, 04 Feb 2021 18:02:39 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Thu, 04 Feb 2021 18:02:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 04 Feb 2021 18:02:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Feb 2021 18:06:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Feb 2021 18:06:56 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 04 Feb 2021 18:07:01 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Feb 2021 18:07:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Feb 2021 18:07:03 GMT
CMD ["php" "-a"]
# Thu, 04 Feb 2021 20:33:10 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 04 Feb 2021 20:33:13 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 04 Feb 2021 20:33:14 GMT
WORKDIR /var/www/html
# Thu, 04 Feb 2021 20:34:28 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 04 Feb 2021 20:34:31 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 04 Feb 2021 20:34:32 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 04 Feb 2021 20:34:33 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 04 Feb 2021 20:34:35 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 04 Feb 2021 20:34:41 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 04 Feb 2021 20:34:42 GMT
VOLUME [/var/www/html]
# Thu, 04 Feb 2021 20:34:43 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 04 Feb 2021 20:34:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Feb 2021 20:34:46 GMT
USER www-data
# Thu, 04 Feb 2021 20:34:47 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:a66f440da051140fefcb0a520bdeb69d763b1eb4fd1b2ed46b4c0a168e335108`  
		Last Modified: Thu, 28 Jan 2021 23:50:33 GMT  
		Size: 2.6 MB (2621759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caa34846effbef1e901021c65a67535efc29a1aa39b259a4c29559d1439f4131`  
		Last Modified: Fri, 29 Jan 2021 01:05:52 GMT  
		Size: 1.7 MB (1684855 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba088c5e0e1fb4c64a8b59354bedcae82636c10a93fe3790125bec5c1e841299`  
		Last Modified: Fri, 29 Jan 2021 01:05:51 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b10584422ada7d37ac091eae04bcee5df4cee5b93cd86068ce55c7ab085ae62`  
		Last Modified: Fri, 29 Jan 2021 01:05:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85692ea7bf5bf0a4f002617411f5234581976013836ea45b6a0d6fe4d026ac1`  
		Last Modified: Thu, 04 Feb 2021 18:55:27 GMT  
		Size: 10.4 MB (10351776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0af173b0724183e0a8adf5f3f513601ad340cff21b6e6215beace05fa5a12d9`  
		Last Modified: Thu, 04 Feb 2021 18:55:25 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a251346c4c05e3a725464c05d7e3551f2a7c659b0396e03a31c7c0a9a091803`  
		Last Modified: Thu, 04 Feb 2021 18:55:31 GMT  
		Size: 13.2 MB (13244751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aed88969c7682157b41ec13dc54420d1ca0cd203f56c4f648a72a4c01cf95446`  
		Last Modified: Thu, 04 Feb 2021 18:55:25 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fab8cdc234431628c87cc966c027c7aece91696c0863822c2e70e92c6434988`  
		Last Modified: Thu, 04 Feb 2021 18:55:25 GMT  
		Size: 17.5 KB (17527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8b586a8c5bf8cd034f285b36d191f44d2da053dfa238f5692368ce0fc927eaf`  
		Last Modified: Thu, 04 Feb 2021 20:39:54 GMT  
		Size: 8.9 MB (8943892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0cf3bddb01ff0218e5d5baab37eecb065deb9f825b11d661fd1e235644de16`  
		Last Modified: Thu, 04 Feb 2021 20:39:50 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38b65a08c18b78081f467ea8b7650f992f4f6766d3207da40df1d03bb863f7d2`  
		Last Modified: Thu, 04 Feb 2021 20:39:50 GMT  
		Size: 4.7 MB (4713191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98db400c2bfd4639a788de17827b8f0cc39d3257a831640c635232a39f1d525e`  
		Last Modified: Thu, 04 Feb 2021 20:39:49 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4762ad4d560ceb24de5630e8a84276d016da31d54591f8b65f010e45362dbdcc`  
		Last Modified: Thu, 04 Feb 2021 20:39:50 GMT  
		Size: 1.2 MB (1206113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a4a189d15bfbf78b8a05de3797741a9f93d83fbc48c36caf8a3b2316b0e8d2`  
		Last Modified: Thu, 04 Feb 2021 20:39:49 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-php7.4` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:9e1e0aa8995b25b5ac1d01e24b50c5f39e5ce8f3b631c0e1cd69dc687e53e33e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.0 MB (41008976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:00e1e7d55b4dc1ba3ed3a2d793d521f062012f373b85ebc1fdbc9fab7e592743`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Thu, 28 Jan 2021 23:58:03 GMT
ADD file:98a89b90a8b442eed5301790dd2bd3a27391c5e4426126eed9d1cf44e70f8857 in / 
# Thu, 28 Jan 2021 23:58:04 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 01:06:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Jan 2021 01:06:44 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Jan 2021 01:06:46 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Jan 2021 01:06:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Jan 2021 01:06:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 29 Jan 2021 01:06:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:06:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:06:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 01:15:02 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 29 Jan 2021 01:15:04 GMT
ENV PHP_VERSION=7.4.14
# Fri, 29 Jan 2021 01:15:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 29 Jan 2021 01:15:09 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 29 Jan 2021 01:15:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 29 Jan 2021 01:15:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:18:13 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 29 Jan 2021 01:18:15 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:18:18 GMT
RUN docker-php-ext-enable sodium
# Fri, 29 Jan 2021 01:18:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 29 Jan 2021 01:18:19 GMT
CMD ["php" "-a"]
# Fri, 29 Jan 2021 03:07:39 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 29 Jan 2021 03:07:41 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 29 Jan 2021 03:07:42 GMT
WORKDIR /var/www/html
# Fri, 29 Jan 2021 03:08:57 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 29 Jan 2021 03:08:59 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 29 Jan 2021 03:09:00 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 29 Jan 2021 03:09:01 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Fri, 29 Jan 2021 03:09:01 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Fri, 29 Jan 2021 03:09:07 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 29 Jan 2021 03:09:11 GMT
VOLUME [/var/www/html]
# Fri, 29 Jan 2021 03:09:12 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 29 Jan 2021 03:09:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 03:09:14 GMT
USER www-data
# Fri, 29 Jan 2021 03:09:14 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:9b1db703a337d301b1d50292acfbabd5fb3796511b962410c554420b85cd78dc`  
		Last Modified: Thu, 28 Jan 2021 23:58:38 GMT  
		Size: 2.4 MB (2423559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85929efbae7230a09dc3cfdea4cf9d3cb6406e6d08ea1f1f27c0f2cbeac922b8`  
		Last Modified: Fri, 29 Jan 2021 01:42:34 GMT  
		Size: 1.6 MB (1555132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e5e29134f861e9b4885f23eae2f99d8886b0dcd558b80afc619e2044102346`  
		Last Modified: Fri, 29 Jan 2021 01:42:33 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7241eb5d2691c2e356b0deeeceebaa6eec6e60e5db535473c1c5940502649f00`  
		Last Modified: Fri, 29 Jan 2021 01:42:33 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7574763d1b6558536f752f790e7c5d46f3d8f8fd1bd9b9be460a9dc9b043dfe8`  
		Last Modified: Fri, 29 Jan 2021 01:43:42 GMT  
		Size: 10.3 MB (10346244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e5f27f5e96ba9a97ce3ca07295dd9b8cd5947c72267a93414ecbc8776730fe7`  
		Last Modified: Fri, 29 Jan 2021 01:43:40 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dc882128b9ec7925a28fc95c7a9276a476611d855fd1b9ca40a5bbeb6cda833`  
		Last Modified: Fri, 29 Jan 2021 01:43:44 GMT  
		Size: 12.4 MB (12388787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c013339dec3edd90f82058c756dc7622eb5b34c083588fd115b93f5e6b39d7df`  
		Last Modified: Fri, 29 Jan 2021 01:43:40 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2e55571fcb91c2a421e6072f6d32608011a5ab98669479e3ab6d7fa1d9b844`  
		Last Modified: Fri, 29 Jan 2021 01:43:40 GMT  
		Size: 17.5 KB (17524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d256a42c458f34907217d3155cc9b1b4a7588eacd06f20328a5659ecbc01ae80`  
		Last Modified: Fri, 29 Jan 2021 03:19:37 GMT  
		Size: 8.7 MB (8661188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:629d6f5f80678b9c3b00ce8b6720804c8d4afae944d19961bb91c17b41962fc9`  
		Last Modified: Fri, 29 Jan 2021 03:19:33 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:287eff1cc974216d154a6311dc59a16ad48aad311e4ff9dd483c5d049f375d09`  
		Last Modified: Fri, 29 Jan 2021 03:19:34 GMT  
		Size: 4.4 MB (4405237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574fe3bcba317ce0b1ea15cfdf5b4293fedaef10fe71b47a91d8030255b1aeab`  
		Last Modified: Fri, 29 Jan 2021 03:19:33 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0904f80436f4c8fbc33e28a5cc1d08b20b9c85991b172524dc6193e857c5e8ab`  
		Last Modified: Fri, 29 Jan 2021 03:19:34 GMT  
		Size: 1.2 MB (1206073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fc8acc232f11bf5f3090cf37829451df93061f67d8a71e26ce129f5cd669eb5`  
		Last Modified: Fri, 29 Jan 2021 03:19:33 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-php7.4` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:96f76e388238cec7ef4dff509b3945a0fc924ad5e9a746715f9a476249e4c9fa
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.1 MB (44131685 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d6e97ef2f6739bdc36151e54d70d9c84a9ee9070fa5d0f2c0c3d7a9bcde375cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Thu, 28 Jan 2021 23:39:33 GMT
ADD file:fecabe41deaeb72acdd63023566d87ae48b013ef80c97fdd993b55d6c727da93 in / 
# Thu, 28 Jan 2021 23:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 01:27:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Jan 2021 01:27:39 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Jan 2021 01:27:43 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Jan 2021 01:27:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Jan 2021 01:27:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 29 Jan 2021 01:27:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:27:50 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:27:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 01:38:22 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 04 Feb 2021 18:01:46 GMT
ENV PHP_VERSION=7.4.15
# Thu, 04 Feb 2021 18:01:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.15.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.15.tar.xz.asc
# Thu, 04 Feb 2021 18:01:50 GMT
ENV PHP_SHA256=9b859c65f0cf7b3eff9d4a28cfab719fb3d36a1db3c20d874a79b5ec44d43cb8
# Thu, 04 Feb 2021 18:01:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 04 Feb 2021 18:01:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Feb 2021 18:06:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Feb 2021 18:06:29 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Thu, 04 Feb 2021 18:06:34 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Feb 2021 18:06:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Feb 2021 18:06:36 GMT
CMD ["php" "-a"]
# Thu, 04 Feb 2021 21:23:55 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 04 Feb 2021 21:23:58 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 04 Feb 2021 21:23:59 GMT
WORKDIR /var/www/html
# Thu, 04 Feb 2021 21:25:24 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 04 Feb 2021 21:25:27 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 04 Feb 2021 21:25:29 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 04 Feb 2021 21:25:30 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 04 Feb 2021 21:25:32 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 04 Feb 2021 21:25:50 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 04 Feb 2021 21:25:52 GMT
VOLUME [/var/www/html]
# Thu, 04 Feb 2021 21:25:53 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 04 Feb 2021 21:25:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Feb 2021 21:25:56 GMT
USER www-data
# Thu, 04 Feb 2021 21:25:58 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:2914792bc417803b2106001990194cc00cdd4b6fd97cd21a368f26148bc8e722`  
		Last Modified: Thu, 28 Jan 2021 23:40:10 GMT  
		Size: 2.7 MB (2711261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:878faaa0cbd74b5e94aae0682e345b19f40d9f47ce41b90494c9ab94e12a1606`  
		Last Modified: Fri, 29 Jan 2021 02:09:31 GMT  
		Size: 1.7 MB (1694574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12efacc7494753eaf44ab2bfe05cc02be70cae3241be0b5fe2378c9f8c7b36c9`  
		Last Modified: Fri, 29 Jan 2021 02:09:30 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1212c0105c6a0060dfb2a16f744f1e40aa7ce3e9957450ee00a8f86934141a10`  
		Last Modified: Fri, 29 Jan 2021 02:09:29 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5fc9398e3b3b0d6f3b6e3c12a2907b7389dc72b53f185cd4c1c7d225333be4e`  
		Last Modified: Thu, 04 Feb 2021 19:34:05 GMT  
		Size: 10.4 MB (10351790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c5ee1479f867785314214f47a36fc41db09c5c54be6b5710e177d74da228008`  
		Last Modified: Thu, 04 Feb 2021 19:34:04 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0752c079c05b5020cf905a63e6af54d540614d87d02e3e7fb6599fa65dba496`  
		Last Modified: Thu, 04 Feb 2021 19:34:09 GMT  
		Size: 14.0 MB (14023238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d42c01b68b2aaed0bab6f839dff18882071d7c0ec0d0621077987f31571f9a5`  
		Last Modified: Thu, 04 Feb 2021 19:34:04 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3db886d27fe51f84b3922f6d5258f8caf66a0ccb8de314055c07ba7bd88619b8`  
		Last Modified: Thu, 04 Feb 2021 19:34:04 GMT  
		Size: 17.5 KB (17536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8b3825021431972532bf289156d2b6cd5a5d474bc676ee0c32a2d298bb6e4d`  
		Last Modified: Thu, 04 Feb 2021 21:35:24 GMT  
		Size: 9.4 MB (9403148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b79fb67471c3467f2f1eec1cffd6936b338a6513d7fcbaaa7be8e453c55c3d3`  
		Last Modified: Thu, 04 Feb 2021 21:35:20 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c819b4cf6c53545a48ed28ea0418a623f4bdd9c3ab51c3ea3042b661f5b636`  
		Last Modified: Thu, 04 Feb 2021 21:35:22 GMT  
		Size: 4.7 MB (4718804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1595b5d00f5b4c1672e47692176809c10b8bfbaac55491be136fd54a7b0ff5c`  
		Last Modified: Thu, 04 Feb 2021 21:35:20 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd73581c3fea1813cbb50d6e15de4939e1b75a688feeaf81d7acb9cbdc834b1`  
		Last Modified: Thu, 04 Feb 2021 21:35:21 GMT  
		Size: 1.2 MB (1206097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3dde3a58b1e0cf21280fd63ef3ec0737f98e01693ce48698b85d60fc8c66a0`  
		Last Modified: Thu, 04 Feb 2021 21:35:20 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-php7.4` - linux; 386

```console
$ docker pull wordpress@sha256:bfbc44296470c12c6b639f69d70291a172c0a8c9ca2910816053929cff2c2bdb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45338195 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e12d58d196fcf11a3ae9bf98b6626952949ac6af5d207a74d2c4e4fdfce2ba9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Thu, 28 Jan 2021 23:38:31 GMT
ADD file:c0e9ea135d66ad6504c77915a7a48b3bead60892d155d3258b746cb4945981c0 in / 
# Thu, 28 Jan 2021 23:38:31 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 01:16:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Jan 2021 01:16:33 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Jan 2021 01:16:34 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Jan 2021 01:16:34 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Jan 2021 01:16:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 29 Jan 2021 01:16:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:16:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:16:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 01:42:47 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 29 Jan 2021 01:42:47 GMT
ENV PHP_VERSION=7.4.14
# Fri, 29 Jan 2021 01:42:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 29 Jan 2021 01:42:48 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 29 Jan 2021 01:42:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 29 Jan 2021 01:42:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:54:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 29 Jan 2021 01:54:56 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:54:57 GMT
RUN docker-php-ext-enable sodium
# Fri, 29 Jan 2021 01:54:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 29 Jan 2021 01:54:57 GMT
CMD ["php" "-a"]
# Fri, 29 Jan 2021 04:55:51 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 29 Jan 2021 04:55:51 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 29 Jan 2021 04:55:52 GMT
WORKDIR /var/www/html
# Fri, 29 Jan 2021 04:57:01 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 29 Jan 2021 04:57:02 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 29 Jan 2021 04:57:02 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 29 Jan 2021 04:57:02 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Fri, 29 Jan 2021 04:57:02 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Fri, 29 Jan 2021 04:57:05 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 29 Jan 2021 04:57:05 GMT
VOLUME [/var/www/html]
# Fri, 29 Jan 2021 04:57:05 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 29 Jan 2021 04:57:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 04:57:06 GMT
USER www-data
# Fri, 29 Jan 2021 04:57:06 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:3fea00a81341ce917db671eb3ad24ef5750cb6928b7f760e3ce4dab619eeb1fa`  
		Last Modified: Thu, 28 Jan 2021 23:39:02 GMT  
		Size: 2.8 MB (2817627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7693c189358487be8693c8f24f54e75dc5e54a6d33edc79a7ddf6851c9f2e670`  
		Last Modified: Fri, 29 Jan 2021 03:00:10 GMT  
		Size: 1.8 MB (1793522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2956bde582e6c6782cd1f42ba90c812f6449eec18badce15706f72fb5fed3db4`  
		Last Modified: Fri, 29 Jan 2021 03:00:07 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63eb950875108b8e92353d43040a08536210b13d2ea2a265b8a93f88149d556f`  
		Last Modified: Fri, 29 Jan 2021 03:00:08 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9b62c85cbb1d3f26bd593ce682416f50129893b909cb500495ae506536f0dd13`  
		Last Modified: Fri, 29 Jan 2021 03:01:20 GMT  
		Size: 10.3 MB (10346200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b7fb39651591022611c42479086e1e8a91dab63f3c89a8ecf0a7b761b62312`  
		Last Modified: Fri, 29 Jan 2021 03:01:18 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d14cdae9f32930efc659334343972fc8ad3c3f35fd08036e487eb0d09b702dd`  
		Last Modified: Fri, 29 Jan 2021 03:01:23 GMT  
		Size: 14.6 MB (14601334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028180e54cd15a973cbbe02716fa568fa4f926faa54f8b328845c1c7ee35bcbc`  
		Last Modified: Fri, 29 Jan 2021 03:01:18 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b86c8a0f5fbcac0ff2515eb29d582b788727946f8eb66bebdbe0c9ea889db3`  
		Last Modified: Fri, 29 Jan 2021 03:01:18 GMT  
		Size: 17.5 KB (17506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:beea959d9d86cb17b14ec9200a77606a297f4d8fa3b36e156aa5e67c91d378ca`  
		Last Modified: Fri, 29 Jan 2021 05:05:43 GMT  
		Size: 9.5 MB (9498413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25fa151e4fd73102e507f2c43d572da530a38f5228e41911e882a0006b95654f`  
		Last Modified: Fri, 29 Jan 2021 05:05:39 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:302f6261d69a2de8e2389e2e327d793201a62deaae8d703c3bcf95a620816c36`  
		Last Modified: Fri, 29 Jan 2021 05:05:41 GMT  
		Size: 5.1 MB (5052378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc271664aab611763b89bc0884cb56a6f1980040098d5ad0de8dc19b623c832`  
		Last Modified: Fri, 29 Jan 2021 05:05:39 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d486566b41bc47e16a9fe044c234c057c05c59bf6532a872c0d787faa6e20a3`  
		Last Modified: Fri, 29 Jan 2021 05:05:40 GMT  
		Size: 1.2 MB (1206061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1898ce98eaf115bf9628d0c040c92b1d157b965611e99824c94a196aad64c6e5`  
		Last Modified: Fri, 29 Jan 2021 05:05:39 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-php7.4` - linux; ppc64le

```console
$ docker pull wordpress@sha256:cfa8dedb7460285bb9dbf1093f80c55604496c29f1a07cfc34f71d2e375fd9bf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.9 MB (45912648 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c20453f917be619e49d6defeb0fc912fcd4c0ff5388ac0337eb4d2c474b3b863`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Thu, 28 Jan 2021 23:55:50 GMT
ADD file:b14fd5f3f7fcd16e2b4ec6932d3e9c07c7400c577cee5fdcb88b0795a70a7bfb in / 
# Thu, 28 Jan 2021 23:55:52 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 00:47:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Jan 2021 00:47:11 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Jan 2021 00:47:28 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Jan 2021 00:47:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Jan 2021 00:47:47 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 29 Jan 2021 00:47:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:47:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:47:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 01:02:02 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 29 Jan 2021 01:02:08 GMT
ENV PHP_VERSION=7.4.14
# Fri, 29 Jan 2021 01:02:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 29 Jan 2021 01:02:18 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 29 Jan 2021 01:02:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 29 Jan 2021 01:02:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:07:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 29 Jan 2021 01:07:22 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:07:47 GMT
RUN docker-php-ext-enable sodium
# Fri, 29 Jan 2021 01:07:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 29 Jan 2021 01:08:06 GMT
CMD ["php" "-a"]
# Fri, 29 Jan 2021 05:18:09 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 29 Jan 2021 05:18:35 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 29 Jan 2021 05:18:44 GMT
WORKDIR /var/www/html
# Fri, 29 Jan 2021 05:20:22 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 29 Jan 2021 05:20:36 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 29 Jan 2021 05:20:40 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 29 Jan 2021 05:20:44 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Fri, 29 Jan 2021 05:20:47 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Fri, 29 Jan 2021 05:21:07 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 29 Jan 2021 05:21:12 GMT
VOLUME [/var/www/html]
# Fri, 29 Jan 2021 05:21:15 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 29 Jan 2021 05:21:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 05:21:28 GMT
USER www-data
# Fri, 29 Jan 2021 05:21:35 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:f3b94a1d8d591af02f1b419642bee91066ecbb9c65099d6903deed310fd1c2ff`  
		Last Modified: Thu, 28 Jan 2021 23:56:32 GMT  
		Size: 2.8 MB (2812517 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9051dfce6625cce4ab1471f70365886b7c23ec19442e08bf3bc297f0a38d57f6`  
		Last Modified: Fri, 29 Jan 2021 01:43:50 GMT  
		Size: 1.7 MB (1741752 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82481345688ea8ca47c72ddbbae52d55e215ba3458011ffc13503f16e7caba02`  
		Last Modified: Fri, 29 Jan 2021 01:43:48 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06851413a731c975b7b2d96c8a3ebb2848c57555cf34ab98ca93d7873280b947`  
		Last Modified: Fri, 29 Jan 2021 01:43:47 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d08db04b0dc095d150e15c37e3d95b3dc809f4d396b8a24694976a60b8eb951`  
		Last Modified: Fri, 29 Jan 2021 01:45:18 GMT  
		Size: 10.3 MB (10346229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48615efec7ae57e12aaa242d1ad7db62b6ad8e13d4d3ac9f688fc08bedce21c1`  
		Last Modified: Fri, 29 Jan 2021 01:45:17 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b3e4568aacb143627bc7c9d4373d96d0c67db36eac8d31d3ede77e2744fdc10`  
		Last Modified: Fri, 29 Jan 2021 01:45:21 GMT  
		Size: 15.3 MB (15265783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32270dba0e963c90e01bc53a42af22592614f22732af34220ae2a6b90ae41d96`  
		Last Modified: Fri, 29 Jan 2021 01:45:17 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a57977547d7e139a8300103c913e8e45249a33a270af8b3846a8b0c7fd4a85d5`  
		Last Modified: Fri, 29 Jan 2021 01:45:17 GMT  
		Size: 17.5 KB (17523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c557651ad4edfa8184632f2ef1aedee97a16882223cf3e62ee409a7634481b36`  
		Last Modified: Fri, 29 Jan 2021 05:46:26 GMT  
		Size: 9.5 MB (9530724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a51048fbc04a7e623d1c8244e3b848bd10513257d5ed6d3cd9b354f4b0350fec`  
		Last Modified: Fri, 29 Jan 2021 05:46:20 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f114f249e1fc84eb5048f6a2a261ec98120ccfa2c56dba2e85083d292fd0561f`  
		Last Modified: Fri, 29 Jan 2021 05:46:21 GMT  
		Size: 5.0 MB (4986804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c29d04c42012dea0333044542c575a7cb7a2051cd3a5ecf6ab6f1fecbccb6f8c`  
		Last Modified: Fri, 29 Jan 2021 05:46:20 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5976cdf15b539c658993310e2546959fb88550d3c5eaadcee5920ad3e2592338`  
		Last Modified: Fri, 29 Jan 2021 05:46:21 GMT  
		Size: 1.2 MB (1206080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6546352d7dca3bac4e15fac89ca6575bee9b9489f7751bdb076e53c2a98f7e00`  
		Last Modified: Fri, 29 Jan 2021 05:46:20 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-php7.4` - linux; s390x

```console
$ docker pull wordpress@sha256:9052187da2f369d0cb8d510b99822395e662ed7410e1b9a284d5093aa91b4d79
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.2 MB (44229538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:278a83b8e4e6bb13835c35929e2aa757a541c8a1e96425371639e1d3fdfc4ff9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Thu, 28 Jan 2021 23:41:35 GMT
ADD file:d97e6c37df0fb8306b072d9c0a32f68f5aff583ba849303926644deacfa25eb9 in / 
# Thu, 28 Jan 2021 23:41:36 GMT
CMD ["/bin/sh"]
# Fri, 29 Jan 2021 00:38:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 29 Jan 2021 00:38:38 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 29 Jan 2021 00:38:40 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 29 Jan 2021 00:38:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 29 Jan 2021 00:38:41 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 29 Jan 2021 00:38:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:38:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:38:43 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 00:48:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 29 Jan 2021 00:48:48 GMT
ENV PHP_VERSION=7.4.14
# Fri, 29 Jan 2021 00:48:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 29 Jan 2021 00:48:49 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 29 Jan 2021 00:48:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 29 Jan 2021 00:48:56 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 29 Jan 2021 00:53:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 29 Jan 2021 00:53:07 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 29 Jan 2021 00:53:09 GMT
RUN docker-php-ext-enable sodium
# Fri, 29 Jan 2021 00:53:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 29 Jan 2021 00:53:11 GMT
CMD ["php" "-a"]
# Fri, 29 Jan 2021 03:09:40 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 29 Jan 2021 03:09:42 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 29 Jan 2021 03:09:43 GMT
WORKDIR /var/www/html
# Fri, 29 Jan 2021 03:10:38 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 29 Jan 2021 03:10:39 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 29 Jan 2021 03:10:40 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 29 Jan 2021 03:10:40 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Fri, 29 Jan 2021 03:10:40 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Fri, 29 Jan 2021 03:10:44 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 29 Jan 2021 03:10:45 GMT
VOLUME [/var/www/html]
# Fri, 29 Jan 2021 03:10:45 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 29 Jan 2021 03:10:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Jan 2021 03:10:46 GMT
USER www-data
# Fri, 29 Jan 2021 03:10:47 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:43901f1af0ef9db6b0bf30ac6f6dacd78bf1ecfeb47ad0a93aa2370fa8e62407`  
		Last Modified: Thu, 28 Jan 2021 23:42:09 GMT  
		Size: 2.6 MB (2602059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ca6a535daf2f11149d562663f17aa1c644768776000a66fbf3c3a408575b41`  
		Last Modified: Fri, 29 Jan 2021 01:20:34 GMT  
		Size: 1.8 MB (1756344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49dba0dd587ac68bb7a364dfb548d9e4c5725a4e26f9c844457805036cfa6cb`  
		Last Modified: Fri, 29 Jan 2021 01:20:33 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef10d9258fa200837167aa8dd3a89838c0c749ff3167f7eaea8db0ef3b421a99`  
		Last Modified: Fri, 29 Jan 2021 01:20:33 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a419e09ebba7b175cd770a5003e8b0f238e93d343a899c2bf3b5634786b86d8`  
		Last Modified: Fri, 29 Jan 2021 01:21:53 GMT  
		Size: 10.3 MB (10346241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155f7d337736f13eb2700224a04ec5e78bcfa237772952d6d77d589706137607`  
		Last Modified: Fri, 29 Jan 2021 01:21:52 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e85d5c2bf1b80bbc4f8cf1cf03c823cfe4869fe3ac859594652e6affb7ddf4`  
		Last Modified: Fri, 29 Jan 2021 01:21:54 GMT  
		Size: 13.6 MB (13599852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:127a004bcfc592622c4127d6d0b550c37fb5842a635f0c0eac203ca87b843319`  
		Last Modified: Fri, 29 Jan 2021 01:21:52 GMT  
		Size: 2.3 KB (2261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6429403d8c64252998c0dac33ea31601ad0855616b3c56768371b9fdcb8c0d8`  
		Last Modified: Fri, 29 Jan 2021 01:21:52 GMT  
		Size: 17.5 KB (17523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a6fc628c6b0344caa667efc1b656b2c23c794a885f59b53c58833a40e80b083`  
		Last Modified: Fri, 29 Jan 2021 03:18:55 GMT  
		Size: 9.8 MB (9830181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f7b333ac3a3cf8c3099c36ff689838df7d156314103be318aca3ebdc3ca3b5c`  
		Last Modified: Fri, 29 Jan 2021 03:18:49 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006077d4e18d87cb7718e1e4bfba53e8ea7e2f567ef1388b7e22db1f0fa83f09`  
		Last Modified: Fri, 29 Jan 2021 03:18:50 GMT  
		Size: 4.9 MB (4866045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25d89861b6e39834b6433a398b7d42bfa1771cd80bb0cd8761f6c1e8c32dbd07`  
		Last Modified: Fri, 29 Jan 2021 03:18:49 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079a2d99f52b422a59ede140ce2c80c2d2d1da6ca23d61c94d06cb88d3983ed1`  
		Last Modified: Fri, 29 Jan 2021 03:18:49 GMT  
		Size: 1.2 MB (1206075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:132dd3159ff997c28b7dc4cb5a657ac9c8255fbe0ebdec91fe1baf9681b4ccb8`  
		Last Modified: Fri, 29 Jan 2021 03:18:49 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
