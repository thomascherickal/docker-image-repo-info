## `wordpress:php8.1-fpm-alpine`

```console
$ docker pull wordpress@sha256:1f5a84d3d732df03ecc916b5b3a3d1425ffc0918e51929ab027ed1b824225f48
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

### `wordpress:php8.1-fpm-alpine` - linux; amd64

```console
$ docker pull wordpress@sha256:575f74236a60e470eb56a44c91999245fbe7e4e75a0a51021ee8a1727c480021
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.7 MB (103723239 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6e178bc4004110a9f33355671edc46e93042d02bb1a9c53e9eb4d1360787929f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 00:59:37 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 00:59:38 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 00:59:39 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 00:59:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 00:59:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 00:59:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:59:40 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:59:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 00:59:40 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 05 Apr 2022 01:24:02 GMT
ENV PHP_VERSION=8.1.4
# Tue, 05 Apr 2022 01:24:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 05 Apr 2022 01:24:02 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 05 Apr 2022 01:24:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 01:24:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 01:35:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 01:35:55 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 01:35:56 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 01:35:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 01:35:56 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 01:35:56 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 01:35:57 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 01:35:57 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 01:35:57 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 12:36:20 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Tue, 05 Apr 2022 12:37:21 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 05 Apr 2022 12:37:22 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Apr 2022 12:37:23 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Apr 2022 06:21:32 GMT
RUN set -eux; 	version='5.9.3'; 	sha1='cab576e112c45806c474b3cbe0d1263a2a879adf'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 07 Apr 2022 06:21:32 GMT
VOLUME [/var/www/html]
# Thu, 07 Apr 2022 06:21:32 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Thu, 07 Apr 2022 06:21:32 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Apr 2022 06:21:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Apr 2022 06:21:33 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60f85627e3d0df735c885c9502afee6c4a98aec08c02a0b31ffd6ee36d1d3ed`  
		Last Modified: Tue, 05 Apr 2022 02:49:01 GMT  
		Size: 1.7 MB (1701412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89395091f2959844751d9669bf4ffa0d72cae1e7710bd34d692c4a724abcfe20`  
		Last Modified: Tue, 05 Apr 2022 02:49:00 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2342a00f1dee7a210bf0e6327fce29393f5b0b67b1dbd297a5d39b322c2c61df`  
		Last Modified: Tue, 05 Apr 2022 02:49:00 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff752c21e64ca241a02a1a78ff7700712039a2fa7b20b59ab7b2bce188d5e9c`  
		Last Modified: Tue, 05 Apr 2022 02:50:40 GMT  
		Size: 11.7 MB (11720210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843ed70f77393571f5ed22d6444e27cedb57e143a5f8c0167996e0e8b0c7fa9f`  
		Last Modified: Tue, 05 Apr 2022 02:50:39 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1686c484d75f31537d5b47e82fd04697996bcebbe2a8b7e9b3e0a94310d6849`  
		Last Modified: Tue, 05 Apr 2022 02:51:31 GMT  
		Size: 12.3 MB (12337518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0823d62113c24cbec725ca07a999bb6116ccc7e5fdfc99da22bb44179fa1f25`  
		Last Modified: Tue, 05 Apr 2022 02:51:29 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6cc7d9b02381f1e8508665c1bb19543b7d5cd5afbeeec7ae210c1951304f73f`  
		Last Modified: Tue, 05 Apr 2022 02:51:29 GMT  
		Size: 18.6 KB (18595 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6b8e337f37cfd52d7d21aa27f51d72489c5d9c3344e6d1458b6c289a09257e`  
		Last Modified: Tue, 05 Apr 2022 02:51:29 GMT  
		Size: 8.6 KB (8620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e75985ce7c8309c84e0f4486bb030896d684ab760c3235069573e21f379ec31`  
		Last Modified: Tue, 05 Apr 2022 12:45:26 GMT  
		Size: 41.1 MB (41111904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd48f95ce88708e61e4d948469220a5874dfdf27438e27f3387b100078a446e2`  
		Last Modified: Tue, 05 Apr 2022 12:45:22 GMT  
		Size: 15.4 MB (15382426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9b5275ddf86eff7282beb6f014c7916cbf143dde345897fa5f8647a1f3f0457`  
		Last Modified: Tue, 05 Apr 2022 12:45:18 GMT  
		Size: 65.2 KB (65163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d31ad3f85b043dde66e76049001a7589e197a4ef468820da7d27735735708898`  
		Last Modified: Tue, 05 Apr 2022 12:45:18 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f2165eb0ce5f3b3749c8f904658f001ecb7175d82f3df83276bd393470052d9`  
		Last Modified: Thu, 07 Apr 2022 08:07:33 GMT  
		Size: 18.6 MB (18553896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:419c159c71e84023a771337a908c520dc1b590979beae8fb79737d59329e23d3`  
		Last Modified: Thu, 07 Apr 2022 08:07:30 GMT  
		Size: 2.3 KB (2340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1e8f78766f028280232eaac1b787cf8dc46ff3202c7c20fe5f55a7d8543e2a`  
		Last Modified: Thu, 07 Apr 2022 08:07:30 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.1-fpm-alpine` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:d23eb8660b1f6caa7c542a54b7f38b65fc0ce6b608873e761c0e5a24497d5de4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.8 MB (99816565 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f79fe00f0f7f51ea6bff657ea958a6c644bf44f65939ec724adadfe87196346`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:42 GMT
ADD file:159dcddaab900372df882a4e94615ed84250e9cea3e74bc0479d98280342f596 in / 
# Mon, 04 Apr 2022 23:49:42 GMT
CMD ["/bin/sh"]
# Mon, 04 Apr 2022 23:53:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 04 Apr 2022 23:53:13 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 04 Apr 2022 23:53:14 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 04 Apr 2022 23:53:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 04 Apr 2022 23:53:16 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 04 Apr 2022 23:53:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 04 Apr 2022 23:53:17 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 04 Apr 2022 23:53:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 04 Apr 2022 23:53:18 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 05 Apr 2022 00:13:28 GMT
ENV PHP_VERSION=8.1.4
# Tue, 05 Apr 2022 00:13:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 05 Apr 2022 00:13:29 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 05 Apr 2022 00:13:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 00:13:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:24:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 00:24:38 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:24:40 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 00:24:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 00:24:41 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 00:24:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 00:24:43 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 00:24:44 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 00:24:44 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 17:19:31 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Tue, 05 Apr 2022 17:21:48 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 05 Apr 2022 17:21:51 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Apr 2022 17:21:52 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Apr 2022 05:23:25 GMT
RUN set -eux; 	version='5.9.3'; 	sha1='cab576e112c45806c474b3cbe0d1263a2a879adf'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 07 Apr 2022 05:23:25 GMT
VOLUME [/var/www/html]
# Thu, 07 Apr 2022 05:23:26 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Thu, 07 Apr 2022 05:23:26 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Apr 2022 05:23:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Apr 2022 05:23:27 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c319b1fc4ed70b8241a7ce6ac0c4015d354bf5cf8c01eb73c50b6709c0c46e49`  
		Last Modified: Mon, 04 Apr 2022 19:09:22 GMT  
		Size: 2.6 MB (2621972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59f4857007e05a14c6f648dc95eb29cd4faae7806674bb49c86a9c22bf5c828e`  
		Last Modified: Tue, 05 Apr 2022 01:33:30 GMT  
		Size: 1.7 MB (1688742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb0f12cd34ba09b6e733247467586fb1354d26dfc93308155099ca243578518`  
		Last Modified: Tue, 05 Apr 2022 01:33:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ebc724c09cd88ae23080a3eb4cc057c4cbe9cbd5c83048ea54c647cbcc8f040`  
		Last Modified: Tue, 05 Apr 2022 01:33:29 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ba6098a8515c7390f35b08e759fc19433c97298e964da5af5b19c97773a5cb`  
		Last Modified: Tue, 05 Apr 2022 01:35:31 GMT  
		Size: 11.7 MB (11720180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f392d49c1a036736ea5afdc6442cb0fccfa317c2840c8a5d4a04be38d0780a33`  
		Last Modified: Tue, 05 Apr 2022 01:35:27 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e1e7da842dd5ad3e0bd5798119588b43e6d6df93382f4b3b9d7e9f13b66b89`  
		Last Modified: Tue, 05 Apr 2022 01:36:56 GMT  
		Size: 11.2 MB (11219847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf1e4882cce0961554359d59bfedf1260ad7e6f3b9458972657c697aace69420`  
		Last Modified: Tue, 05 Apr 2022 01:36:47 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da81aa97c99fb187e3c5b2e22f2183fb646a583d07135baeeb6c6a117e4664f0`  
		Last Modified: Tue, 05 Apr 2022 01:36:47 GMT  
		Size: 18.4 KB (18388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e0a272ec18f91f1673e3420f2a4cbef7d04a13c4f6d3868171e6591c9350c7`  
		Last Modified: Tue, 05 Apr 2022 01:36:47 GMT  
		Size: 8.6 KB (8620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef8414182afadcab70aefcce281923c2147f75ed84739ff29e6ab08e4c146b15`  
		Last Modified: Tue, 05 Apr 2022 17:40:23 GMT  
		Size: 38.8 MB (38788400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae56f262c90a3d9a015d99dbdba05a230891f7be1fe8591fcbd74348e2eee576`  
		Last Modified: Tue, 05 Apr 2022 17:40:06 GMT  
		Size: 15.1 MB (15122456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b529f06465dc980106c926b0293fc7758f9caa66bce6c756d8ca6a64126c2b`  
		Last Modified: Tue, 05 Apr 2022 17:39:56 GMT  
		Size: 65.1 KB (65128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7a1fcd472d5ac6239db038308b84a23110cc697919f8ba18ab11fa2249e2d0`  
		Last Modified: Tue, 05 Apr 2022 17:39:56 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f170889b1290293fd739eeb013eaca9671d3eb4d46c31fafd419df25e851f9`  
		Last Modified: Thu, 07 Apr 2022 05:36:16 GMT  
		Size: 18.6 MB (18553895 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370d60217d074f143060e8abd3a8da34eeaba02a28ea266d4fa9e47a079d240c`  
		Last Modified: Thu, 07 Apr 2022 05:36:02 GMT  
		Size: 2.3 KB (2339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f336d2827547fd30ee47739f502890ba2637b0db20c01b10e308f7d43e1f82`  
		Last Modified: Thu, 07 Apr 2022 05:36:02 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.1-fpm-alpine` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:a57d0c9588f085b9314b21aef075b416c8547bbe80ea44a041051ffc2dbc754f
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.6 MB (96630842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2efb46265b32d4e32f45b123d293b621a8ba258ac4d1f843666f7ffdf9d8d051`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 04 Apr 2022 23:57:34 GMT
ADD file:20f8cdddc53a4a8bd78945fc32fe08e9f80ab3b16dc20a9aa4ba73b79f2bc71c in / 
# Mon, 04 Apr 2022 23:57:35 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 00:44:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 00:44:29 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 00:44:31 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 00:44:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 00:44:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 00:44:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:44:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:44:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 00:44:34 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 05 Apr 2022 01:07:25 GMT
ENV PHP_VERSION=8.1.4
# Tue, 05 Apr 2022 01:07:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 05 Apr 2022 01:07:27 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 05 Apr 2022 01:07:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 01:07:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 01:16:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 01:16:59 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 01:17:02 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 01:17:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 01:17:03 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 01:17:04 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 01:17:05 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 01:17:05 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 01:17:06 GMT
CMD ["php-fpm"]
# Wed, 06 Apr 2022 00:27:40 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Wed, 06 Apr 2022 00:29:50 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Wed, 06 Apr 2022 00:29:53 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 06 Apr 2022 00:29:54 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Apr 2022 15:46:28 GMT
RUN set -eux; 	version='5.9.3'; 	sha1='cab576e112c45806c474b3cbe0d1263a2a879adf'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 07 Apr 2022 15:46:29 GMT
VOLUME [/var/www/html]
# Thu, 07 Apr 2022 15:46:30 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Thu, 07 Apr 2022 15:46:30 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Apr 2022 15:46:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Apr 2022 15:46:31 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:57fb4b5f1a47c953ca5703f0f81ce14e5d01cf23aa79558b5adb961cc526e320`  
		Last Modified: Mon, 04 Apr 2022 19:09:36 GMT  
		Size: 2.4 MB (2424323 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31e79621416caf77f775491eca7e32b6744cb98a7f314d25662db9d47388f78c`  
		Last Modified: Tue, 05 Apr 2022 02:39:26 GMT  
		Size: 1.6 MB (1556468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c8e6096135db80ad99d3893e56fed755390988cde114bfa2eadb0344135aa68`  
		Last Modified: Tue, 05 Apr 2022 02:39:26 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e579551e9fe0160cdaf60f2b80ab01b627b8bfea2c89907509913896a5f1b118`  
		Last Modified: Tue, 05 Apr 2022 02:39:25 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5840248a03e2bc629aba5fe7a23d0f24d2253f696cc6370d481cdc54ea58935`  
		Last Modified: Tue, 05 Apr 2022 02:42:55 GMT  
		Size: 11.7 MB (11720159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:040b4d8277d4c6eb01cc62db92e54abc10a2cded018539c51f77c3680c4a526e`  
		Last Modified: Tue, 05 Apr 2022 02:42:52 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:379322d677f555f93f8ec88f975e7fcdca6a1fa741a216ea400abe226d9f4663`  
		Last Modified: Tue, 05 Apr 2022 02:44:22 GMT  
		Size: 10.5 MB (10541976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aa8865105901e37ef2032dcb8b5a70d5385cccf5a65e63b295985bebca39b8b`  
		Last Modified: Tue, 05 Apr 2022 02:44:15 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ea0f650cdee6fc74476a40c0f9eb0443cc1b1bcc0bdb8d2381b08e20af614a`  
		Last Modified: Tue, 05 Apr 2022 02:44:15 GMT  
		Size: 18.4 KB (18362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16191f2c3cc17c07a1e2f6b11e55ed8e89be432a3d0fb3aa4d7a6da2f252e36`  
		Last Modified: Tue, 05 Apr 2022 02:44:15 GMT  
		Size: 8.6 KB (8620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:527b588109e7f681c85e3ade26fe5955c5b88ba79f1ec95c1a660675e83dc022`  
		Last Modified: Wed, 06 Apr 2022 00:55:28 GMT  
		Size: 36.8 MB (36809632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e631999102bbc9446fe05cd014de1f9be6ee6fb75b91ca36a4d60de0747eccc4`  
		Last Modified: Wed, 06 Apr 2022 00:55:15 GMT  
		Size: 14.9 MB (14923324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a85e5ef00fca84bea03db4cb96b55630b8f5d5eab291b036473180687e666a8b`  
		Last Modified: Wed, 06 Apr 2022 00:55:05 GMT  
		Size: 65.2 KB (65154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5a2b96235c29000f823b5f368c8eb29373422106ca6949fcfb42b4420d98290`  
		Last Modified: Wed, 06 Apr 2022 00:55:05 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e5bb3daef56326e203bd7cc3c8220263e2794b7d95ecc76af7b8d0d7b45a648`  
		Last Modified: Thu, 07 Apr 2022 16:00:59 GMT  
		Size: 18.6 MB (18553883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8061373653d30b3f9f49718754e6b78c8ed71ab1d68b5db37f6c81b5f2f85319`  
		Last Modified: Thu, 07 Apr 2022 16:00:45 GMT  
		Size: 2.3 KB (2341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d2291e3d9df86d31cbc3fd0284ca93983ec2a18e560334f68cbfe3bbf4fe962`  
		Last Modified: Thu, 07 Apr 2022 16:00:46 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.1-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:cfb389d7d444b230833fe612a665a4e6380d8837ce9ba633cc87d7721cec1b6a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.5 MB (102480696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16bb9e9be3e7dd29c628ae4803fb916cc54c8bdf762e15d1dfaab4b8caa129e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:31 GMT
ADD file:90e56af13188c7f0283d244a0d70b853d8bef8587a41f1da8eac3a2aba8964ef in / 
# Mon, 04 Apr 2022 23:39:31 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 00:14:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 00:14:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 00:14:51 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 00:14:52 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 00:14:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 00:14:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:14:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:14:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 00:14:57 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 05 Apr 2022 00:39:03 GMT
ENV PHP_VERSION=8.1.4
# Tue, 05 Apr 2022 00:39:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 05 Apr 2022 00:39:05 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 05 Apr 2022 00:39:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 00:39:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:50:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 00:50:15 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:50:16 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 00:50:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 00:50:18 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 00:50:19 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 00:50:20 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 00:50:21 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 00:50:22 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 15:45:52 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Tue, 05 Apr 2022 15:46:49 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 05 Apr 2022 15:46:50 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Apr 2022 15:46:51 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Apr 2022 06:13:26 GMT
RUN set -eux; 	version='5.9.3'; 	sha1='cab576e112c45806c474b3cbe0d1263a2a879adf'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 07 Apr 2022 06:13:27 GMT
VOLUME [/var/www/html]
# Thu, 07 Apr 2022 06:13:28 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Thu, 07 Apr 2022 06:13:29 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Apr 2022 06:13:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Apr 2022 06:13:30 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:9981e73032c8833e387a8f96986e560edbed12c38119e0edb0439c9c2234eac9`  
		Last Modified: Mon, 04 Apr 2022 19:09:10 GMT  
		Size: 2.7 MB (2716477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f69c83c314e8e18362c8a6739f6f7857ed89cc606ea05f0a95d6eb922fbc3f5`  
		Last Modified: Tue, 05 Apr 2022 01:52:13 GMT  
		Size: 1.7 MB (1696240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c8f271730dc83953a1ddf4c1d17b33fcb696501a3331a55c9ed5ccfec44542c`  
		Last Modified: Tue, 05 Apr 2022 01:52:13 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08d1df3f0f228d28d8f270e64056adb7297fcca517c48468be36d482e2f383dd`  
		Last Modified: Tue, 05 Apr 2022 01:52:12 GMT  
		Size: 219.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9605e84f1e4eb41317faa75a1c1ea130935cae7f12b693a047735c315bda12b5`  
		Last Modified: Tue, 05 Apr 2022 01:54:17 GMT  
		Size: 11.7 MB (11720005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752671a7f3fd2db646b4ac053647be92b34212858e4f07657a5dde0eb6ee53fb`  
		Last Modified: Tue, 05 Apr 2022 01:54:16 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f49a7aec53f3f6818c652af186cd348a05b3934f0ff877bb8e8db142607c81b3`  
		Last Modified: Tue, 05 Apr 2022 01:55:19 GMT  
		Size: 12.4 MB (12394633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d25c774bef743971c852692d8e1e07b82db317734d86e7b20a1b19efec39b95`  
		Last Modified: Tue, 05 Apr 2022 01:55:18 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a7059ab80b32bb2c0bb5e04dd86b05617c95b633c819a10c4c459a8d879e665`  
		Last Modified: Tue, 05 Apr 2022 01:55:17 GMT  
		Size: 18.3 KB (18309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5469ae29ce7838dcb8122bb3c1580e2dc7200e0ae953dc2cf2f1f7cda8fdda`  
		Last Modified: Tue, 05 Apr 2022 01:55:17 GMT  
		Size: 8.6 KB (8621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:151384c3ec679eb3a7f4244b764e9e08eb8c792e8a45c34aeae2a8857b7ccda0`  
		Last Modified: Tue, 05 Apr 2022 16:00:08 GMT  
		Size: 39.9 MB (39944198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19862fad38601a035b07649260ea03970c298881f5c6ee3c6ebd04277d33f224`  
		Last Modified: Tue, 05 Apr 2022 16:00:05 GMT  
		Size: 15.4 MB (15354510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9986ea71a40ead29b91d2c78990114ca53472eab4541f36d5290e3caf0c1dde8`  
		Last Modified: Tue, 05 Apr 2022 16:00:00 GMT  
		Size: 65.1 KB (65076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d6780bd6cadfbf6118a4be767a5d7ccefb6eb2abd37288055474409ab8da29`  
		Last Modified: Tue, 05 Apr 2022 16:00:00 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bdabec6d335b8c148d4827b0c030d01e2ca6e6536d7e010577430927f4c4be2`  
		Last Modified: Thu, 07 Apr 2022 06:21:02 GMT  
		Size: 18.6 MB (18553764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66edf4a271d9497ca93dcf78900c9ebbd8417e0e2dfd1c19106c8f5ecfbaf3b8`  
		Last Modified: Thu, 07 Apr 2022 06:20:59 GMT  
		Size: 2.3 KB (2339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f040210ff07edc88e3575db8044399642832420d8d67171c359e74851ebb231e`  
		Last Modified: Thu, 07 Apr 2022 06:20:59 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.1-fpm-alpine` - linux; 386

```console
$ docker pull wordpress@sha256:ead9030b28fbc36fb6f152e159880eceeb5b427d8d0f39c8d2b044d314a89124
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.7 MB (104724006 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:87349e02753a8cf7f3aa71e4ef78a7a6f893e15167a70c04166bc186def3123e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:25 GMT
ADD file:7d51a0f8691eb78c9062fd31984423a93d276a67b4ed5d1a706e1c2cd9fea23a in / 
# Mon, 04 Apr 2022 23:38:25 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 00:05:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 00:05:49 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 00:05:49 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 00:05:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 00:05:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 00:05:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:05:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:05:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 00:05:55 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 05 Apr 2022 00:22:05 GMT
ENV PHP_VERSION=8.1.4
# Tue, 05 Apr 2022 00:22:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 05 Apr 2022 00:22:07 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 05 Apr 2022 00:22:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 00:22:16 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:29:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 00:29:16 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:29:16 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 00:29:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 00:29:18 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 00:29:19 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 00:29:20 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 00:29:21 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 00:29:22 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 07:12:41 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Tue, 05 Apr 2022 07:13:33 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 05 Apr 2022 07:13:34 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Apr 2022 07:13:35 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Apr 2022 06:16:08 GMT
RUN set -eux; 	version='5.9.3'; 	sha1='cab576e112c45806c474b3cbe0d1263a2a879adf'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 07 Apr 2022 06:16:09 GMT
VOLUME [/var/www/html]
# Thu, 07 Apr 2022 06:16:10 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Thu, 07 Apr 2022 06:16:11 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Apr 2022 06:16:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Apr 2022 06:16:12 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:73b28a5955ec7fb46f2cf0434e4901a889f7dda3f8c9ec496300feb256c7eda8`  
		Last Modified: Mon, 04 Apr 2022 19:10:03 GMT  
		Size: 2.8 MB (2818974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c45a8803aeb5badfcbafc3a64d45ef0d99401331488cc5495a9bf7e66c3c475`  
		Last Modified: Tue, 05 Apr 2022 01:23:59 GMT  
		Size: 1.8 MB (1800021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8efaa6aa5ded5cf73ecb3fc3a3fb655e5cadfea53b9ab939d90bf4ddb8653d0`  
		Last Modified: Tue, 05 Apr 2022 01:23:59 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13f0f938930408ae4fa469fe3ce2586fc2b3be3450492deeabddfac3f9533860`  
		Last Modified: Tue, 05 Apr 2022 01:23:59 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:421feb0f02e6ae95405ca274470f0fdc87caa441ee6a9eaa1e76218b1db6fb0b`  
		Last Modified: Tue, 05 Apr 2022 01:26:21 GMT  
		Size: 11.7 MB (11719987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1769976716c27553c8cde0f611a84495731c6934ff8cfcd80a9d644fa1ee933`  
		Last Modified: Tue, 05 Apr 2022 01:26:19 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab029e0d2ce3bac169d25f1323b0497f9654dbe78d7c272f84b242024ff2cc1`  
		Last Modified: Tue, 05 Apr 2022 01:27:25 GMT  
		Size: 12.6 MB (12622301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:291d556ff60220f93c54844f988c23409e018b987da3b506a467f8de256c9dab`  
		Last Modified: Tue, 05 Apr 2022 01:27:23 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:507d526143b376768ce847cafd09c411e084aeb18b5c2d061907ceaa3fa07182`  
		Last Modified: Tue, 05 Apr 2022 01:27:23 GMT  
		Size: 18.5 KB (18476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22cbf41ad9c5a059856761fb843a33043d0d35824782e79f716d64ffbc346c1b`  
		Last Modified: Tue, 05 Apr 2022 01:27:23 GMT  
		Size: 8.6 KB (8619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d35366a2c26917ce297040749da58ea56469c716acb75d1c9fa770eaf068f781`  
		Last Modified: Tue, 05 Apr 2022 07:26:06 GMT  
		Size: 41.5 MB (41521378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee23a992eeca4498661faba0dfe77037d8ba93d26fabd5275e6066ea2ef1e48c`  
		Last Modified: Tue, 05 Apr 2022 07:26:01 GMT  
		Size: 15.6 MB (15586606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8008213150c12fdc7082db5b2d6b2a38c775537c34e6b7d175285156cb99ea59`  
		Last Modified: Tue, 05 Apr 2022 07:25:56 GMT  
		Size: 65.0 KB (65021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:320616092cf445b22f834ff38550913103d2877c35519345f9ba5fd32a58af4d`  
		Last Modified: Tue, 05 Apr 2022 07:25:56 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfca723aa179fbcc8836916d81da2b33b2752b721327ca22605ff48877a2e32`  
		Last Modified: Thu, 07 Apr 2022 06:24:07 GMT  
		Size: 18.6 MB (18553768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89d619110daba945d9d6199c776da4d4bc09b64c77975e48e1b7e57930794b70`  
		Last Modified: Thu, 07 Apr 2022 06:24:04 GMT  
		Size: 2.3 KB (2340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec8b24b263d09f2ff7538f7231a75f20aa3c78bc949cde4156845e8aac1aaf8d`  
		Last Modified: Thu, 07 Apr 2022 06:24:04 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.1-fpm-alpine` - linux; ppc64le

```console
$ docker pull wordpress@sha256:94ae8cd39efdc856462220c6e6c51f9a4e29afffdca73d0d4f4ad10f6639c76b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105576089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7b582ea985c6358cdd27d465a53c0a7e967e9ce196218992724c0c24f83605d9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Tue, 05 Apr 2022 00:23:30 GMT
ADD file:960cf6f9d3d1cfcb36c2d67dd4c3eaba7db1d0c7afe97968512248d7f234ad47 in / 
# Tue, 05 Apr 2022 00:23:32 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 01:16:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 01:16:42 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 01:16:56 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 01:16:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 01:17:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 01:17:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 01:17:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 01:17:14 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 01:17:17 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 05 Apr 2022 01:43:25 GMT
ENV PHP_VERSION=8.1.4
# Tue, 05 Apr 2022 01:43:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 05 Apr 2022 01:43:32 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 05 Apr 2022 01:43:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 01:43:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 01:55:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 01:55:07 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 01:55:24 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 01:55:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 01:55:34 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 01:55:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 01:55:47 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 01:55:50 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 01:55:53 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 22:34:35 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Tue, 05 Apr 2022 22:36:10 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 05 Apr 2022 22:36:19 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Apr 2022 22:36:26 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Apr 2022 12:02:35 GMT
RUN set -eux; 	version='5.9.3'; 	sha1='cab576e112c45806c474b3cbe0d1263a2a879adf'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 07 Apr 2022 12:02:42 GMT
VOLUME [/var/www/html]
# Thu, 07 Apr 2022 12:02:44 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Thu, 07 Apr 2022 12:02:45 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Apr 2022 12:02:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Apr 2022 12:02:52 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:1877acf2d48ed8bcb5bd9756a95aca0c077457be7cf4fcef25807f4e9be88db1`  
		Last Modified: Mon, 04 Apr 2022 19:09:49 GMT  
		Size: 2.8 MB (2811186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb67fc22738d58442db1bd40a3c6f60cb5038ef87b356fda058eae811b9e66a1`  
		Last Modified: Tue, 05 Apr 2022 03:22:51 GMT  
		Size: 1.7 MB (1744650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7c452ba09cd632ffe58aa658dc18133d1783bb3b475ac3001e7cb6492a41dcb`  
		Last Modified: Tue, 05 Apr 2022 03:22:51 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03960c8a570255096ca4926f8aac09cdf62550255cb84376f5dab02635482972`  
		Last Modified: Tue, 05 Apr 2022 03:22:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:006c6225409c7be98c3fa0e57558b382b57694a02280a35a4e9c4f9b0d3dcf43`  
		Last Modified: Tue, 05 Apr 2022 03:25:18 GMT  
		Size: 11.7 MB (11720200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b444b16ec3dcee90e96afd8fe4291aa87d1ef4f052a779ab17fe82698a334f0`  
		Last Modified: Tue, 05 Apr 2022 03:25:17 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:344b8ccfe3fedce8d4bf38f658e0f607ad79f75daaf27668420aa1b03018ce6c`  
		Last Modified: Tue, 05 Apr 2022 03:26:30 GMT  
		Size: 12.7 MB (12723198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71af482c99c42f46ec6fc5ef5283791f93dfd60c7f306b0a6a1845ea0bd47bf1`  
		Last Modified: Tue, 05 Apr 2022 03:26:27 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60187b35d92a598c4ce737a3acc9151d139899700b5ca8f898a58222b108bc88`  
		Last Modified: Tue, 05 Apr 2022 03:26:27 GMT  
		Size: 18.4 KB (18399 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30dd93ed01add4a8c4dc5afe485b33107e82ac341289c3cfdce4b73d64a372b7`  
		Last Modified: Tue, 05 Apr 2022 03:26:27 GMT  
		Size: 8.6 KB (8622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee8c742478befe316af49bbb2b7de6418e84843abd026ac2edc5274a9ac70a3`  
		Last Modified: Tue, 05 Apr 2022 22:56:57 GMT  
		Size: 42.3 MB (42339742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7aab391c0a668c5570828daa909d545093b65e322d277a836583f3baa3be082`  
		Last Modified: Tue, 05 Apr 2022 22:56:51 GMT  
		Size: 15.6 MB (15582120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494ac4446c0852163d5de1c64dedc97da3a18fc9a2fa964dffbd1c1a50983e9d`  
		Last Modified: Tue, 05 Apr 2022 22:56:46 GMT  
		Size: 65.1 KB (65130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f8b43b0469b76dd98bedb046b59f0ce7d20f478d09b52e21013633815fc96d`  
		Last Modified: Tue, 05 Apr 2022 22:56:46 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4dbbdb79ce103c7c8c512c429bda35a05d77d76f18fd5e56f8cc84a29a1bbf2a`  
		Last Modified: Thu, 07 Apr 2022 12:12:01 GMT  
		Size: 18.6 MB (18553893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e24dd77d44550806dc1889f7be48cbe22e7e4c45be6176bbd3b5f8d6144b14be`  
		Last Modified: Thu, 07 Apr 2022 12:11:57 GMT  
		Size: 2.3 KB (2343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f5d603e14fe4344d3b185929b038528b28f6578b5495e06a092f350e6661ce`  
		Last Modified: Thu, 07 Apr 2022 12:11:57 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.1-fpm-alpine` - linux; s390x

```console
$ docker pull wordpress@sha256:5cdb34cf00dd7fc66fc4f42cef7619a4021e186c6eaa6cb80cdaec1f925cec0b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.8 MB (94824650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3a58f5cfc5a3d0e3f956e69a70f2084d356c93c60fe0cc06676c1359f9c78aa1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 04 Apr 2022 23:41:39 GMT
ADD file:f22e4b2be87d3c59c8c609acf79015938dc1fba0b26d7c1b59bd0fc36d63a906 in / 
# Mon, 04 Apr 2022 23:41:39 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 00:02:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 05 Apr 2022 00:02:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 05 Apr 2022 00:02:59 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 05 Apr 2022 00:02:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 05 Apr 2022 00:03:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 05 Apr 2022 00:03:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:03:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 05 Apr 2022 00:03:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 05 Apr 2022 00:03:00 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 05 Apr 2022 00:16:08 GMT
ENV PHP_VERSION=8.1.4
# Tue, 05 Apr 2022 00:16:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.4.tar.xz.asc
# Tue, 05 Apr 2022 00:16:08 GMT
ENV PHP_SHA256=05a8c0ac30008154fb38a305560543fc172ba79fb957084a99b8d3b10d5bdb4b
# Tue, 05 Apr 2022 00:16:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 05 Apr 2022 00:16:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:21:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 05 Apr 2022 00:21:55 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 05 Apr 2022 00:21:56 GMT
RUN docker-php-ext-enable sodium
# Tue, 05 Apr 2022 00:21:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 05 Apr 2022 00:21:56 GMT
WORKDIR /var/www/html
# Tue, 05 Apr 2022 00:21:56 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 05 Apr 2022 00:21:56 GMT
STOPSIGNAL SIGQUIT
# Tue, 05 Apr 2022 00:21:57 GMT
EXPOSE 9000
# Tue, 05 Apr 2022 00:21:57 GMT
CMD ["php-fpm"]
# Tue, 05 Apr 2022 13:08:30 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Tue, 05 Apr 2022 13:09:12 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 05 Apr 2022 13:09:13 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 05 Apr 2022 13:09:13 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Apr 2022 05:02:42 GMT
RUN set -eux; 	version='5.9.3'; 	sha1='cab576e112c45806c474b3cbe0d1263a2a879adf'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 07 Apr 2022 05:02:44 GMT
VOLUME [/var/www/html]
# Thu, 07 Apr 2022 05:02:44 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Thu, 07 Apr 2022 05:02:44 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Apr 2022 05:02:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Apr 2022 05:02:44 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:a27b630f446c3da376a30cf610e4bfa6847f8b87c83702c29e72b986f4e52d28`  
		Last Modified: Mon, 04 Apr 2022 23:42:37 GMT  
		Size: 2.6 MB (2600375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df780ceebfdd113d5a6f5772c1d4abeb603e14b99c871ea2281632b11cf6f759`  
		Last Modified: Tue, 05 Apr 2022 01:09:34 GMT  
		Size: 1.8 MB (1760653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca5640ab2fd0b3501350a8a837b003d809c84b6169e11a74c71e7a193175a3e3`  
		Last Modified: Tue, 05 Apr 2022 01:09:35 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4910c970dadd8c90e6942fd635f2d508e9f2a2ecd4c5281578cf6470fa8bc432`  
		Last Modified: Tue, 05 Apr 2022 01:09:34 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6275c65e0f4211e10201152dbb8bd94189eabdc679678f1d24002b9f0f94337`  
		Last Modified: Tue, 05 Apr 2022 01:11:22 GMT  
		Size: 11.7 MB (11720226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59e8523c33ddd8039bcd9d8cd874deae798bf5e0aa8d787ef70b0ddd999377e1`  
		Last Modified: Tue, 05 Apr 2022 01:11:21 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241b10e56802ec24f776fe1d0b9d9d95ea3d912e754b03b661345dab1e01ad15`  
		Last Modified: Tue, 05 Apr 2022 01:12:03 GMT  
		Size: 11.5 MB (11532105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86655782fbae70b68e87c9f2608bdbe02ae36b35d5ad50ce67bcc3e2039bb1d7`  
		Last Modified: Tue, 05 Apr 2022 01:12:02 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42ddb3c3843d322192b3ce321fce0873a55b278fecd29ae696f3772d58181b6`  
		Last Modified: Tue, 05 Apr 2022 01:12:02 GMT  
		Size: 18.4 KB (18417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80ab4776a633ad7230767a1d8530ce7c8b016fcea3dd57457cda4d1d01a8ba0f`  
		Last Modified: Tue, 05 Apr 2022 01:12:02 GMT  
		Size: 8.6 KB (8615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98890c5bd5b93fda292dfc3d8de486ad1cac6b57cf9b2ff94e224e32b1a07a5`  
		Last Modified: Tue, 05 Apr 2022 13:20:25 GMT  
		Size: 33.1 MB (33069348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b6991ee2d9c1a5d179fd7d14e8cafd4abd2e5b71e4146e01af3415ef58e3fed`  
		Last Modified: Tue, 05 Apr 2022 13:20:23 GMT  
		Size: 15.5 MB (15493072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06973119aafcdbcae6d7ec22ff51f62b865a962fabae4ead475a64a6f654b4da`  
		Last Modified: Tue, 05 Apr 2022 13:20:20 GMT  
		Size: 59.0 KB (59000 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dd5406d156a4471482f97f25b743a2f85cee1c26c613dbdaf876c2b2403b768`  
		Last Modified: Tue, 05 Apr 2022 13:20:20 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8ef8b0714eedd48818ae4fe16785b15c822f9591859eb5ea366845a9d1c1fb1`  
		Last Modified: Thu, 07 Apr 2022 05:08:36 GMT  
		Size: 18.6 MB (18553899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a2b430838a75d7f90b34604931d2b518aa7ebda66335b497944eb3433d92003`  
		Last Modified: Thu, 07 Apr 2022 05:08:34 GMT  
		Size: 2.3 KB (2339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8610a4dc4185f67bd93c482dca8158fdaf5a1f748ddff36c883cd2004ad5700f`  
		Last Modified: Thu, 07 Apr 2022 05:08:34 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
