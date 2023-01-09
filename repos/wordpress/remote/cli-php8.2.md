## `wordpress:cli-php8.2`

```console
$ docker pull wordpress@sha256:63e13a4fcbb21a916dd457c89695c8e463210e97f2235e183468e8881af4ada2
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

### `wordpress:cli-php8.2` - linux; amd64

```console
$ docker pull wordpress@sha256:f0f014e9d114cd28bc45d9cf3911aab62e537ffcf0d455ce08d36f517a7d78a9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.2 MB (56195826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d941820bf559e14ef6f38bce5e605e5a2d4ad422357a9f2629968cacefcaf694`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Tue, 22 Nov 2022 22:19:28 GMT
ADD file:587cae71969871d3c6456d844a8795df9b64b12c710c275295a1182b46f630e7 in / 
# Tue, 22 Nov 2022 22:19:29 GMT
CMD ["/bin/sh"]
# Wed, 30 Nov 2022 21:39:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 30 Nov 2022 21:39:10 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 30 Nov 2022 21:39:10 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 30 Nov 2022 21:39:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 30 Nov 2022 21:39:11 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 30 Nov 2022 21:39:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:39:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:39:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 30 Nov 2022 21:39:12 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 05 Jan 2023 23:48:44 GMT
ENV PHP_VERSION=8.2.1
# Thu, 05 Jan 2023 23:48:44 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.1.tar.xz.asc
# Thu, 05 Jan 2023 23:48:44 GMT
ENV PHP_SHA256=650d3bd7a056cabf07f6a0f6f1dd8ba45cd369574bbeaa36de7d1ece212c17af
# Thu, 05 Jan 2023 23:48:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 05 Jan 2023 23:48:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Jan 2023 23:52:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Jan 2023 23:52:33 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 05 Jan 2023 23:52:34 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Jan 2023 23:52:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Jan 2023 23:52:35 GMT
CMD ["php" "-a"]
# Fri, 06 Jan 2023 04:52:13 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 06 Jan 2023 04:52:13 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 06 Jan 2023 04:52:14 GMT
WORKDIR /var/www/html
# Fri, 06 Jan 2023 04:53:12 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 06 Jan 2023 04:53:13 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Jan 2023 04:53:13 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 06 Jan 2023 04:53:13 GMT
ENV WORDPRESS_CLI_VERSION=2.7.1
# Fri, 06 Jan 2023 04:53:13 GMT
ENV WORDPRESS_CLI_SHA512=956b5e3e1a076bd5441c082ee754e3ff4517ec965b93c621f455c2bf5719358c36e67d52f676492700b59d42cacb34a50d382535c035f19da7a0b98bc41860de
# Fri, 06 Jan 2023 04:53:17 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 06 Jan 2023 04:53:17 GMT
VOLUME [/var/www/html]
# Fri, 06 Jan 2023 04:53:17 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 06 Jan 2023 04:53:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 04:53:17 GMT
USER www-data
# Fri, 06 Jan 2023 04:53:17 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:c158987b05517b6f2c5913f3acef1f2182a32345a304fe357e3ace5fadcad715`  
		Last Modified: Tue, 22 Nov 2022 22:19:52 GMT  
		Size: 3.4 MB (3370706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2b6029f6920d234861e6cee7ca87a1840de19c6049c86038f1fb9432e32ea6d`  
		Last Modified: Wed, 30 Nov 2022 22:06:19 GMT  
		Size: 1.9 MB (1864199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55761811b31b62dd8f7c87e712cac077dacc6a20312b0e2a382c9bdb8315777c`  
		Last Modified: Wed, 30 Nov 2022 22:06:19 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9750fd99fe831a06b99ef6e82d1c1be04f9bf478c24ea2d52d63ac918c90df13`  
		Last Modified: Wed, 30 Nov 2022 22:06:19 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a26e12d2877aa957e2a70a65fa3e9c6b87d5330f5365deccc01c1efe2d014db`  
		Last Modified: Fri, 06 Jan 2023 01:48:07 GMT  
		Size: 12.1 MB (12052184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac17728cfa135794931b41212669253765941d433f83c4b03bb8a67682e1cc1d`  
		Last Modified: Fri, 06 Jan 2023 01:48:06 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a31524880183504f352cc4c24345466f94d1fd289ccdfae6eff028c6acca48ec`  
		Last Modified: Fri, 06 Jan 2023 01:48:09 GMT  
		Size: 19.3 MB (19307049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe98dfc590283a9a05d07f54e4f3caa38ba9feae1a410820e92cbb3812556256`  
		Last Modified: Fri, 06 Jan 2023 01:48:06 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44153a4fd928ad3de2a4be64aae1c2c12de162c75c4a9a87acb6e36c44b14604`  
		Last Modified: Fri, 06 Jan 2023 01:48:06 GMT  
		Size: 19.1 KB (19122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae128e9d313c7d10ec28a9b9dab766716bc3ef9cd79806a68075a46cdc13a709`  
		Last Modified: Fri, 06 Jan 2023 04:59:47 GMT  
		Size: 9.6 MB (9605768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d06c6d4ce3332a224b286ac557be8a08ecec23147bb814554d47e5d6955f8566`  
		Last Modified: Fri, 06 Jan 2023 04:59:44 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d105e743306d5165397390b057dadd277db831a8a2c21d2f55bd5785b308da20`  
		Last Modified: Fri, 06 Jan 2023 04:59:46 GMT  
		Size: 8.5 MB (8535775 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02bc27053bb236319f52586a58998f28339e8e2aebe72d81019b947d3807bdb1`  
		Last Modified: Fri, 06 Jan 2023 04:59:44 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fca2f3cfee0e105099a53a4064c596b12996189a7dd7ea2008bd009efd869cc`  
		Last Modified: Fri, 06 Jan 2023 04:59:45 GMT  
		Size: 1.4 MB (1435608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60ec80a57aa252ca075e0d7233f843d15add47a8e705c6ffd226f247f768074f`  
		Last Modified: Fri, 06 Jan 2023 04:59:44 GMT  
		Size: 408.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-php8.2` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:948d8324f44fcb673269662941a12e2c842390e92ee8e8e775f03333941646aa
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.3 MB (53346146 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:248acbd7ee0013a8de68ba32c71ac89d7e332446ec82de6e3fde7783a375ded2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Tue, 22 Nov 2022 22:55:46 GMT
ADD file:132c76d7f7dae2f51f589ee460f1870a2cec6e9dc7ff8e38e88fcee2cfbe70da in / 
# Tue, 22 Nov 2022 22:55:46 GMT
CMD ["/bin/sh"]
# Wed, 30 Nov 2022 21:31:01 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 30 Nov 2022 21:31:03 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 30 Nov 2022 21:31:03 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 30 Nov 2022 21:31:03 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 30 Nov 2022 21:31:04 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 30 Nov 2022 21:31:04 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:31:04 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:31:04 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 30 Nov 2022 21:31:04 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 05 Jan 2023 23:49:54 GMT
ENV PHP_VERSION=8.2.1
# Thu, 05 Jan 2023 23:49:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.1.tar.xz.asc
# Thu, 05 Jan 2023 23:49:55 GMT
ENV PHP_SHA256=650d3bd7a056cabf07f6a0f6f1dd8ba45cd369574bbeaa36de7d1ece212c17af
# Thu, 05 Jan 2023 23:50:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 05 Jan 2023 23:50:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Jan 2023 23:55:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Jan 2023 23:55:10 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 05 Jan 2023 23:55:11 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Jan 2023 23:55:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Jan 2023 23:55:11 GMT
CMD ["php" "-a"]
# Fri, 06 Jan 2023 02:46:40 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 06 Jan 2023 02:46:41 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 06 Jan 2023 02:46:41 GMT
WORKDIR /var/www/html
# Fri, 06 Jan 2023 02:47:56 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 06 Jan 2023 02:47:57 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Jan 2023 02:47:57 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 06 Jan 2023 02:47:57 GMT
ENV WORDPRESS_CLI_VERSION=2.7.1
# Fri, 06 Jan 2023 02:47:58 GMT
ENV WORDPRESS_CLI_SHA512=956b5e3e1a076bd5441c082ee754e3ff4517ec965b93c621f455c2bf5719358c36e67d52f676492700b59d42cacb34a50d382535c035f19da7a0b98bc41860de
# Fri, 06 Jan 2023 02:48:01 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 06 Jan 2023 02:48:01 GMT
VOLUME [/var/www/html]
# Fri, 06 Jan 2023 02:48:01 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 06 Jan 2023 02:48:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 02:48:01 GMT
USER www-data
# Fri, 06 Jan 2023 02:48:01 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:c2eb4db52fbe1266a78d8c185d33544a2916faa7d82fb5f50909fe233e0579da`  
		Last Modified: Tue, 22 Nov 2022 22:56:39 GMT  
		Size: 3.1 MB (3107138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:519fe767bb0c7928a1dbb3eed5885ac27b686566653a40e08b8377c7efeb5965`  
		Last Modified: Wed, 30 Nov 2022 22:00:41 GMT  
		Size: 1.8 MB (1848421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d73d4fd50e3aae901afb655f4fb90048c5f350001b4d52bb8d1bc50424c93a`  
		Last Modified: Wed, 30 Nov 2022 22:00:41 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c342b7908a6480c9e4c98966c37148ce29d0f29d1ceabe2775acbbf4e4dd0698`  
		Last Modified: Wed, 30 Nov 2022 22:00:41 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60a768ecc3e0d81c78e6354398d27e0e10ea285b8818957fea56d9e1c57eba1e`  
		Last Modified: Fri, 06 Jan 2023 01:20:20 GMT  
		Size: 12.1 MB (12052142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb24b6b4b01d726b927aefdab1de28e834fcc72685c11e88da2c793c0e04de5`  
		Last Modified: Fri, 06 Jan 2023 01:20:18 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a24023eadeaf23134f2753c53e3e55f60a7b0dae360d6897897a8812a51b4d`  
		Last Modified: Fri, 06 Jan 2023 01:20:23 GMT  
		Size: 17.5 MB (17470400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d5ac98f14f727852f82873b9a82bcb9e4191192b7277d0e4bd813881e07138`  
		Last Modified: Fri, 06 Jan 2023 01:20:18 GMT  
		Size: 2.4 KB (2444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe2ad5a799fa06db5495c24d77b65a81e563249846a0b924cb71a0c0e7e646d8`  
		Last Modified: Fri, 06 Jan 2023 01:20:18 GMT  
		Size: 18.9 KB (18857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512caa5ebdccecdeb1db97a85bc42ce01f239f2d7cf70ff9433c57e0d073dda2`  
		Last Modified: Fri, 06 Jan 2023 02:52:26 GMT  
		Size: 9.2 MB (9231242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3abab159b999c79e75ab039f6ececa45d2436a17545c61bdbb7e738265c8cbd3`  
		Last Modified: Fri, 06 Jan 2023 02:52:21 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd19a1681f7e0962a79a6feb8971eaff921d49bcc9cb61553c3dce86b5236e15`  
		Last Modified: Fri, 06 Jan 2023 02:52:23 GMT  
		Size: 8.2 MB (8177070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04b6385862114edfe027cbff0b7ff3e03d9ea205af9965f9b3418cea45921436`  
		Last Modified: Fri, 06 Jan 2023 02:52:21 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6503db41669e417523a77fa020bb063061c9b2e87abc1775c3878ffe6d44c615`  
		Last Modified: Fri, 06 Jan 2023 02:52:22 GMT  
		Size: 1.4 MB (1435536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3d464b69e9c46d645535e95048506c79fe5e39300c32ebf87b4369439424a85`  
		Last Modified: Fri, 06 Jan 2023 02:52:21 GMT  
		Size: 409.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-php8.2` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:7de1abcb8846bdbaef79da9f01541d1ea11f65f8299a674cdeeef2d10d3c9c04
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.3 MB (51279916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b0921b703a1b4145f9e64c79b00e8eea15c9755d2861781cbbdb5481ae0d217`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Tue, 22 Nov 2022 22:57:20 GMT
ADD file:080010d9005e8e0dae3e98c7f9afff3e3a40ed32579ca01946efc6ede8316bad in / 
# Tue, 22 Nov 2022 22:57:20 GMT
CMD ["/bin/sh"]
# Wed, 30 Nov 2022 21:47:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 30 Nov 2022 21:47:29 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 30 Nov 2022 21:47:29 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 30 Nov 2022 21:47:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 30 Nov 2022 21:47:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 30 Nov 2022 21:47:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:47:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:47:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 30 Nov 2022 21:47:30 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 05 Jan 2023 23:20:27 GMT
ENV PHP_VERSION=8.2.1
# Thu, 05 Jan 2023 23:20:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.1.tar.xz.asc
# Thu, 05 Jan 2023 23:20:27 GMT
ENV PHP_SHA256=650d3bd7a056cabf07f6a0f6f1dd8ba45cd369574bbeaa36de7d1ece212c17af
# Thu, 05 Jan 2023 23:20:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 05 Jan 2023 23:20:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Jan 2023 23:23:25 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Jan 2023 23:23:26 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 05 Jan 2023 23:23:27 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Jan 2023 23:23:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Jan 2023 23:23:27 GMT
CMD ["php" "-a"]
# Fri, 06 Jan 2023 05:52:09 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 06 Jan 2023 05:52:10 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 06 Jan 2023 05:52:10 GMT
WORKDIR /var/www/html
# Fri, 06 Jan 2023 05:53:16 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 06 Jan 2023 05:53:17 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Jan 2023 05:53:17 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 06 Jan 2023 05:53:17 GMT
ENV WORDPRESS_CLI_VERSION=2.7.1
# Fri, 06 Jan 2023 05:53:17 GMT
ENV WORDPRESS_CLI_SHA512=956b5e3e1a076bd5441c082ee754e3ff4517ec965b93c621f455c2bf5719358c36e67d52f676492700b59d42cacb34a50d382535c035f19da7a0b98bc41860de
# Fri, 06 Jan 2023 05:53:20 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 06 Jan 2023 05:53:20 GMT
VOLUME [/var/www/html]
# Fri, 06 Jan 2023 05:53:20 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 06 Jan 2023 05:53:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 05:53:20 GMT
USER www-data
# Fri, 06 Jan 2023 05:53:20 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:cb2ec849933dd31db64abae3fdcb6923c490d9795577bee1ee1be04eab0376ee`  
		Last Modified: Tue, 22 Nov 2022 22:58:12 GMT  
		Size: 2.9 MB (2865346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca108fdbcd11a67cf41e6ad58105ac2d95dffcd2febfae5df098b1577776e2b4`  
		Last Modified: Wed, 30 Nov 2022 22:22:22 GMT  
		Size: 1.7 MB (1703388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a3c36f0f232387119c44145dd35f68a589d293ea19f9fbff2f5dabfba05b7c`  
		Last Modified: Wed, 30 Nov 2022 22:22:21 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92740214b90b0b116f7b164af3e785bb3999df1307a4eac482afb0eedbf3904b`  
		Last Modified: Wed, 30 Nov 2022 22:22:21 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e1b44468dc893501512e4bc075fda121d59ed8941b41e1197b9b77d9b5e2d6`  
		Last Modified: Fri, 06 Jan 2023 01:42:40 GMT  
		Size: 12.1 MB (12052146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77788bda1d7c39b06d0b4462df6251ab21019938e841e79ab689507d77577d99`  
		Last Modified: Fri, 06 Jan 2023 01:42:38 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3b58bc0776c6cf87a8119318ed5962e19ab8b2856396495670e33c54c4aea2`  
		Last Modified: Fri, 06 Jan 2023 01:42:42 GMT  
		Size: 16.4 MB (16362155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8d3794fad625bf110123dfbfc9a04f6c8d4ed82d84b7d1e87ddb64be99e2c43`  
		Last Modified: Fri, 06 Jan 2023 01:42:38 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd71fc8c01e1ba10c5e1bb560880600c1ddb15763d5190dce1d2423a3473e7a`  
		Last Modified: Fri, 06 Jan 2023 01:42:39 GMT  
		Size: 18.9 KB (18877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2d6e896a3ff21360ccfc2e88b41c8923fcccc30116fdfeda127fb6052b9eeda`  
		Last Modified: Fri, 06 Jan 2023 06:04:08 GMT  
		Size: 8.9 MB (8949304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f324de4b46d36ea1c9a35617ab9525d4698c56a41360c2fd2438a5a6885a3f4`  
		Last Modified: Fri, 06 Jan 2023 06:04:04 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d2a35a57d24091a8cc0c01c3e25fb85647db2c7d20324a29c1d821fa0ff3ac2`  
		Last Modified: Fri, 06 Jan 2023 06:04:06 GMT  
		Size: 7.9 MB (7887807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73f5a63ef68dd8e007b442551692c1540f81e6339463218c16b14b2f88945847`  
		Last Modified: Fri, 06 Jan 2023 06:04:04 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1e2b0b9342de431e5ec65162207e706aa7d1fb2651331061de03001ee50c398`  
		Last Modified: Fri, 06 Jan 2023 06:04:05 GMT  
		Size: 1.4 MB (1435543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f2022a6deb3ca53e5f2d3a5f6045695d51cb523109a4d7c52b0d177d2159f4`  
		Last Modified: Fri, 06 Jan 2023 06:04:04 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-php8.2` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:b4c8fb946e287d5fbadef5f571bbb0206fe47d5f37fc7789903740eb916f4a70
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.5 MB (53470853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64760ff02d48a52502a5ccb2037e1d9437527587895ad50988173fc1d77ab577`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Mon, 09 Jan 2023 17:04:48 GMT
ADD file:3080f19f39259a4b77cc53975de0184c78d4335ceb9ffb77a2838d0539ad6f85 in / 
# Mon, 09 Jan 2023 17:04:49 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 18:17:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 09 Jan 2023 18:17:30 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 09 Jan 2023 18:17:30 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 09 Jan 2023 18:17:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 09 Jan 2023 18:17:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 09 Jan 2023 18:17:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 09 Jan 2023 18:17:31 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 09 Jan 2023 18:17:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 09 Jan 2023 18:17:31 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 09 Jan 2023 18:17:31 GMT
ENV PHP_VERSION=8.2.1
# Mon, 09 Jan 2023 18:17:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.1.tar.xz.asc
# Mon, 09 Jan 2023 18:17:31 GMT
ENV PHP_SHA256=650d3bd7a056cabf07f6a0f6f1dd8ba45cd369574bbeaa36de7d1ece212c17af
# Mon, 09 Jan 2023 18:17:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Mon, 09 Jan 2023 18:17:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 09 Jan 2023 18:21:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 09 Jan 2023 18:21:18 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Mon, 09 Jan 2023 18:21:19 GMT
RUN docker-php-ext-enable sodium
# Mon, 09 Jan 2023 18:21:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 09 Jan 2023 18:21:19 GMT
CMD ["php" "-a"]
# Mon, 09 Jan 2023 23:05:32 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Mon, 09 Jan 2023 23:05:33 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Mon, 09 Jan 2023 23:05:33 GMT
WORKDIR /var/www/html
# Mon, 09 Jan 2023 23:06:23 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Mon, 09 Jan 2023 23:06:24 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Mon, 09 Jan 2023 23:06:24 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Mon, 09 Jan 2023 23:06:24 GMT
ENV WORDPRESS_CLI_VERSION=2.7.1
# Mon, 09 Jan 2023 23:06:24 GMT
ENV WORDPRESS_CLI_SHA512=956b5e3e1a076bd5441c082ee754e3ff4517ec965b93c621f455c2bf5719358c36e67d52f676492700b59d42cacb34a50d382535c035f19da7a0b98bc41860de
# Mon, 09 Jan 2023 23:06:27 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Mon, 09 Jan 2023 23:06:27 GMT
VOLUME [/var/www/html]
# Mon, 09 Jan 2023 23:06:27 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Mon, 09 Jan 2023 23:06:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 23:06:27 GMT
USER www-data
# Mon, 09 Jan 2023 23:06:27 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:a9eaa45ef418e883481a13c7d84fa9904f2ec56789c52a87ba5a9e6483f2b74f`  
		Last Modified: Mon, 09 Jan 2023 17:05:12 GMT  
		Size: 3.3 MB (3259241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021af8555e126429275b6ab3ac7327a8b7ac0ceaec3b3c2bf56d28dc7dfdd163`  
		Last Modified: Mon, 09 Jan 2023 18:45:00 GMT  
		Size: 1.9 MB (1862569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b591f8ea528cfc9afa8b8ce8654330c57213176778adbfcd2e2605de8454339`  
		Last Modified: Mon, 09 Jan 2023 18:44:59 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41561169430256adabeea302a941064edd0d1fbd6fa0ddc5bc53be766ac23c97`  
		Last Modified: Mon, 09 Jan 2023 18:44:59 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e41aed43a20471b63ecf9c43f316a50b9ff8d36da3baf273795945e0142c901`  
		Last Modified: Mon, 09 Jan 2023 18:44:58 GMT  
		Size: 12.1 MB (12052170 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1d269065a68e9b5e2a612d9c62381684d29171a81dffac8914d066e88010782`  
		Last Modified: Mon, 09 Jan 2023 18:44:57 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78d8b1fcd696330589dd8f83c3fc138ab45362d95c1467c7e7961447d834bd60`  
		Last Modified: Mon, 09 Jan 2023 18:45:00 GMT  
		Size: 16.7 MB (16697943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31ae1d47f9b0d36ea7b30e158e47c4ef052ef37f50cc7df6b8e6294d0e577a01`  
		Last Modified: Mon, 09 Jan 2023 18:44:57 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d25618d85752cf63b613f0a8145c9ea8dbae3b7a1c75dbb115c6ac864a1280`  
		Last Modified: Mon, 09 Jan 2023 18:44:57 GMT  
		Size: 18.7 KB (18739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e4aed3d0c6ce8a5e0024a75ac7bb88a71a26c80e362f3fddf6d2cddb66a5aa4`  
		Last Modified: Mon, 09 Jan 2023 23:09:23 GMT  
		Size: 9.7 MB (9729989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c39d6d94b469518654237e231bac08b4328a372d900bb926892128da091be028`  
		Last Modified: Mon, 09 Jan 2023 23:09:20 GMT  
		Size: 142.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5736fc6051f236268ab63f52579d7816876cbb718d57c079c39a0f0abaaa7f62`  
		Last Modified: Mon, 09 Jan 2023 23:09:21 GMT  
		Size: 8.4 MB (8409284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c16037f207e188950a54ff8da424a1bd3803dc66895bfa76eda9769033e1bf8`  
		Last Modified: Mon, 09 Jan 2023 23:09:20 GMT  
		Size: 385.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e29b58a2519d52dd019438dfb077407e9e57e7a60cab6ee51235f808de406b83`  
		Last Modified: Mon, 09 Jan 2023 23:09:20 GMT  
		Size: 1.4 MB (1435513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3ac20cb10a060981d8a9b5cf8210d8c4f4f13ade1fb60758ec361bd76d9274d`  
		Last Modified: Mon, 09 Jan 2023 23:09:20 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-php8.2` - linux; 386

```console
$ docker pull wordpress@sha256:93f5f54c6f68bc0efe741a45c0fbb1415e76192bd625f728bfd4ee55601a856c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.8 MB (54815365 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:272e342c7f6f15e1dc5395e03d02c2aec1e6539f3264d1cb007ac376899894e5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Mon, 09 Jan 2023 17:05:00 GMT
ADD file:d03619a0ef81726c34189e849b80cc92da908eb36e116f28275d5765e6d0919a in / 
# Mon, 09 Jan 2023 17:05:00 GMT
CMD ["/bin/sh"]
# Mon, 09 Jan 2023 17:56:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 09 Jan 2023 17:56:18 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 09 Jan 2023 17:56:19 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 09 Jan 2023 17:56:20 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 09 Jan 2023 17:56:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 09 Jan 2023 17:56:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 09 Jan 2023 17:56:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 09 Jan 2023 17:56:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 09 Jan 2023 17:56:25 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 09 Jan 2023 17:56:26 GMT
ENV PHP_VERSION=8.2.1
# Mon, 09 Jan 2023 17:56:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.1.tar.xz.asc
# Mon, 09 Jan 2023 17:56:28 GMT
ENV PHP_SHA256=650d3bd7a056cabf07f6a0f6f1dd8ba45cd369574bbeaa36de7d1ece212c17af
# Mon, 09 Jan 2023 17:56:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Mon, 09 Jan 2023 17:56:37 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 09 Jan 2023 17:59:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 09 Jan 2023 17:59:54 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Mon, 09 Jan 2023 17:59:55 GMT
RUN docker-php-ext-enable sodium
# Mon, 09 Jan 2023 17:59:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 09 Jan 2023 17:59:56 GMT
CMD ["php" "-a"]
# Mon, 09 Jan 2023 22:36:41 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Mon, 09 Jan 2023 22:36:42 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Mon, 09 Jan 2023 22:36:43 GMT
WORKDIR /var/www/html
# Mon, 09 Jan 2023 22:37:38 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Mon, 09 Jan 2023 22:37:38 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Mon, 09 Jan 2023 22:37:39 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Mon, 09 Jan 2023 22:37:40 GMT
ENV WORDPRESS_CLI_VERSION=2.7.1
# Mon, 09 Jan 2023 22:37:41 GMT
ENV WORDPRESS_CLI_SHA512=956b5e3e1a076bd5441c082ee754e3ff4517ec965b93c621f455c2bf5719358c36e67d52f676492700b59d42cacb34a50d382535c035f19da7a0b98bc41860de
# Mon, 09 Jan 2023 22:37:45 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Mon, 09 Jan 2023 22:37:46 GMT
VOLUME [/var/www/html]
# Mon, 09 Jan 2023 22:37:48 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Mon, 09 Jan 2023 22:37:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 09 Jan 2023 22:37:49 GMT
USER www-data
# Mon, 09 Jan 2023 22:37:50 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:40e5b0b2e2bde18974628cadecd8a2f190f45f06c32846c16885d69b2908bf68`  
		Last Modified: Mon, 09 Jan 2023 17:05:42 GMT  
		Size: 3.4 MB (3408318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:698dd141c7d486e8a54f0221b4999d81f5f1ddd0ad1cfe9fcdcc77bf725ba2f3`  
		Last Modified: Mon, 09 Jan 2023 18:26:17 GMT  
		Size: 2.0 MB (1978285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de64f9608f5138392e573bde482c2eba7ee6bab6c98a119f90715c31b13d629d`  
		Last Modified: Mon, 09 Jan 2023 18:26:16 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9727b29c81e5caccd4a630b6c5dd9c0b031dbe4995edd56282f34c90925ea029`  
		Last Modified: Mon, 09 Jan 2023 18:26:16 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8f7cc4967ff2fe1c7c9530fa8b6658a6567c4ef9c0acbe3a2553e34f71f1075`  
		Last Modified: Mon, 09 Jan 2023 18:26:15 GMT  
		Size: 12.1 MB (12052045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5200762cb33c48ee2dd4841574760be019eb858ccf0c07cd4e9e0a4efa73706c`  
		Last Modified: Mon, 09 Jan 2023 18:26:14 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bdef6fb905759b10160702acfc8a94ea5ca5d5d131a0b58ce5a80c02b7c2100`  
		Last Modified: Mon, 09 Jan 2023 18:26:17 GMT  
		Size: 17.2 MB (17181885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8115f8a85334988c705c2e523a2ce44bd11d822900fd4903105be905076a85d`  
		Last Modified: Mon, 09 Jan 2023 18:26:14 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc71b57daf77eab6f30bb5d080ca6caab8d650c01912349b0c6209b835f9d171`  
		Last Modified: Mon, 09 Jan 2023 18:26:14 GMT  
		Size: 18.9 KB (18854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f997f2073d590dc8967cf2b50b84071ce85776855708ac439d6e5a5fb03f56f`  
		Last Modified: Mon, 09 Jan 2023 22:42:42 GMT  
		Size: 9.8 MB (9788678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697a3e0cbe0c9d526adeaa263fb5312835261e090647913b367d13ee0cd7fe1e`  
		Last Modified: Mon, 09 Jan 2023 22:42:42 GMT  
		Size: 8.9 MB (8946765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:182fe62311c1ae89cd8541691ed2b355c5a9a29f2127021735af5b718344cffb`  
		Last Modified: Mon, 09 Jan 2023 22:42:40 GMT  
		Size: 388.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18bd5f8c6a081e00d5c4d2a66550e4d3baea79d975a2551642c7b768687256dc`  
		Last Modified: Mon, 09 Jan 2023 22:42:41 GMT  
		Size: 1.4 MB (1435346 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd706916ac2b1c28814f32d5405580787291452ff20cc420daeff9166a0cc96`  
		Last Modified: Mon, 09 Jan 2023 22:42:41 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-php8.2` - linux; ppc64le

```console
$ docker pull wordpress@sha256:390481ea7d1f0f5845d351a9520526c0e516568b151998b3a98ec8ac538fc17f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.5 MB (57520939 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0170c0cd22a877eae15e3632fd25a4fc51fc466f93d94b3311e433ebd027a52d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Wed, 23 Nov 2022 00:18:18 GMT
ADD file:a8e68f93c597f70ce637ef578c72c9b41b4b8d80b552b8e5570d4efcc1d02ff5 in / 
# Wed, 23 Nov 2022 00:18:18 GMT
CMD ["/bin/sh"]
# Wed, 30 Nov 2022 21:38:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 30 Nov 2022 21:38:40 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 30 Nov 2022 21:38:42 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 30 Nov 2022 21:38:42 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 30 Nov 2022 21:38:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 30 Nov 2022 21:38:43 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:38:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 21:38:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 30 Nov 2022 21:38:44 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 05 Jan 2023 23:34:14 GMT
ENV PHP_VERSION=8.2.1
# Thu, 05 Jan 2023 23:34:14 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.1.tar.xz.asc
# Thu, 05 Jan 2023 23:34:14 GMT
ENV PHP_SHA256=650d3bd7a056cabf07f6a0f6f1dd8ba45cd369574bbeaa36de7d1ece212c17af
# Thu, 05 Jan 2023 23:34:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 05 Jan 2023 23:34:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 05 Jan 2023 23:38:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 05 Jan 2023 23:38:22 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Thu, 05 Jan 2023 23:38:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 05 Jan 2023 23:38:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 05 Jan 2023 23:38:25 GMT
CMD ["php" "-a"]
# Fri, 06 Jan 2023 06:33:06 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 06 Jan 2023 06:33:08 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 06 Jan 2023 06:33:08 GMT
WORKDIR /var/www/html
# Fri, 06 Jan 2023 06:34:52 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 06 Jan 2023 06:34:54 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Jan 2023 06:34:54 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 06 Jan 2023 06:34:54 GMT
ENV WORDPRESS_CLI_VERSION=2.7.1
# Fri, 06 Jan 2023 06:34:55 GMT
ENV WORDPRESS_CLI_SHA512=956b5e3e1a076bd5441c082ee754e3ff4517ec965b93c621f455c2bf5719358c36e67d52f676492700b59d42cacb34a50d382535c035f19da7a0b98bc41860de
# Fri, 06 Jan 2023 06:34:59 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 06 Jan 2023 06:35:00 GMT
VOLUME [/var/www/html]
# Fri, 06 Jan 2023 06:35:01 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 06 Jan 2023 06:35:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 06:35:01 GMT
USER www-data
# Fri, 06 Jan 2023 06:35:02 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:69314845b945e4b33e4ee552d0e4156645f71c81b6cb71108c1e32e139aec052`  
		Last Modified: Wed, 23 Nov 2022 00:19:02 GMT  
		Size: 3.4 MB (3384500 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6bb0b5b6ebfcb59d7bb376eda2a3a450213bafa678bcca93b0af952b4d0c1c18`  
		Last Modified: Wed, 30 Nov 2022 22:10:33 GMT  
		Size: 1.9 MB (1938378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ed945cdf32e78d05dd306e297a89c2b21ac37e2c170d24aa2f5194ea02358fb`  
		Last Modified: Wed, 30 Nov 2022 22:10:32 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bed7d0ee32d4b74590d0ef4b007add6ad78f90481324806ba82f06942037372`  
		Last Modified: Wed, 30 Nov 2022 22:10:32 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab718c532b7d5281f738e3b1088dcc40fda5c588bcd3edd0a23215c69c802292`  
		Last Modified: Fri, 06 Jan 2023 01:28:23 GMT  
		Size: 12.1 MB (12052176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bfc66268a7571567ca8dd9994ef769dc23c44ca897b3691698b4f319ff0edbb`  
		Last Modified: Fri, 06 Jan 2023 01:28:21 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b36e615ed568b13bf3d5ccfa6ec26365446b5c156b3a87feda1b13556add363a`  
		Last Modified: Fri, 06 Jan 2023 01:28:27 GMT  
		Size: 20.1 MB (20064711 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb3d52084ae5ebbbf38a9d32e3e9a94e612eb0006cfd757a0e32be710270dca2`  
		Last Modified: Fri, 06 Jan 2023 01:28:22 GMT  
		Size: 2.4 KB (2445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4894d30cecb5e9184deedaae81ae3c6a58e589875ac134f518ec223f2020e0e5`  
		Last Modified: Fri, 06 Jan 2023 01:28:22 GMT  
		Size: 18.9 KB (18873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3acb3bafba79119f4d79b0e92142014a757bbcf29f89c75a5cd56200608892df`  
		Last Modified: Fri, 06 Jan 2023 06:45:27 GMT  
		Size: 9.9 MB (9869705 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3f19a3ada1a8c918119a75a978e575a2a43debccb1c157b72d3ae6868893a6`  
		Last Modified: Fri, 06 Jan 2023 06:45:22 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a812ba2fd6bea91960d482fc1b3eef90c7f5dc58c7574be222dd263c72281ed0`  
		Last Modified: Fri, 06 Jan 2023 06:45:24 GMT  
		Size: 8.8 MB (8751606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f4241df85cf2598531cfd613abde96debcbaafb4b40695bebb474ca8b51c7e`  
		Last Modified: Fri, 06 Jan 2023 06:45:22 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64a7c4f8838276ce22e4d176b0e2a80bf3f27aab487159bc92c1253f82d1a114`  
		Last Modified: Fri, 06 Jan 2023 06:45:23 GMT  
		Size: 1.4 MB (1435569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:331a5ad86a57892cb2fd763fc8320ed72a29c98509b209c122054376a89576b8`  
		Last Modified: Fri, 06 Jan 2023 06:45:22 GMT  
		Size: 411.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:cli-php8.2` - linux; s390x

```console
$ docker pull wordpress@sha256:db1a29918042c448b4c8b5c9152994e7f0e62ab6edd33c1391b9a18d44f031af
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.2 MB (55231697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26dab8884030b145fde3f7a315a08793cc9dcb4278d9e8aedb50c019e2910e0f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["wp","shell"]`

```dockerfile
# Tue, 22 Nov 2022 22:47:02 GMT
ADD file:d8cbd162b64e4b7a8b83086be37ef5ee69e955ac955ebbe59e70c6be2a2d1a9f in / 
# Tue, 22 Nov 2022 22:47:03 GMT
CMD ["/bin/sh"]
# Wed, 30 Nov 2022 20:56:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 30 Nov 2022 20:56:11 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 30 Nov 2022 20:56:11 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 30 Nov 2022 20:56:11 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 30 Nov 2022 20:56:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 30 Nov 2022 20:56:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 20:56:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 30 Nov 2022 20:56:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 30 Nov 2022 20:56:12 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 05 Jan 2023 23:56:38 GMT
ENV PHP_VERSION=8.2.1
# Thu, 05 Jan 2023 23:56:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.1.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.1.tar.xz.asc
# Thu, 05 Jan 2023 23:56:39 GMT
ENV PHP_SHA256=650d3bd7a056cabf07f6a0f6f1dd8ba45cd369574bbeaa36de7d1ece212c17af
# Thu, 05 Jan 2023 23:56:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 05 Jan 2023 23:56:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 06 Jan 2023 00:00:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--enable-phpdbg 		--enable-phpdbg-readline 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 06 Jan 2023 00:00:44 GMT
COPY multi:6edd033b037aa2d7697fc3b9f82c2f162146c1920a0c6d25a165dc56783204db in /usr/local/bin/ 
# Fri, 06 Jan 2023 00:00:48 GMT
RUN docker-php-ext-enable sodium
# Fri, 06 Jan 2023 00:00:48 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 06 Jan 2023 00:00:49 GMT
CMD ["php" "-a"]
# Fri, 06 Jan 2023 04:24:47 GMT
RUN apk add --no-cache 		bash 		less 		mysql-client
# Fri, 06 Jan 2023 04:24:49 GMT
RUN set -ex; 	mkdir -p /var/www/html; 	chown -R www-data:www-data /var/www/html
# Fri, 06 Jan 2023 04:24:49 GMT
WORKDIR /var/www/html
# Fri, 06 Jan 2023 04:25:54 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 06 Jan 2023 04:25:55 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 06 Jan 2023 04:25:55 GMT
ENV WORDPRESS_CLI_GPG_KEY=63AF7AA15067C05616FDDD88A3A2E8F226F0BC06
# Fri, 06 Jan 2023 04:25:56 GMT
ENV WORDPRESS_CLI_VERSION=2.7.1
# Fri, 06 Jan 2023 04:25:56 GMT
ENV WORDPRESS_CLI_SHA512=956b5e3e1a076bd5441c082ee754e3ff4517ec965b93c621f455c2bf5719358c36e67d52f676492700b59d42cacb34a50d382535c035f19da7a0b98bc41860de
# Fri, 06 Jan 2023 04:25:59 GMT
RUN set -ex; 		apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -o /usr/local/bin/wp.gpg -fL "https://github.com/wp-cli/wp-cli/releases/download/v${WORDPRESS_CLI_VERSION}/wp-cli-${WORDPRESS_CLI_VERSION}.phar.gpg"; 		GNUPGHOME="$(mktemp -d)"; export GNUPGHOME; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$WORDPRESS_CLI_GPG_KEY"; 	gpg --batch --decrypt --output /usr/local/bin/wp /usr/local/bin/wp.gpg; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" /usr/local/bin/wp.gpg; unset GNUPGHOME; 		echo "$WORDPRESS_CLI_SHA512 */usr/local/bin/wp" | sha512sum -c -; 	chmod +x /usr/local/bin/wp; 		apk del --no-network .fetch-deps; 		wp --allow-root --version
# Fri, 06 Jan 2023 04:25:59 GMT
VOLUME [/var/www/html]
# Fri, 06 Jan 2023 04:25:59 GMT
COPY file:b6efa5ff0423d61c2df0c8941b896844a8272d8516cdda0fcae8daaf56baac18 in /usr/local/bin/ 
# Fri, 06 Jan 2023 04:26:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 06 Jan 2023 04:26:00 GMT
USER www-data
# Fri, 06 Jan 2023 04:26:00 GMT
CMD ["wp" "shell"]
```

-	Layers:
	-	`sha256:844b8973ca9523380e35625da9a5fd2d50338c403129146541e13d0722c056f7`  
		Last Modified: Tue, 22 Nov 2022 22:47:59 GMT  
		Size: 3.2 MB (3170814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b6609bd910046178bd3eac570c2c1fc59cad29fb887adaab5d6693e71d47026`  
		Last Modified: Wed, 30 Nov 2022 21:21:53 GMT  
		Size: 1.9 MB (1910084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffc11912a116f8a8ce368f5345478751ea66ff55a5b6f480e750cb6e236b8691`  
		Last Modified: Wed, 30 Nov 2022 21:21:53 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c64f2471f65bf6185d022a4d96096ed5e3f00c2a9697e44113bd0c8728997e1`  
		Last Modified: Wed, 30 Nov 2022 21:21:53 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57683ee7d2997e0d36941f510f2682fbe3b45cc7cde9693808520948c518168e`  
		Last Modified: Fri, 06 Jan 2023 01:54:20 GMT  
		Size: 12.1 MB (12052190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de6ab11c36a0fd4f3dff0d9a5c311cb90907e0914858eb9461a382686d0a9c1`  
		Last Modified: Fri, 06 Jan 2023 01:54:19 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9a01fdf097da5964ffedb1f9baf0f8ec90ed403f66215021b8c85d551683a87`  
		Last Modified: Fri, 06 Jan 2023 01:54:22 GMT  
		Size: 17.9 MB (17927976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a033b6012af4224f669512ca2147b4dc2b41cc5745da927c81c2b2c28aacfe7`  
		Last Modified: Fri, 06 Jan 2023 01:54:19 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76531888f6c22de6e05f8059af98491c5e64d827cefe82e3dcb15f9596312641`  
		Last Modified: Fri, 06 Jan 2023 01:54:19 GMT  
		Size: 18.9 KB (18890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62f43d1b870d7b02ba10121af94933d12540a862feb8ba509aa4669bbb274406`  
		Last Modified: Fri, 06 Jan 2023 04:33:14 GMT  
		Size: 10.2 MB (10156672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db15898e1dcbdddc51a8b44b4ef87ef3c7403202d58d088329104d6e2864b641`  
		Last Modified: Fri, 06 Jan 2023 04:33:10 GMT  
		Size: 145.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6b788e449c4aa1fb1b91a976de081098762abef21e77dbd9b7ad1fa2f934b5`  
		Last Modified: Fri, 06 Jan 2023 04:33:11 GMT  
		Size: 8.6 MB (8554051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20471f74d7d5e722cec4e4775d9718c6cc3a24cd69aa2f2d5297f806f3b377a4`  
		Last Modified: Fri, 06 Jan 2023 04:33:10 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67800762e8fea4a514f3cc964b95d9b232a794e7d6205714a984a9a3fd7552e9`  
		Last Modified: Fri, 06 Jan 2023 04:33:10 GMT  
		Size: 1.4 MB (1435594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cfad244d51d2532a6e3455e61b2c6ccafbf625fe19ddb57f601b188c3dc8a330`  
		Last Modified: Fri, 06 Jan 2023 04:33:10 GMT  
		Size: 410.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
