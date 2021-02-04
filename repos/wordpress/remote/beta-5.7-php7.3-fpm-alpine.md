## `wordpress:beta-5.7-php7.3-fpm-alpine`

```console
$ docker pull wordpress@sha256:e38d93dd8565456c185f891cee3b0476ee7dea7a48b9bc31ec0ea4620d6a34f5
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

### `wordpress:beta-5.7-php7.3-fpm-alpine` - linux; amd64

```console
$ docker pull wordpress@sha256:a35300b74e9ce053c3e77a0bc68290cfa21987775d55e421f4df8341cb59d69f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.1 MB (83133513 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd35e61c43e4770ba93fc94c7606152247e223c8524fc03708a7c4458d144f90`
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
# Fri, 29 Jan 2021 02:21:25 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 29 Jan 2021 02:21:25 GMT
ENV PHP_VERSION=7.3.26
# Fri, 29 Jan 2021 02:21:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.26.tar.xz.asc
# Fri, 29 Jan 2021 02:21:25 GMT
ENV PHP_SHA256=d93052f4cb2882090b6a37fd1e0c764be1605a2461152b7f6b8f04fa48875208
# Fri, 29 Jan 2021 02:21:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 29 Jan 2021 02:21:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 29 Jan 2021 02:33:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 29 Jan 2021 02:33:39 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 29 Jan 2021 02:33:40 GMT
RUN docker-php-ext-enable sodium
# Fri, 29 Jan 2021 02:33:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 29 Jan 2021 02:33:41 GMT
WORKDIR /var/www/html
# Fri, 29 Jan 2021 02:33:42 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 29 Jan 2021 02:33:42 GMT
STOPSIGNAL SIGQUIT
# Fri, 29 Jan 2021 02:33:42 GMT
EXPOSE 9000
# Fri, 29 Jan 2021 02:33:42 GMT
CMD ["php-fpm"]
# Fri, 29 Jan 2021 04:51:39 GMT
RUN set -eux; 	apk add --no-cache 		bash 		sed 		ghostscript 		imagemagick 	;
# Fri, 29 Jan 2021 04:52:35 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 29 Jan 2021 04:52:37 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 29 Jan 2021 04:52:38 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 03 Feb 2021 21:41:32 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Wed, 03 Feb 2021 21:41:32 GMT
VOLUME [/var/www/html]
# Wed, 03 Feb 2021 21:41:32 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Wed, 03 Feb 2021 21:41:33 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Wed, 03 Feb 2021 21:41:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Feb 2021 21:41:33 GMT
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
	-	`sha256:31735e307a740bf9468ca943cd5f28030fa18652c8dc282337239eb28aa1e548`  
		Last Modified: Fri, 29 Jan 2021 02:52:57 GMT  
		Size: 12.2 MB (12157910 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:846066245b44a011033d53ad4e884093c9fbf6163543fb7ff9184d64608df486`  
		Last Modified: Fri, 29 Jan 2021 02:52:54 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69dc481aefeb58d9644d6080f2958116af1378ac7f92987e17be29cea986b374`  
		Last Modified: Fri, 29 Jan 2021 02:52:59 GMT  
		Size: 14.5 MB (14526431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b96aa96c4504c31c6eee1e9f38a1857f4d0684e11e3b0b261020a3757e48e23`  
		Last Modified: Fri, 29 Jan 2021 02:52:54 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c4acdbf93ef5b40d66b47d928719605e40f66bee3a5dd246f5db84504d2b651`  
		Last Modified: Fri, 29 Jan 2021 02:52:54 GMT  
		Size: 17.3 KB (17335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b1f7bd61506e200fd102145294ac7d914317580995f4db3bad54045d7f087e0`  
		Last Modified: Fri, 29 Jan 2021 02:52:54 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:212da5e462e6b92ef23ebea0d3f65d9a0d919ad446da9d95f433d9e0c75ff86a`  
		Last Modified: Fri, 29 Jan 2021 05:03:33 GMT  
		Size: 35.0 MB (34976298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd68a83c76cd5c7cd5ff76a32708617774b18a81aeb74d07c4ccf90e53faf5fc`  
		Last Modified: Fri, 29 Jan 2021 05:03:26 GMT  
		Size: 1.3 MB (1320177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba00cf1e79a9fcdb8b6f3f89487c1f2a37607bc317a87dd44c9dd9d800727393`  
		Last Modified: Fri, 29 Jan 2021 05:03:26 GMT  
		Size: 63.2 KB (63198 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11b30c31fc5e4193a96c07b0260dcc0e93ad6a5f2e664b0c14b01893ea7f0e5`  
		Last Modified: Fri, 29 Jan 2021 05:03:26 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fdb0d1c1e1c1f210745541c48d8307ce9c5bcaa595b3b8b138aa76d547ebaf1`  
		Last Modified: Wed, 03 Feb 2021 21:45:35 GMT  
		Size: 15.5 MB (15549247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db51f81eddd8041d7611db246e65181ddde9aced139b46ff841c444b5e14cab`  
		Last Modified: Wed, 03 Feb 2021 21:45:31 GMT  
		Size: 2.1 KB (2095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a91fc6bd9ec16af31086542754666b521526924fffa92f61a2342b5f9640a773`  
		Last Modified: Wed, 03 Feb 2021 21:45:32 GMT  
		Size: 1.6 KB (1636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-5.7-php7.3-fpm-alpine` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:4224fd14b9ec3f84c6280116d7ffe0d5c3f8d61682be1e64e59f3df548eaa6ae
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **79.5 MB (79524909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:971a905b54d1fa2cf258ebf9f3fbc1a43c4fec45e285193a864e69e5ae983216`
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
# Fri, 29 Jan 2021 00:56:32 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 04 Feb 2021 18:33:59 GMT
ENV PHP_VERSION=7.3.27
# Thu, 04 Feb 2021 18:34:00 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.27.tar.xz.asc
# Thu, 04 Feb 2021 18:34:01 GMT
ENV PHP_SHA256=65f616e2d5b6faacedf62830fa047951b0136d5da34ae59e6744cbaf5dca148d
# Thu, 04 Feb 2021 18:34:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 04 Feb 2021 18:34:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Feb 2021 18:37:24 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Feb 2021 18:37:27 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 04 Feb 2021 18:37:32 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Feb 2021 18:37:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Feb 2021 18:37:35 GMT
WORKDIR /var/www/html
# Thu, 04 Feb 2021 18:37:37 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 04 Feb 2021 18:37:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 Feb 2021 18:37:39 GMT
EXPOSE 9000
# Thu, 04 Feb 2021 18:37:39 GMT
CMD ["php-fpm"]
# Thu, 04 Feb 2021 20:31:05 GMT
RUN set -eux; 	apk add --no-cache 		bash 		sed 		ghostscript 		imagemagick 	;
# Thu, 04 Feb 2021 20:32:27 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 04 Feb 2021 20:32:30 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 04 Feb 2021 20:32:33 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 04 Feb 2021 20:37:45 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 04 Feb 2021 20:37:47 GMT
VOLUME [/var/www/html]
# Thu, 04 Feb 2021 20:37:48 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Thu, 04 Feb 2021 20:37:49 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Thu, 04 Feb 2021 20:37:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Feb 2021 20:37:52 GMT
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
	-	`sha256:af39b4faf4d9e1d5b7aeda5aa8aead295ce03dce8a9626b7de38095c0a6aca9c`  
		Last Modified: Thu, 04 Feb 2021 18:57:33 GMT  
		Size: 12.2 MB (12157786 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e6fa365ddc759fff47b1bbcc029aaedf78adef8ea7568e01f953273f54124c`  
		Last Modified: Thu, 04 Feb 2021 18:57:30 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a82c7f5cd0b9bf6559cbb2383663eb1fd2f9acdfc499bfc97f619a0ce05ec386`  
		Last Modified: Thu, 04 Feb 2021 18:57:35 GMT  
		Size: 13.5 MB (13457857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baa2bd29f99fece9a75f24f03cb1c6aed9be52ac6e3411d25584e9c4dad19d63`  
		Last Modified: Thu, 04 Feb 2021 18:57:30 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4395a33f821ad55704b0168c0dc5ddcbfc972248302d84e3c7b1bfa8c0a4286`  
		Last Modified: Thu, 04 Feb 2021 18:57:30 GMT  
		Size: 17.3 KB (17343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d240c3eca5c4ae02078cc2b9b65130a4764c1cf0fd057704930d978c935cb7c2`  
		Last Modified: Thu, 04 Feb 2021 18:57:30 GMT  
		Size: 8.4 KB (8414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc76347138de40f2a0393a526d9c1d018097f83a9b63bdddeec13e365829b3df`  
		Last Modified: Thu, 04 Feb 2021 20:39:37 GMT  
		Size: 32.7 MB (32707045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b3cecba1723a93256f99ce576cf6f40f08439ff1081b24c868a89dc2c68e775`  
		Last Modified: Thu, 04 Feb 2021 20:39:24 GMT  
		Size: 1.2 MB (1248796 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:255b4d3dc99d9b758813d92d2a1a01dae07796dfa7ef7e3c3d5e2a1f668d07fe`  
		Last Modified: Thu, 04 Feb 2021 20:39:24 GMT  
		Size: 63.3 KB (63296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e542fb7c85391bc0fa9790ccc18ff4771e35318abdd5c5bd93b5b4f5566341fa`  
		Last Modified: Thu, 04 Feb 2021 20:39:24 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca35acf990f16853a3d760755d88c31ac2491c0e7467cd01b62e1fbbeca7c7c`  
		Last Modified: Thu, 04 Feb 2021 20:41:00 GMT  
		Size: 15.5 MB (15549348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19cda2907f962ee0463a09cda96e1165780bc25c5cfc77b3e94756b5d6e7dbe2`  
		Last Modified: Thu, 04 Feb 2021 20:40:54 GMT  
		Size: 2.1 KB (2092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:473df421342b426740003914be1c0b78847af2471ff5a0252a622aeb457985be`  
		Last Modified: Thu, 04 Feb 2021 20:40:55 GMT  
		Size: 1.6 KB (1633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-5.7-php7.3-fpm-alpine` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:b29004f30cb8f8a6f956baf77bc0bb7bd2fa67b541f16f7a2b57452ec46aabd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.6 MB (76648228 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:704c0a2b32b551bed90698d3e07ea06916ffd77cb9c47738fd174fff55689ca7`
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
# Fri, 29 Jan 2021 01:31:18 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 29 Jan 2021 01:31:20 GMT
ENV PHP_VERSION=7.3.26
# Fri, 29 Jan 2021 01:31:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.26.tar.xz.asc
# Fri, 29 Jan 2021 01:31:22 GMT
ENV PHP_SHA256=d93052f4cb2882090b6a37fd1e0c764be1605a2461152b7f6b8f04fa48875208
# Fri, 29 Jan 2021 01:31:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 29 Jan 2021 01:31:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:34:49 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 29 Jan 2021 01:34:51 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:34:56 GMT
RUN docker-php-ext-enable sodium
# Fri, 29 Jan 2021 01:34:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 29 Jan 2021 01:34:58 GMT
WORKDIR /var/www/html
# Fri, 29 Jan 2021 01:35:00 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 29 Jan 2021 01:35:01 GMT
STOPSIGNAL SIGQUIT
# Fri, 29 Jan 2021 01:35:02 GMT
EXPOSE 9000
# Fri, 29 Jan 2021 01:35:03 GMT
CMD ["php-fpm"]
# Fri, 29 Jan 2021 03:03:54 GMT
RUN set -eux; 	apk add --no-cache 		bash 		sed 		ghostscript 		imagemagick 	;
# Fri, 29 Jan 2021 03:05:23 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 29 Jan 2021 03:05:26 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 29 Jan 2021 03:05:28 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 03 Feb 2021 22:54:52 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Wed, 03 Feb 2021 22:54:54 GMT
VOLUME [/var/www/html]
# Wed, 03 Feb 2021 22:54:55 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Wed, 03 Feb 2021 22:54:56 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Wed, 03 Feb 2021 22:54:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Feb 2021 22:54:58 GMT
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
	-	`sha256:f615af94e773a9a50b570d6ca168f99e319a4646ecc47b9c609088603cd269d3`  
		Last Modified: Fri, 29 Jan 2021 01:45:43 GMT  
		Size: 12.2 MB (12157924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d39a1cc374168e9a87d6d81bee68cc1155ebb7ea5e914de9b799e11f6d1802e`  
		Last Modified: Fri, 29 Jan 2021 01:45:37 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:183a8fd88e7c3df306e14bf163ce625c2ffed76880efef8a185266ad471375cd`  
		Last Modified: Fri, 29 Jan 2021 01:45:41 GMT  
		Size: 12.6 MB (12598593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9a1da2403e4f61ff31676ce6f5f31fc05f37150d469623b1de4f064a25df51`  
		Last Modified: Fri, 29 Jan 2021 01:45:37 GMT  
		Size: 2.3 KB (2264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44288adff087d6059efd313c5f34aea31becac772986b4e35198e421ae60d185`  
		Last Modified: Fri, 29 Jan 2021 01:45:37 GMT  
		Size: 17.3 KB (17328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb8b1be31980fe3004ba1a0af8835bf8e14119c3c88894efe2722b9949b34098`  
		Last Modified: Fri, 29 Jan 2021 01:45:37 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb574259f0aed56f2cb4320677476e96c35297150c38f6a0d029f6beaa112dc2`  
		Last Modified: Fri, 29 Jan 2021 03:18:58 GMT  
		Size: 31.0 MB (31043192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fa65628d8c198928c903b1ab06011832f02353e79e8f07eae9b409ce5007f9`  
		Last Modified: Fri, 29 Jan 2021 03:18:38 GMT  
		Size: 1.2 MB (1223038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a776318f2f8f5a6032e42c36587efc635e1720ed67e8ac2ce099bffe532793`  
		Last Modified: Fri, 29 Jan 2021 03:18:38 GMT  
		Size: 63.3 KB (63302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58151c1c969dc24526138be15d61472ae6db04afdc158707ea7990eceec0ae62`  
		Last Modified: Fri, 29 Jan 2021 03:18:38 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50aca44c147c090619692fd76af3fa9546cf88ef57c3aba18e6b71f9a0e10e8e`  
		Last Modified: Wed, 03 Feb 2021 23:00:11 GMT  
		Size: 15.5 MB (15549342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7b68bf87ce35ff5f59c306925dadcf298f27f0c45ab34489365fe3e9506e022`  
		Last Modified: Wed, 03 Feb 2021 23:00:05 GMT  
		Size: 2.1 KB (2093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6762e688bd8f7df0466c2888389b151f7b28a1b226c38de77b4307efbbfad29f`  
		Last Modified: Wed, 03 Feb 2021 23:00:05 GMT  
		Size: 1.6 KB (1635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-5.7-php7.3-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:95cbbbbcc9a38e25721e7bc851a51e9c34ab8a59f3c31afa24955abed8470ec5
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81278167 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1fecd97adeea87810db243d8dee2e3013ba497c50f22fa4a8b71acd6de601cd7`
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
# Fri, 29 Jan 2021 01:58:00 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 04 Feb 2021 19:09:53 GMT
ENV PHP_VERSION=7.3.27
# Thu, 04 Feb 2021 19:09:53 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.27.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.27.tar.xz.asc
# Thu, 04 Feb 2021 19:09:54 GMT
ENV PHP_SHA256=65f616e2d5b6faacedf62830fa047951b0136d5da34ae59e6744cbaf5dca148d
# Thu, 04 Feb 2021 19:09:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 04 Feb 2021 19:10:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 04 Feb 2021 19:13:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 04 Feb 2021 19:13:29 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 04 Feb 2021 19:13:35 GMT
RUN docker-php-ext-enable sodium
# Thu, 04 Feb 2021 19:13:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 04 Feb 2021 19:13:37 GMT
WORKDIR /var/www/html
# Thu, 04 Feb 2021 19:13:42 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 04 Feb 2021 19:13:44 GMT
STOPSIGNAL SIGQUIT
# Thu, 04 Feb 2021 19:13:45 GMT
EXPOSE 9000
# Thu, 04 Feb 2021 19:13:46 GMT
CMD ["php-fpm"]
# Thu, 04 Feb 2021 21:21:23 GMT
RUN set -eux; 	apk add --no-cache 		bash 		sed 		ghostscript 		imagemagick 	;
# Thu, 04 Feb 2021 21:23:03 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Thu, 04 Feb 2021 21:23:09 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 04 Feb 2021 21:23:12 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 04 Feb 2021 21:30:02 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 04 Feb 2021 21:30:06 GMT
VOLUME [/var/www/html]
# Thu, 04 Feb 2021 21:30:06 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Thu, 04 Feb 2021 21:30:07 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Thu, 04 Feb 2021 21:30:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 04 Feb 2021 21:30:10 GMT
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
	-	`sha256:4fda008c38df05a28ad4e2510bbf3cca9412324c9a53c461025e22cde9f1e193`  
		Last Modified: Thu, 04 Feb 2021 19:38:24 GMT  
		Size: 12.2 MB (12157804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8a70125a5c67de5206d6ea81311f63e37d8747f7f15a2e9b919ed2bed61f85`  
		Last Modified: Thu, 04 Feb 2021 19:38:22 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eeaac4b4cface6d46c8fad2f649941baf84094386b7ebfecd61b1eab27abac1`  
		Last Modified: Thu, 04 Feb 2021 19:38:25 GMT  
		Size: 14.2 MB (14215196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7439c088d755adc2ee428818499fd3970fc7f34066378eb85f51d92d264782`  
		Last Modified: Thu, 04 Feb 2021 19:38:22 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9656d07cd6b03f4b041a9c6de96e5413234f850b99aaef1701a63b1536422bb8`  
		Last Modified: Thu, 04 Feb 2021 19:38:22 GMT  
		Size: 17.4 KB (17351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abb73e1baa966c1e36a4288dc958cdd8e9ba18221fa46d63c9e28f1aef376072`  
		Last Modified: Thu, 04 Feb 2021 19:38:22 GMT  
		Size: 8.4 KB (8407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e8c70376ab79a76d456e7466ecd40e075c78525a2587797e5a9f493314c7f8`  
		Last Modified: Thu, 04 Feb 2021 21:35:02 GMT  
		Size: 33.6 MB (33566458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7d4c6aa870ffa6f51ad1f3addf48cce4eecafcfc2814dc487e9dbeef828eed6`  
		Last Modified: Thu, 04 Feb 2021 21:34:51 GMT  
		Size: 1.3 MB (1286131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d8a378dd493c90b639ef0ac215b765bf914b3d46fae9ed83584f980e77a3c2d`  
		Last Modified: Thu, 04 Feb 2021 21:34:51 GMT  
		Size: 63.2 KB (63243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c44a3594829b1d7b5d72d97c3c67eae53f148e621681b49df799ad7ee637a69e`  
		Last Modified: Thu, 04 Feb 2021 21:34:51 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:824f35de186e1816273f05fe01c60b332e75fe066e8826f2721e3dcff79be6a9`  
		Last Modified: Thu, 04 Feb 2021 21:38:00 GMT  
		Size: 15.5 MB (15549333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfe7c9f8b90cd3a6c289d1c07145fd262f5e108db9820e514c0b4b8f22185a8f`  
		Last Modified: Thu, 04 Feb 2021 21:37:56 GMT  
		Size: 2.1 KB (2091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bdd9fb020965f2c9153d0ee691bef789b3ab934849291f49762ee8b390ea9f3`  
		Last Modified: Thu, 04 Feb 2021 21:37:56 GMT  
		Size: 1.6 KB (1635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-5.7-php7.3-fpm-alpine` - linux; 386

```console
$ docker pull wordpress@sha256:ef343a85cdc89d1d18d7c4222660823b4191f4e54acf5fb589542b767379f3de
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **83.8 MB (83830672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93c8198839d9e10d2316bc050dcdd0fc8726172ed0d034e1f21f79586a84d496`
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
# Fri, 29 Jan 2021 02:33:35 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 29 Jan 2021 02:33:35 GMT
ENV PHP_VERSION=7.3.26
# Fri, 29 Jan 2021 02:33:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.26.tar.xz.asc
# Fri, 29 Jan 2021 02:33:36 GMT
ENV PHP_SHA256=d93052f4cb2882090b6a37fd1e0c764be1605a2461152b7f6b8f04fa48875208
# Fri, 29 Jan 2021 02:33:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 29 Jan 2021 02:33:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 29 Jan 2021 02:46:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 29 Jan 2021 02:46:34 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 29 Jan 2021 02:46:36 GMT
RUN docker-php-ext-enable sodium
# Fri, 29 Jan 2021 02:46:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 29 Jan 2021 02:46:36 GMT
WORKDIR /var/www/html
# Fri, 29 Jan 2021 02:46:37 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 29 Jan 2021 02:46:37 GMT
STOPSIGNAL SIGQUIT
# Fri, 29 Jan 2021 02:46:38 GMT
EXPOSE 9000
# Fri, 29 Jan 2021 02:46:38 GMT
CMD ["php-fpm"]
# Fri, 29 Jan 2021 04:52:46 GMT
RUN set -eux; 	apk add --no-cache 		bash 		sed 		ghostscript 		imagemagick 	;
# Fri, 29 Jan 2021 04:53:54 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 29 Jan 2021 04:53:56 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 29 Jan 2021 04:53:57 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 03 Feb 2021 19:52:12 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Wed, 03 Feb 2021 19:52:12 GMT
VOLUME [/var/www/html]
# Wed, 03 Feb 2021 19:52:12 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Wed, 03 Feb 2021 19:52:12 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Wed, 03 Feb 2021 19:52:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Feb 2021 19:52:13 GMT
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
	-	`sha256:66487efb43a17f6f08597f83995b26be55c853f7c039cfcb270d73983ae597c7`  
		Last Modified: Fri, 29 Jan 2021 03:02:49 GMT  
		Size: 12.2 MB (12157897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37745acac3ded70514d82a83756c0044577977b15936b0070957cf299ccaca17`  
		Last Modified: Fri, 29 Jan 2021 03:02:44 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e283ee05b16869a5b80718d8916d4fda3baca2df611b60e258861e178a3ea27`  
		Last Modified: Fri, 29 Jan 2021 03:02:54 GMT  
		Size: 14.9 MB (14851426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75c30936c1109a9f392966ac77cf8e892b59675a28f358b3ffd7e6f6dc6819f2`  
		Last Modified: Fri, 29 Jan 2021 03:02:44 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a876d50fe789da08e5a231424a3bf40fe45c8cee7898c964327d75e0c9af159`  
		Last Modified: Fri, 29 Jan 2021 03:02:44 GMT  
		Size: 17.3 KB (17330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a496e4d63a02d9432eef4f07d24d702f197e4bd2166a5c496bf48bdd244290`  
		Last Modified: Fri, 29 Jan 2021 03:02:44 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8912f889d1650cc48e86f18a0b96f64773710d678d0d524bca65109c161eb8c8`  
		Last Modified: Fri, 29 Jan 2021 05:05:14 GMT  
		Size: 35.2 MB (35241630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df979e08c5352da1286a71843028aee1a4187d8a6c9163a364e2ff327a0a6bb`  
		Last Modified: Fri, 29 Jan 2021 05:05:02 GMT  
		Size: 1.3 MB (1322051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722ddf9c098cbf09827add178ff94a21a6d59e244340a22cd9d17e0a09a9bec3`  
		Last Modified: Fri, 29 Jan 2021 05:05:02 GMT  
		Size: 63.2 KB (63187 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba6b0c3d40f236e5fc1d56b7014e1915958c1d3edaf249aaa459a246f4c7b205`  
		Last Modified: Fri, 29 Jan 2021 05:05:02 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd912513f8bc8da4b597143ed11501ea2291d6b13672c520bf6e6e1912011cbc`  
		Last Modified: Wed, 03 Feb 2021 19:56:36 GMT  
		Size: 15.5 MB (15549248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e303a4a21360a38f3898d5dde84ec0ddd5dc944f36a8200602395bfbf521e3`  
		Last Modified: Wed, 03 Feb 2021 19:56:29 GMT  
		Size: 2.1 KB (2092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7609ed3b4f6baa9622e78b3ee4321f146698c04fa8dccec62cabcea9acff6765`  
		Last Modified: Wed, 03 Feb 2021 19:56:30 GMT  
		Size: 1.6 KB (1639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-5.7-php7.3-fpm-alpine` - linux; ppc64le

```console
$ docker pull wordpress@sha256:fde001975b3cb4b8f83d1a491d4673f62d1e90bdd5305789d3318a37f6b45ccd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.5 MB (84542135 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19714a0d530c0ce4f111314eb2c01c50df150fecd2ebe37ae11b6092bbf49406`
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
# Fri, 29 Jan 2021 01:28:14 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 29 Jan 2021 01:28:22 GMT
ENV PHP_VERSION=7.3.26
# Fri, 29 Jan 2021 01:28:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.26.tar.xz.asc
# Fri, 29 Jan 2021 01:28:33 GMT
ENV PHP_SHA256=d93052f4cb2882090b6a37fd1e0c764be1605a2461152b7f6b8f04fa48875208
# Fri, 29 Jan 2021 01:28:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 29 Jan 2021 01:28:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:33:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 29 Jan 2021 01:33:27 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:33:41 GMT
RUN docker-php-ext-enable sodium
# Fri, 29 Jan 2021 01:33:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 29 Jan 2021 01:33:53 GMT
WORKDIR /var/www/html
# Fri, 29 Jan 2021 01:34:06 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 29 Jan 2021 01:34:10 GMT
STOPSIGNAL SIGQUIT
# Fri, 29 Jan 2021 01:34:17 GMT
EXPOSE 9000
# Fri, 29 Jan 2021 01:34:23 GMT
CMD ["php-fpm"]
# Fri, 29 Jan 2021 05:10:31 GMT
RUN set -eux; 	apk add --no-cache 		bash 		sed 		ghostscript 		imagemagick 	;
# Fri, 29 Jan 2021 05:12:10 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 29 Jan 2021 05:12:33 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 29 Jan 2021 05:12:52 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 03 Feb 2021 22:20:13 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Wed, 03 Feb 2021 22:20:20 GMT
VOLUME [/var/www/html]
# Wed, 03 Feb 2021 22:20:23 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Wed, 03 Feb 2021 22:20:24 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Wed, 03 Feb 2021 22:20:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Feb 2021 22:20:36 GMT
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
	-	`sha256:97f7e73031a5aa140cfea6e33c0af9c5ebc01f082f8de555092069a4a5cd84bb`  
		Last Modified: Fri, 29 Jan 2021 01:47:25 GMT  
		Size: 12.2 MB (12157924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94595185fc3b5b3b42a0e9adb70dbf823f4f8f0dc8da487b07ca23dc68fe8e4`  
		Last Modified: Fri, 29 Jan 2021 01:47:20 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc9845277c6ba8f1ba8018fe78a1c8e8cdbc0a63c270bc4908ff9e0427774f59`  
		Last Modified: Fri, 29 Jan 2021 01:47:24 GMT  
		Size: 15.6 MB (15594831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be62ef3f77248dfec0e96b022d381a8d3852793c168b40721011c14ffcc9183f`  
		Last Modified: Fri, 29 Jan 2021 01:47:20 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075ed36dd06d0eb919d70b526c117359170a920e9897c0b034300c1d64564946`  
		Last Modified: Fri, 29 Jan 2021 01:47:20 GMT  
		Size: 17.3 KB (17331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:540fbd5478fd7a3c81ed54683ab56199f03fa6b2807e5d38e2db231ff87e2c84`  
		Last Modified: Fri, 29 Jan 2021 01:47:20 GMT  
		Size: 8.4 KB (8411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdbe18dc561704e3fb518bb79693600bc17e15c0182d2cd969bc27028c36fdb9`  
		Last Modified: Fri, 29 Jan 2021 05:45:34 GMT  
		Size: 35.2 MB (35236541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6b5ca27406c46b623e80df6c94837608efa54a70faf191ada17e95a805ba01`  
		Last Modified: Fri, 29 Jan 2021 05:45:22 GMT  
		Size: 1.4 MB (1351817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6086171d7aecc3c5ebc91dc966000e34718d2aace3c1578ebe9fae5bff65916`  
		Last Modified: Fri, 29 Jan 2021 05:45:22 GMT  
		Size: 63.2 KB (63250 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8baa2881e77b8b073f2aaf5b7daa8a303e3710ded726d48df9c46b6c7873f4b0`  
		Last Modified: Fri, 29 Jan 2021 05:45:21 GMT  
		Size: 396.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357974d7d15e7303958a5eda5f1e1b39515e8703e2053e405bdd51bfd03255d1`  
		Last Modified: Wed, 03 Feb 2021 22:29:11 GMT  
		Size: 15.5 MB (15549340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c172cda008a68e555a0e8aeec99dabc4422400764d5b294a3927b53b86d77f92`  
		Last Modified: Wed, 03 Feb 2021 22:29:07 GMT  
		Size: 2.1 KB (2093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6da773d40aa7fbffcf8d252902318e9a81ca57e041f80077d72ceaee9cb32873`  
		Last Modified: Wed, 03 Feb 2021 22:29:07 GMT  
		Size: 1.6 KB (1637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:beta-5.7-php7.3-fpm-alpine` - linux; s390x

```console
$ docker pull wordpress@sha256:caba82ce457708f921262fc0d79afd819948fb34f9833f735559de198d0108c3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73540100 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:09667b65e5673ca39249815a0cc3f1d628e116b52d39496941fd7655f9a0a02f`
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
# Fri, 29 Jan 2021 01:08:02 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 29 Jan 2021 01:08:03 GMT
ENV PHP_VERSION=7.3.26
# Fri, 29 Jan 2021 01:08:03 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.26.tar.xz.asc
# Fri, 29 Jan 2021 01:08:04 GMT
ENV PHP_SHA256=d93052f4cb2882090b6a37fd1e0c764be1605a2461152b7f6b8f04fa48875208
# Fri, 29 Jan 2021 01:08:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 29 Jan 2021 01:08:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:12:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 29 Jan 2021 01:12:23 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 29 Jan 2021 01:12:24 GMT
RUN docker-php-ext-enable sodium
# Fri, 29 Jan 2021 01:12:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 29 Jan 2021 01:12:25 GMT
WORKDIR /var/www/html
# Fri, 29 Jan 2021 01:12:27 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 29 Jan 2021 01:12:27 GMT
STOPSIGNAL SIGQUIT
# Fri, 29 Jan 2021 01:12:28 GMT
EXPOSE 9000
# Fri, 29 Jan 2021 01:12:28 GMT
CMD ["php-fpm"]
# Fri, 29 Jan 2021 03:06:54 GMT
RUN set -eux; 	apk add --no-cache 		bash 		sed 		ghostscript 		imagemagick 	;
# Fri, 29 Jan 2021 03:07:53 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps
# Fri, 29 Jan 2021 03:07:55 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 29 Jan 2021 03:07:56 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 03 Feb 2021 20:21:02 GMT
RUN set -eux; 	version='5.7-beta1'; 	sha1='abff1a094f816136e9a5c2da0ba7b2e188fb304d'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Wed, 03 Feb 2021 20:21:04 GMT
VOLUME [/var/www/html]
# Wed, 03 Feb 2021 20:21:04 GMT
COPY --chown=www-data:www-datafile:0c72cdf4bfc53e48a50a27b4181a810916f30eb16f37044bd4298ee8328646d5 in /usr/src/wordpress/ 
# Wed, 03 Feb 2021 20:21:04 GMT
COPY file:eb627edb8cc2c73847c3ec2586b852ebd606f4562928fd73ce4c5efc0763085d in /usr/local/bin/ 
# Wed, 03 Feb 2021 20:21:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Feb 2021 20:21:05 GMT
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
	-	`sha256:023648cca599fa2e0a0ff96179dbb6c2f8868b842cd1da2d10fdad94fb14986d`  
		Last Modified: Fri, 29 Jan 2021 01:23:24 GMT  
		Size: 12.2 MB (12157927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96a4a3e2e139c21df13fa1887bdea9eb6b2a9919be1998dc923da0fa6ef3dad8`  
		Last Modified: Fri, 29 Jan 2021 01:23:22 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b22944a464c968d2e3d2f241ff114c06da147ce7672749caee40e8c9efe3803`  
		Last Modified: Fri, 29 Jan 2021 01:23:26 GMT  
		Size: 13.9 MB (13900928 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c61caa4c4f4e0d9b8ae930cf004c0a3346a897698eb08f12a6b629dfa723a15`  
		Last Modified: Fri, 29 Jan 2021 01:23:22 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ffb78a35ac7103190a1eb3938ebeb29410dc79890251a31aabc02854275250c`  
		Last Modified: Fri, 29 Jan 2021 01:23:22 GMT  
		Size: 17.3 KB (17336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be03b86eb66a5e5b45288e002379d6b671028661b8d756b3f7e94cb0f8121670`  
		Last Modified: Fri, 29 Jan 2021 01:23:22 GMT  
		Size: 8.4 KB (8411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111c3494e132a00dfa9a5be40c5a390005ac6f015c589e580c2f4e2822b14d77`  
		Last Modified: Fri, 29 Jan 2021 03:18:19 GMT  
		Size: 26.2 MB (26182724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a75d73976c6a369ce59f40b8037d94ad482ab64aef1a0fba3b5f7e17d03f2f23`  
		Last Modified: Fri, 29 Jan 2021 03:18:14 GMT  
		Size: 1.3 MB (1299770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63a05c344e38f96d4c58d3399f2505d36c83c8b4d25788239d1bc6160d6a7b16`  
		Last Modified: Fri, 29 Jan 2021 03:18:13 GMT  
		Size: 56.9 KB (56858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d3747209fb5f05ab85d512cd2db55cc50fbdcc7db03a1c988e28ac0564830fe`  
		Last Modified: Fri, 29 Jan 2021 03:18:13 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c475e952cdb157e48fe4732ef54ab130bece88bc60ca963210c6b4a904ea0598`  
		Last Modified: Wed, 03 Feb 2021 20:27:26 GMT  
		Size: 15.5 MB (15549337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a7c9cd4e168290c43c53510de957285e7b1139168c3c000ef934df388a8ffa`  
		Last Modified: Wed, 03 Feb 2021 20:27:23 GMT  
		Size: 2.1 KB (2093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad9912f3c68f93ab388a6d051bf19558d2659c426e91c49a79ec831ea50919a7`  
		Last Modified: Wed, 03 Feb 2021 20:27:24 GMT  
		Size: 1.6 KB (1637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
