## `wordpress:cli-2-php7.3`

```console
$ docker pull wordpress@sha256:5624eb776398084610291d11e93ea756563f8bc6e32f0f9d51182e0630833e7f
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

### `wordpress:cli-2-php7.3` - linux; amd64

```console
$ docker pull wordpress@sha256:7a5c2aaeb083d63cf19c54d79041fb2295ad148e80f6be4c747e12ace0be3a06
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.2 MB (48231966 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:90a77b4450dd5ef2b8be0be59e4a18d9964c00c0148e5fd6e5288c151157a566`
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
# Thu, 17 Dec 2020 09:38:32 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 17 Dec 2020 09:38:32 GMT
ENV PHP_VERSION=7.3.25
# Thu, 17 Dec 2020 09:38:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Thu, 17 Dec 2020 09:38:32 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Thu, 17 Dec 2020 09:38:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 09:38:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 09:44:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 09:44:55 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 17 Dec 2020 09:44:56 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 09:44:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 09:44:57 GMT
CMD ["php" "-a"]
# Thu, 17 Dec 2020 18:47:50 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 17 Dec 2020 18:47:51 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 17 Dec 2020 18:47:53 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 17 Dec 2020 18:47:54 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 17 Dec 2020 18:47:54 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 18:47:54 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 17 Dec 2020 18:47:54 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 17 Dec 2020 18:47:54 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 17 Dec 2020 18:47:56 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Thu, 17 Dec 2020 18:47:56 GMT
VOLUME [/var/www/html]
# Thu, 17 Dec 2020 18:47:57 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 17 Dec 2020 18:47:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 18:47:57 GMT
USER www-data
# Thu, 17 Dec 2020 18:47:57 GMT
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
	-	`sha256:4ef1d3220c63e2f51180b0495b28d88db27a61ebb631b335801861a377d65422`  
		Last Modified: Thu, 17 Dec 2020 11:08:41 GMT  
		Size: 12.2 MB (12155939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d558dbbe44f2eee6f47745405921fac8b3c707831cbb2e64ebc2bed0c607b978`  
		Last Modified: Thu, 17 Dec 2020 11:08:39 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17dfefe42c21e2f46fbdcebe3becd00970e97ba4a749d7ad03923ba780874f0b`  
		Last Modified: Thu, 17 Dec 2020 11:08:44 GMT  
		Size: 14.4 MB (14391378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19468d138ea7eca5a1aad67e892e01cec6fb985b64c62433a6ddaecd6da658cb`  
		Last Modified: Thu, 17 Dec 2020 11:08:40 GMT  
		Size: 2.3 KB (2256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b06da981aaccfb96ac524dfc4bb4051f60547d768f5d87ebd5aef44390d42d3`  
		Last Modified: Thu, 17 Dec 2020 11:08:40 GMT  
		Size: 16.7 KB (16710 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97f959592dc8315be3176058587ca8e5690f598727fdcd9fedd0e95d14a434e`  
		Last Modified: Thu, 17 Dec 2020 18:51:46 GMT  
		Size: 7.0 MB (7036622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:269ec665634f48c2b292da3590c3498a1cdcc84741a71500bd051efb44c1cfd0`  
		Last Modified: Thu, 17 Dec 2020 18:51:44 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d8f3615af1013e1ec8ffde01bc0164628967058e7f7c0c46612cf4ffeca636a`  
		Last Modified: Thu, 17 Dec 2020 18:51:46 GMT  
		Size: 9.3 MB (9281049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cb6cb640b484ca6915f3667d8adbf8b3a84da67cd5c9cadfc5d89093e7ee3ea`  
		Last Modified: Thu, 17 Dec 2020 18:51:43 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c85b6e074d0cf490d2aa9eef334b890dc4f8576614f2253d750522f40c9e697a`  
		Last Modified: Thu, 17 Dec 2020 18:51:43 GMT  
		Size: 1.2 MB (1205148 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458ebe891f8db9850dc7e293e093a0613293065bd45f7c2292d6530260171eda`  
		Last Modified: Thu, 17 Dec 2020 18:51:43 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.3` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:37506df1de4ca490c5a5942290ac08590e3d698e0b10b4b07dc75e4cc896f82b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46179049 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cdca38e9801d1805019b8f25db418099271ccfadb1183bc2fb687c1f90e7904`
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
# Thu, 17 Dec 2020 04:41:00 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 07 Jan 2021 18:20:37 GMT
ENV PHP_VERSION=7.3.26
# Thu, 07 Jan 2021 18:20:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.26.tar.xz.asc
# Thu, 07 Jan 2021 18:20:40 GMT
ENV PHP_SHA256=d93052f4cb2882090b6a37fd1e0c764be1605a2461152b7f6b8f04fa48875208
# Thu, 07 Jan 2021 18:20:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 07 Jan 2021 18:20:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 07 Jan 2021 18:24:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 07 Jan 2021 18:24:46 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 07 Jan 2021 18:24:52 GMT
RUN docker-php-ext-enable sodium
# Thu, 07 Jan 2021 18:24:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 07 Jan 2021 18:24:59 GMT
CMD ["php" "-a"]
# Thu, 07 Jan 2021 20:19:32 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 07 Jan 2021 20:19:35 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Jan 2021 20:19:38 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 07 Jan 2021 20:19:41 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 07 Jan 2021 20:19:42 GMT
WORKDIR /var/www/html
# Thu, 07 Jan 2021 20:19:42 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 07 Jan 2021 20:19:43 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 07 Jan 2021 20:19:44 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 07 Jan 2021 20:19:48 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Thu, 07 Jan 2021 20:19:49 GMT
VOLUME [/var/www/html]
# Thu, 07 Jan 2021 20:19:49 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 07 Jan 2021 20:19:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Jan 2021 20:19:51 GMT
USER www-data
# Thu, 07 Jan 2021 20:19:52 GMT
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
	-	`sha256:270ea9943775ed9fc82e73fcaeb5d27ec141598d9358b004d1d7b9dc0993fea9`  
		Last Modified: Thu, 07 Jan 2021 18:50:36 GMT  
		Size: 12.2 MB (12157411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f827f595d1bb9996f9479022ece7c9d25ccfc19204ef84c4a0faa0ac2900bedf`  
		Last Modified: Thu, 07 Jan 2021 18:50:36 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b45f87d65bd1e4a5d844f16888b69a50a5ceb43d69d1347beea24e09bad2803`  
		Last Modified: Thu, 07 Jan 2021 18:50:37 GMT  
		Size: 13.3 MB (13349282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b13cee45a941f56af42baf3f53c64f425f4bd8570b0435c5d09f84a7af39cf9`  
		Last Modified: Thu, 07 Jan 2021 18:50:35 GMT  
		Size: 2.3 KB (2256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b38db76da6b14c2cf0d956e3910536bc0e50d055ca6449df6f05358260d1670`  
		Last Modified: Thu, 07 Jan 2021 18:50:34 GMT  
		Size: 16.7 KB (16708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d32041b7aaca482b0eefde71faa1251b00a03618b694490a22e3e900d5549a`  
		Last Modified: Thu, 07 Jan 2021 20:23:07 GMT  
		Size: 6.7 MB (6657566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a49e015fcd1a0f2c3d9a8d5e3c898a85a0af4a49ee11886997898aa0ec5f5608`  
		Last Modified: Thu, 07 Jan 2021 20:23:02 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95e4f200c86400d1c030834156f8c6f04a573c2f26e17dff0f61847f66f23c6f`  
		Last Modified: Thu, 07 Jan 2021 20:23:04 GMT  
		Size: 8.9 MB (8873155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbab4ec578be1734ed1ef04686a754b6fa947ae90825ef6a4a4f107a524e6589`  
		Last Modified: Thu, 07 Jan 2021 20:23:02 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1dce574202fbb213cd7942e9d48268241a2ec5cc138969024fddaf8012b46250`  
		Last Modified: Thu, 07 Jan 2021 20:23:02 GMT  
		Size: 1.2 MB (1205252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5f7aefce6d7e98f0d851c8eb98ca0e66574d9087cc1830b41adac070f0aa70b`  
		Last Modified: Thu, 07 Jan 2021 20:23:03 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.3` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:eea316cb402c3bb41b22cc61e053b66e774dac73d6e3e3be80f909cfe2a633b9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44592403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:518ed2837f501581986b2d391c7a411ba28950dd5cf70324142922e24b26942e`
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
# Thu, 17 Dec 2020 04:35:19 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 17 Dec 2020 04:35:20 GMT
ENV PHP_VERSION=7.3.25
# Thu, 17 Dec 2020 04:35:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Thu, 17 Dec 2020 04:35:23 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Thu, 17 Dec 2020 04:35:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 04:35:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:38:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 04:38:56 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:39:00 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 04:39:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 04:39:02 GMT
CMD ["php" "-a"]
# Thu, 17 Dec 2020 10:41:30 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 17 Dec 2020 10:41:32 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 17 Dec 2020 10:41:40 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 17 Dec 2020 10:41:43 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 17 Dec 2020 10:41:44 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 10:41:45 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 17 Dec 2020 10:41:46 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 17 Dec 2020 10:41:46 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 17 Dec 2020 10:41:51 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Thu, 17 Dec 2020 10:41:51 GMT
VOLUME [/var/www/html]
# Thu, 17 Dec 2020 10:41:52 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 17 Dec 2020 10:41:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 10:41:54 GMT
USER www-data
# Thu, 17 Dec 2020 10:41:55 GMT
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
	-	`sha256:c66ab96f59a61995af9c9d1b524cf90ba330278673842490ea571c046671d2f8`  
		Last Modified: Thu, 17 Dec 2020 05:31:59 GMT  
		Size: 12.2 MB (12155955 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51dd9ff671de10fd8d5409e617c343a9aa21dc3b701f7be62647740ee4026e31`  
		Last Modified: Thu, 17 Dec 2020 05:31:57 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c045fa7974eb8b185119de919a01e8d62b6c3a43d6a3ec46e00d0ef727dfc509`  
		Last Modified: Thu, 17 Dec 2020 05:32:01 GMT  
		Size: 12.5 MB (12497461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8b7840e525e8202ee7b9eeaea515c487e50ec98fcf7d25226735b4307dfb4db`  
		Last Modified: Thu, 17 Dec 2020 05:31:57 GMT  
		Size: 2.3 KB (2258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dd0931a5d75036051416148562fe600ba9fa5249e67e592ad10f1926aa9f3b`  
		Last Modified: Thu, 17 Dec 2020 05:31:57 GMT  
		Size: 16.7 KB (16677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05ef63fd9040e2b019c60b026a466b8ce721b1f51891e4317d5e5300860a80e2`  
		Last Modified: Thu, 17 Dec 2020 10:46:52 GMT  
		Size: 6.5 MB (6480740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9d4e769e33c395eebd72347c7ae125e6cc21f142798cb5cb38d425680c12a77`  
		Last Modified: Thu, 17 Dec 2020 10:46:48 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fef38e3c5755869314fbbfe62ef34a004e8fd1089bb53131eb5bee0b51d0f1e`  
		Last Modified: Thu, 17 Dec 2020 10:46:51 GMT  
		Size: 8.6 MB (8609081 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc80282c5027217515b83338a8041546810c9d0658a902e127f70c816d56c43`  
		Last Modified: Thu, 17 Dec 2020 10:46:48 GMT  
		Size: 143.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75fe443f58a314c2c7d66b3bd5008605f70fef2be6bba36f979e944c79b5dd30`  
		Last Modified: Thu, 17 Dec 2020 10:46:48 GMT  
		Size: 1.2 MB (1205188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97b2fa3dbb1f076072f624e9508d2d172a0e91f3baf9f2961a4fb3c52bb88235`  
		Last Modified: Thu, 17 Dec 2020 10:46:47 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.3` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:bd8693ac9c20bf3b68db4226e80564f95ad6ee2140b6439b2ade165888c775cb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47769160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3debc63a9429ba387e9b7ec197886935f8c4fd43b98e694171a316a556971846`
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
# Thu, 17 Dec 2020 06:22:49 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 17 Dec 2020 06:22:50 GMT
ENV PHP_VERSION=7.3.25
# Thu, 17 Dec 2020 06:22:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Thu, 17 Dec 2020 06:22:52 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Thu, 17 Dec 2020 06:22:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 06:22:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 06:25:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 06:25:51 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 17 Dec 2020 06:25:55 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 06:25:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 06:25:57 GMT
CMD ["php" "-a"]
# Thu, 17 Dec 2020 12:38:13 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 17 Dec 2020 12:38:16 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 17 Dec 2020 12:38:19 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 17 Dec 2020 12:38:21 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 17 Dec 2020 12:38:22 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 12:38:23 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 17 Dec 2020 12:38:24 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 17 Dec 2020 12:38:25 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 17 Dec 2020 12:38:29 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Thu, 17 Dec 2020 12:38:30 GMT
VOLUME [/var/www/html]
# Thu, 17 Dec 2020 12:38:31 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 17 Dec 2020 12:38:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 12:38:33 GMT
USER www-data
# Thu, 17 Dec 2020 12:38:34 GMT
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
	-	`sha256:a00c5423d18e70b1cbe28e53ae2b8cb7b3d9a0da65de2564859a1e085ff78feb`  
		Last Modified: Thu, 17 Dec 2020 07:13:20 GMT  
		Size: 12.2 MB (12155981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8ac51c339684f799177fdf6e60e9bb136f5b05f56c5d70d462fa194fe6abb73`  
		Last Modified: Thu, 17 Dec 2020 07:13:19 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b01968b19359a3df4b363e17817e45deb7920309123ab1b6796b4314ee39010`  
		Last Modified: Thu, 17 Dec 2020 07:13:23 GMT  
		Size: 14.1 MB (14129283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e022a34034692eebef33b5c5ff2341a51fdf1c9482e5415c70f0dacde289362`  
		Last Modified: Thu, 17 Dec 2020 07:13:19 GMT  
		Size: 2.3 KB (2262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e838b483c5940bf22a464bc5de41d4919095a301ef45043c72199c6c78e38bae`  
		Last Modified: Thu, 17 Dec 2020 07:13:19 GMT  
		Size: 16.7 KB (16715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:446c3523d7a91662b02dac96a0be5cc4249b13385a60c5cac49bf1e5a54c5391`  
		Last Modified: Thu, 17 Dec 2020 12:43:50 GMT  
		Size: 6.9 MB (6865481 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:462850c81ed8b6fede1e74f5be430606a7fe6ea0ea48b719277f82ac5de25d4e`  
		Last Modified: Thu, 17 Dec 2020 12:43:46 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e9b174a2c7e50aedaf0df436a7bd5c4786ac092ccf66047a023a61b1f249f1c`  
		Last Modified: Thu, 17 Dec 2020 12:43:49 GMT  
		Size: 9.3 MB (9339312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51f6c88f88d167ed85ba92e9d534d643dea93abf07c3e215e87374cc44379b82`  
		Last Modified: Thu, 17 Dec 2020 12:43:46 GMT  
		Size: 144.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c3dbfb918ac12a23d3e21a012dd08dab8a61d3ace1202117844bccef921b1e1`  
		Last Modified: Thu, 17 Dec 2020 12:43:47 GMT  
		Size: 1.2 MB (1205177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1995dfac86555a6ccb714a13f21cd82198ed2817fbec8636b0b711a5281a4c6`  
		Last Modified: Thu, 17 Dec 2020 12:43:46 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.3` - linux; 386

```console
$ docker pull wordpress@sha256:959f25d63c42c70bfab62301828a0d8f847d5dc46b0096376d28ac9b285e7fb1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48947852 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4953ef1991a8ca446fa4f60fa57ef77fcf06bfb21b4accde89feaa90844896e9`
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
# Thu, 17 Dec 2020 04:23:31 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 17 Dec 2020 04:23:31 GMT
ENV PHP_VERSION=7.3.25
# Thu, 17 Dec 2020 04:23:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Thu, 17 Dec 2020 04:23:32 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Thu, 17 Dec 2020 04:23:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 04:23:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:29:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 04:29:20 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 17 Dec 2020 04:29:21 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 04:29:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 04:29:22 GMT
CMD ["php" "-a"]
# Thu, 17 Dec 2020 09:36:36 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 17 Dec 2020 09:36:37 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 17 Dec 2020 09:36:40 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 17 Dec 2020 09:36:42 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 17 Dec 2020 09:36:42 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 09:36:42 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 17 Dec 2020 09:36:43 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 17 Dec 2020 09:36:43 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 17 Dec 2020 09:36:46 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Thu, 17 Dec 2020 09:36:47 GMT
VOLUME [/var/www/html]
# Thu, 17 Dec 2020 09:36:47 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 17 Dec 2020 09:36:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 09:36:47 GMT
USER www-data
# Thu, 17 Dec 2020 09:36:48 GMT
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
	-	`sha256:0f0e47ca46462ad813417ee1f5279771a9a358d19c4ea25b40d385da7ad7125e`  
		Last Modified: Thu, 17 Dec 2020 05:46:48 GMT  
		Size: 12.2 MB (12155937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86ab2cb22a5cb6704621c5b07408c767c61b5e80245335c6c998b341a4f2c2d1`  
		Last Modified: Thu, 17 Dec 2020 05:46:45 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99376a260f3a4eab44c6f5c4b04c0dbe87c84654e776030a16565b67db1c83ab`  
		Last Modified: Thu, 17 Dec 2020 05:46:51 GMT  
		Size: 14.7 MB (14735058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb9f162a0be5d0695a32a59224d4b640cdb3d4c5ee591141b7d4cf93b538d773`  
		Last Modified: Thu, 17 Dec 2020 05:46:46 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8922b46c44067291aa6c06aa00232b4ee45af24fdc9b43eb9f58cd59bfd98f62`  
		Last Modified: Thu, 17 Dec 2020 05:46:46 GMT  
		Size: 16.7 KB (16702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c065b45d811fa392c1aaefe2940d1b34e0eda881f86b0a50a79f50c50042551`  
		Last Modified: Thu, 17 Dec 2020 09:41:37 GMT  
		Size: 7.2 MB (7162592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03d20d68112389b17701a76ff8089432477d8d4994345ed7978dd5d6ddb36fdc`  
		Last Modified: Thu, 17 Dec 2020 09:41:31 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5326cc0abebaf3b84569f92fc088fd20fa9ad5a6c88965cc6c4104264021b42`  
		Last Modified: Thu, 17 Dec 2020 09:41:38 GMT  
		Size: 9.4 MB (9433344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7328e586cdb6d87ce862d8b2b4720c900452939ee06cdd0fd22de2097fa0e9`  
		Last Modified: Thu, 17 Dec 2020 09:41:31 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdbe0b24f83ee53afb01bb3aa9a7a00550fd1b9075e4f14d06ea40d6a08fa38`  
		Last Modified: Thu, 17 Dec 2020 09:41:32 GMT  
		Size: 1.2 MB (1205124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1d3ae7bfee109fabcca47c72eafec8e83c1ae6f11079ecef9582650f6d5d1ce`  
		Last Modified: Thu, 17 Dec 2020 09:41:31 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.3` - linux; ppc64le

```console
$ docker pull wordpress@sha256:a79d41c360e438231cad28652a6e279d5bf795238dd55725297974b2107a0d6a
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.5 MB (49494262 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4d1884aa643ab98c7531ada5307c10cc6ba7cd1732a644952a0a2117cc9d3bfa`
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
# Thu, 17 Dec 2020 06:51:08 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 17 Dec 2020 06:51:14 GMT
ENV PHP_VERSION=7.3.25
# Thu, 17 Dec 2020 06:51:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Thu, 17 Dec 2020 06:51:23 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Thu, 17 Dec 2020 06:51:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 06:51:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 06:55:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 06:55:55 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 17 Dec 2020 06:56:04 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 06:56:06 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 06:56:11 GMT
CMD ["php" "-a"]
# Thu, 17 Dec 2020 16:18:59 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 17 Dec 2020 16:19:11 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 17 Dec 2020 16:19:25 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 17 Dec 2020 16:19:37 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 17 Dec 2020 16:19:44 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 16:19:49 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 17 Dec 2020 16:19:55 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 17 Dec 2020 16:19:59 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 17 Dec 2020 16:20:13 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Thu, 17 Dec 2020 16:20:21 GMT
VOLUME [/var/www/html]
# Thu, 17 Dec 2020 16:20:25 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 17 Dec 2020 16:20:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 16:20:50 GMT
USER www-data
# Thu, 17 Dec 2020 16:21:05 GMT
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
	-	`sha256:8fb13d267c3c9cddcf3bef2cd6d4182c6efa3497e4d5346fffcb060366828d0a`  
		Last Modified: Thu, 17 Dec 2020 08:08:49 GMT  
		Size: 12.2 MB (12155975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:653ef413f8c49ef4d8246e4fdff54a0c0c92126aad680ad956ccdafdb8569d35`  
		Last Modified: Thu, 17 Dec 2020 08:08:48 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5301b7d20e8fe4698c106c3f895d363f27daea8f6f107b3756d89d4479f35a08`  
		Last Modified: Thu, 17 Dec 2020 08:08:52 GMT  
		Size: 15.4 MB (15401450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65f79840e522874378233138e6b31818411e2578f7839e8f71400c5b790390b6`  
		Last Modified: Thu, 17 Dec 2020 08:08:48 GMT  
		Size: 2.3 KB (2259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63423fd788ea143a61a9285075b35f97fd3f161da4053f8dd48eee206003f672`  
		Last Modified: Thu, 17 Dec 2020 08:08:48 GMT  
		Size: 16.7 KB (16717 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d31d0e073b8ed2f082a44737e62944a15e4dc580f37f743d96a71d211aed29f`  
		Last Modified: Thu, 17 Dec 2020 16:28:27 GMT  
		Size: 7.1 MB (7054280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a140405ba61061eb417116472fef80dbc49cad80cdf82bc0a9b1bd1d26bac18`  
		Last Modified: Thu, 17 Dec 2020 16:28:21 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8d671c3e0e4822a9680ddd6ebe6eeab5d18ee05613967297bf317af20b46898`  
		Last Modified: Thu, 17 Dec 2020 16:28:23 GMT  
		Size: 9.5 MB (9466879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8441eabfd7147daaf26d2d44d1f33f1139eb6f2d33927ba50a2e04f342afe57`  
		Last Modified: Thu, 17 Dec 2020 16:28:21 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d7811c7739a585d6befec98579bfb79b845238f062ed5980a768e5f46e22f3`  
		Last Modified: Thu, 17 Dec 2020 16:28:21 GMT  
		Size: 1.2 MB (1205207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:030bd44588bf15569c7d73a7323521769c19c2abfe2bfeaecfab3761dcbd5a39`  
		Last Modified: Thu, 17 Dec 2020 16:28:21 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-2-php7.3` - linux; s390x

```console
$ docker pull wordpress@sha256:8d6dca554d68614a3cd8ab65ef4f76aef9e1010b089774c56dc94942337fa1d5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.6 MB (47588909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a84050b01de449dadf9f5f39c8a1a093864177d32ff1d9b3cef7aece8ddff1`
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
# Thu, 17 Dec 2020 06:55:49 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 17 Dec 2020 06:55:49 GMT
ENV PHP_VERSION=7.3.25
# Thu, 17 Dec 2020 06:55:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.25.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.25.tar.xz.asc
# Thu, 17 Dec 2020 06:55:51 GMT
ENV PHP_SHA256=c71c00ad03079efb78d1a6b8623ca4f725be697dbd9a46debacbcc9a2475f329
# Thu, 17 Dec 2020 06:55:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Dec 2020 06:56:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Dec 2020 07:01:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Dec 2020 07:01:32 GMT
COPY multi:afab483600631d4d87fe030871bbb016f1c2b73c0b72609d857bace419af7f5d in /usr/local/bin/ 
# Thu, 17 Dec 2020 07:01:35 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Dec 2020 07:01:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Dec 2020 07:01:36 GMT
CMD ["php" "-a"]
# Thu, 17 Dec 2020 13:12:18 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 17 Dec 2020 13:12:21 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 17 Dec 2020 13:12:26 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Thu, 17 Dec 2020 13:12:29 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Thu, 17 Dec 2020 13:12:30 GMT
WORKDIR /var/www/html
# Thu, 17 Dec 2020 13:12:31 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Thu, 17 Dec 2020 13:12:31 GMT
ENV WORDPRESS_CLI_VERSION=2.4.0
# Thu, 17 Dec 2020 13:12:32 GMT
ENV WORDPRESS_CLI_SHA512=4049c7e45e14276a70a41c3b0864be7a6a8cfa8ea65ebac8b184a4f503a91baa1a0d29260d03248bc74aef70729824330fb6b396336172a624332e16f64e37ef
# Thu, 17 Dec 2020 13:12:37 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fSL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del .fetch-deps; 		wp --allow-root --version
# Thu, 17 Dec 2020 13:12:37 GMT
VOLUME [/var/www/html]
# Thu, 17 Dec 2020 13:12:38 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Thu, 17 Dec 2020 13:12:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 13:12:39 GMT
USER www-data
# Thu, 17 Dec 2020 13:12:40 GMT
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
	-	`sha256:a6ceea48c85e63da004abb38bbaff8d01277ffb3ef2240346d8998e6d0a64f04`  
		Last Modified: Thu, 17 Dec 2020 08:10:47 GMT  
		Size: 12.2 MB (12155967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeef22281bf62ed4b2e7281f9c13adf9a0d48fe3dbffc66d06e4b17cd5746f35`  
		Last Modified: Thu, 17 Dec 2020 08:10:47 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff5358415b590b43d12c5650671691b6c13602b8724919869b9eab99a5933dac`  
		Last Modified: Thu, 17 Dec 2020 08:10:50 GMT  
		Size: 13.7 MB (13714729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9f62adb553416ce5227a0ebaaaa1cfa6ca50d603f738690603b8c45fe9417d`  
		Last Modified: Thu, 17 Dec 2020 08:10:46 GMT  
		Size: 2.3 KB (2257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a6a54267a53b786b37b1f7b5326a0465de68558a23df9829ad770ed0aa56c6`  
		Last Modified: Thu, 17 Dec 2020 08:10:46 GMT  
		Size: 16.7 KB (16707 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e7ed74b5c404f517c44241568f27566b8df37161b0e3276261af4581b6a7d66`  
		Last Modified: Thu, 17 Dec 2020 13:18:39 GMT  
		Size: 6.8 MB (6785702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54fb24eeede18e6b5001d863781de1572cbe4a322e997b1d27056bd47189b91b`  
		Last Modified: Thu, 17 Dec 2020 13:18:35 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160586b92634b2e19da7b8298c040b3d950c0768be9ed3ae41ebcbe4efa23d39`  
		Last Modified: Thu, 17 Dec 2020 13:18:47 GMT  
		Size: 9.8 MB (9755645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcfc68321da0d84d19a1d839d899a4a1b44c62e8015f5f0d8ebf3cbba7ccab1b`  
		Last Modified: Thu, 17 Dec 2020 13:18:35 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5ccc510fcdb43b0e04df4a3504fb1940e325b74599c3ada5015cba6c300de34`  
		Last Modified: Thu, 17 Dec 2020 13:18:35 GMT  
		Size: 1.2 MB (1205165 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b20038ecbf24edc0ec9c999dc2b4bc19c68c06b5392bbb8cd2ee168e8faa9bb`  
		Last Modified: Thu, 17 Dec 2020 13:18:34 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
