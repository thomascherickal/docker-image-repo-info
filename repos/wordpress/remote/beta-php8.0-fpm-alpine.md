## `wordpress:beta-php8.0-fpm-alpine`

```console
$ docker pull wordpress@sha256:21ba9b79ea36311603b8a798e066c89ecf09d2bdcba9096f42ae40e83b59a796
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

### `wordpress:beta-php8.0-fpm-alpine` - linux; amd64

```console
$ docker pull wordpress@sha256:dc8870a5ae7620a96db9d91b3bbe7868b00e4937be3aaef36024808c930f6396
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.5 MB (65520846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d8e05f4652dfc3f1450071d1d7e85465ac8104e62fd3f9d3980255ce6f82aac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Fri, 29 Jan 2021 01:18:41 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 29 Jan 2021 01:18:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:18:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:18:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 01:18:43 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 05 Feb 2021 04:34:13 GMT
ENV PHP_VERSION=8.0.2
# Fri, 05 Feb 2021 04:34:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Fri, 05 Feb 2021 04:34:13 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Fri, 05 Feb 2021 04:34:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 05 Feb 2021 04:34:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 05 Feb 2021 04:45:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 05 Feb 2021 04:45:34 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 05 Feb 2021 04:45:35 GMT
RUN docker-php-ext-enable sodium
# Fri, 05 Feb 2021 04:45:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 05 Feb 2021 04:45:36 GMT
WORKDIR /var/www/html
# Fri, 05 Feb 2021 04:45:37 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 05 Feb 2021 04:45:37 GMT
STOPSIGNAL SIGQUIT
# Fri, 05 Feb 2021 04:45:37 GMT
EXPOSE 9000
# Fri, 05 Feb 2021 04:45:37 GMT
CMD ["php-fpm"]
# Fri, 05 Feb 2021 05:11:47 GMT
RUN set -eux; 	apk add --no-cache 		bash 		sed 		ghostscript 	;
# Fri, 05 Feb 2021 05:12:27 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 05 Feb 2021 05:12:29 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 05 Feb 2021 05:12:30 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 05 Feb 2021 05:15:15 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 05 Feb 2021 05:15:15 GMT
VOLUME [/var/www/html]
# Fri, 05 Feb 2021 05:15:16 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Fri, 05 Feb 2021 05:15:16 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Fri, 05 Feb 2021 05:15:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Feb 2021 05:15:16 GMT
CMD ["php-fpm"]
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
	-	`sha256:f97922f128cad26e403a70408b34335288fe29ba6f529dcdd9789842461f4e96`  
		Last Modified: Fri, 05 Feb 2021 05:05:48 GMT  
		Size: 10.7 MB (10669910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fb2adf5e68e5567659282ff6c6fe91a65941224183b4c2439c7da23e6c53d79`  
		Last Modified: Fri, 05 Feb 2021 05:05:46 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a99d9fc85f4cc14d5658ac38d615aef7c79f674ce08e1251eb62a510c5b84c0`  
		Last Modified: Fri, 05 Feb 2021 05:05:50 GMT  
		Size: 15.0 MB (15018782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bd698115ac6d7b9064310fad9c089e52e797866dd0e601ea5c1b559b9ed1bf`  
		Last Modified: Fri, 05 Feb 2021 05:05:46 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8980c1b3c358915b4278bc9c9b49ca637bffd0861476b74bb3ae111ad92f6c8`  
		Last Modified: Fri, 05 Feb 2021 05:05:46 GMT  
		Size: 17.5 KB (17518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed05f5ca9a9a4ba25508e4a4db8d17791a9baa5c0afec0c36f4ed16b269d6b6`  
		Last Modified: Fri, 05 Feb 2021 05:05:46 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3273264ea4d4ae769048eeb86bba9c839b1216b5a3347798d9ec1dc56a1da0d`  
		Last Modified: Fri, 05 Feb 2021 05:18:56 GMT  
		Size: 19.3 MB (19270119 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6bd8e388c14b015814e920bee2124e05edcaa1dd675a6b91124e3c3aa1ebf9e`  
		Last Modified: Fri, 05 Feb 2021 05:18:51 GMT  
		Size: 431.8 KB (431757 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d8a3fb6b6c567bc2504c42d84077b85262fae80a1fd856bffa89a89d26650e0`  
		Last Modified: Fri, 05 Feb 2021 05:18:51 GMT  
		Size: 40.5 KB (40451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a14ccdbd44b8dffd5b87d32bf462b49e18237cef52b5a2e2a6466b45f08ffcd`  
		Last Modified: Fri, 05 Feb 2021 05:18:51 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3254793e37568f1aa9cd9e95a65f0ccb30e7a16012a825d6185620907ab52e1`  
		Last Modified: Fri, 05 Feb 2021 05:20:04 GMT  
		Size: 15.5 MB (15549245 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be49fae4d7208e1e0eedc8d625d8fb23d2a6777c5f5b9ddfdfb3fd552515c244`  
		Last Modified: Fri, 05 Feb 2021 05:20:00 GMT  
		Size: 2.1 KB (2092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f76603fa0b639eb0fcad38d7b9be9d4e5ad36af72982fc47ad326a39d1375dcb`  
		Last Modified: Fri, 05 Feb 2021 05:20:00 GMT  
		Size: 1.6 KB (1633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-php8.0-fpm-alpine` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:8b38363619b3cd26b2b84346c12d460841b009039a9b8e346e82f2edec214180
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.5 MB (63489284 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:083e6984e21648df3fb3008800b53f1d0a078b22fa2d1a186f6380b13b416a57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Fri, 29 Jan 2021 00:37:53 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 29 Jan 2021 00:37:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:37:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:37:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 00:37:56 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 05 Feb 2021 02:32:18 GMT
ENV PHP_VERSION=8.0.2
# Fri, 05 Feb 2021 02:32:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Fri, 05 Feb 2021 02:32:20 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Fri, 05 Feb 2021 02:32:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 05 Feb 2021 02:32:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 05 Feb 2021 02:36:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 05 Feb 2021 02:36:03 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 05 Feb 2021 02:36:09 GMT
RUN docker-php-ext-enable sodium
# Fri, 05 Feb 2021 02:36:10 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 05 Feb 2021 02:36:11 GMT
WORKDIR /var/www/html
# Fri, 05 Feb 2021 02:36:14 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 05 Feb 2021 02:36:15 GMT
STOPSIGNAL SIGQUIT
# Fri, 05 Feb 2021 02:36:16 GMT
EXPOSE 9000
# Fri, 05 Feb 2021 02:36:17 GMT
CMD ["php-fpm"]
# Fri, 05 Feb 2021 02:52:22 GMT
RUN set -eux; 	apk add --no-cache 		bash 		sed 		ghostscript 	;
# Fri, 05 Feb 2021 02:53:16 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 05 Feb 2021 02:53:21 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 05 Feb 2021 02:53:23 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 05 Feb 2021 02:55:35 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 05 Feb 2021 02:55:36 GMT
VOLUME [/var/www/html]
# Fri, 05 Feb 2021 02:55:37 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Fri, 05 Feb 2021 02:55:38 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Fri, 05 Feb 2021 02:55:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Feb 2021 02:55:39 GMT
CMD ["php-fpm"]
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
	-	`sha256:84b3e2936679b0bb44255c89b9ec9c1481f063a2a4b845128a1daebaaba4b0b4`  
		Last Modified: Fri, 05 Feb 2021 02:48:22 GMT  
		Size: 10.7 MB (10669917 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc7680429433d29a09109b1d7868802a31e32488c31c2ef0f07e4a4c9c8fe2b1`  
		Last Modified: Fri, 05 Feb 2021 02:48:20 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ff6fc7598e556dc53407c972e6150dcefbe402a83f764d470009dd9f1c8854c`  
		Last Modified: Fri, 05 Feb 2021 02:48:24 GMT  
		Size: 13.7 MB (13652207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d62b112a28e7ac15884600fd1bf2085b409062a411c6203fecc317e8645196f`  
		Last Modified: Fri, 05 Feb 2021 02:48:20 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28cdedb9b92c5fea7cd39784f45d4a2e06595a73a35c491fd635a49ca484390a`  
		Last Modified: Fri, 05 Feb 2021 02:48:20 GMT  
		Size: 17.5 KB (17531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f24bf495fd990b88438086539eb2bf1647d7b7b6a0675bbfb1c4f2a53d0ac27b`  
		Last Modified: Fri, 05 Feb 2021 02:48:20 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed63b6bb4faf3860fb23af57e61e7a8e42370b86eb3bae5b43570cf177c32e3a`  
		Last Modified: Fri, 05 Feb 2021 02:57:04 GMT  
		Size: 18.8 MB (18833663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a96ada5c0e2809c4efc7452271532d389d07373ea33a271422c7299ca1bd5ba`  
		Last Modified: Fri, 05 Feb 2021 02:56:56 GMT  
		Size: 402.4 KB (402401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8238ebcdfd9515ceb342e1cdfe5bab8fff3569fac720479261758dffc4b50c9f`  
		Last Modified: Fri, 05 Feb 2021 02:56:56 GMT  
		Size: 40.6 KB (40632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b103e735755feb4c5645f47747ca9fea69ae45b8c06246fb02270b985c38a3`  
		Last Modified: Fri, 05 Feb 2021 02:56:56 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c2c51a3613783db7da238cdfad394bf72a1775e9bdb05748a9450504a16389d`  
		Last Modified: Fri, 05 Feb 2021 02:57:46 GMT  
		Size: 15.5 MB (15549336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42df5f19d25d33743309402b78ea97fc0cfb8312715da3f8d55ba8b0dbb8bc16`  
		Last Modified: Fri, 05 Feb 2021 02:57:41 GMT  
		Size: 2.1 KB (2092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd6124f3f74469194c627f3c277054e2f25148daa1ccaee65b30def5a5c5b102`  
		Last Modified: Fri, 05 Feb 2021 02:57:41 GMT  
		Size: 1.6 KB (1633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-php8.0-fpm-alpine` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:10a4efe5437e61065da3e0292c9ac99160407af7bfc4658a164e79f9fd7f05af
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.5 MB (61451721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ab404c75a4595ee14eabc83c91445ffecb604a52fc97a126d563bfd6fe9fdf7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Fri, 29 Jan 2021 01:10:17 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 29 Jan 2021 01:10:18 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:10:19 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:10:20 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 01:10:20 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 05 Feb 2021 03:17:23 GMT
ENV PHP_VERSION=8.0.2
# Fri, 05 Feb 2021 03:17:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Fri, 05 Feb 2021 03:17:24 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Fri, 05 Feb 2021 03:17:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 05 Feb 2021 03:17:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 05 Feb 2021 03:20:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 05 Feb 2021 03:20:21 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 05 Feb 2021 03:20:24 GMT
RUN docker-php-ext-enable sodium
# Fri, 05 Feb 2021 03:20:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 05 Feb 2021 03:20:25 GMT
WORKDIR /var/www/html
# Fri, 05 Feb 2021 03:20:27 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 05 Feb 2021 03:20:27 GMT
STOPSIGNAL SIGQUIT
# Fri, 05 Feb 2021 03:20:28 GMT
EXPOSE 9000
# Fri, 05 Feb 2021 03:20:29 GMT
CMD ["php-fpm"]
# Fri, 05 Feb 2021 03:41:10 GMT
RUN set -eux; 	apk add --no-cache 		bash 		sed 		ghostscript 	;
# Fri, 05 Feb 2021 03:41:54 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 05 Feb 2021 03:41:57 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 05 Feb 2021 03:41:59 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 05 Feb 2021 03:45:02 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 05 Feb 2021 03:45:03 GMT
VOLUME [/var/www/html]
# Fri, 05 Feb 2021 03:45:03 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Fri, 05 Feb 2021 03:45:04 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Fri, 05 Feb 2021 03:45:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Feb 2021 03:45:06 GMT
CMD ["php-fpm"]
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
	-	`sha256:6292848217672dae9befaf41ccb502cc8b5f69b68bd5fa42c9458132b7b60737`  
		Last Modified: Fri, 05 Feb 2021 03:33:31 GMT  
		Size: 10.7 MB (10669920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca46eb8346588855aac504ceae48b77c533a6dc5f02f147bf94d8984e89c4f2`  
		Last Modified: Fri, 05 Feb 2021 03:33:28 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e8ed0a0bcb01b9a5fe6bdeef4c3a6416c83bb125c92a8ff0b196a0ed74465c`  
		Last Modified: Fri, 05 Feb 2021 03:33:32 GMT  
		Size: 12.8 MB (12791967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:614b67faa5e42ed405c629a8a999009d8cde999f5f4974895d5405483895ad20`  
		Last Modified: Fri, 05 Feb 2021 03:33:28 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7739abb1857d03001086779df1c5044514b31c433a20000eb537fb8655913e5f`  
		Last Modified: Fri, 05 Feb 2021 03:33:29 GMT  
		Size: 17.5 KB (17525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2dfb21df7e2a6bece0282ac43ac0e1c64bd314eb9429cc9b8fed275d9845ece`  
		Last Modified: Fri, 05 Feb 2021 03:33:28 GMT  
		Size: 8.6 KB (8573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1829c353239aa327feb59152ba59ef41c4466f5ba353f0fb19d0463dd8acfc72`  
		Last Modified: Fri, 05 Feb 2021 03:49:58 GMT  
		Size: 18.0 MB (18005675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b202c56989c4b8402c086951033e6fc293017af8f3c075de6f323efaad0f57e`  
		Last Modified: Fri, 05 Feb 2021 03:49:51 GMT  
		Size: 381.0 KB (381003 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adc16504c3b77523606d3c38022e6c4f12e8cd95a67ec77a4951d0c57827dd4c`  
		Last Modified: Fri, 05 Feb 2021 03:49:52 GMT  
		Size: 40.6 KB (40631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ccf2d705ef48d2d779c94b02b511225c883268b2dbc5711b0a0e910486f9989`  
		Last Modified: Fri, 05 Feb 2021 03:49:52 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4db95aed50dfc93da29ea023b46d3d85801d811064889c09ae6c1dbc2745e0fb`  
		Last Modified: Fri, 05 Feb 2021 03:51:45 GMT  
		Size: 15.5 MB (15549334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c260fa69a66dc370724b7b78e5a688ac06cd267ebabe57ba7e55a9ddd3909c1f`  
		Last Modified: Fri, 05 Feb 2021 03:51:39 GMT  
		Size: 2.1 KB (2092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb823a3d13d87a280bac7ffd7368caf2e677ed1acd4cb45db4f1c4caf5fac73`  
		Last Modified: Fri, 05 Feb 2021 03:51:40 GMT  
		Size: 1.6 KB (1632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-php8.0-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:383c4d1b8b98858d0d1c35f3e995047b53cd42a80ec29d10ec4f1e9fbb8b8bfb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.9 MB (64896684 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1b66d72394245b984e3baaf415da0b7d15162e40416ab51f779a125f802a14ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Fri, 29 Jan 2021 01:32:58 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 29 Jan 2021 01:32:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:33:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:33:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 01:33:01 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 05 Feb 2021 03:04:00 GMT
ENV PHP_VERSION=8.0.2
# Fri, 05 Feb 2021 03:04:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Fri, 05 Feb 2021 03:04:02 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Fri, 05 Feb 2021 03:04:10 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 05 Feb 2021 03:04:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 05 Feb 2021 03:08:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 05 Feb 2021 03:08:34 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 05 Feb 2021 03:08:38 GMT
RUN docker-php-ext-enable sodium
# Fri, 05 Feb 2021 03:08:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 05 Feb 2021 03:08:40 GMT
WORKDIR /var/www/html
# Fri, 05 Feb 2021 03:08:42 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 05 Feb 2021 03:08:43 GMT
STOPSIGNAL SIGQUIT
# Fri, 05 Feb 2021 03:08:45 GMT
EXPOSE 9000
# Fri, 05 Feb 2021 03:08:48 GMT
CMD ["php-fpm"]
# Fri, 05 Feb 2021 03:32:46 GMT
RUN set -eux; 	apk add --no-cache 		bash 		sed 		ghostscript 	;
# Fri, 05 Feb 2021 03:33:38 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 05 Feb 2021 03:33:41 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 05 Feb 2021 03:33:43 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 05 Feb 2021 03:36:38 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 05 Feb 2021 03:36:43 GMT
VOLUME [/var/www/html]
# Fri, 05 Feb 2021 03:36:43 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Fri, 05 Feb 2021 03:36:44 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Fri, 05 Feb 2021 03:36:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Feb 2021 03:36:46 GMT
CMD ["php-fpm"]
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
	-	`sha256:35893689924d67497e8332cba78ee30da688928960de78033b0dac4f7f2dc5b5`  
		Last Modified: Fri, 05 Feb 2021 03:23:33 GMT  
		Size: 10.7 MB (10669936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0e3b9ddc66e476714a1f49bc765dac3ab0a3ead34453a3930339477847b2684`  
		Last Modified: Fri, 05 Feb 2021 03:23:30 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e889be233e8088033b1e2b936d8b7974e8926ee9b8e66ffe64b78c5800853d39`  
		Last Modified: Fri, 05 Feb 2021 03:23:35 GMT  
		Size: 14.4 MB (14443499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18775aebd658b38cb25223664c4e1832d2cecdebde0224090770adc17a2a1ffe`  
		Last Modified: Fri, 05 Feb 2021 03:23:30 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3969b96dee3bc12df1e8999c1b94c5cd5e9d96923444463e8465a66939e19de7`  
		Last Modified: Fri, 05 Feb 2021 03:23:30 GMT  
		Size: 17.5 KB (17538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69e09c9792ccd55e8c799944099ed652d891f542f231429e229ada8a84743152`  
		Last Modified: Fri, 05 Feb 2021 03:23:31 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01afc429fcffddea3a4154e6978740173a46eb8edb541b27a534f48c8d34466f`  
		Last Modified: Fri, 05 Feb 2021 03:41:42 GMT  
		Size: 19.3 MB (19329943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1540edb1a28b828628d8ea71a8829aee7654617f734724ef9da514f3a5db76ee`  
		Last Modified: Fri, 05 Feb 2021 03:41:33 GMT  
		Size: 423.2 KB (423151 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1893e8ee358650a5603084b06fe4a4dc6344e2c62c7cf7008c28a1a4c4d45ed2`  
		Last Modified: Fri, 05 Feb 2021 03:41:33 GMT  
		Size: 40.5 KB (40472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:091ce824f80d0f10a16de483a225447db73751e45f9bc78487eadfbebfba9189`  
		Last Modified: Fri, 05 Feb 2021 03:41:33 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a9959abafaf77c360bed284312a98bebaa33d14251bafb6bf4d3e6d32bab5dd`  
		Last Modified: Fri, 05 Feb 2021 03:43:13 GMT  
		Size: 15.5 MB (15549332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3308cf6c865994e6a74603d0bd37eb58cae43281e43179bf88219ec9b33ebef`  
		Last Modified: Fri, 05 Feb 2021 03:43:07 GMT  
		Size: 2.1 KB (2093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03e9930b62b0f773b2960df5bdaada13a5b6aedc738ced73504c29c3a34349c`  
		Last Modified: Fri, 05 Feb 2021 03:43:07 GMT  
		Size: 1.6 KB (1633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-php8.0-fpm-alpine` - linux; 386

```console
$ docker pull wordpress@sha256:082d4b64c4f59c52f8bb04a3a9b604fea9d985e0f9799f0f2aff76a4d45f4a71
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.2 MB (66210927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:60f1d5de088c793f8c1cb13e632cd0482e5f64c6ebc52e5a953231f5205516cc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Fri, 29 Jan 2021 01:29:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 29 Jan 2021 01:29:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:29:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 01:29:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 01:29:32 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 05 Feb 2021 03:06:58 GMT
ENV PHP_VERSION=8.0.2
# Fri, 05 Feb 2021 03:06:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Fri, 05 Feb 2021 03:06:59 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Fri, 05 Feb 2021 03:07:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 05 Feb 2021 03:07:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 05 Feb 2021 03:19:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 05 Feb 2021 03:19:31 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 05 Feb 2021 03:19:32 GMT
RUN docker-php-ext-enable sodium
# Fri, 05 Feb 2021 03:19:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 05 Feb 2021 03:19:33 GMT
WORKDIR /var/www/html
# Fri, 05 Feb 2021 03:19:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 05 Feb 2021 03:19:34 GMT
STOPSIGNAL SIGQUIT
# Fri, 05 Feb 2021 03:19:34 GMT
EXPOSE 9000
# Fri, 05 Feb 2021 03:19:35 GMT
CMD ["php-fpm"]
# Fri, 05 Feb 2021 03:51:41 GMT
RUN set -eux; 	apk add --no-cache 		bash 		sed 		ghostscript 	;
# Fri, 05 Feb 2021 03:52:25 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 05 Feb 2021 03:52:26 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 05 Feb 2021 03:52:27 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 05 Feb 2021 03:55:03 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 05 Feb 2021 03:55:04 GMT
VOLUME [/var/www/html]
# Fri, 05 Feb 2021 03:55:04 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Fri, 05 Feb 2021 03:55:05 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Fri, 05 Feb 2021 03:55:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Feb 2021 03:55:05 GMT
CMD ["php-fpm"]
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
	-	`sha256:f2449685a69b001556e4eeffc50155461e4878ac3b549b23e0551d83c0af5184`  
		Last Modified: Fri, 05 Feb 2021 03:43:59 GMT  
		Size: 10.7 MB (10669886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebd925359669293f678ccb8827090e7df6609c283d75a3d1188be4eb5c34460`  
		Last Modified: Fri, 05 Feb 2021 03:43:56 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2cad5d0ede455bbb5cde2fc80ee78007c8fef314638bd16558cbbe043f291c6`  
		Last Modified: Fri, 05 Feb 2021 03:44:06 GMT  
		Size: 15.0 MB (15045226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5f2b5f92ceec2a1a747eddcf27d552eb5b0fd7fafb31920957f8cc5dac153e0`  
		Last Modified: Fri, 05 Feb 2021 03:43:56 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b543edce38217571acdc95717d613d79413d18168f14540af586f86c86c8ade`  
		Last Modified: Fri, 05 Feb 2021 03:43:56 GMT  
		Size: 17.5 KB (17508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cb89c47ec4dd8eefbaebe8dfc614a21f66d6539cad6bd163bfb22854801131`  
		Last Modified: Fri, 05 Feb 2021 03:43:56 GMT  
		Size: 8.6 KB (8569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dd45f0a373433a5abfaa85456a8b34a5dbeeb7782c09dfad6c9c4e6903be277`  
		Last Modified: Fri, 05 Feb 2021 04:00:44 GMT  
		Size: 19.8 MB (19802004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:252488996d0245e853733c1d2dfbf286349ee6ce11e7153a20aa897f06145d24`  
		Last Modified: Fri, 05 Feb 2021 04:00:37 GMT  
		Size: 458.6 KB (458578 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01f4173ff1ab48febcb3ebbd8dd648f92de53ad07d5f2a99ae5bdb2fc0a02ea0`  
		Last Modified: Fri, 05 Feb 2021 04:00:37 GMT  
		Size: 40.4 KB (40431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14f0e22089cea4c88bf1ba9130d81e659e2daccdc9b20fd453d57531d7a6f65f`  
		Last Modified: Fri, 05 Feb 2021 04:00:36 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b0b24e7459ab3ef1522eec7dad127c0d5a4146068eff188f7b8414000de2fc1`  
		Last Modified: Fri, 05 Feb 2021 04:02:24 GMT  
		Size: 15.5 MB (15549241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3effe83544da512fdfbc20d16818c1b948292bb3097b52cc111c7df78f91a74a`  
		Last Modified: Fri, 05 Feb 2021 04:02:15 GMT  
		Size: 2.1 KB (2095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2a4c937c3ab2bf60963ff9a5eeed09d0d0fd62581f31e467ec36d436256f04e`  
		Last Modified: Fri, 05 Feb 2021 04:02:15 GMT  
		Size: 1.6 KB (1633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-php8.0-fpm-alpine` - linux; ppc64le

```console
$ docker pull wordpress@sha256:ecee8e46b7dacc3782cc1d621f70a0b0217781f07296bcede4e15e9f2364e763
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.8 MB (66810009 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9fa4ab404d74a9e89fc3e5553b0254d6103a77c288bbcd7866f428595b86688`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Fri, 29 Jan 2021 00:54:04 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 29 Jan 2021 00:54:17 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:54:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:54:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 00:54:32 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 05 Feb 2021 11:01:08 GMT
ENV PHP_VERSION=8.0.2
# Fri, 05 Feb 2021 11:01:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Fri, 05 Feb 2021 11:01:25 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Fri, 05 Feb 2021 11:01:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 05 Feb 2021 11:01:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 05 Feb 2021 11:07:31 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 05 Feb 2021 11:07:37 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 05 Feb 2021 11:07:51 GMT
RUN docker-php-ext-enable sodium
# Fri, 05 Feb 2021 11:07:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 05 Feb 2021 11:08:06 GMT
WORKDIR /var/www/html
# Fri, 05 Feb 2021 11:08:16 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 05 Feb 2021 11:08:23 GMT
STOPSIGNAL SIGQUIT
# Fri, 05 Feb 2021 11:08:28 GMT
EXPOSE 9000
# Fri, 05 Feb 2021 11:08:33 GMT
CMD ["php-fpm"]
# Fri, 05 Feb 2021 11:43:31 GMT
RUN set -eux; 	apk add --no-cache 		bash 		sed 		ghostscript 	;
# Fri, 05 Feb 2021 11:44:25 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 05 Feb 2021 11:44:35 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 05 Feb 2021 11:44:50 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 05 Feb 2021 11:50:39 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 05 Feb 2021 11:50:44 GMT
VOLUME [/var/www/html]
# Fri, 05 Feb 2021 11:50:46 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Fri, 05 Feb 2021 11:50:47 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Fri, 05 Feb 2021 11:50:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Feb 2021 11:51:00 GMT
CMD ["php-fpm"]
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
	-	`sha256:97d463c6539adf19a7ac60a342dcd95bd07974e661bbd42ac3377d5626bb8765`  
		Last Modified: Fri, 05 Feb 2021 11:27:58 GMT  
		Size: 10.7 MB (10669915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b68301e231cbe0f7129b71356dcd3e8e6a3d1d34f9759d45b4e268b029e1dba`  
		Last Modified: Fri, 05 Feb 2021 11:27:53 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a72324c0e464662ac4ba15abb890a88740300b90472102042c5fb71dad89c924`  
		Last Modified: Fri, 05 Feb 2021 11:27:57 GMT  
		Size: 15.8 MB (15750644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2035a6ed59daf2ab44e021b542a409f3abcd41f8af4c8a3af3151d2843eca12c`  
		Last Modified: Fri, 05 Feb 2021 11:27:53 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b4c8d56a75c5c397849ddc529aeeb6fb5ff041bf7e4d08dab5b2073e6e9b7bf`  
		Last Modified: Fri, 05 Feb 2021 11:27:53 GMT  
		Size: 17.5 KB (17525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3477a39dd5c881b88cf21cd5da54f713171396115629adcaa69d66c1025bf287`  
		Last Modified: Fri, 05 Feb 2021 11:27:53 GMT  
		Size: 8.6 KB (8568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2791ff9ce5c049b539cd2377a4472c8312d9789dfb60b7aee54b57221ca7f484`  
		Last Modified: Fri, 05 Feb 2021 11:54:08 GMT  
		Size: 19.7 MB (19739024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca65b8bb5b88866670c57214e709bb588b255b958fa9ab2f654e3e1686e5abe`  
		Last Modified: Fri, 05 Feb 2021 11:54:00 GMT  
		Size: 471.8 KB (471832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ee9cfb10ff3efa937fb1a2e81cd1cc94ebde7e66b2ad9bb50ad4f87ea5abf19`  
		Last Modified: Fri, 05 Feb 2021 11:54:00 GMT  
		Size: 40.5 KB (40483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b86420d30694a5f54308260d56c9bb9fb6edc6e51e73408b7469af5c5305792`  
		Last Modified: Fri, 05 Feb 2021 11:54:00 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7206988a986f759b98409e293f78c528844ea40ef6f9fc1ce1597404f79ec1d`  
		Last Modified: Fri, 05 Feb 2021 11:56:04 GMT  
		Size: 15.5 MB (15549334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0660866278b33eccdce21b2154a938bee9ca745f694b5939fff02b22d4ab35`  
		Last Modified: Fri, 05 Feb 2021 11:56:01 GMT  
		Size: 2.1 KB (2094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7de48d24db626ff6bfa4c468e176ba9759e042d6020bb6b554b2ccca65727c6`  
		Last Modified: Fri, 05 Feb 2021 11:56:01 GMT  
		Size: 1.6 KB (1632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-php8.0-fpm-alpine` - linux; s390x

```console
$ docker pull wordpress@sha256:3b93127c09e8466dcde89b60067388346b5c09ebc05a7fb7d292e51caeadb392
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **64.7 MB (64738823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:130a66c648bf33cad974f27824c39d036b456d233ce652873eb435937dd89a76`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Fri, 29 Jan 2021 00:43:28 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 29 Jan 2021 00:43:28 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:43:29 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 29 Jan 2021 00:43:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 29 Jan 2021 00:43:30 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 05 Feb 2021 09:30:08 GMT
ENV PHP_VERSION=8.0.2
# Fri, 05 Feb 2021 09:30:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.2.tar.xz?a=1 PHP_ASC_URL=https://www.php.net/distributions/php-8.0.2.tar.xz.asc?a=1
# Fri, 05 Feb 2021 09:30:09 GMT
ENV PHP_SHA256=84dd6e36f48c3a71ff5dceba375c1f6b34b71d4fa9e06b720780127176468ccc
# Fri, 05 Feb 2021 09:30:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 05 Feb 2021 09:30:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 05 Feb 2021 09:38:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 05 Feb 2021 09:38:21 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 05 Feb 2021 09:38:29 GMT
RUN docker-php-ext-enable sodium
# Fri, 05 Feb 2021 09:38:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 05 Feb 2021 09:38:30 GMT
WORKDIR /var/www/html
# Fri, 05 Feb 2021 09:38:32 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 05 Feb 2021 09:38:32 GMT
STOPSIGNAL SIGQUIT
# Fri, 05 Feb 2021 09:38:33 GMT
EXPOSE 9000
# Fri, 05 Feb 2021 09:38:34 GMT
CMD ["php-fpm"]
# Fri, 05 Feb 2021 10:45:08 GMT
RUN set -eux; 	apk add --no-cache 		bash 		sed 		ghostscript 	;
# Fri, 05 Feb 2021 10:46:00 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 05 Feb 2021 10:46:02 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 05 Feb 2021 10:46:04 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 05 Feb 2021 10:49:30 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 05 Feb 2021 10:49:32 GMT
VOLUME [/var/www/html]
# Fri, 05 Feb 2021 10:49:32 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Fri, 05 Feb 2021 10:49:33 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Fri, 05 Feb 2021 10:49:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 05 Feb 2021 10:49:34 GMT
CMD ["php-fpm"]
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
	-	`sha256:fda00c02df65e979bd22bc4cd5e21ddf1360a6a18e310503f924887bfed1075f`  
		Last Modified: Fri, 05 Feb 2021 10:28:23 GMT  
		Size: 10.7 MB (10669924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f02b115d01411b044e0312d8e75e723720e7ce070b07826831c1ada6b356de`  
		Last Modified: Fri, 05 Feb 2021 10:28:06 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea39c45932b3d78a33510cf9cd6f33b50e18b0424a34b5f5cb908f26e17e9040`  
		Last Modified: Fri, 05 Feb 2021 10:28:10 GMT  
		Size: 14.0 MB (14035851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178a0e1294606b9bdc06c6556a5042f29cbbcc22ffbba50ed65cbdd4ad1af9e9`  
		Last Modified: Fri, 05 Feb 2021 10:28:10 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a8488d2cb44e19d2d5c6c1db7316b90cdb07a690ef43647cce2e90544ab0c47`  
		Last Modified: Fri, 05 Feb 2021 10:28:10 GMT  
		Size: 17.5 KB (17528 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edb12ff61c6c7f39a5fd411cbdfdf88206fbec605bef10ef81e72e7f98e4e0fe`  
		Last Modified: Fri, 05 Feb 2021 10:28:10 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a65b7a8767fbc6e2ce21d0cb260af0ec7734e997fb6e9441ffa18ad71d6aac`  
		Last Modified: Fri, 05 Feb 2021 11:03:04 GMT  
		Size: 19.6 MB (19618956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d35d24f7fa1e376288fd5492cf9c7b66ec0e45172f1811d5a60c819570ce2eb`  
		Last Modified: Fri, 05 Feb 2021 11:02:34 GMT  
		Size: 431.4 KB (431390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccba9544edf5c92033505fc7b3f6bb263749e7d4d6fcfb010e5b184c117d8762`  
		Last Modified: Fri, 05 Feb 2021 11:02:34 GMT  
		Size: 40.5 KB (40465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26cbc8dc36938be05495e328c9aea89fee50b06de4c3b9d0b83a6ebcda11c8da`  
		Last Modified: Fri, 05 Feb 2021 11:02:34 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb706c4a9128d1978a6f1b3a7f2e83306d65d8b76e120e3cf9a6fbcd0f64c147`  
		Last Modified: Fri, 05 Feb 2021 11:19:37 GMT  
		Size: 15.5 MB (15549334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1b11d85b5e2692f940c4e1f0677fb3081f80bdfdc79520ca29dbc857edb38d7`  
		Last Modified: Fri, 05 Feb 2021 11:19:37 GMT  
		Size: 2.1 KB (2091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5267c33ccc3a3e5e5a1df1ed6cc2ef860273e79d71900491cb7f542d73c73868`  
		Last Modified: Fri, 05 Feb 2021 11:19:37 GMT  
		Size: 1.6 KB (1632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
