## `wordpress:cli-2.6.0-php8.0`

```console
$ docker pull wordpress@sha256:632da40402d8a839fba053d28294cf6154976f54317feeb23577861e52c2345c
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

### `wordpress:cli-2.6.0-php8.0` - linux; amd64

```console
$ docker pull wordpress@sha256:bd4a81d67e712af78de5b008babc5930b0f51f404301677519754d22e461d9c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.5 MB (61542102 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58eba168b4c6bc16243f97d2ec71270e0d34fbd79ffd65f4d26d06da365f54d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 19:45:12 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 23 Mar 2022 19:45:13 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 23 Mar 2022 19:45:14 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 23 Mar 2022 19:45:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Mar 2022 19:45:14 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Mar 2022 19:45:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Mar 2022 19:45:15 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Mar 2022 19:45:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Mar 2022 19:57:35 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 23 Mar 2022 19:57:35 GMT
ENV PHP_VERSION=8.0.17
# Wed, 23 Mar 2022 19:57:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Wed, 23 Mar 2022 19:57:36 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Wed, 23 Mar 2022 19:57:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 23 Mar 2022 19:57:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 23 Mar 2022 20:03:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 23 Mar 2022 20:03:16 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Wed, 23 Mar 2022 20:03:17 GMT
RUN docker-php-ext-enable sodium
# Wed, 23 Mar 2022 20:03:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 23 Mar 2022 20:03:17 GMT
CMD ["php" "-a"]
# Thu, 24 Mar 2022 00:48:31 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 24 Mar 2022 00:48:32 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 24 Mar 2022 00:48:32 GMT
WORKDIR /var/www/html
# Thu, 24 Mar 2022 00:49:31 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 24 Mar 2022 00:49:32 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 24 Mar 2022 00:49:32 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 24 Mar 2022 00:49:32 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Thu, 24 Mar 2022 00:49:32 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Thu, 24 Mar 2022 00:49:34 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 24 Mar 2022 00:49:34 GMT
VOLUME [/var/www/html]
# Thu, 24 Mar 2022 00:49:35 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 24 Mar 2022 00:49:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 00:49:35 GMT
USER www-data
# Thu, 24 Mar 2022 00:49:35 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8db862ea11831182b44c30af5fe9a9d7a0a33ede23de2482832ad09902c2c38a`  
		Last Modified: Wed, 23 Mar 2022 20:28:51 GMT  
		Size: 1.7 MB (1701405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c92df0fd37d665420d042811c859bba6dddf421523f9accdf306497e001f757a`  
		Last Modified: Wed, 23 Mar 2022 20:28:50 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b033a355a5348fb8a2e760174881344dec92127fa99714b67e5155c80e6b072`  
		Last Modified: Wed, 23 Mar 2022 20:28:50 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8f4811712ba447fcc242454d933d0b4db4b038f48e8def62d6d35abe53dbbc3`  
		Last Modified: Wed, 23 Mar 2022 20:30:26 GMT  
		Size: 10.8 MB (10790987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c827bccd8fb4b84cc71ce568ed3592a8572e1955297dd7407a6d48e395f6a7dd`  
		Last Modified: Wed, 23 Mar 2022 20:30:25 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bd4c37e6acfeae6d778ba1935adf3727c762aa3540ea04e11ee343e9922c1d`  
		Last Modified: Wed, 23 Mar 2022 20:30:28 GMT  
		Size: 15.8 MB (15757544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b57b9eb2f51b067e95ecba6280b1ea79408d712fe1febf65bf1747182c5716f5`  
		Last Modified: Wed, 23 Mar 2022 20:30:25 GMT  
		Size: 2.3 KB (2302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9117f85ac9d568492309a409d2066e84dfc82e45997911ee248d63449e0129`  
		Last Modified: Wed, 23 Mar 2022 20:30:25 GMT  
		Size: 18.4 KB (18393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39cb0874ac946d5d63ea4a2687166e14a087b580f7c54778f426c6ab870b15ae`  
		Last Modified: Thu, 24 Mar 2022 00:55:08 GMT  
		Size: 9.3 MB (9309989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f4448e0527c66ae7afabbd618889cbcc995b087ffdfe93b77436a23b1d2a409`  
		Last Modified: Thu, 24 Mar 2022 00:55:04 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5677e9731af4c3e1c8ae9f6daaee2614ac26d792e7be88948e1012e60536e3`  
		Last Modified: Thu, 24 Mar 2022 00:55:07 GMT  
		Size: 19.8 MB (19762128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cff0f80ef349a9e9bc77c50cb2a2d990fd37d31cda1253273652b7fee00bef74`  
		Last Modified: Thu, 24 Mar 2022 00:55:04 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4c23f686d37d11a32163b19cb5a86d852deac8220cf892e85a8feea16bf766f`  
		Last Modified: Thu, 24 Mar 2022 00:55:04 GMT  
		Size: 1.4 MB (1383701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce68acbee1f3cf0cc5e7a2580278e14ae0acc15829065974c8a5eac382234f6`  
		Last Modified: Thu, 24 Mar 2022 00:55:04 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.6.0-php8.0` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:ff02acf5c4346ec95ac947c70560b47d68b2054a1de8b6faa85d1f6835f20dcc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.1 MB (59062508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df662fe693febceaf43ea8ad5859dc606dc581248c1ad2fc0dcc870ab9f9077b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Wed, 23 Mar 2022 15:49:35 GMT
ADD file:fd7f6da4a48df653ae6dd18e6d5959008daf5ce429845c974982dc7d213342d9 in / 
# Wed, 23 Mar 2022 15:49:35 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 20:22:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 23 Mar 2022 20:22:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 23 Mar 2022 20:22:52 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 23 Mar 2022 20:22:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Mar 2022 20:22:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Mar 2022 20:22:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Mar 2022 20:22:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Mar 2022 20:22:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Mar 2022 20:33:20 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 23 Mar 2022 20:33:20 GMT
ENV PHP_VERSION=8.0.17
# Wed, 23 Mar 2022 20:33:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Wed, 23 Mar 2022 20:33:21 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Wed, 23 Mar 2022 20:33:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 23 Mar 2022 20:33:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 23 Mar 2022 20:37:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 23 Mar 2022 20:37:51 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Wed, 23 Mar 2022 20:37:54 GMT
RUN docker-php-ext-enable sodium
# Wed, 23 Mar 2022 20:37:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 23 Mar 2022 20:37:54 GMT
CMD ["php" "-a"]
# Thu, 24 Mar 2022 04:25:12 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 24 Mar 2022 04:25:13 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 24 Mar 2022 04:25:14 GMT
WORKDIR /var/www/html
# Thu, 24 Mar 2022 04:27:23 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 24 Mar 2022 04:27:25 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 24 Mar 2022 04:27:25 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 24 Mar 2022 04:27:26 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Thu, 24 Mar 2022 04:27:26 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Thu, 24 Mar 2022 04:27:30 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 24 Mar 2022 04:27:31 GMT
VOLUME [/var/www/html]
# Thu, 24 Mar 2022 04:27:31 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 24 Mar 2022 04:27:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 04:27:32 GMT
USER www-data
# Thu, 24 Mar 2022 04:27:32 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:4e012d7cd81aa4570d9d209a75131b32f34a3533d5d449d23fd875513922588e`  
		Last Modified: Wed, 23 Mar 2022 15:51:07 GMT  
		Size: 2.6 MB (2624816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d354caa9ab8aef049f3e3cdc52ff9a303d3d0e6751121a0954e9e4294547d4c`  
		Last Modified: Wed, 23 Mar 2022 21:04:35 GMT  
		Size: 1.7 MB (1688767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b401fec0babd4f66dfccc06126336327e4f5dae3c7b5af44a85a8520a001960`  
		Last Modified: Wed, 23 Mar 2022 21:04:34 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45da67b0fdd59e6b9d3b25ccd42fdbd8fb76adfc96bae13af5a4e221228d4cc5`  
		Last Modified: Wed, 23 Mar 2022 21:04:34 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b9f9c2b09a3f0de6391324fde9a7da76147716e691592789349b355d3852797`  
		Last Modified: Wed, 23 Mar 2022 21:06:55 GMT  
		Size: 10.8 MB (10790982 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33e77d6b4ffb785d424a6b40050da0fdf1c9149d3be95b30fc15fd88e2d276b5`  
		Last Modified: Wed, 23 Mar 2022 21:06:53 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcdef77882903893aff7a3125fb1c2b98b8da3bf3dfc0d49f5a40dda70c50b3`  
		Last Modified: Wed, 23 Mar 2022 21:07:03 GMT  
		Size: 14.4 MB (14380870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdc02bc21161579799fb4a6fa1e8aa80406ccb85ffdd8ec32d2e835ab8847b95`  
		Last Modified: Wed, 23 Mar 2022 21:06:53 GMT  
		Size: 2.3 KB (2302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4542ae1d5d583891dc0a05f68f29f222df32635a436d4a6574020e5473245af0`  
		Last Modified: Wed, 23 Mar 2022 21:06:53 GMT  
		Size: 18.4 KB (18395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4117770d27c2606a8f9bd23d90c91372eeee9cfdc4d4295e2227f03ca17ef8d9`  
		Last Modified: Thu, 24 Mar 2022 04:37:05 GMT  
		Size: 8.9 MB (8895175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef60dea9c5bcd0fcdfc88041a723a3c354efc217b5169f70c004903c0b445809`  
		Last Modified: Thu, 24 Mar 2022 04:36:58 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bb39dd920785dfea2ae4abd5cb57dfbdb738c2f17016e701f1ef07c621dc0d5`  
		Last Modified: Thu, 24 Mar 2022 04:37:09 GMT  
		Size: 19.3 MB (19274524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:640ec0ceea750a6fc51f92e488123d6dd08aad249fb31f9f9d007cc161e434c1`  
		Last Modified: Thu, 24 Mar 2022 04:36:57 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7163a122269488222e42955e84eb458948a6ae3e06a2807d51919290e1b295c6`  
		Last Modified: Thu, 24 Mar 2022 04:36:58 GMT  
		Size: 1.4 MB (1383710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f744cc188721e6229ce5d106e779ffd963a32610830f87156d43df9db4ce16a`  
		Last Modified: Thu, 24 Mar 2022 04:36:57 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.6.0-php8.0` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:08814c2fa7419e9629db630659ac008111181bdc384858c7d184f17efba55172
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.1 MB (57061287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0d5ff711c4411f24e94b9946de663bf47308eb9c4f13b8baa5be1af9fe0e5a1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Wed, 23 Mar 2022 15:57:29 GMT
ADD file:462f633d612f6502dcfa539fcfd8b1fc90da097b08ad6b984e485bc73e57bd41 in / 
# Wed, 23 Mar 2022 15:57:29 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 22:25:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 23 Mar 2022 22:25:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 23 Mar 2022 22:26:00 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 23 Mar 2022 22:26:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Mar 2022 22:26:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Mar 2022 22:26:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Mar 2022 22:26:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Mar 2022 22:26:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Mar 2022 22:37:57 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 23 Mar 2022 22:37:57 GMT
ENV PHP_VERSION=8.0.17
# Wed, 23 Mar 2022 22:37:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Wed, 23 Mar 2022 22:37:58 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Wed, 23 Mar 2022 22:38:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 23 Mar 2022 22:38:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 23 Mar 2022 22:42:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 23 Mar 2022 22:42:13 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Wed, 23 Mar 2022 22:42:16 GMT
RUN docker-php-ext-enable sodium
# Wed, 23 Mar 2022 22:42:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 23 Mar 2022 22:42:16 GMT
CMD ["php" "-a"]
# Thu, 24 Mar 2022 07:10:02 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 24 Mar 2022 07:10:04 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 24 Mar 2022 07:10:04 GMT
WORKDIR /var/www/html
# Thu, 24 Mar 2022 07:12:08 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 24 Mar 2022 07:12:10 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 24 Mar 2022 07:12:10 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 24 Mar 2022 07:12:11 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Thu, 24 Mar 2022 07:12:11 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Thu, 24 Mar 2022 07:12:16 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 24 Mar 2022 07:12:16 GMT
VOLUME [/var/www/html]
# Thu, 24 Mar 2022 07:12:16 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 24 Mar 2022 07:12:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 07:12:17 GMT
USER www-data
# Thu, 24 Mar 2022 07:12:18 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:dfd6a1b07255bd60715939c7488b4714efdc3519f793d4d8b238b910091c1642`  
		Last Modified: Wed, 23 Mar 2022 15:58:58 GMT  
		Size: 2.4 MB (2427061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6493b36aa91bc2d006c3436da48a310b2195fcb4e4427179984035b756d10f83`  
		Last Modified: Wed, 23 Mar 2022 23:19:59 GMT  
		Size: 1.6 MB (1556458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2de37f9bd8d4b2409f74dda140b9d1dd512ead2cdc1d48930b328ddb8c54a934`  
		Last Modified: Wed, 23 Mar 2022 23:19:58 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc66dbc0b66591a35d1e78eecdf4d2b78f6299de43aae95eb9cafe7575e7d63`  
		Last Modified: Wed, 23 Mar 2022 23:19:58 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2099d9836b566c3faf1dac48f3bec88f887d66df0223f0678631dc3cc0f00cc`  
		Last Modified: Wed, 23 Mar 2022 23:22:57 GMT  
		Size: 10.8 MB (10790968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d5a8f7a3c7f62fe99dee77ae510d917affc4f71a3f1cab0bb4c5a63f5e0f92c`  
		Last Modified: Wed, 23 Mar 2022 23:22:55 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ed48351df25781f66d38358c929ff693f04522338a8bbd06b969e9208bd4d5`  
		Last Modified: Wed, 23 Mar 2022 23:23:01 GMT  
		Size: 13.5 MB (13512008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:579c19734dc0ae7958f33027492d167691f96fbd16290a218dd9fd842055f56f`  
		Last Modified: Wed, 23 Mar 2022 23:22:55 GMT  
		Size: 2.3 KB (2301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b964a5134139fb1f755110e5aac2365183ae3a72bc9ea04f0c85200c68de6bb1`  
		Last Modified: Wed, 23 Mar 2022 23:22:55 GMT  
		Size: 18.4 KB (18367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9796eb0a36d76f0bda98937ec9d11eef04f0bc54d9fbb2c231714d4e8d63cdb1`  
		Last Modified: Thu, 24 Mar 2022 07:26:57 GMT  
		Size: 8.6 MB (8603495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a15f0bde63fb87c44c8595123510f3c40e1e9e027d5c41ccbea73c95c2782b`  
		Last Modified: Thu, 24 Mar 2022 07:26:49 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cd65bb6626380226968b0abdedba79ae7407fa203e7577d1e35362373d98bd`  
		Last Modified: Thu, 24 Mar 2022 07:26:59 GMT  
		Size: 18.8 MB (18764015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7727b1597f20e534694a49efbf06207eb610d50d0f4b8304e35e0efd297fa22`  
		Last Modified: Thu, 24 Mar 2022 07:26:49 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0ce3b70ef06959e556f28649b76852bb235144a432299bfcaa53b5fe7e243f1`  
		Last Modified: Thu, 24 Mar 2022 07:26:50 GMT  
		Size: 1.4 MB (1383646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b26e7652ff9340e43cdb75eb975b7037cbd787af0fe4a93e3937d33e35795b`  
		Last Modified: Thu, 24 Mar 2022 07:26:49 GMT  
		Size: 412.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.6.0-php8.0` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:f8fc122ba6b223f2f923e29cb2d117b2340aa6d14b11f462a0c3a52df7c2142d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.7 MB (60710088 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9475cafb3780d60bdaf427df8b9a912afafd3c965aa5eddfe025e0e82695a655`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Thu, 17 Mar 2022 03:19:52 GMT
ADD file:cd7d91362950471ca4678cf3833dc47119ab519dea51424c847bbbb21e1649d4 in / 
# Thu, 17 Mar 2022 03:19:52 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 14:43:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Mar 2022 14:43:51 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Mar 2022 14:43:52 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Mar 2022 14:43:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 14:43:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 14:43:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 14:43:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 14:43:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Mar 2022 16:13:01 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 18 Mar 2022 19:38:42 GMT
ENV PHP_VERSION=8.0.17
# Fri, 18 Mar 2022 19:38:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Fri, 18 Mar 2022 19:38:44 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Fri, 18 Mar 2022 19:39:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 18 Mar 2022 19:39:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 19:42:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 19:42:35 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 18 Mar 2022 19:42:36 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 19:42:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 19:42:37 GMT
CMD ["php" "-a"]
# Sat, 19 Mar 2022 20:47:15 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Sat, 19 Mar 2022 20:47:15 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Sat, 19 Mar 2022 20:47:16 GMT
WORKDIR /var/www/html
# Sat, 19 Mar 2022 20:48:12 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Sat, 19 Mar 2022 20:48:13 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 19 Mar 2022 20:48:14 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Sat, 19 Mar 2022 20:48:15 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Sat, 19 Mar 2022 20:48:16 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Sat, 19 Mar 2022 20:48:58 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Sat, 19 Mar 2022 20:48:59 GMT
VOLUME [/var/www/html]
# Sat, 19 Mar 2022 20:49:01 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Sat, 19 Mar 2022 20:49:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 20:49:02 GMT
USER www-data
# Sat, 19 Mar 2022 20:49:03 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:148d739a8e6b9342daa1f5b428d3a3c6118f340f21df28c16e06f918ef150147`  
		Last Modified: Thu, 17 Mar 2022 03:20:45 GMT  
		Size: 2.7 MB (2714807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:378b20e8477c36cc1be174280f5a2b65311c1515ce96a0b184115b8d3d91621a`  
		Last Modified: Thu, 17 Mar 2022 18:16:57 GMT  
		Size: 1.7 MB (1696239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:179204a5f49bd0b91f31ca967d0f446d0e6ad07893fda380dff2a54390545d7e`  
		Last Modified: Thu, 17 Mar 2022 18:16:56 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f48a1f9fed16bd6666e8e1b7b1a6e5d1eb34f5f3fd7d73c33e17463f497aa55f`  
		Last Modified: Thu, 17 Mar 2022 18:16:56 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:277f0c436da8e1a31c635b25e525ed6f8ba107018fd7df4a21aaa83aeaf1a686`  
		Last Modified: Fri, 18 Mar 2022 20:38:40 GMT  
		Size: 10.8 MB (10790761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334fa98aca235784abf93985b2657b476ba81c62e51c87a0dad27e55136f79c0`  
		Last Modified: Fri, 18 Mar 2022 20:38:39 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2530fc9d53e625388eddd236549f20cd47df27bcc149309414cb4334791cfb07`  
		Last Modified: Fri, 18 Mar 2022 20:38:42 GMT  
		Size: 15.2 MB (15180201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f736b4ee7be933d70710ae9373d94398f043b1810891dac8b5c0f5f56eeb36d1`  
		Last Modified: Fri, 18 Mar 2022 20:38:39 GMT  
		Size: 2.3 KB (2301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1afb1f675b4b4af25eea9fc5ef28338739c9d52c0ffe2b7a1794f90825a41482`  
		Last Modified: Fri, 18 Mar 2022 20:38:39 GMT  
		Size: 18.3 KB (18312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c89fc48e7be0ddc2b597bfca450c9e90c488ebefecdd090c6f8d9c011b90934`  
		Last Modified: Sat, 19 Mar 2022 20:57:31 GMT  
		Size: 9.3 MB (9343988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:738f0bbf4cb3478e226562d9d1f82169d806d4fa52a411f3761ef6824045d2ab`  
		Last Modified: Sat, 19 Mar 2022 20:57:32 GMT  
		Size: 19.6 MB (19577289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce28603c8166c64a0c4cc26725fad8e36d8214b251237a307c94d1c0902d41f9`  
		Last Modified: Sat, 19 Mar 2022 20:57:29 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92c019a971d13cc0fb99260bdc47b76c52a6702f8626f07fbc3f3b9e7d08acea`  
		Last Modified: Sat, 19 Mar 2022 20:57:30 GMT  
		Size: 1.4 MB (1383442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807d37935e6b0c11999770645706fb352b156cd2c870ec6bb8994e4f58fed53b`  
		Last Modified: Sat, 19 Mar 2022 20:57:30 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.6.0-php8.0` - linux; 386

```console
$ docker pull wordpress@sha256:fa8fd7cb7e274b34860bb904c511f4a92d63070dba38197024320a3624b0c31d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.5 MB (62473289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:67675a7813a85359fdff529ecfffe782e028ed862d4baa5644da9f23bbd76bcf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Thu, 17 Mar 2022 08:13:03 GMT
ADD file:22216bc654d9177244235f242fa83cae3b283b3c145cad7ccf11c0d29f5f0ff2 in / 
# Thu, 17 Mar 2022 08:13:03 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 23:57:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Mar 2022 23:57:43 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Mar 2022 23:57:44 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Mar 2022 23:57:44 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 23:57:45 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 23:57:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 23:57:45 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 23:57:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 18 Mar 2022 03:36:26 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 18 Mar 2022 22:07:29 GMT
ENV PHP_VERSION=8.0.17
# Fri, 18 Mar 2022 22:07:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Fri, 18 Mar 2022 22:07:29 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Fri, 18 Mar 2022 22:08:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 18 Mar 2022 22:08:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:15:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 22:15:01 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Fri, 18 Mar 2022 22:15:02 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 22:15:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 22:15:02 GMT
CMD ["php" "-a"]
# Sat, 19 Mar 2022 11:57:35 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Sat, 19 Mar 2022 11:57:36 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Sat, 19 Mar 2022 11:57:36 GMT
WORKDIR /var/www/html
# Sat, 19 Mar 2022 11:58:46 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Sat, 19 Mar 2022 11:58:46 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 19 Mar 2022 11:58:46 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Sat, 19 Mar 2022 11:58:47 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Sat, 19 Mar 2022 11:58:47 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Sat, 19 Mar 2022 11:58:49 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Sat, 19 Mar 2022 11:58:50 GMT
VOLUME [/var/www/html]
# Sat, 19 Mar 2022 11:58:50 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Sat, 19 Mar 2022 11:58:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 11:58:50 GMT
USER www-data
# Sat, 19 Mar 2022 11:58:50 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:93317a1f65ec94b67aefe728a598022610246404e3a68d391c76cd0e5244a2a0`  
		Last Modified: Thu, 17 Mar 2022 08:13:56 GMT  
		Size: 2.8 MB (2821789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b85ed7943e33403f16e09d278f9c192289e46abd931b3dae7dea4556fd3a5c`  
		Last Modified: Fri, 18 Mar 2022 08:28:13 GMT  
		Size: 1.8 MB (1800228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20d130a920a6ad3da405eeae397a9b3f2f7b8daf56b19bcd3ad75b14ca680c0`  
		Last Modified: Fri, 18 Mar 2022 08:28:12 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b27c54a134a9b3043eba2ddc74fe9e80629c03e7165d26bf890fc38488cc16`  
		Last Modified: Fri, 18 Mar 2022 08:28:11 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc192f25754c8f7dc1f256b6429393bae85fcd338ceeb55a484c8c436079feea`  
		Last Modified: Fri, 18 Mar 2022 23:00:15 GMT  
		Size: 10.8 MB (10790988 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0724b02c82a5d0c5494a5d993e7203919fc90d17bc037609474f5c40fd6852db`  
		Last Modified: Fri, 18 Mar 2022 23:00:13 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b769c245b04365d5e93b99eda35a4f292f99b4c99224853ecf7e0ba7ef696ca8`  
		Last Modified: Fri, 18 Mar 2022 23:00:18 GMT  
		Size: 16.1 MB (16082337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c7427f7422f025c8696f2a3ac40805ed0e74016ce9c5352bf8af303c755d163`  
		Last Modified: Fri, 18 Mar 2022 23:00:14 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ec71f4d1ce263d2f54e9185d0a5295f2992aa9fe902de4991a638a1f511f607`  
		Last Modified: Fri, 18 Mar 2022 23:00:13 GMT  
		Size: 18.4 KB (18383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1474e1736affdc8eba27ad30ee97384266f305bc98f595f90326d006776daa1b`  
		Last Modified: Sat, 19 Mar 2022 12:13:39 GMT  
		Size: 9.4 MB (9447082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c717f186564de625540f25fabe3317ad49316c252fa0c18a7d3c719dc6b1f9`  
		Last Modified: Sat, 19 Mar 2022 12:13:34 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70dce119f61becb9b47677d2b7cc16d1d0940453d4420483a63104fda38db36`  
		Last Modified: Sat, 19 Mar 2022 12:13:38 GMT  
		Size: 20.1 MB (20123547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac42cd2872c0ba9ec82a7a8261ad71693c8a67d0760c0350d01badf686755475`  
		Last Modified: Sat, 19 Mar 2022 12:13:34 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd5d8c1fdd8ae49a9d66f14b61d68e611ed2e56a5b59dc0bd262a99b1a8c55b8`  
		Last Modified: Sat, 19 Mar 2022 12:13:35 GMT  
		Size: 1.4 MB (1383666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7553d035b793d90f76c7478c8490199a81a2471caebeb2feeb3eac1372b378b`  
		Last Modified: Sat, 19 Mar 2022 12:13:34 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.6.0-php8.0` - linux; ppc64le

```console
$ docker pull wordpress@sha256:92f603723157f3bf46d688a4a17ceb7b8daecc0979bdb6acae34855712d63bfa
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **62.8 MB (62817273 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70d62519c9426c1434795c9944b73b0ced7186812793609761fcebf75ee7eb84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Wed, 23 Mar 2022 15:24:30 GMT
ADD file:3392b3547a6a1366b9a6ada72065830d8886708bbfc70472c607e742dfd07994 in / 
# Wed, 23 Mar 2022 15:24:32 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 22:04:28 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 23 Mar 2022 22:04:39 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 23 Mar 2022 22:04:49 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 23 Mar 2022 22:04:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Mar 2022 22:05:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Mar 2022 22:05:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Mar 2022 22:05:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Mar 2022 22:05:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Mar 2022 22:18:05 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 23 Mar 2022 22:18:08 GMT
ENV PHP_VERSION=8.0.17
# Wed, 23 Mar 2022 22:18:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Wed, 23 Mar 2022 22:18:15 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Wed, 23 Mar 2022 22:18:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 23 Mar 2022 22:18:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 23 Mar 2022 22:23:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 23 Mar 2022 22:23:35 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Wed, 23 Mar 2022 22:23:42 GMT
RUN docker-php-ext-enable sodium
# Wed, 23 Mar 2022 22:23:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 23 Mar 2022 22:23:48 GMT
CMD ["php" "-a"]
# Thu, 24 Mar 2022 09:04:52 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 24 Mar 2022 09:05:07 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 24 Mar 2022 09:05:13 GMT
WORKDIR /var/www/html
# Thu, 24 Mar 2022 09:06:54 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 24 Mar 2022 09:07:09 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 24 Mar 2022 09:07:14 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 24 Mar 2022 09:07:17 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Thu, 24 Mar 2022 09:07:31 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Thu, 24 Mar 2022 09:07:48 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Thu, 24 Mar 2022 09:07:52 GMT
VOLUME [/var/www/html]
# Thu, 24 Mar 2022 09:07:54 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 24 Mar 2022 09:07:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 24 Mar 2022 09:07:59 GMT
USER www-data
# Thu, 24 Mar 2022 09:08:07 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:58323f60457d1c04dce77185ce8c0377ac10135b55fdf4506e87d24e67780d7d`  
		Last Modified: Wed, 23 Mar 2022 15:25:23 GMT  
		Size: 2.8 MB (2814037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f78867943bb57fcac766b3eb0b022125f22323ef1867a2a727cc5c9d010c94`  
		Last Modified: Wed, 23 Mar 2022 22:57:07 GMT  
		Size: 1.7 MB (1744638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba7b3ac49454cdc93d74a8a9baf849cf874409439c0452d6e75b385c1eb8068b`  
		Last Modified: Wed, 23 Mar 2022 22:57:06 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68badc43ad09521b584065557959196c069547e694debc7f5ea441eee76f06c5`  
		Last Modified: Wed, 23 Mar 2022 22:57:06 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63caa854675aa3324c7328b8c18c9c3daf22a1ffb22bbfa0e995249fac33867`  
		Last Modified: Wed, 23 Mar 2022 22:59:15 GMT  
		Size: 10.8 MB (10790995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1603f4c42423835185201691e3210a43e8f71b6469fd0f86fb9e8bfe85fcb744`  
		Last Modified: Wed, 23 Mar 2022 22:59:14 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db814e111390bf1a0aceb36da8832f6f401072bac75362d10f8e308bdc832e6`  
		Last Modified: Wed, 23 Mar 2022 22:59:18 GMT  
		Size: 16.5 MB (16486590 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41248cdfd49a4772adb2f77bfe9e2004f9335db7142ceb8168244a4b4e911bd5`  
		Last Modified: Wed, 23 Mar 2022 22:59:14 GMT  
		Size: 2.3 KB (2300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:044c8b60aa568fb0b047560540fac701dded371c5d1bb9e4310620c9b3551a7e`  
		Last Modified: Wed, 23 Mar 2022 22:59:15 GMT  
		Size: 18.4 KB (18391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6658a2fdbff88285b0707627bb3bd76046eee786ccbdbfd8c08e664643b5130`  
		Last Modified: Thu, 24 Mar 2022 09:20:07 GMT  
		Size: 9.5 MB (9490032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ade43bb386138a816d74f4eda5e08dc7ab6ad4e7eddd5611c6e6fdd90c74cdda`  
		Last Modified: Thu, 24 Mar 2022 09:20:01 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c066bcae5649608eb040f44c3510ea804c0f7c09ff6fb7ba82a1cb3ec38673c2`  
		Last Modified: Thu, 24 Mar 2022 09:20:06 GMT  
		Size: 20.1 MB (20083665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e49920836d7369ae3cef3966b6edc00838af643f8fb97bf6c9527b3131130ed`  
		Last Modified: Thu, 24 Mar 2022 09:20:01 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50c982bdb820cb141a7ae7165a10e051d6391cf5e18433d623f08070f2fd2a07`  
		Last Modified: Thu, 24 Mar 2022 09:20:02 GMT  
		Size: 1.4 MB (1383654 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e657d49ae4c1e693309eb15de4410b651171858cb126d81824d6c9d6d9f2cb5`  
		Last Modified: Thu, 24 Mar 2022 09:20:01 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2.6.0-php8.0` - linux; s390x

```console
$ docker pull wordpress@sha256:ebed11187fa2599ce2926d868481b4e143a415e6e2469f5262dd2cdb9174a81c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.0 MB (60950330 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:70e381499ac593043367d4422f8ab5792777044e08423510c230eae9bc791a00`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Wed, 23 Mar 2022 15:41:27 GMT
ADD file:c6fe4c8affcc912e0de86d8691aecb959ac828259f09843a569ec4e5714d6c6f in / 
# Wed, 23 Mar 2022 15:41:27 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 21:22:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 23 Mar 2022 21:22:28 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 23 Mar 2022 21:22:29 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 23 Mar 2022 21:22:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 23 Mar 2022 21:22:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 23 Mar 2022 21:22:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Mar 2022 21:22:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 23 Mar 2022 21:22:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 23 Mar 2022 21:29:41 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Wed, 23 Mar 2022 21:29:41 GMT
ENV PHP_VERSION=8.0.17
# Wed, 23 Mar 2022 21:29:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.17.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.17.tar.xz.asc
# Wed, 23 Mar 2022 21:29:42 GMT
ENV PHP_SHA256=4e7d94bb3d144412cb8b2adeb599fb1c6c1d7b357b0d0d0478dc5ef53532ebc5
# Wed, 23 Mar 2022 21:29:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 23 Mar 2022 21:29:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 23 Mar 2022 21:32:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 23 Mar 2022 21:32:30 GMT
COPY multi:a00980ff863125d6071b93844e0a51dc89719405d95217aba6860be950a05740 in /usr/local/bin/ 
# Wed, 23 Mar 2022 21:32:31 GMT
RUN docker-php-ext-enable sodium
# Wed, 23 Mar 2022 21:32:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 23 Mar 2022 21:32:31 GMT
CMD ["php" "-a"]
# Wed, 23 Mar 2022 23:56:15 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Wed, 23 Mar 2022 23:56:16 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Wed, 23 Mar 2022 23:56:16 GMT
WORKDIR /var/www/html
# Wed, 23 Mar 2022 23:56:55 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 23 Mar 2022 23:56:56 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 23 Mar 2022 23:56:56 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Wed, 23 Mar 2022 23:56:56 GMT
ENV WORDPRESS_CLI_VERSION=2.6.0
# Wed, 23 Mar 2022 23:56:56 GMT
ENV WORDPRESS_CLI_SHA512=d73f9161a1f03b8ecaac7b196b6051fe847b3c402b9c92b1f6f3acbe5b1cf91f7260c0e499b8947bab75920ecec918b39533ca65fa5a1fd3eb6ce7b8e2c58e7d
# Wed, 23 Mar 2022 23:56:58 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Wed, 23 Mar 2022 23:56:59 GMT
VOLUME [/var/www/html]
# Wed, 23 Mar 2022 23:56:59 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Wed, 23 Mar 2022 23:56:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 23 Mar 2022 23:56:59 GMT
USER www-data
# Wed, 23 Mar 2022 23:56:59 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:cf2f18c21a46b2d59a7a34a051c9c289710e89cdef47cc582fdb9d65a1e68e44`  
		Last Modified: Wed, 23 Mar 2022 15:42:18 GMT  
		Size: 2.6 MB (2601698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:231067ec1ee4b0c99cf93639423e826ad61a33431a1cc48af60e85a60fa8b3ef`  
		Last Modified: Wed, 23 Mar 2022 21:53:24 GMT  
		Size: 1.8 MB (1760648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb50267f7ed7a09bcfdb4ffe51bf855be87cd4ec459433b976be8ba2252ef3d0`  
		Last Modified: Wed, 23 Mar 2022 21:53:24 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e02902b39382b4f02ab26615348f1aaa83fe1c88f07e870abc85e70db4d7ee`  
		Last Modified: Wed, 23 Mar 2022 21:53:24 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81e9788657640e8d439943aebb57e422823bbe86ccab871fd8b446bbb5aa1dc9`  
		Last Modified: Wed, 23 Mar 2022 21:54:54 GMT  
		Size: 10.8 MB (10790997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e58b36380c306e1de0f5003b22a485fffad47c673a5bb5808ea71d4896790d`  
		Last Modified: Wed, 23 Mar 2022 21:54:53 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e2b0ed2153d889553a9aff5af3c5580f02a8a3d1a4588efc690409a1bd2056`  
		Last Modified: Wed, 23 Mar 2022 21:54:55 GMT  
		Size: 14.8 MB (14775796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744c0be832751bbfcc42aab212432fd79e00e04964e2a2bd0ca2b3a3a9368b98`  
		Last Modified: Wed, 23 Mar 2022 21:54:53 GMT  
		Size: 2.3 KB (2301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1f616416aaaebeb0f2ef9cc0dd2923903a0937c2af80f13f14d02f8fb710c6`  
		Last Modified: Wed, 23 Mar 2022 21:54:53 GMT  
		Size: 18.4 KB (18412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:369602738583486fcbec622a548e7237449b3597ba3033cd4db26578a2123573`  
		Last Modified: Thu, 24 Mar 2022 00:04:08 GMT  
		Size: 9.8 MB (9779349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec26c92fb9f185a07d2ad95ce07832c01c62d0a3be8a67dfc130c3e84177e0be`  
		Last Modified: Thu, 24 Mar 2022 00:04:06 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6636e08ecd9fee3d9b3bffe80757aaa054ecc046216553c5fcd6ac02b66d4b66`  
		Last Modified: Thu, 24 Mar 2022 00:04:08 GMT  
		Size: 19.8 MB (19834477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4007d454b77380aec69d93d6c8ea41587f88e17626a00146262568dae316f1`  
		Last Modified: Thu, 24 Mar 2022 00:04:05 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b5bd08350e9056b3abe364701f9fa01569a8dbae53a696dc7e20b414ef658d6`  
		Last Modified: Thu, 24 Mar 2022 00:04:06 GMT  
		Size: 1.4 MB (1383690 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9a4c2074b79d484c77b2edeb9caa6be21ace916502192b05260bba44bef60dc`  
		Last Modified: Thu, 24 Mar 2022 00:04:06 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
