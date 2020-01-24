## `wordpress:cli-2-php7.4`

```console
$ docker pull wordpress@sha256:6acf4c2241c4b9a53b2dd046edcc2b9c11912d96bdbb56c3526a2dd0c90d4357
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `wordpress:cli-2-php7.4` - linux; amd64

```console
$ docker pull wordpress@sha256:097f81fa7b225aa061c190f1ca66c55a90ee01140b80d93594c669f5a1c74049
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46327614 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32ee9727d086a30fe1e6a52dba26607f49a57e3efa6420c427624482a3da6bdf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:18:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 18 Jan 2020 03:18:28 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 18 Jan 2020 03:18:29 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:18:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 18 Jan 2020 03:18:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 18 Jan 2020 03:18:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 03:18:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 03:18:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 18 Jan 2020 03:18:30 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 18 Jan 2020 03:18:30 GMT
ENV PHP_VERSION=7.4.1
# Sat, 18 Jan 2020 03:18:31 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.1.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.1.tar.xz.asc/from/this/mirror
# Sat, 18 Jan 2020 03:18:31 GMT
ENV PHP_SHA256=561bb866bdd509094be00f4ece7c3543ec971c4d878645ee81437e291cffc762 PHP_MD5=
# Sat, 18 Jan 2020 03:18:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 18 Jan 2020 03:18:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:23:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 18 Jan 2020 03:23:31 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:23:32 GMT
RUN docker-php-ext-enable sodium
# Sat, 18 Jan 2020 03:23:32 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 18 Jan 2020 03:23:32 GMT
CMD ["php" "-a"]
# Sat, 18 Jan 2020 06:10:13 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Sat, 18 Jan 2020 06:10:13 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 18 Jan 2020 06:10:15 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Sat, 18 Jan 2020 06:10:15 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Sat, 18 Jan 2020 06:10:16 GMT
WORKDIR /var/www/html
# Sat, 18 Jan 2020 06:10:16 GMT
VOLUME [/var/www/html]
# Sat, 18 Jan 2020 06:10:16 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Sat, 18 Jan 2020 06:10:16 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Sat, 18 Jan 2020 06:10:16 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Sat, 18 Jan 2020 06:10:18 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Sat, 18 Jan 2020 06:10:18 GMT
COPY file:7798dc600ff57df68d7de781fd8834d5a9371b2ab13ab9649086b34ee0e38fcf in /usr/local/bin/ 
# Sat, 18 Jan 2020 06:10:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Jan 2020 06:10:19 GMT
USER www-data
# Sat, 18 Jan 2020 06:10:19 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1c0a1817becf025301783a94fa11de700972e7d7c117ca7e45d080db0ec1a11`  
		Last Modified: Sat, 18 Jan 2020 04:09:35 GMT  
		Size: 1.4 MB (1354634 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd5b3ea1fc31791c18f464b5b95dd3d9b8ff97aef4b64e0202f3da7f5550e80`  
		Last Modified: Sat, 18 Jan 2020 04:09:35 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db87396003bdeb76e6e367a5ae26be9642a89986dcda71b3491412c579cb6859`  
		Last Modified: Sat, 18 Jan 2020 04:09:35 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb8dcdef007bfc6cf90ed68b8f9eb2231d0b98791b297423f61ec872de081312`  
		Last Modified: Sat, 18 Jan 2020 04:09:36 GMT  
		Size: 10.3 MB (10264374 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd70a2c2d149fcd9425ff9107be5bca94d52046b7854aa9a2a7a948468c3d2`  
		Last Modified: Sat, 18 Jan 2020 04:09:34 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fddf3b96c29f403a431f9493a06740c6c1fbaf4df5b00a026635b69b1ad096b`  
		Last Modified: Sat, 18 Jan 2020 04:09:37 GMT  
		Size: 14.6 MB (14572426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780a347441981dbe18eb9a44da7f19d0102b5cd006c6751103fc8940ef0efdbe`  
		Last Modified: Sat, 18 Jan 2020 04:09:34 GMT  
		Size: 2.2 KB (2215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0de901fdc85d2e33621472a8cc9f7e5eaa1b5f3f9feff98cb7fcf6aa4297011a`  
		Last Modified: Sat, 18 Jan 2020 04:09:34 GMT  
		Size: 73.1 KB (73143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d378136cf91ec5d056409922f732958a1e87fad63ae425a198793f09ff272cd`  
		Last Modified: Sat, 18 Jan 2020 06:12:11 GMT  
		Size: 6.7 MB (6670043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a67388d8cad789072d3d5125c09ff3a32f5376f8805e9e0d127fbc8217df5cc2`  
		Last Modified: Sat, 18 Jan 2020 06:12:07 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd793f607d3579c6c1acaacc82f1a760f484049adbf8698fc3e7f63bf92a9c43`  
		Last Modified: Sat, 18 Jan 2020 06:12:10 GMT  
		Size: 9.3 MB (9323334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1430fcb026b728d7690d901258d4b0a3ff75757cf0ab55d4b5e1aec7ce5f26c`  
		Last Modified: Sat, 18 Jan 2020 06:12:08 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fae911659e08bd1d5eba628ec6eff6a5b1f0ea9572fa4d4179db1cbb73c1ef`  
		Last Modified: Sat, 18 Jan 2020 06:12:08 GMT  
		Size: 1.3 MB (1261592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d241977a37e06cbb5641b25ba8b8acd33c52c9c85c5c947983ce428ce6686a5`  
		Last Modified: Sat, 18 Jan 2020 06:12:07 GMT  
		Size: 416.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.4` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:b7f235c97cebb5317c4e491eb9762300fba7f36c8aeaca195dec21b5b36a1f65
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.4 MB (44449286 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dbb914578a37fc76cfb704aa6ccbc01badefcebb9c4298bd56fbdfc4fcdcba4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:40:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 18 Jan 2020 03:40:03 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 18 Jan 2020 03:40:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:40:07 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 18 Jan 2020 03:40:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 18 Jan 2020 03:40:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 03:40:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 03:40:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 18 Jan 2020 03:40:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jan 2020 21:46:38 GMT
ENV PHP_VERSION=7.4.2
# Thu, 23 Jan 2020 21:46:39 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 21:46:40 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Thu, 23 Jan 2020 21:46:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 23 Jan 2020 21:46:45 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:50:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 21:50:36 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:50:40 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 21:50:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 21:50:43 GMT
CMD ["php" "-a"]
# Fri, 24 Jan 2020 00:21:49 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 24 Jan 2020 00:21:53 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 24 Jan 2020 00:21:57 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 24 Jan 2020 00:22:00 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 24 Jan 2020 00:22:01 GMT
WORKDIR /var/www/html
# Fri, 24 Jan 2020 00:22:02 GMT
VOLUME [/var/www/html]
# Fri, 24 Jan 2020 00:22:03 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 24 Jan 2020 00:22:04 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Fri, 24 Jan 2020 00:22:05 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Fri, 24 Jan 2020 00:22:09 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Fri, 24 Jan 2020 00:22:10 GMT
COPY file:7798dc600ff57df68d7de781fd8834d5a9371b2ab13ab9649086b34ee0e38fcf in /usr/local/bin/ 
# Fri, 24 Jan 2020 00:22:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 00:22:15 GMT
USER www-data
# Fri, 24 Jan 2020 00:22:18 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de5c701ead53742b2a88bf4f606bd05029ec59ccaf522450bfa76be8cea0cf02`  
		Last Modified: Sat, 18 Jan 2020 04:28:12 GMT  
		Size: 1.3 MB (1321088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:574e3d03f7d4228e33415f8592e7ec2a89fe1616e0ab6366ea68045b09d7f280`  
		Last Modified: Sat, 18 Jan 2020 04:28:12 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ba27e9ff828195f46a3edb0b1e28b5d10451b66ae080c20794f6d005cffbd72`  
		Last Modified: Sat, 18 Jan 2020 04:28:12 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a2dbd67605058278b9b5cbd203ba19fdfa36b6aabd60c1be85e85ffde9afde8`  
		Last Modified: Thu, 23 Jan 2020 22:59:45 GMT  
		Size: 10.3 MB (10271108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e072408beb050c5fe6bf972732eeec84ebcb7a87992aacc2e89731f6f74620b7`  
		Last Modified: Thu, 23 Jan 2020 22:59:37 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eefe35b2a9be84292edca86e2687a93819179facbd9e7c35d2ecfcbb87c46068`  
		Last Modified: Thu, 23 Jan 2020 22:59:51 GMT  
		Size: 13.6 MB (13598525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6121cbbb0ebda6403050cd66f64f14577f46da699786c6f5ed7a7b8d73372d0`  
		Last Modified: Thu, 23 Jan 2020 22:59:37 GMT  
		Size: 2.2 KB (2215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df617f57867952b84aa41b6504f2c5d62636af68dd0b24deec4a5e51181b795d`  
		Last Modified: Thu, 23 Jan 2020 22:59:37 GMT  
		Size: 72.7 KB (72677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d770ffbf793317df2ebc12adab1f1cdb2d96361da50facb0f226488fa35421`  
		Last Modified: Fri, 24 Jan 2020 00:25:05 GMT  
		Size: 6.4 MB (6375864 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88299fc5d4e5988319c4f964533f4fd438b24a5a114ae4a6d879a0127a78eb86`  
		Last Modified: Fri, 24 Jan 2020 00:24:58 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93100ee94796dc152e74ac23fde0364d65f169794601db4b7de573f49d3a29ba`  
		Last Modified: Fri, 24 Jan 2020 00:25:08 GMT  
		Size: 8.9 MB (8926041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8be16b6c0c1afec7f6fa1782cc1b11ebc675c8fbc2bcdc2e74516301e2db728b`  
		Last Modified: Fri, 24 Jan 2020 00:24:58 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba3de6fdbbc57330206f10ac2b0cf17105c4c4b46ac7e39d581e1e482bd5944`  
		Last Modified: Fri, 24 Jan 2020 00:24:58 GMT  
		Size: 1.3 MB (1261235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d75e9ad497759b9a535c7cc7dcfd095e14e1abf6107a199b3b1deab136a4022e`  
		Last Modified: Fri, 24 Jan 2020 00:24:58 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.4` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:e8925fbab466124769425322076a01e4809a86022a7c129e1fa0d6c6b7a04907
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.7 MB (42729752 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57328a772e100d9823c21d39bd81d3dac587e1f70dfdd9ce3aeb33a4fe40e5c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:21:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 18 Jan 2020 05:22:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 18 Jan 2020 05:22:16 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 05:22:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 18 Jan 2020 05:22:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 18 Jan 2020 05:22:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 05:22:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 05:22:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 18 Jan 2020 05:22:49 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jan 2020 21:30:14 GMT
ENV PHP_VERSION=7.4.2
# Thu, 23 Jan 2020 21:30:15 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 21:30:16 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Thu, 23 Jan 2020 21:30:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 23 Jan 2020 21:30:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:32:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 21:32:59 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Thu, 23 Jan 2020 21:33:02 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 21:33:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 21:33:04 GMT
CMD ["php" "-a"]
# Fri, 24 Jan 2020 04:17:16 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 24 Jan 2020 04:17:18 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 24 Jan 2020 04:17:21 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 24 Jan 2020 04:17:23 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 24 Jan 2020 04:17:24 GMT
WORKDIR /var/www/html
# Fri, 24 Jan 2020 04:17:25 GMT
VOLUME [/var/www/html]
# Fri, 24 Jan 2020 04:17:26 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 24 Jan 2020 04:17:26 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Fri, 24 Jan 2020 04:17:27 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Fri, 24 Jan 2020 04:17:31 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Fri, 24 Jan 2020 04:17:32 GMT
COPY file:7798dc600ff57df68d7de781fd8834d5a9371b2ab13ab9649086b34ee0e38fcf in /usr/local/bin/ 
# Fri, 24 Jan 2020 04:17:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 04:17:33 GMT
USER www-data
# Fri, 24 Jan 2020 04:17:34 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eecb809efefba021b07183ae486164fd475667a42a78ab308bd01b8d7dd8c1e`  
		Last Modified: Sat, 18 Jan 2020 06:09:11 GMT  
		Size: 1.2 MB (1227271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf6ec95513b0eab50a07131cbee828abed358fb86fd276018e1bae6f04611ed9`  
		Last Modified: Sat, 18 Jan 2020 06:09:10 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:459d1b57d2f034e68934a4116a4434479186cfce56d1235af4f1c1b9de08acbc`  
		Last Modified: Sat, 18 Jan 2020 06:09:08 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f021521208098f88f7de0b01f4c3e9d14c4fe1015865a8826f2d03ec1ee4b7be`  
		Last Modified: Thu, 23 Jan 2020 23:41:50 GMT  
		Size: 10.3 MB (10271103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed5af0d8217fe8ce04eefc9816cf5050559ebf0b94eaafe180cb69d1d8bee2a6`  
		Last Modified: Thu, 23 Jan 2020 23:41:43 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91bb77df7edbd55c061d6ddf81f68f6846b779ff584df913e486f537c1a7afb7`  
		Last Modified: Thu, 23 Jan 2020 23:41:47 GMT  
		Size: 12.7 MB (12748897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2cb3e15983bfda6b84a9cc78b203f86bc545869c901857c794da1cfb0ff1f1`  
		Last Modified: Thu, 23 Jan 2020 23:41:42 GMT  
		Size: 2.2 KB (2217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eeb635ae76ece5e12e817d55b846c6fb7ae52b60f25c041e6d483b32a5866de`  
		Last Modified: Thu, 23 Jan 2020 23:41:42 GMT  
		Size: 72.7 KB (72673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b742615c0029673a3a7ccbb464ba3d888739e822c57b6e66a904dd34072b9450`  
		Last Modified: Fri, 24 Jan 2020 04:24:00 GMT  
		Size: 6.1 MB (6068826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd199312789cb40dffbcbc2d6ab723a9d6f4785ed8ad28a088b47e094efa3d6a`  
		Last Modified: Fri, 24 Jan 2020 04:23:51 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0bb0dd7d94954ba4b12ab9918a06edf1935569f067ac3096aaa0b536b19584f`  
		Last Modified: Fri, 24 Jan 2020 04:23:55 GMT  
		Size: 8.7 MB (8654981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36dad5d2dacfcf2f1cc396136a5dee1300d0a0f847ac272b20b12bde5ca55584`  
		Last Modified: Fri, 24 Jan 2020 04:23:51 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d767b326c3df94a809377952c95a2435dda2b55523300fdac17f83fcb307e19`  
		Last Modified: Fri, 24 Jan 2020 04:23:53 GMT  
		Size: 1.3 MB (1261258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547de6dcc6a46ab615d2ea9e0258bd30941b99adb6d76b08077aaa56d096e73d`  
		Last Modified: Fri, 24 Jan 2020 04:23:52 GMT  
		Size: 414.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.4` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:01e84de62871e6fb96320692ef40cdc062e39ee6f702700af748c220a0d5df52
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.0 MB (45953118 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7a8d640bded730a1f4e23bf648142077591c82005eda8145d63521e8e4652f6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:29:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 18 Jan 2020 02:29:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 18 Jan 2020 02:29:16 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 02:29:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 18 Jan 2020 02:29:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 18 Jan 2020 02:29:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 02:29:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 02:29:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 18 Jan 2020 02:29:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 24 Jan 2020 00:09:58 GMT
ENV PHP_VERSION=7.4.2
# Fri, 24 Jan 2020 00:10:02 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Fri, 24 Jan 2020 00:10:03 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Fri, 24 Jan 2020 00:10:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 24 Jan 2020 00:10:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 24 Jan 2020 00:14:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 24 Jan 2020 00:14:05 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Fri, 24 Jan 2020 00:14:09 GMT
RUN docker-php-ext-enable sodium
# Fri, 24 Jan 2020 00:14:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 24 Jan 2020 00:14:11 GMT
CMD ["php" "-a"]
# Fri, 24 Jan 2020 05:56:39 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 24 Jan 2020 05:56:41 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 24 Jan 2020 05:56:43 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 24 Jan 2020 05:56:45 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 24 Jan 2020 05:56:46 GMT
WORKDIR /var/www/html
# Fri, 24 Jan 2020 05:56:46 GMT
VOLUME [/var/www/html]
# Fri, 24 Jan 2020 05:56:47 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 24 Jan 2020 05:56:48 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Fri, 24 Jan 2020 05:56:48 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Fri, 24 Jan 2020 05:56:52 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Fri, 24 Jan 2020 05:56:53 GMT
COPY file:7798dc600ff57df68d7de781fd8834d5a9371b2ab13ab9649086b34ee0e38fcf in /usr/local/bin/ 
# Fri, 24 Jan 2020 05:56:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 05:56:54 GMT
USER www-data
# Fri, 24 Jan 2020 05:56:55 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34df684e328567a0a35db6301bcecffeb8c2ab6a69340a96db5d3e73a9fde3da`  
		Last Modified: Sat, 18 Jan 2020 03:18:17 GMT  
		Size: 1.4 MB (1359426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dbaaf99effdf014f4ce62ee67d7cf9f23205c645f22d554e6e925ef12ffcd70`  
		Last Modified: Sat, 18 Jan 2020 03:18:17 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99838bf36837f5d2206ac07b2f399dca053921c575c4e9ea8fce917f1672383a`  
		Last Modified: Sat, 18 Jan 2020 03:18:17 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa724be546925194dbbb305717c1ec1404bd825d4e768f5fa30758fc836a1dda`  
		Last Modified: Fri, 24 Jan 2020 02:37:49 GMT  
		Size: 10.3 MB (10271109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70b0bc8c61926931859ef4bf710fb73b709a407ca1086dfe704e7654934b4bdd`  
		Last Modified: Fri, 24 Jan 2020 02:37:45 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07be412705d63c11275e2018adae846b8861d4f678a21f2c43e2c22ae0bcee6d`  
		Last Modified: Fri, 24 Jan 2020 02:37:49 GMT  
		Size: 14.4 MB (14366228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73cafd3dde7ad30752409223dc0b26b0a5f4fa98d9a875225e2566bd99806655`  
		Last Modified: Fri, 24 Jan 2020 02:37:45 GMT  
		Size: 2.2 KB (2216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59195632759b7e9a57fb9ac253284ecbea9055d01c12f9caa49d23ca8f40bc1c`  
		Last Modified: Fri, 24 Jan 2020 02:37:45 GMT  
		Size: 72.7 KB (72676 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32b34fc582080a887c54d5fdf1935b451bbb56d48f7801ee0776e08cb08944d`  
		Last Modified: Fri, 24 Jan 2020 06:03:13 GMT  
		Size: 6.5 MB (6508057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42c4602026e6694f78ff0684db1ae2b48797342fceb467a3f785bfc2f5ff1a52`  
		Last Modified: Fri, 24 Jan 2020 06:03:06 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:480fc761d3e9ac5bafc99da4bcd8438c469e6a84cd05eb93002679aa74f6f91e`  
		Last Modified: Fri, 24 Jan 2020 06:03:09 GMT  
		Size: 9.4 MB (9386175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1563ca8f332cb996e8ddf5d65ae3566379a84e1d1a462cca8d37d75e92a756be`  
		Last Modified: Fri, 24 Jan 2020 06:03:06 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e04f75aeeb102b3bbb65e966598020595e11dce605ac2bf5774f5d7f6c063bd`  
		Last Modified: Fri, 24 Jan 2020 06:03:07 GMT  
		Size: 1.3 MB (1261182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f132984a0d82a5f8ded0c7baf9ca04d2bc6e86ba6f178ee2c21d1b36db72e51`  
		Last Modified: Fri, 24 Jan 2020 06:03:06 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.4` - linux; 386

```console
$ docker pull wordpress@sha256:44b0ee906474d07c911f810db786f3d7a428d3e8fb29739d1137dbc4f946e175
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.1 MB (47087520 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cfe476648b6542ba8452fa00ed65b67126b71bf953c01de1fbc75d4d35e9dccb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:41:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 18 Jan 2020 05:41:36 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 18 Jan 2020 05:41:37 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 05:41:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 18 Jan 2020 05:41:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 18 Jan 2020 05:41:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 05:41:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 05:41:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 18 Jan 2020 05:41:39 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jan 2020 23:13:49 GMT
ENV PHP_VERSION=7.4.2
# Thu, 23 Jan 2020 23:13:49 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 23:13:49 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Thu, 23 Jan 2020 23:13:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 23 Jan 2020 23:13:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 23:21:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 23:21:57 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Thu, 23 Jan 2020 23:21:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 23:21:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 23:22:00 GMT
CMD ["php" "-a"]
# Fri, 24 Jan 2020 08:12:20 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 24 Jan 2020 08:12:21 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 24 Jan 2020 08:12:23 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 24 Jan 2020 08:12:25 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 24 Jan 2020 08:12:25 GMT
WORKDIR /var/www/html
# Fri, 24 Jan 2020 08:12:25 GMT
VOLUME [/var/www/html]
# Fri, 24 Jan 2020 08:12:25 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 24 Jan 2020 08:12:26 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Fri, 24 Jan 2020 08:12:26 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Fri, 24 Jan 2020 08:12:29 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Fri, 24 Jan 2020 08:12:30 GMT
COPY file:7798dc600ff57df68d7de781fd8834d5a9371b2ab13ab9649086b34ee0e38fcf in /usr/local/bin/ 
# Fri, 24 Jan 2020 08:12:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 08:12:30 GMT
USER www-data
# Fri, 24 Jan 2020 08:12:31 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6686b8c2d7ff02237fc9b12daa86e7e7328b7031b6585a20cd6b5fd618f77486`  
		Last Modified: Sat, 18 Jan 2020 06:45:55 GMT  
		Size: 1.5 MB (1452582 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:564ce419d6f56887ea2bd9699c37517ecd579e747f1a2698e764ad6f74e66b4c`  
		Last Modified: Sat, 18 Jan 2020 06:45:54 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694ef48cddae433ef86445fc9786eb75673c1c0c6d903fd7a81b2c56fb7e1b86`  
		Last Modified: Sat, 18 Jan 2020 06:45:54 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f3628b223c4b093cf7c2d7723ccd39dfcb6977a659c9c183e7673f22f44865b`  
		Last Modified: Fri, 24 Jan 2020 02:36:11 GMT  
		Size: 10.3 MB (10271099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e167c61f346105deafdbe6bff7f521715a3d31cd4c9ca27d6dca67654d916c`  
		Last Modified: Fri, 24 Jan 2020 02:36:08 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53425617927914b1561c930b3ce2f90644de41394e731ca71a5d66feeba55d5b`  
		Last Modified: Fri, 24 Jan 2020 02:36:19 GMT  
		Size: 15.0 MB (14974599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809347a8b4ae69caee1b666ac61ec86e0f2dd5d64744592a59f65fd9bb49c7c9`  
		Last Modified: Fri, 24 Jan 2020 02:36:10 GMT  
		Size: 2.2 KB (2216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31917077d16c99b9c58e44f9267cbda55763d759a59379d7e4ca1f9fd6acf60a`  
		Last Modified: Fri, 24 Jan 2020 02:36:09 GMT  
		Size: 72.3 KB (72331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61561c861ef661e68015d6f6dfc82081e44027e462d461e59803a08da4d3c41d`  
		Last Modified: Fri, 24 Jan 2020 08:18:39 GMT  
		Size: 6.8 MB (6756222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565815eade7b139b02f0f9f9469bf63e87e1083176afd233ca2ef9d1f045b1d3`  
		Last Modified: Fri, 24 Jan 2020 08:18:34 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:312313772fb5ee074d1eca34231ed0ddcbabaf3b3292d4a4a323cfbcb0ab6ff8`  
		Last Modified: Fri, 24 Jan 2020 08:18:40 GMT  
		Size: 9.5 MB (9488139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743efb9534fe5f3e38cd5af16ca3a5effd41af2e48a05c40c944a53f9f0069e5`  
		Last Modified: Fri, 24 Jan 2020 08:18:34 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94481943d9bf6bc44934180209a4338aad6f3345590634ec887fe39886cecc1`  
		Last Modified: Fri, 24 Jan 2020 08:18:35 GMT  
		Size: 1.3 MB (1260871 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c714ae2641f52f2cf9fa2e381ff10429fb50fe2006bce01c2ad2e1008b3323e`  
		Last Modified: Fri, 24 Jan 2020 08:18:34 GMT  
		Size: 417.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.4` - linux; ppc64le

```console
$ docker pull wordpress@sha256:e8af4e925de909a0fbda87204819d30927287e14de429047fc2168dab9f25086
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.7 MB (47684136 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a775388614ea0fc3ce17e0d4469e6b25e5103d1de809eacddc5f7a555d229703`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:24:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 18 Jan 2020 03:24:16 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 18 Jan 2020 03:24:20 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:24:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 18 Jan 2020 03:24:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 18 Jan 2020 03:24:28 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 03:24:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 18 Jan 2020 03:24:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Sat, 18 Jan 2020 03:24:34 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Jan 2020 23:32:44 GMT
ENV PHP_VERSION=7.4.2
# Thu, 23 Jan 2020 23:32:47 GMT
ENV PHP_URL=https://www.php.net/get/php-7.4.2.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.4.2.tar.xz.asc/from/this/mirror
# Thu, 23 Jan 2020 23:32:50 GMT
ENV PHP_SHA256=98284deac017da0d426117ecae7599a1f1bf62ae3911e8bc16c4403a8f4bdf13 PHP_MD5=
# Thu, 23 Jan 2020 23:33:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 23 Jan 2020 23:33:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 23 Jan 2020 23:36:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 23 Jan 2020 23:36:54 GMT
COPY multi:0b7e4a1b9cd5748d214539db3c6bee9b30805d1933690492830b56ffcd31f68d in /usr/local/bin/ 
# Thu, 23 Jan 2020 23:37:00 GMT
RUN docker-php-ext-enable sodium
# Thu, 23 Jan 2020 23:37:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 23 Jan 2020 23:37:04 GMT
CMD ["php" "-a"]
# Fri, 24 Jan 2020 10:43:17 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 24 Jan 2020 10:43:23 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 24 Jan 2020 10:43:29 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 24 Jan 2020 10:43:35 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 24 Jan 2020 10:43:38 GMT
WORKDIR /var/www/html
# Fri, 24 Jan 2020 10:43:39 GMT
VOLUME [/var/www/html]
# Fri, 24 Jan 2020 10:43:42 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 24 Jan 2020 10:43:44 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Fri, 24 Jan 2020 10:43:47 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Fri, 24 Jan 2020 10:43:53 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Fri, 24 Jan 2020 10:43:54 GMT
COPY file:7798dc600ff57df68d7de781fd8834d5a9371b2ab13ab9649086b34ee0e38fcf in /usr/local/bin/ 
# Fri, 24 Jan 2020 10:43:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 10:43:58 GMT
USER www-data
# Fri, 24 Jan 2020 10:44:02 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eccdcd97be351ef8da754f6efea3745b7060b1fe92ab96e4b8f5ff85b6322da9`  
		Last Modified: Sat, 18 Jan 2020 04:12:49 GMT  
		Size: 1.4 MB (1397881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea78a138902aeee431e9b31b236dfea5d4f95a1e155aada946ca57f6650a4da9`  
		Last Modified: Sat, 18 Jan 2020 04:12:49 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fda899b5dd7be53564e6266c17b869d98468c50bc887279c51acacfa831de39f`  
		Last Modified: Sat, 18 Jan 2020 04:12:49 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c24c1e693453ad6efa656fcfa28e76c0786f80b4467d83c277d1116117942973`  
		Last Modified: Fri, 24 Jan 2020 02:32:44 GMT  
		Size: 10.3 MB (10271124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb71fc05f0fe0d365d8b9891f304e0cf2c1f6f0d2200ecdc0ea9a1c569117a1d`  
		Last Modified: Fri, 24 Jan 2020 02:32:41 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcf26116548345ee1f676a6c1fabb768cd60750eb7a3a0ac7f09724350dde3b1`  
		Last Modified: Fri, 24 Jan 2020 02:32:54 GMT  
		Size: 15.5 MB (15539990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc4f870d6f2e6bbade33c0f28534b50765c4b56a093dc7565bd3ec3b37a7c603`  
		Last Modified: Fri, 24 Jan 2020 02:32:41 GMT  
		Size: 2.2 KB (2211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6a738ee51d709e4c4db983f9206a240500a2fc0dbaf3c76f6da2f99e5f6eb3b`  
		Last Modified: Fri, 24 Jan 2020 02:32:41 GMT  
		Size: 73.0 KB (72992 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b96c85b9fa53a634f723c297fc6b59b251f92cb4626814d0e9d5a8d529c10645`  
		Last Modified: Fri, 24 Jan 2020 10:52:52 GMT  
		Size: 6.8 MB (6797990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abc67bc763a14a530208fdd5763490a1c330862bdd0c89148468d32c55156871`  
		Last Modified: Fri, 24 Jan 2020 10:52:41 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d9386b58582b59c89c3f23ef3f966901e911d177375585dcd4d6d51b5e07df`  
		Last Modified: Fri, 24 Jan 2020 10:52:45 GMT  
		Size: 9.5 MB (9515329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255060848db5405c91d4f36ce864b67fddab2f49d05409ffb435d605028d0de0`  
		Last Modified: Fri, 24 Jan 2020 10:52:41 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41a94d131eee3b8d4a538aae02122902c1c95f8dd9f1b15f0beef26d6580ccd5`  
		Last Modified: Fri, 24 Jan 2020 10:52:43 GMT  
		Size: 1.3 MB (1261520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1edac81cfd36a02ce3ab444b1315930dc5c1b60d06376796924fd2ebbe87201`  
		Last Modified: Fri, 24 Jan 2020 10:52:41 GMT  
		Size: 415.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
