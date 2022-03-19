## `wordpress:php7.3-fpm-alpine`

```console
$ docker pull wordpress@sha256:d25cb7a3958cca0d2c7c1511a68021e1f95b5a95aeb4bb08805f97cd1794e332
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

### `wordpress:php7.3-fpm-alpine` - linux; amd64

```console
$ docker pull wordpress@sha256:0e2eef8b6a82377132b5f84a887752f15f421d1c83125d522f7939e9f327b703
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.8 MB (104836537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1c324981145e193d0a889284c470673eaf8bfd7e339f98a6c98daa90d4677cab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 07:06:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 07:06:03 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 07:06:04 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 07:06:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 07:06:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 07:06:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 07:06:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 07:06:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 08:29:55 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 30 Nov 2021 08:29:55 GMT
ENV PHP_VERSION=7.3.33
# Tue, 30 Nov 2021 08:29:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.33.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.33.tar.xz.asc
# Tue, 30 Nov 2021 08:29:56 GMT
ENV PHP_SHA256=166eaccde933381da9516a2b70ad0f447d7cec4b603d07b9a916032b215b90cc
# Tue, 30 Nov 2021 08:30:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 30 Nov 2021 08:30:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Mar 2022 10:28:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Mar 2022 10:28:20 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 11 Mar 2022 10:28:22 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Mar 2022 10:28:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Mar 2022 10:28:22 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 10:28:23 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Mar 2022 10:28:23 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Mar 2022 10:28:23 GMT
EXPOSE 9000
# Fri, 11 Mar 2022 10:28:23 GMT
CMD ["php-fpm"]
# Fri, 11 Mar 2022 15:12:35 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 11 Mar 2022 15:13:41 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 		--with-webp-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 11 Mar 2022 15:13:42 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 11 Mar 2022 15:13:42 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Mon, 14 Mar 2022 19:21:55 GMT
RUN set -eux; 	version='5.9.2'; 	sha1='19653440effafce0f768a1ba5092710717835bdc'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Mon, 14 Mar 2022 19:21:56 GMT
VOLUME [/var/www/html]
# Mon, 14 Mar 2022 19:21:56 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Mon, 14 Mar 2022 19:21:56 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Mon, 14 Mar 2022 19:21:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Mar 2022 19:21:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7da25b2876b1c935b05d7e6efa3e8cd559d031cf30b246d7659ed438726acd`  
		Last Modified: Tue, 30 Nov 2021 09:03:50 GMT  
		Size: 1.7 MB (1709704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc599114627e3bd98e0204b93b161e03065bf9a228bb02ae202469655f12b8d`  
		Last Modified: Tue, 30 Nov 2021 09:03:48 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927a0b37a45a98d7d74a6d7d1567230eca834fb89417274557de7986d1f39401`  
		Last Modified: Tue, 30 Nov 2021 09:03:48 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1619ff5538b1e4ebc908d780ea7c32bb2016499cd22ea2f390f1c60a4a0f489c`  
		Last Modified: Tue, 30 Nov 2021 09:09:15 GMT  
		Size: 12.2 MB (12164227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8ddb7c5740a7d36a99b46e74eee94458e885b5f128e97192d575c6a714bd43f`  
		Last Modified: Tue, 30 Nov 2021 09:09:14 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d3f7d3d2fe87f699aa305b099225ac503dcbb700b1bf8f2ec2c89392f6645a`  
		Last Modified: Fri, 11 Mar 2022 11:35:57 GMT  
		Size: 13.0 MB (12973212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f51347d60cd2f26fe265c3bfe3015ec63cad12674aeabb68ba600dd017c016`  
		Last Modified: Fri, 11 Mar 2022 11:35:54 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87830486670955ea6343db2ed947e300a1d4f11c9cf6be46508c6041a4726e6b`  
		Last Modified: Fri, 11 Mar 2022 11:35:54 GMT  
		Size: 18.4 KB (18382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcaf90bfb7367a6d560621aa302c9c09ad8aaa0833f7906398fc07620d14d7a2`  
		Last Modified: Fri, 11 Mar 2022 11:35:54 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052a044f9cc87a2253f2fa4c1911093f878ac2164691b4f946e62015f4c654ff`  
		Last Modified: Fri, 11 Mar 2022 15:37:31 GMT  
		Size: 41.2 MB (41159639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e624323231ccfd881e562c9903c7e71f1230c8dae0aa9c435ea56d2044856734`  
		Last Modified: Fri, 11 Mar 2022 15:37:26 GMT  
		Size: 15.4 MB (15357422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6adb9b6d76418efffe2cf677ca85d80b7f9858d56d9c14d6bed383697623201a`  
		Last Modified: Fri, 11 Mar 2022 15:37:22 GMT  
		Size: 65.2 KB (65173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b89ce329cb9496047d36119967755d8e190cf705cb5491b8926ce4743621282`  
		Last Modified: Fri, 11 Mar 2022 15:37:22 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e413ab936d57aff47e640f2a386da53145be2a31e7714b3c85ecf5816b1d982`  
		Last Modified: Mon, 14 Mar 2022 19:27:24 GMT  
		Size: 18.6 MB (18553168 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ef4c2c2e8ca6d845bd2db1d1fa30700bf33aea77dcb7e3a2bbd640f020b8b0`  
		Last Modified: Mon, 14 Mar 2022 19:27:21 GMT  
		Size: 2.3 KB (2341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:807773c8d9c72f166ba18ab09af614173367735c1b3a794c056c70c66c4771f4`  
		Last Modified: Mon, 14 Mar 2022 19:27:21 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.3-fpm-alpine` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:be0b299918b5b7f8ea4ae9328c0f922df39f90f07de00ab2be5aa772b116b6d1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.7 MB (99746289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edd4a7c8f736d9844a81851b0ba4df56cd411e6bfa3764391325e40a56b02188`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 02:26:45 GMT
ADD file:9c8618405ef54d562132919ffe49c862d014b402e0e4813b87bf01574fa04c0e in / 
# Thu, 17 Mar 2022 02:26:45 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 07:57:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Mar 2022 07:58:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Mar 2022 07:58:04 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Mar 2022 07:58:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 07:58:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 07:58:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 07:58:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 07:58:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Mar 2022 08:56:29 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 17 Mar 2022 08:56:30 GMT
ENV PHP_VERSION=7.3.33
# Thu, 17 Mar 2022 08:56:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.33.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.33.tar.xz.asc
# Thu, 17 Mar 2022 08:56:31 GMT
ENV PHP_SHA256=166eaccde933381da9516a2b70ad0f447d7cec4b603d07b9a916032b215b90cc
# Thu, 17 Mar 2022 08:57:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Mar 2022 08:57:12 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Mar 2022 09:06:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Mar 2022 09:06:52 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 17 Mar 2022 09:06:55 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Mar 2022 09:06:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Mar 2022 09:06:56 GMT
WORKDIR /var/www/html
# Thu, 17 Mar 2022 09:06:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 17 Mar 2022 09:06:57 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Mar 2022 09:06:58 GMT
EXPOSE 9000
# Thu, 17 Mar 2022 09:06:58 GMT
CMD ["php-fpm"]
# Thu, 17 Mar 2022 12:59:47 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Thu, 17 Mar 2022 13:01:59 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 		--with-webp-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 17 Mar 2022 13:02:02 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 17 Mar 2022 13:02:03 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 17 Mar 2022 13:02:10 GMT
RUN set -eux; 	version='5.9.2'; 	sha1='19653440effafce0f768a1ba5092710717835bdc'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 17 Mar 2022 13:02:11 GMT
VOLUME [/var/www/html]
# Thu, 17 Mar 2022 13:02:12 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Thu, 17 Mar 2022 13:02:12 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 17 Mar 2022 13:02:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 13:02:13 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:787f016efa9bc7812361be134f731e845b97fba19169cf3615e7048c0412380e`  
		Last Modified: Thu, 17 Mar 2022 02:28:24 GMT  
		Size: 2.6 MB (2624973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f434a07170d3fcef8823359200e8903ff5e29ae4f37e9e03cdf4d93161047c9d`  
		Last Modified: Thu, 17 Mar 2022 09:22:43 GMT  
		Size: 1.7 MB (1688751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a11f75b4af480b6ec718198304a48491171a73b009588f8cff856386be2782e`  
		Last Modified: Thu, 17 Mar 2022 09:22:42 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04026b5344cf4c6a68cb1e65840d9cfc5ba017f55e306a39c4b4e0aaed495aaa`  
		Last Modified: Thu, 17 Mar 2022 09:22:41 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b919a38bd90741e028d3a24f40b0873adb94db92bab989fbc7adbb0c4c2e1107`  
		Last Modified: Thu, 17 Mar 2022 09:31:29 GMT  
		Size: 12.2 MB (12164132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5b4ece8d22fffa6dc536760e0c4472f41385cee01880f9d1a4db94d0beb904e`  
		Last Modified: Thu, 17 Mar 2022 09:31:26 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4495ddff33af130cd01e344fb01a8bc02e411c5d342a10d2120571867e1829cf`  
		Last Modified: Thu, 17 Mar 2022 09:32:19 GMT  
		Size: 10.7 MB (10730538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6213d851141101263293d8a2cb1ceb5b1472ba86ba3c48494f9c92df9cbc372a`  
		Last Modified: Thu, 17 Mar 2022 09:32:11 GMT  
		Size: 2.3 KB (2302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:257e799f9f3fedf2f11e2fef9db31c3153693c642c540cc47a04f7db7028c885`  
		Last Modified: Thu, 17 Mar 2022 09:32:12 GMT  
		Size: 18.2 KB (18217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02839b76929736d96bff5e16a74fc2cd3c44ce7cfb9bd08f992c6f495fec3ef3`  
		Last Modified: Thu, 17 Mar 2022 09:32:11 GMT  
		Size: 8.4 KB (8414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfec3fc714ac59842c3b8f31667e181d713a60cbd706ee10c1b53ed181209c10`  
		Last Modified: Thu, 17 Mar 2022 13:24:57 GMT  
		Size: 38.8 MB (38785584 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d04d583ae126f466f74a8fa0f8ba50e4b78968d0dc81f9f29ca7ec3ba85ffabe`  
		Last Modified: Thu, 17 Mar 2022 13:24:41 GMT  
		Size: 15.1 MB (15098787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da91b2d8882482635752997678c9c28ad32b0d706ed97ecacdcb7efd4a8d9be0`  
		Last Modified: Thu, 17 Mar 2022 13:24:31 GMT  
		Size: 65.0 KB (64952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18f7e975c9ccff5f1c428c3cd28f44955b679613dcab80af1d1722e3d267d1de`  
		Last Modified: Thu, 17 Mar 2022 13:24:31 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c6e9cc8d5ed2758ec4b60a10909fc993c1399e7063739fe80d2e0bc7fca4367`  
		Last Modified: Thu, 17 Mar 2022 13:24:44 GMT  
		Size: 18.6 MB (18553155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b839d7e34bf66bc838c3c76f22decb67c818e8df52638b8748846c64132a935e`  
		Last Modified: Thu, 17 Mar 2022 13:24:31 GMT  
		Size: 2.3 KB (2338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a50b5dff2a76c0d157b4f704747bc3ba5a73ccf1844cba879d2461a14477e6b1`  
		Last Modified: Thu, 17 Mar 2022 13:24:30 GMT  
		Size: 1.7 KB (1729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.3-fpm-alpine` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:17e00fd62fac73a439a00c9e158fa46c2308f59c1b5e079b704218c1c39c71c8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.8 MB (97766582 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd33ede1ad4ee36699692dce174353f808aae056c14123d0e00d75c8078f1480`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 05:27:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 05:27:16 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 05:27:18 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 05:27:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 05:27:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 05:27:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 05:27:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 05:27:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 06:16:35 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 30 Nov 2021 06:16:36 GMT
ENV PHP_VERSION=7.3.33
# Tue, 30 Nov 2021 06:16:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.33.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.33.tar.xz.asc
# Tue, 30 Nov 2021 06:16:37 GMT
ENV PHP_SHA256=166eaccde933381da9516a2b70ad0f447d7cec4b603d07b9a916032b215b90cc
# Tue, 30 Nov 2021 06:16:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 30 Nov 2021 06:16:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Mar 2022 06:41:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Mar 2022 06:41:57 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 11 Mar 2022 06:41:59 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Mar 2022 06:41:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Mar 2022 06:42:00 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 06:42:01 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Mar 2022 06:42:02 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Mar 2022 06:42:02 GMT
EXPOSE 9000
# Fri, 11 Mar 2022 06:42:03 GMT
CMD ["php-fpm"]
# Fri, 11 Mar 2022 19:08:19 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 11 Mar 2022 19:10:27 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 		--with-webp-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 11 Mar 2022 19:10:29 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 11 Mar 2022 19:10:31 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Mon, 14 Mar 2022 19:49:53 GMT
RUN set -eux; 	version='5.9.2'; 	sha1='19653440effafce0f768a1ba5092710717835bdc'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Mon, 14 Mar 2022 19:49:54 GMT
VOLUME [/var/www/html]
# Mon, 14 Mar 2022 19:49:55 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Mon, 14 Mar 2022 19:49:55 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Mon, 14 Mar 2022 19:49:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Mar 2022 19:49:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484fe107211badcebee7c4211e5ed91c7e5212cdd6d7edbb292a63ec60572bdd`  
		Last Modified: Tue, 30 Nov 2021 06:57:00 GMT  
		Size: 1.6 MB (1568802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93353d0a7113f37ba224b9ee296684e49f27c1c9440d3a3c5d310749213da97f`  
		Last Modified: Tue, 30 Nov 2021 06:56:59 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137db50a58959a68358c190d2a143088b82ab25d97cb889876fbc0728e446058`  
		Last Modified: Tue, 30 Nov 2021 06:57:00 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f11f999c0833459bfa7c43ee12a033db7ca9b4a1be63f3452f342606d89eb36`  
		Last Modified: Tue, 30 Nov 2021 07:06:57 GMT  
		Size: 12.2 MB (12164222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:352a5152490684f5fa09067085521c14fbdf9d855c435bff657e924028bd5afc`  
		Last Modified: Tue, 30 Nov 2021 07:06:55 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b84805f5957c312e2dd28f6bd372dd382e49d3f05a725c7845f1c2b9316afd26`  
		Last Modified: Fri, 11 Mar 2022 11:28:58 GMT  
		Size: 11.2 MB (11237322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ed4693d25830fe752d4fb7707d08a6a04ab6cc502197f30f622c8fded86dbb6`  
		Last Modified: Fri, 11 Mar 2022 11:28:51 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b93042094e0136e49ecf33df4b604fdf21d0221c00b81da8053dbb0574446c1`  
		Last Modified: Fri, 11 Mar 2022 11:28:51 GMT  
		Size: 18.4 KB (18363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d900bd233690fc929168188c152b756053934ab26888608ed15229b23da35945`  
		Last Modified: Fri, 11 Mar 2022 11:28:51 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86a6207a8849a4fcc6977f6203e2e54e87b2431e0bcf129a640cc18c8cd7f82`  
		Last Modified: Fri, 11 Mar 2022 19:58:03 GMT  
		Size: 36.8 MB (36810206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12828399dab48b1e81b348c083030732451782785c75ab410e547f834c886fd2`  
		Last Modified: Fri, 11 Mar 2022 19:57:49 GMT  
		Size: 14.9 MB (14897348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe3056e92ad591b92abdc63b663035df9b577920e785c2947b7f7a345bae2d60`  
		Last Modified: Fri, 11 Mar 2022 19:57:39 GMT  
		Size: 65.2 KB (65178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51306cd426916cd194e5425fa55c8771733170f2524706a5c7fc4abef7786502`  
		Last Modified: Fri, 11 Mar 2022 19:57:39 GMT  
		Size: 389.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ad14da0480c88ec12e8054caf62d05fa626296c220b0c799de5ba8ba871e8d4`  
		Last Modified: Mon, 14 Mar 2022 20:05:19 GMT  
		Size: 18.6 MB (18553176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9090545d3ed52e6688157c3dc143c583fceba1198c18a350e4be9c3cfb0ee947`  
		Last Modified: Mon, 14 Mar 2022 20:05:04 GMT  
		Size: 2.3 KB (2340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3bdc30e8898d70a44fd30bf80e2d573ba4ade1479549579bac3d8a81d3f83b4`  
		Last Modified: Mon, 14 Mar 2022 20:05:06 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.3-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:e2eec76d88cc0113667beb45a02c670664b8f90761f520df4f1e3f0189cc8ccd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.8 MB (101760718 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17c90f0a8f5f7bb71edb28fccd3f935e1cdfec8cd976e2b179d3a5a113ca7b51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Thu, 17 Mar 2022 17:51:49 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 17 Mar 2022 17:51:50 GMT
ENV PHP_VERSION=7.3.33
# Thu, 17 Mar 2022 17:51:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.33.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.33.tar.xz.asc
# Thu, 17 Mar 2022 17:51:52 GMT
ENV PHP_SHA256=166eaccde933381da9516a2b70ad0f447d7cec4b603d07b9a916032b215b90cc
# Thu, 17 Mar 2022 17:52:58 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Mar 2022 17:53:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:59:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Mar 2022 17:59:19 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 17 Mar 2022 17:59:20 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Mar 2022 17:59:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Mar 2022 17:59:21 GMT
WORKDIR /var/www/html
# Thu, 17 Mar 2022 17:59:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 17 Mar 2022 17:59:23 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Mar 2022 17:59:24 GMT
EXPOSE 9000
# Thu, 17 Mar 2022 17:59:25 GMT
CMD ["php-fpm"]
# Fri, 18 Mar 2022 13:49:13 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 18 Mar 2022 13:50:10 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 		--with-webp-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 18 Mar 2022 13:50:12 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 18 Mar 2022 13:50:12 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 18 Mar 2022 13:50:16 GMT
RUN set -eux; 	version='5.9.2'; 	sha1='19653440effafce0f768a1ba5092710717835bdc'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Fri, 18 Mar 2022 13:50:16 GMT
VOLUME [/var/www/html]
# Fri, 18 Mar 2022 13:50:18 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Fri, 18 Mar 2022 13:50:19 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Fri, 18 Mar 2022 13:50:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Mar 2022 13:50:20 GMT
CMD ["php-fpm"]
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
	-	`sha256:4199b553a60d8ecee4c5936a63d72991f8f44f61eb979e2e047d6502660c29d3`  
		Last Modified: Thu, 17 Mar 2022 18:41:29 GMT  
		Size: 12.2 MB (12163926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e312673bec00c0286da04e31ecd601b691eb29664630d29dc3c6d6851ef59644`  
		Last Modified: Thu, 17 Mar 2022 18:41:27 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292c76593e80d98233ef08d92ba0e0237d9b2f176a8654d213643b9f2b44f8c0`  
		Last Modified: Thu, 17 Mar 2022 18:42:04 GMT  
		Size: 11.3 MB (11264823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26ec184d4da9217690cfd9388cc5a63eceec101f5fe51313930a556f272814e1`  
		Last Modified: Thu, 17 Mar 2022 18:42:02 GMT  
		Size: 2.3 KB (2301 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26b193191a190540fefd15d6f76af9e0c5fd5c7751738141feae48400d174751`  
		Last Modified: Thu, 17 Mar 2022 18:42:02 GMT  
		Size: 18.1 KB (18125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:494e53974927862b6490af68d6f097c73741ec804997439e33b04861a858a1ef`  
		Last Modified: Thu, 17 Mar 2022 18:42:02 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70407d634c77067d89d8a1d62ed0191655fa7a462213043106a5c0821aadbbb4`  
		Last Modified: Fri, 18 Mar 2022 14:14:25 GMT  
		Size: 39.9 MB (39940061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b548a45eb9453acb307554d1fd4ff880d2397c191b95556e513fdbf850eec16`  
		Last Modified: Fri, 18 Mar 2022 14:14:21 GMT  
		Size: 15.3 MB (15327572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81aa5b4a6f49ec04c75025963ff91673da76b160266bf259ddec918299eb8c64`  
		Last Modified: Fri, 18 Mar 2022 14:14:17 GMT  
		Size: 64.9 KB (64896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42d66aeb87fdf63a3191ca30fd0add9ee93f7edbe0e16696f775ae34b9e1b890`  
		Last Modified: Fri, 18 Mar 2022 14:14:17 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f3516b5d4d27ca0688ec8dba7ba5e861c2d2c6edac24dec98df1c7129a5c2c5`  
		Last Modified: Fri, 18 Mar 2022 14:14:20 GMT  
		Size: 18.6 MB (18553140 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e361fc4cb53b2e5c56fbca337ffd34852a15305150bead4efc1bfd8b4583148d`  
		Last Modified: Fri, 18 Mar 2022 14:14:17 GMT  
		Size: 2.3 KB (2337 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:251837dbc4120d90a608bc4767d17e8960cfe8ffbf569e9d339486a5e62c1f23`  
		Last Modified: Fri, 18 Mar 2022 14:14:17 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.3-fpm-alpine` - linux; 386

```console
$ docker pull wordpress@sha256:73db81c4365cd43b87f9e1871e2816b2876290770e55efee1f2a3f831e40cb1e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.3 MB (104326055 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cca36c085bbec767762d06c0d80fe60d91737c7cf13d86516cacf8d7e0c7b29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Fri, 18 Mar 2022 07:30:51 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Fri, 18 Mar 2022 07:30:51 GMT
ENV PHP_VERSION=7.3.33
# Fri, 18 Mar 2022 07:30:51 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.33.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.33.tar.xz.asc
# Fri, 18 Mar 2022 07:30:51 GMT
ENV PHP_SHA256=166eaccde933381da9516a2b70ad0f447d7cec4b603d07b9a916032b215b90cc
# Fri, 18 Mar 2022 07:31:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 18 Mar 2022 07:31:11 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 18 Mar 2022 07:44:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 18 Mar 2022 07:44:26 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 18 Mar 2022 07:44:27 GMT
RUN docker-php-ext-enable sodium
# Fri, 18 Mar 2022 07:44:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 18 Mar 2022 07:44:28 GMT
WORKDIR /var/www/html
# Fri, 18 Mar 2022 07:44:28 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 18 Mar 2022 07:44:28 GMT
STOPSIGNAL SIGQUIT
# Fri, 18 Mar 2022 07:44:28 GMT
EXPOSE 9000
# Fri, 18 Mar 2022 07:44:28 GMT
CMD ["php-fpm"]
# Sat, 19 Mar 2022 11:41:22 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Sat, 19 Mar 2022 11:42:28 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 		--with-webp-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Sat, 19 Mar 2022 11:42:30 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 19 Mar 2022 11:42:31 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Sat, 19 Mar 2022 11:42:35 GMT
RUN set -eux; 	version='5.9.2'; 	sha1='19653440effafce0f768a1ba5092710717835bdc'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Sat, 19 Mar 2022 11:42:35 GMT
VOLUME [/var/www/html]
# Sat, 19 Mar 2022 11:42:36 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Sat, 19 Mar 2022 11:42:36 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Sat, 19 Mar 2022 11:42:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 19 Mar 2022 11:42:36 GMT
CMD ["php-fpm"]
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
	-	`sha256:fe7705643558d4cbe22e88f3f7cc5000c83104a8da13840737c1a71021dd4174`  
		Last Modified: Fri, 18 Mar 2022 10:38:23 GMT  
		Size: 12.2 MB (12164131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71f8dbfe5b822334f402e2d3e8604d87f7c38db6a97999b85daa530e6fd7632f`  
		Last Modified: Fri, 18 Mar 2022 10:38:21 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2872c00ff5f5da3de4e6390529638aaf20bf4cdb9d92bbc1ad152bb9c4d43e7`  
		Last Modified: Fri, 18 Mar 2022 10:39:08 GMT  
		Size: 11.8 MB (11753087 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d2a6ba2ae125e3e82bce909cc98f556ec0a2079af613df86d29224b8e5e8ba`  
		Last Modified: Fri, 18 Mar 2022 10:39:04 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4074edef68d5e7f7f47cfcaedc7ccd5e169c5ec0bf2c917c93aad957c3505039`  
		Last Modified: Fri, 18 Mar 2022 10:39:04 GMT  
		Size: 18.2 KB (18211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7bded8d57894250ee4d939a3c5f06aa8d42aeffdb5435b09d64ef4e92ab8d8`  
		Last Modified: Fri, 18 Mar 2022 10:39:05 GMT  
		Size: 8.4 KB (8412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16ce7991fa2203e860158aca1cdadb864364bcd26485d922166979e0b2bf11fa`  
		Last Modified: Sat, 19 Mar 2022 12:08:31 GMT  
		Size: 41.6 MB (41568135 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8d5eb47d316158065db9d5cacb23b90742703bc6542fe183729faea3e3a509`  
		Last Modified: Sat, 19 Mar 2022 12:08:25 GMT  
		Size: 15.6 MB (15565158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fbe363a32fcd3135631bed2b67a0022beb5cf85a110d2816cbd8f31e6d13eb8`  
		Last Modified: Sat, 19 Mar 2022 12:08:19 GMT  
		Size: 65.0 KB (64975 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:356b027faa86c916226315aa79b13f88134f55b5c0d9959a00cec30e7413e8a4`  
		Last Modified: Sat, 19 Mar 2022 12:08:18 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bba9a969c7a5ad18d59ef4b851cda87adc3ef5acc17d5e237296b9b9cb0c954`  
		Last Modified: Sat, 19 Mar 2022 12:08:23 GMT  
		Size: 18.6 MB (18553145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be208100dabcdfe6f0332b579177dfe6cbb3e1e81635e0b3a7d4bd00405e9238`  
		Last Modified: Sat, 19 Mar 2022 12:08:18 GMT  
		Size: 2.3 KB (2334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8a021f81e322e6c83c14a0ee58371bb960f1b913020d8a3053f67b73238e5a`  
		Last Modified: Sat, 19 Mar 2022 12:08:18 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.3-fpm-alpine` - linux; ppc64le

```console
$ docker pull wordpress@sha256:2da3d3374ef72e34898af271f6e51a4a21505eebb5b405fd3f9cd8feee36e1bc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.9 MB (106922003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:78e6524c1255f451b40dcce560b0abbdd72f1efd8341d69128d399107e596755`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 06:02:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 06:03:14 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 06:03:32 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 06:03:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 06:03:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 06:03:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 06:03:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 06:04:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 06:57:59 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Tue, 30 Nov 2021 06:58:00 GMT
ENV PHP_VERSION=7.3.33
# Tue, 30 Nov 2021 06:58:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.33.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.33.tar.xz.asc
# Tue, 30 Nov 2021 06:58:03 GMT
ENV PHP_SHA256=166eaccde933381da9516a2b70ad0f447d7cec4b603d07b9a916032b215b90cc
# Tue, 30 Nov 2021 06:58:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 30 Nov 2021 06:58:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 11 Mar 2022 08:56:38 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 11 Mar 2022 08:56:43 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Fri, 11 Mar 2022 08:56:52 GMT
RUN docker-php-ext-enable sodium
# Fri, 11 Mar 2022 08:56:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 11 Mar 2022 08:56:57 GMT
WORKDIR /var/www/html
# Fri, 11 Mar 2022 08:57:10 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 11 Mar 2022 08:57:14 GMT
STOPSIGNAL SIGQUIT
# Fri, 11 Mar 2022 08:57:17 GMT
EXPOSE 9000
# Fri, 11 Mar 2022 08:57:21 GMT
CMD ["php-fpm"]
# Fri, 11 Mar 2022 21:04:14 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 11 Mar 2022 21:05:49 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 		--with-webp-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 11 Mar 2022 21:05:57 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 11 Mar 2022 21:06:04 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Mon, 14 Mar 2022 21:24:43 GMT
RUN set -eux; 	version='5.9.2'; 	sha1='19653440effafce0f768a1ba5092710717835bdc'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Mon, 14 Mar 2022 21:24:47 GMT
VOLUME [/var/www/html]
# Mon, 14 Mar 2022 21:24:49 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Mon, 14 Mar 2022 21:24:50 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Mon, 14 Mar 2022 21:24:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 14 Mar 2022 21:24:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603762061fb50079a4b6eb13347fd9a84cc1456d628cf781c89924a54bc419c1`  
		Last Modified: Tue, 30 Nov 2021 07:26:39 GMT  
		Size: 1.8 MB (1756276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645c08440cfaddc2735de2e28697acff0bc71db4cc7242494a44f92c94134e32`  
		Last Modified: Tue, 30 Nov 2021 07:26:39 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5de97a9a329d566f48c2edce253e4ccda6f021041e92326728b7499d13c823b`  
		Last Modified: Tue, 30 Nov 2021 07:26:39 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2461993c8ca4d3d5e6565c8022e85fae8553e9d8c53cc01bfbfefa5620c1214a`  
		Last Modified: Tue, 30 Nov 2021 07:33:03 GMT  
		Size: 12.2 MB (12164225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c771e480c75405db973c12d7a3e1381e913e5ee9e3abf18830ffaa8d5fc54b`  
		Last Modified: Tue, 30 Nov 2021 07:33:02 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e3d153115304621dc89edd47973651406f68ab8340282a6099510e8b626ea6`  
		Last Modified: Fri, 11 Mar 2022 10:16:39 GMT  
		Size: 13.6 MB (13636664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84266c9fdb49c5079459137edd7a3b2fdeba1cd332e11fff819d0373dc51b667`  
		Last Modified: Fri, 11 Mar 2022 10:16:37 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f70147bb31065ec326fb9ff88f126d24b6cdcdd0504118940b4f04f828ac0596`  
		Last Modified: Fri, 11 Mar 2022 10:16:37 GMT  
		Size: 18.4 KB (18369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6aadeb2e2e8f7a759b6de5c0ae2dcafc053eecff4e8ca256edd13ad0252dddb4`  
		Last Modified: Fri, 11 Mar 2022 10:16:37 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7a4ccd61acae05565f9697a6f15e6bdcbbe4186b7c59ec4e986b05a484352c3`  
		Last Modified: Fri, 11 Mar 2022 22:18:40 GMT  
		Size: 42.3 MB (42337411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceae376c5e61b5083617282513f8aa3d12bd308b177301ce551242231667da4f`  
		Last Modified: Fri, 11 Mar 2022 22:18:35 GMT  
		Size: 15.6 MB (15558777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4001234d8b0e1124dcb3f574369241ba7b0d1e9f8e44a405fa59a7cfa00a3962`  
		Last Modified: Fri, 11 Mar 2022 22:18:30 GMT  
		Size: 65.1 KB (65111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076d56210b275933ed4d7116c8d704f6e7bd707666b50a789d39fe3ef6349440`  
		Last Modified: Fri, 11 Mar 2022 22:18:30 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9443339f642bc369abfb63f80c2ab87b52c1501105f25181c06726deeb97aca`  
		Last Modified: Mon, 14 Mar 2022 21:38:04 GMT  
		Size: 18.6 MB (18553177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddfb39bad7159d33b2e95e1bc246405956f4347d770938a21880323080982269`  
		Last Modified: Mon, 14 Mar 2022 21:38:01 GMT  
		Size: 2.3 KB (2343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c835d308494f02bc565b85deb7606bdcc544cbaf494f6be99433f058e555d5b7`  
		Last Modified: Mon, 14 Mar 2022 21:38:00 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php7.3-fpm-alpine` - linux; s390x

```console
$ docker pull wordpress@sha256:814eca676b521ec378a6191b7cd4257316e26676c1451741bb245aa6db2602e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.8 MB (94803879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bda469d278f8910bfe42dd14c16174607911e0d8cfbf0831c0885ff610501ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 17 Mar 2022 03:04:28 GMT
ADD file:f623c69acb1859b41ef29e8f20f4e6c7072d9c6d7210d745afc615251bfe418f in / 
# Thu, 17 Mar 2022 03:04:28 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 09:19:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 17 Mar 2022 09:19:49 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 17 Mar 2022 09:19:50 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 17 Mar 2022 09:19:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 17 Mar 2022 09:19:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 17 Mar 2022 09:19:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 09:19:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 17 Mar 2022 09:19:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 17 Mar 2022 11:34:39 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 17 Mar 2022 11:34:39 GMT
ENV PHP_VERSION=7.3.33
# Thu, 17 Mar 2022 11:34:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.33.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.33.tar.xz.asc
# Thu, 17 Mar 2022 11:34:39 GMT
ENV PHP_SHA256=166eaccde933381da9516a2b70ad0f447d7cec4b603d07b9a916032b215b90cc
# Thu, 17 Mar 2022 11:35:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 17 Mar 2022 11:35:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:40:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 17 Mar 2022 11:40:53 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 17 Mar 2022 11:40:53 GMT
RUN docker-php-ext-enable sodium
# Thu, 17 Mar 2022 11:40:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 17 Mar 2022 11:40:54 GMT
WORKDIR /var/www/html
# Thu, 17 Mar 2022 11:40:54 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 17 Mar 2022 11:40:54 GMT
STOPSIGNAL SIGQUIT
# Thu, 17 Mar 2022 11:40:54 GMT
EXPOSE 9000
# Thu, 17 Mar 2022 11:40:54 GMT
CMD ["php-fpm"]
# Thu, 17 Mar 2022 23:02:32 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Thu, 17 Mar 2022 23:03:12 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype-dir=/usr 		--with-jpeg-dir=/usr 		--with-png-dir=/usr 		--with-webp-dir=/usr 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Thu, 17 Mar 2022 23:03:14 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 17 Mar 2022 23:03:14 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 17 Mar 2022 23:03:18 GMT
RUN set -eux; 	version='5.9.2'; 	sha1='19653440effafce0f768a1ba5092710717835bdc'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 17 Mar 2022 23:03:20 GMT
VOLUME [/var/www/html]
# Thu, 17 Mar 2022 23:03:20 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Thu, 17 Mar 2022 23:03:20 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 17 Mar 2022 23:03:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Mar 2022 23:03:20 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d51040c5bfbf434887bfed2557335a411e6ef760d04cc178d455d1c3ec1b721c`  
		Last Modified: Thu, 17 Mar 2022 03:05:26 GMT  
		Size: 2.6 MB (2601715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a174f78affd2f7f6d96d3c25f978ba8963a8a078973ba8c674dcfc539da1301b`  
		Last Modified: Thu, 17 Mar 2022 11:57:11 GMT  
		Size: 1.8 MB (1760653 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb55fc644063786762e3851a4a84c38cf1f4fb9d0e0bb8448c4a0e928b2c28b2`  
		Last Modified: Thu, 17 Mar 2022 11:57:11 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94201f7612026faed96b2a7eb4d4c53a783aa565ff942aac5b1714a6767dafd1`  
		Last Modified: Thu, 17 Mar 2022 11:57:11 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9b05c8b11208083e4e71940fa9d064b3bf2821a36c948997d486492beb99846`  
		Last Modified: Thu, 17 Mar 2022 12:12:13 GMT  
		Size: 12.2 MB (12164149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357c30c761277ef71480eb08d5a0293e5150928b12e14fb063223666349a1715`  
		Last Modified: Thu, 17 Mar 2022 12:12:13 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff6867e3a162e46a8d70625761b9b45b54c28327a7045718cfe51c2ef35fdd3f`  
		Last Modified: Thu, 17 Mar 2022 12:12:34 GMT  
		Size: 11.1 MB (11093995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49ebb3614a1f692a09ed6c13bd11fa04d878d682de5342f4a2b0b7543ec2fa9b`  
		Last Modified: Thu, 17 Mar 2022 12:12:32 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ce85378f00f227cb651aef6dd8741f1bbbc14a978bdf1fa333542ec5c2630fb`  
		Last Modified: Thu, 17 Mar 2022 12:12:33 GMT  
		Size: 18.2 KB (18234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77083608ba0b94fdade68715e1a043b64727985d7e159c8f8db9bcfa5da6a8a0`  
		Last Modified: Thu, 17 Mar 2022 12:12:33 GMT  
		Size: 8.4 KB (8412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87fe9af4a2ce8b7d8c1c9fa602723da0b8c6b0b448abe569b976ef02ee589715`  
		Last Modified: Thu, 17 Mar 2022 23:17:37 GMT  
		Size: 33.1 MB (33068435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ec362d1b798f0012554e3b596ff93d2106cda95c4bdbe56a05c4090a6a79029`  
		Last Modified: Thu, 17 Mar 2022 23:17:35 GMT  
		Size: 15.5 MB (15467535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a1dc460cd886ca343af43c9d3d15ebf56251f855753c95081f1d0c031d44dbd`  
		Last Modified: Thu, 17 Mar 2022 23:17:32 GMT  
		Size: 58.8 KB (58802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:347668b413c262df3b8923d596cb2c5ddcb560efc3ce9330c7421fcf882c2dbd`  
		Last Modified: Thu, 17 Mar 2022 23:17:32 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89f3c79e37c81ea464d6c817492646692b9628d69763147f8400edbd04e3f0e0`  
		Last Modified: Thu, 17 Mar 2022 23:17:34 GMT  
		Size: 18.6 MB (18553167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a5a29c590ebf6e5ec6d073b7bf568400af0011ba3e0f253195c0346236206d4`  
		Last Modified: Thu, 17 Mar 2022 23:17:32 GMT  
		Size: 2.3 KB (2334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:144dae3ef1c447e5479a7b85ce25bcc3534c9b63c51fa5673491a45a3f30b694`  
		Last Modified: Thu, 17 Mar 2022 23:17:32 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
