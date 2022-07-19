## `wordpress:6-fpm-alpine`

```console
$ docker pull wordpress@sha256:f07fd0019162bfa7a912a09e1e14e85bfb0f8ba695d68799afdfa4bf2d112de2
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

### `wordpress:6-fpm-alpine` - linux; amd64

```console
$ docker pull wordpress@sha256:48714846ae91a7227133ea3b17bfd8013f2297f6a8e0db17b3a9548b4e56579b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.5 MB (99494519 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c637564fc89075ce3a920dede587b93c6f621bc9d3bf940573d3f06cf1d4c3c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 18 Jul 2022 21:00:15 GMT
ADD file:a2648378045615c3785c752423b1afc8dc1c2b213393344f4d0ca17e7255c1cb in / 
# Mon, 18 Jul 2022 21:00:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 00:27:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 19 Jul 2022 00:27:06 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 19 Jul 2022 00:27:06 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 19 Jul 2022 00:27:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 19 Jul 2022 00:27:07 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 19 Jul 2022 00:27:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 19 Jul 2022 00:27:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 19 Jul 2022 00:27:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 19 Jul 2022 01:09:52 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 19 Jul 2022 01:09:52 GMT
ENV PHP_VERSION=7.4.30
# Tue, 19 Jul 2022 01:09:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Tue, 19 Jul 2022 01:09:52 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Tue, 19 Jul 2022 01:09:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 19 Jul 2022 01:09:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Jul 2022 01:17:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Jul 2022 01:17:49 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 19 Jul 2022 01:17:50 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Jul 2022 01:17:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Jul 2022 01:17:50 GMT
WORKDIR /var/www/html
# Tue, 19 Jul 2022 01:17:51 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 19 Jul 2022 01:17:51 GMT
STOPSIGNAL SIGQUIT
# Tue, 19 Jul 2022 01:17:51 GMT
EXPOSE 9000
# Tue, 19 Jul 2022 01:17:51 GMT
CMD ["php-fpm"]
# Tue, 19 Jul 2022 06:27:31 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Tue, 19 Jul 2022 06:28:23 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 19 Jul 2022 06:28:25 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 19 Jul 2022 06:28:25 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 19 Jul 2022 06:28:28 GMT
RUN set -eux; 	version='6.0.1'; 	sha1='a1c02b6b754d74c08a70d5a8b604bdb72f1b276a'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Tue, 19 Jul 2022 06:28:29 GMT
VOLUME [/var/www/html]
# Tue, 19 Jul 2022 06:28:29 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Tue, 19 Jul 2022 06:28:29 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Tue, 19 Jul 2022 06:28:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 06:28:29 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:530afca65e2ea04227630ae746e0c85b2bd1a179379cbf2b6501b49c4cab2ccc`  
		Last Modified: Mon, 18 Jul 2022 19:09:35 GMT  
		Size: 2.8 MB (2798806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09cfb8455962e8dee2ec89d1aca6167797ee8fb124669b4f37e54aa82accbd11`  
		Last Modified: Tue, 19 Jul 2022 01:26:20 GMT  
		Size: 1.7 MB (1705561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72bc08afeabf24400f8800b72194e328506b82a27cefb34b8b9f573393b8bc2`  
		Last Modified: Tue, 19 Jul 2022 01:26:19 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb7a732550aeef70ff8ae6f2fdc1f988da20f7adbd4fa74770ad6e4f15be150`  
		Last Modified: Tue, 19 Jul 2022 01:26:20 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45484466a2a50b56b0c5b88f3cf0605d4247fac17de1b136c4d98779fea574b2`  
		Last Modified: Tue, 19 Jul 2022 01:31:30 GMT  
		Size: 10.4 MB (10439063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:104dedd8731096601de57cba82168617d4cc7fb16c94c63f9d051641ba43f3c9`  
		Last Modified: Tue, 19 Jul 2022 01:31:29 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63372c64902eab0b5eb4901e97d0825f03becca674ba88172b1de03f7803c460`  
		Last Modified: Tue, 19 Jul 2022 01:32:11 GMT  
		Size: 11.5 MB (11456232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d349eb4b2c2d4bfd53b1045e842f6014eea483e8b28399234947d68e9c81911`  
		Last Modified: Tue, 19 Jul 2022 01:32:08 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fae90fb5562fd8e3651a570dfada232d1ace20d7dab20422b6dbbd1a8b1e57`  
		Last Modified: Tue, 19 Jul 2022 01:32:08 GMT  
		Size: 18.4 KB (18370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7180dd0fdfadac1b24467a2c327c9ff26a253f511dbe5d5d587a2dbc1b6a64cd`  
		Last Modified: Tue, 19 Jul 2022 01:32:08 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743ac734fef41ffd05cf3318fed83e4f1406b9ca142edcc9a2525274570c2a52`  
		Last Modified: Tue, 19 Jul 2022 06:35:59 GMT  
		Size: 47.7 MB (47701872 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe25f5c0d91651af1ce4683b27644a22c7994f3247e086ae9710e7fa3119430c`  
		Last Modified: Tue, 19 Jul 2022 06:35:52 GMT  
		Size: 4.3 MB (4297071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b1ce5772c1e90e2907035c9e469d4fc8b4c2fd87ec95591b6e9f7d3535ed2a7`  
		Last Modified: Tue, 19 Jul 2022 06:35:49 GMT  
		Size: 65.5 KB (65491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52681a7a71b7c7fd35390518acb4221aef8ff73885a26dd891e9493dae3a1eb7`  
		Last Modified: Tue, 19 Jul 2022 06:35:50 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:290ef5dc91722129839145fa87ff1b9d5a1126ea7c2cd2dd271ac3ef4be3b3fb`  
		Last Modified: Tue, 19 Jul 2022 06:35:52 GMT  
		Size: 21.0 MB (20994680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39dc17e185583882e7b9e9435658f645f66df61e28ec7dd5c246c0d7d0dd0ef8`  
		Last Modified: Tue, 19 Jul 2022 06:35:49 GMT  
		Size: 2.3 KB (2336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdd8f28d1a9da3a3b4a40d4529e0c12ae87284bac156406c7422f5f8e2fe8428`  
		Last Modified: Tue, 19 Jul 2022 06:35:49 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:6-fpm-alpine` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:4105c3a3dce79e57d17bd57ffff32e9c74ddc19c02326fb91980b0b5ad865cbf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.9 MB (93872547 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5044484404dd63d4532bb1b3a0501fbc5c586d30c2d6060d45b2b7bb0dbd030c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 18 Jul 2022 19:49:37 GMT
ADD file:7a20333469e71664904a0cb8f61613250f2bd092b4a27bfa7bbae1dc7e21b7ed in / 
# Mon, 18 Jul 2022 19:49:37 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 02:54:46 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 19 Jul 2022 02:54:49 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 19 Jul 2022 02:54:51 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 19 Jul 2022 02:54:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 19 Jul 2022 02:54:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 19 Jul 2022 02:54:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 19 Jul 2022 02:54:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 19 Jul 2022 02:54:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 19 Jul 2022 03:50:25 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 19 Jul 2022 03:50:26 GMT
ENV PHP_VERSION=7.4.30
# Tue, 19 Jul 2022 03:50:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Tue, 19 Jul 2022 03:50:28 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Tue, 19 Jul 2022 03:50:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 19 Jul 2022 03:50:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Jul 2022 04:03:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Jul 2022 04:03:28 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 19 Jul 2022 04:03:30 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Jul 2022 04:03:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Jul 2022 04:03:31 GMT
WORKDIR /var/www/html
# Tue, 19 Jul 2022 04:03:33 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 19 Jul 2022 04:03:33 GMT
STOPSIGNAL SIGQUIT
# Tue, 19 Jul 2022 04:03:34 GMT
EXPOSE 9000
# Tue, 19 Jul 2022 04:03:34 GMT
CMD ["php-fpm"]
# Tue, 19 Jul 2022 06:34:45 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Tue, 19 Jul 2022 06:37:02 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 19 Jul 2022 06:37:05 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 19 Jul 2022 06:37:06 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 19 Jul 2022 06:37:15 GMT
RUN set -eux; 	version='6.0.1'; 	sha1='a1c02b6b754d74c08a70d5a8b604bdb72f1b276a'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Tue, 19 Jul 2022 06:37:16 GMT
VOLUME [/var/www/html]
# Tue, 19 Jul 2022 06:37:16 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Tue, 19 Jul 2022 06:37:17 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Tue, 19 Jul 2022 06:37:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 06:37:18 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b7885075fcd06a866d12dfd56eb704045eaadbd22dc03a224cd98715be566677`  
		Last Modified: Mon, 18 Jul 2022 19:08:42 GMT  
		Size: 2.6 MB (2606431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f3a20f98c3862e8b151953d654ed54191d3b27050e2581dffbfb6e8c9137978`  
		Last Modified: Tue, 19 Jul 2022 04:19:22 GMT  
		Size: 1.7 MB (1693959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2b70338f2368181e0f61f4907a974178bd8b93cdf93d44a432380e99c5d154`  
		Last Modified: Tue, 19 Jul 2022 04:19:21 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f0a1e200dbbea4736643651e71bfdcf1414cc80f1047b39f7d6732be05ff46a`  
		Last Modified: Tue, 19 Jul 2022 04:19:21 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36eb5ea720841366892ab8b1b9f845918ff958d0765ddca92a4053f5f4eaeedc`  
		Last Modified: Tue, 19 Jul 2022 04:26:11 GMT  
		Size: 10.4 MB (10439064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:178e2607b4ea7a6d804d57ccc121695776ed6ad645d79fd21f224839a8b3e53f`  
		Last Modified: Tue, 19 Jul 2022 04:26:08 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58ecb4ee0a044a259b43eb5fd9db13f7c3eb73a9da740e252cd388e91ae70ced`  
		Last Modified: Tue, 19 Jul 2022 04:27:17 GMT  
		Size: 10.7 MB (10723563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2881dd3b5f0281d5d9c7c1257be3aa26a93f013aa796d2dd7284971a90f2de8`  
		Last Modified: Tue, 19 Jul 2022 04:27:09 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62b4d33ec72613dd0f3c98fe6c5e6a56f96d93d3db079bba3e1ee443b3afbf4f`  
		Last Modified: Tue, 19 Jul 2022 04:27:09 GMT  
		Size: 18.4 KB (18376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d270e0ed9a558af8298dbeaa0cbff244c675782d97aead78e1dee12bee8ac9d`  
		Last Modified: Tue, 19 Jul 2022 04:27:09 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73c9590b4a6bc3d7e7ceddc26366b6615761b4adc624b44bdd01889e111f0ce0`  
		Last Modified: Tue, 19 Jul 2022 06:55:28 GMT  
		Size: 43.3 MB (43271360 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1f821416853bf0cd8ec0282f11db64ed56a2266572e5467c83ef30661bdd61`  
		Last Modified: Tue, 19 Jul 2022 06:55:04 GMT  
		Size: 4.0 MB (4042235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76106d6e83c1e24d92aa641a940cb884f8a1336b7dec66b2617355d9d1b3ced9`  
		Last Modified: Tue, 19 Jul 2022 06:54:59 GMT  
		Size: 65.5 KB (65506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3d9fff93b747a857d7281289e40b7065c77bccbbf872cc35062a87665df8ab3`  
		Last Modified: Tue, 19 Jul 2022 06:54:59 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a75be0e9e0cc933fe6fa491d0cb10daa42a1539316db7e11b5cb66e32bb0f35`  
		Last Modified: Tue, 19 Jul 2022 06:55:14 GMT  
		Size: 21.0 MB (20994683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:401ad1391da3bc1bca7f04780a4ad9294d25c3d10cf84c9001f44aa8227407e0`  
		Last Modified: Tue, 19 Jul 2022 06:54:59 GMT  
		Size: 2.3 KB (2334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3cd657c18cee9daf860a1268acdb1099fca3562458b8f15bf6fdd9c9f8df28`  
		Last Modified: Tue, 19 Jul 2022 06:54:59 GMT  
		Size: 1.7 KB (1730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:6-fpm-alpine` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:dc51aeeab3f77183e7241309b75c626e38560b13808f82499ac5dba8b199168a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **90.7 MB (90687247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53cf58ae31f7084e3b6ed92b326f94663cba5af98661749111e7f0a05b53024a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 19:01:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 19:01:25 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 19:01:27 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 19:01:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 19:01:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 19:01:30 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:01:30 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:01:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 19:36:20 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 10 Jun 2022 01:05:52 GMT
ENV PHP_VERSION=7.4.30
# Fri, 10 Jun 2022 01:05:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Fri, 10 Jun 2022 01:05:53 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Fri, 10 Jun 2022 01:06:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 10 Jun 2022 01:06:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 10 Jun 2022 01:15:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 10 Jun 2022 01:15:37 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 10 Jun 2022 01:15:39 GMT
RUN docker-php-ext-enable sodium
# Fri, 10 Jun 2022 01:15:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 10 Jun 2022 01:15:40 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 01:15:42 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 10 Jun 2022 01:15:43 GMT
STOPSIGNAL SIGQUIT
# Fri, 10 Jun 2022 01:15:43 GMT
EXPOSE 9000
# Fri, 10 Jun 2022 01:15:44 GMT
CMD ["php-fpm"]
# Fri, 10 Jun 2022 11:50:35 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 10 Jun 2022 11:52:43 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 10 Jun 2022 11:52:46 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 10 Jun 2022 11:52:47 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 14 Jul 2022 03:49:46 GMT
RUN set -eux; 	version='6.0.1'; 	sha1='a1c02b6b754d74c08a70d5a8b604bdb72f1b276a'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Thu, 14 Jul 2022 03:49:47 GMT
VOLUME [/var/www/html]
# Thu, 14 Jul 2022 03:49:47 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Thu, 14 Jul 2022 03:49:48 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 14 Jul 2022 03:49:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Jul 2022 03:49:49 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a68c4c667bd6865eca9aa9f496ecc527223b3162b260cad2e40c45ad49edc479`  
		Last Modified: Wed, 25 May 2022 20:09:19 GMT  
		Size: 1.6 MB (1560829 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da6bb9188dd796f59353a38be6412d00920f7c1da1effa359dc5c9a5724c0fb0`  
		Last Modified: Wed, 25 May 2022 20:09:18 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adbde557014a2ec2c7a2e22a836cdf6978cf4aaea9b738859980a1d98c9b1282`  
		Last Modified: Wed, 25 May 2022 20:09:18 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f55f45c8735a38d4ce9c757dc54208b5b5c6fd108e857819adad578690a3533`  
		Last Modified: Fri, 10 Jun 2022 02:23:31 GMT  
		Size: 10.4 MB (10439057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee24507d8c8a92ea45eb3d59d63701f8fbb127ec5c817f39785660038e5d2959`  
		Last Modified: Fri, 10 Jun 2022 02:23:28 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b6ff04d51566ad04878ad85f1795c9756b5ceaf7cb5dfd69fef639fcd910e38`  
		Last Modified: Fri, 10 Jun 2022 02:24:35 GMT  
		Size: 10.1 MB (10089688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2a5b5fa3d6b58501df3e0a01891794cc166e39bae408bd98d5199e980003c1`  
		Last Modified: Fri, 10 Jun 2022 02:24:28 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23120e785cdf070ae5b689e3533e35ea33c93ccd3146511b9a1ab4f1b039434b`  
		Last Modified: Fri, 10 Jun 2022 02:24:28 GMT  
		Size: 18.3 KB (18332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b67103336ca42956fa4d06b1af2fd84c618526f1bc4921e829bb361237179f3`  
		Last Modified: Fri, 10 Jun 2022 02:24:29 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2094be002fdd634c65d4de9d9f2422929d5d3fbb63aad3c7ec6f82d3887bc1e2`  
		Last Modified: Fri, 10 Jun 2022 12:34:07 GMT  
		Size: 41.2 MB (41240787 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db78c80e30449430ea5673247b0fe1cfcf057fb6ef53c417e77410b0740c1d0e`  
		Last Modified: Fri, 10 Jun 2022 12:33:46 GMT  
		Size: 3.8 MB (3849363 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:160f7b21c037356308b2cd26d2064c673e8df439743ff7d2b98c26b3d96f7b70`  
		Last Modified: Fri, 10 Jun 2022 12:33:42 GMT  
		Size: 65.4 KB (65449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e99953247a8e5fa06f3feefc816ad964ed5a9b0bcb3a31a5e3ffdb035573989`  
		Last Modified: Fri, 10 Jun 2022 12:33:42 GMT  
		Size: 395.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1191687ee4f1383b733148cae5c6250523b0a05414431cd72db3f922084190a8`  
		Last Modified: Thu, 14 Jul 2022 04:17:26 GMT  
		Size: 21.0 MB (20994696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a2f9235a4afde41076406146b56c1686e9d457359018699cdccf09e2bca59b6`  
		Last Modified: Thu, 14 Jul 2022 04:17:11 GMT  
		Size: 2.3 KB (2344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0fe08a674eb1597b69d3f72f5e343dcb57a591d863d8dc8fdd7f757b6d2ab02`  
		Last Modified: Thu, 14 Jul 2022 04:17:11 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:6-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:8a2d5a020692a92bc5ef87b558eeac5f48a2c7c3c8f1d1ea5cae4aa7da9b0646
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.6 MB (97588172 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f34897d95e52941aeec5af4ca1c080f03446e1de07eff901bb01dd1361b64530`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 18 Jul 2022 21:57:05 GMT
ADD file:9ccb70abba88b6de789b29f17770246f765ffbb072fe598580bfc29ce3213f1c in / 
# Mon, 18 Jul 2022 21:57:05 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 03:14:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 19 Jul 2022 03:14:57 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 19 Jul 2022 03:14:58 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 19 Jul 2022 03:14:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 19 Jul 2022 03:15:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 19 Jul 2022 03:15:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 19 Jul 2022 03:15:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 19 Jul 2022 03:15:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 19 Jul 2022 04:06:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 19 Jul 2022 04:06:20 GMT
ENV PHP_VERSION=7.4.30
# Tue, 19 Jul 2022 04:06:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Tue, 19 Jul 2022 04:06:22 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Tue, 19 Jul 2022 04:06:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 19 Jul 2022 04:06:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Jul 2022 04:13:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Jul 2022 04:13:56 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 19 Jul 2022 04:13:57 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Jul 2022 04:13:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Jul 2022 04:13:59 GMT
WORKDIR /var/www/html
# Tue, 19 Jul 2022 04:14:00 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 19 Jul 2022 04:14:01 GMT
STOPSIGNAL SIGQUIT
# Tue, 19 Jul 2022 04:14:02 GMT
EXPOSE 9000
# Tue, 19 Jul 2022 04:14:03 GMT
CMD ["php-fpm"]
# Tue, 19 Jul 2022 07:12:11 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Tue, 19 Jul 2022 07:13:09 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 19 Jul 2022 07:13:10 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 19 Jul 2022 07:13:11 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 19 Jul 2022 07:13:15 GMT
RUN set -eux; 	version='6.0.1'; 	sha1='a1c02b6b754d74c08a70d5a8b604bdb72f1b276a'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Tue, 19 Jul 2022 07:13:15 GMT
VOLUME [/var/www/html]
# Tue, 19 Jul 2022 07:13:17 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Tue, 19 Jul 2022 07:13:18 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Tue, 19 Jul 2022 07:13:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 07:13:19 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f97344484467e4c4ebb85aae724170073799295a3442c50ab532e249bd27b412`  
		Last Modified: Mon, 18 Jul 2022 19:08:29 GMT  
		Size: 2.7 MB (2694720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09e5d6c316a066af896390af8c46674b59f76a8a7944d745d97f07baa51331e9`  
		Last Modified: Tue, 19 Jul 2022 04:26:56 GMT  
		Size: 1.7 MB (1704103 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e91bb00cf3b67a671a451b05b313e1cdf88da5050cc552ebd31cac2cf9ee7fb6`  
		Last Modified: Tue, 19 Jul 2022 04:26:55 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96d399c457bfcaf74cbdbcb45d847f80dab959ac4d6106cf448656b5a4d0ee09`  
		Last Modified: Tue, 19 Jul 2022 04:26:55 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1ab6bf4612b9e5b5dc5a9f422538d1e855809d5ed4f38f5119bef0d600b7349`  
		Last Modified: Tue, 19 Jul 2022 04:33:20 GMT  
		Size: 10.4 MB (10438832 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68151d5dfc7365352aa38fe0d25ac1c920f2f16bcae62800022a46514444e25b`  
		Last Modified: Tue, 19 Jul 2022 04:33:19 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7553bbb85bd8d554d7a6ed6d4944651bc5bf0a0b28139cab280d6ea75fbeb939`  
		Last Modified: Tue, 19 Jul 2022 04:34:16 GMT  
		Size: 11.3 MB (11284120 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dddc53836e1a3d317eda48fc423141ff93ec43a73be4e54bf72d494b8bcad33f`  
		Last Modified: Tue, 19 Jul 2022 04:34:14 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b25bdb10f8542486a1997accbd518fec05f62635f7edc81e21e8e76ccef8e75`  
		Last Modified: Tue, 19 Jul 2022 04:34:14 GMT  
		Size: 18.3 KB (18281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b012eb8681c3139b551ec433f22ae3a07ddecebe06b7a6a333a2746470fabab`  
		Last Modified: Tue, 19 Jul 2022 04:34:14 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:359d76cb633d4df606fb5782676c48e871079e70c29367fc8e7654fabb73fcd7`  
		Last Modified: Tue, 19 Jul 2022 07:23:49 GMT  
		Size: 46.1 MB (46101188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5a99e6a974ead9de1e7436ec24531ae474bcf85691172833014dc385f692cf0`  
		Last Modified: Tue, 19 Jul 2022 07:23:43 GMT  
		Size: 4.3 MB (4267531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:852341ff5685baecfdb9800ad8ae209bcd2d3a204c47dfb7d4838f051487ffbd`  
		Last Modified: Tue, 19 Jul 2022 07:23:40 GMT  
		Size: 65.4 KB (65403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2c784082ebe78b7b6939e3f7c13ab4f6a1e546b039328c608acaf792aa50f9`  
		Last Modified: Tue, 19 Jul 2022 07:23:40 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c08050ba55b0999e984c4cbf54407524e991d3b06f73172e7574d1830ea98db`  
		Last Modified: Tue, 19 Jul 2022 07:23:44 GMT  
		Size: 21.0 MB (20996697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514a74be7a93c5c3651c740ab30f0f2464547878683ae7a47a28bbf6a0b7d52f`  
		Last Modified: Tue, 19 Jul 2022 07:23:40 GMT  
		Size: 2.3 KB (2336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ccc6deb1a43692823609d8cf8819490c9fa1acbc01aab21fad8ed25b5975e2`  
		Last Modified: Tue, 19 Jul 2022 07:23:40 GMT  
		Size: 1.7 KB (1726 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:6-fpm-alpine` - linux; 386

```console
$ docker pull wordpress@sha256:4896912ca0c0c39626bc5dfd7c8e3d19ca84b17ed43ac0e031f73e24a3e9090a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **98.7 MB (98712433 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6407409005b63bcf1cbf4796c87a1e0ce3aea53503034757787f3ecf2482ccbb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 21:41:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Mon, 18 Jul 2022 21:41:31 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Mon, 18 Jul 2022 21:41:32 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Mon, 18 Jul 2022 21:41:33 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 18 Jul 2022 21:41:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Mon, 18 Jul 2022 21:41:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 Jul 2022 21:41:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 18 Jul 2022 21:41:37 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 18 Jul 2022 22:22:31 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Mon, 18 Jul 2022 22:22:31 GMT
ENV PHP_VERSION=7.4.30
# Mon, 18 Jul 2022 22:22:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Mon, 18 Jul 2022 22:22:33 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Mon, 18 Jul 2022 22:22:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Mon, 18 Jul 2022 22:22:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 18 Jul 2022 22:29:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 18 Jul 2022 22:30:01 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 18 Jul 2022 22:30:01 GMT
RUN docker-php-ext-enable sodium
# Mon, 18 Jul 2022 22:30:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 18 Jul 2022 22:30:03 GMT
WORKDIR /var/www/html
# Mon, 18 Jul 2022 22:30:04 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Mon, 18 Jul 2022 22:30:05 GMT
STOPSIGNAL SIGQUIT
# Mon, 18 Jul 2022 22:30:06 GMT
EXPOSE 9000
# Mon, 18 Jul 2022 22:30:07 GMT
CMD ["php-fpm"]
# Tue, 19 Jul 2022 03:22:35 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Tue, 19 Jul 2022 03:23:26 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 19 Jul 2022 03:23:27 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 19 Jul 2022 03:23:28 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 19 Jul 2022 03:23:32 GMT
RUN set -eux; 	version='6.0.1'; 	sha1='a1c02b6b754d74c08a70d5a8b604bdb72f1b276a'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Tue, 19 Jul 2022 03:23:32 GMT
VOLUME [/var/www/html]
# Tue, 19 Jul 2022 03:23:34 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Tue, 19 Jul 2022 03:23:35 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Tue, 19 Jul 2022 03:23:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 03:23:36 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b497c2c5ebbc20f14d6736375ca0223ad07215dcc8af96c5bbce7c290f69ea2a`  
		Last Modified: Mon, 18 Jul 2022 22:43:39 GMT  
		Size: 1.8 MB (1808030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cce9082517109c8caf9a17724781a05e7c300af26cb96f1a17a34b407ec5354`  
		Last Modified: Mon, 18 Jul 2022 22:43:38 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11354c8cb04ba6f087c3a31b39b85cfce6d35433d6481e761df799bbbefae5a7`  
		Last Modified: Mon, 18 Jul 2022 22:43:38 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d50bb39b34fdeab1dbf20a25fbca9bc04d4861f0aed5d8d9ea45c0d0b852ec2`  
		Last Modified: Mon, 18 Jul 2022 22:50:13 GMT  
		Size: 10.4 MB (10438811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3167b372ebd0af0c05e19edbd61705af0992fab1848ad9d2d556c5f45b791166`  
		Last Modified: Mon, 18 Jul 2022 22:50:11 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5972c8363379b666db84e65d56598940e2695dd123fb803316eb550f5a72e70a`  
		Last Modified: Mon, 18 Jul 2022 22:51:00 GMT  
		Size: 11.8 MB (11764513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1dccdb59a8f0d2ed751de48bac6fe57a0a8cb575da07604658ec60f54fa8036`  
		Last Modified: Mon, 18 Jul 2022 22:50:58 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4b70a815a00beaa30fb575b1ff4be5bfe141c1417159b064b5eab0d694c0073`  
		Last Modified: Mon, 18 Jul 2022 22:50:58 GMT  
		Size: 18.3 KB (18263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c49e8744efb0fbbc8e12ed10416be2c18ca07b80bcb691dd73213e77adc08dfc`  
		Last Modified: Mon, 18 Jul 2022 22:50:58 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82b99eaacf356ab78af8f060353aabff82dddf3eab06504b62f7ec3dc23af33a`  
		Last Modified: Tue, 19 Jul 2022 03:33:44 GMT  
		Size: 46.3 MB (46308939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2e1b31ac7e0e71cd347663f62899d4b8e144c6954d60cdf10567ab1110d8056`  
		Last Modified: Tue, 19 Jul 2022 03:33:37 GMT  
		Size: 4.5 MB (4492188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6b83e1b5232803abc7945f781cf7fca9feb5dc3c1c4914efd64bcaa43652826`  
		Last Modified: Tue, 19 Jul 2022 03:33:34 GMT  
		Size: 65.4 KB (65369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41e21d2c07fd0150192a77949293fe4a5786d4953ca2057d586b55ddda9e7f26`  
		Last Modified: Tue, 19 Jul 2022 03:33:34 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc89797fa6fec2f2b9e11d95d7aded98b8d10aee09ef81b2d10d8f3d63cce4ad`  
		Last Modified: Tue, 19 Jul 2022 03:33:37 GMT  
		Size: 21.0 MB (20996687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44387fbd126f42d164a1bddd21ef0eca032735c9878862bd31c5111600f72af9`  
		Last Modified: Tue, 19 Jul 2022 03:33:34 GMT  
		Size: 2.3 KB (2338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8533efa26ea3271b9333982776f1ba9e6061f6ed7561e33474479dec1ad6ce1`  
		Last Modified: Tue, 19 Jul 2022 03:33:34 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:6-fpm-alpine` - linux; ppc64le

```console
$ docker pull wordpress@sha256:3d4a3cc5487c5be2f5980e1d21f491c9cdd57c084c770c3c0a6e6ba3de0718bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.6 MB (105559710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e6da5d208d6d4a390d99ace74b16cdc49b5ccf03e17e652495cbcee04135f56`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 May 2022 19:16:51 GMT
ADD file:6a5450c8a7cee3ceda59e7cb350c54df4139b0f7b7cf49c8b31bb9c01646c3cd in / 
# Mon, 23 May 2022 19:16:53 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 19:57:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 19:57:35 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 19:57:43 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 19:57:45 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 19:57:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 19:57:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:57:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:57:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 20:39:29 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 10 Jun 2022 01:18:31 GMT
ENV PHP_VERSION=7.4.30
# Fri, 10 Jun 2022 01:18:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Fri, 10 Jun 2022 01:18:36 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Fri, 10 Jun 2022 01:18:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 10 Jun 2022 01:18:55 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 10 Jun 2022 01:30:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 10 Jun 2022 01:30:22 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 10 Jun 2022 01:30:30 GMT
RUN docker-php-ext-enable sodium
# Fri, 10 Jun 2022 01:30:36 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 10 Jun 2022 01:30:45 GMT
WORKDIR /var/www/html
# Fri, 10 Jun 2022 01:31:02 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 10 Jun 2022 01:31:10 GMT
STOPSIGNAL SIGQUIT
# Fri, 10 Jun 2022 01:31:14 GMT
EXPOSE 9000
# Fri, 10 Jun 2022 01:31:19 GMT
CMD ["php-fpm"]
# Fri, 10 Jun 2022 13:52:20 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 10 Jun 2022 13:53:57 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 10 Jun 2022 13:54:22 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 10 Jun 2022 13:54:36 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Wed, 13 Jul 2022 20:41:56 GMT
RUN set -eux; 	version='6.0.1'; 	sha1='a1c02b6b754d74c08a70d5a8b604bdb72f1b276a'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Wed, 13 Jul 2022 20:42:05 GMT
VOLUME [/var/www/html]
# Wed, 13 Jul 2022 20:42:07 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Wed, 13 Jul 2022 20:42:09 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Wed, 13 Jul 2022 20:42:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 13 Jul 2022 20:42:16 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d3deabf2a506ef6f5fa7c2a68bf27047574cef9908b30a97ff2d01ae539b089a`  
		Last Modified: Mon, 23 May 2022 19:09:13 GMT  
		Size: 2.8 MB (2789745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1091cbad9101b41d3fd65de74d3265b02346722f13f77c4a456e33979dd226da`  
		Last Modified: Wed, 25 May 2022 21:08:36 GMT  
		Size: 1.8 MB (1759345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:570e34510ef12ed73f2ed4ab7167c3408a7a0c69498928d0be0c6d46e2250ea3`  
		Last Modified: Wed, 25 May 2022 21:08:35 GMT  
		Size: 1.3 KB (1265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcbd0bbe87c55d5c71424cd10832856ec6580b2de2bf35112f9a41f574cef70f`  
		Last Modified: Wed, 25 May 2022 21:08:35 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1f0aa6f687f35037b93a837f89277971563112819d3690f0c0eea4c12004a26`  
		Last Modified: Fri, 10 Jun 2022 02:26:45 GMT  
		Size: 10.4 MB (10439069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061f5766accc0f414923ec7aa7f6a287b61aebbfec3a3d3ac134d3e133751423`  
		Last Modified: Fri, 10 Jun 2022 02:26:44 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f434232a81894400b6bd5fa5d13479882ef5922ead51fad6c9b3d24f2e759cf2`  
		Last Modified: Fri, 10 Jun 2022 02:27:41 GMT  
		Size: 12.2 MB (12216355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd85c32209bec5cf962ed8b87f509a25dcf5b188904d37a8a506af31c1b2821`  
		Last Modified: Fri, 10 Jun 2022 02:27:38 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6471f7601dc079aebc4080a667ced2cef6a865ea658b559d8e27a0996bdcb421`  
		Last Modified: Fri, 10 Jun 2022 02:27:38 GMT  
		Size: 18.3 KB (18341 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a6724421624336036837135c2774bf822d0df0e3c91f1e221f702f4dc0b099a`  
		Last Modified: Fri, 10 Jun 2022 02:27:39 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee2d039d60c79042373b032672ddb80066f90c8f19ad25cd6084db5f396dce`  
		Last Modified: Fri, 10 Jun 2022 15:06:59 GMT  
		Size: 52.8 MB (52759041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb5d6df5bde365c1217912b0201c39cfdbe3b8951c8c4ca4cd857c324810c27`  
		Last Modified: Fri, 10 Jun 2022 15:06:38 GMT  
		Size: 4.5 MB (4500242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d65f3c53f77ae71385cf3a621530d561a37f03197297db337d826f78cdb4555f`  
		Last Modified: Fri, 10 Jun 2022 15:06:32 GMT  
		Size: 65.5 KB (65472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162c131eb1be9879ec7a3f0e507438d8194318a829ff3289766e23cdde87daf5`  
		Last Modified: Fri, 10 Jun 2022 15:06:32 GMT  
		Size: 397.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce485d47ffa5ad958a768af13c0e70be68b3e7eeeb9449f35f71e031bcf4ef09`  
		Last Modified: Wed, 13 Jul 2022 21:39:04 GMT  
		Size: 21.0 MB (20994697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02a11d8e71e0dd42f53ba244fd0bf6d127cd3ecac705eb0a34a793a9879759af`  
		Last Modified: Wed, 13 Jul 2022 21:39:01 GMT  
		Size: 2.3 KB (2345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa71ba2976d61d3bbacf787dd71bd64264654655f507523fbc3f3a3625ae0b28`  
		Last Modified: Wed, 13 Jul 2022 21:39:00 GMT  
		Size: 1.7 KB (1737 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:6-fpm-alpine` - linux; s390x

```console
$ docker pull wordpress@sha256:9ac61dcf2e7fba3361d6cda22b363b79437175092ededc22c28f56fb284611bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **89.3 MB (89265101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7df686e88b39c039a2e45506aca8ddee5ad6a307ee7a037b5dd43f1c0848871d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 18 Jul 2022 20:41:35 GMT
ADD file:deaa573cd61e07709846a5300fb627a8610e9754129c085ed483ff8897d0c002 in / 
# Mon, 18 Jul 2022 20:41:36 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 02:11:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 19 Jul 2022 02:11:25 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 19 Jul 2022 02:11:27 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 19 Jul 2022 02:11:28 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 19 Jul 2022 02:11:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 19 Jul 2022 02:11:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 19 Jul 2022 02:11:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 19 Jul 2022 02:11:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 19 Jul 2022 03:04:22 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Tue, 19 Jul 2022 03:04:23 GMT
ENV PHP_VERSION=7.4.30
# Tue, 19 Jul 2022 03:04:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.30.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.30.tar.xz.asc
# Tue, 19 Jul 2022 03:04:24 GMT
ENV PHP_SHA256=ea72a34f32c67e79ac2da7dfe96177f3c451c3eefae5810ba13312ed398ba70d
# Tue, 19 Jul 2022 03:04:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Tue, 19 Jul 2022 03:04:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 19 Jul 2022 03:14:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 	ln -sv /usr/include/gnu-libiconv/*.h /usr/include/; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 19 Jul 2022 03:14:20 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 19 Jul 2022 03:14:22 GMT
RUN docker-php-ext-enable sodium
# Tue, 19 Jul 2022 03:14:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 19 Jul 2022 03:14:22 GMT
WORKDIR /var/www/html
# Tue, 19 Jul 2022 03:14:23 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 19 Jul 2022 03:14:23 GMT
STOPSIGNAL SIGQUIT
# Tue, 19 Jul 2022 03:14:23 GMT
EXPOSE 9000
# Tue, 19 Jul 2022 03:14:24 GMT
CMD ["php-fpm"]
# Tue, 19 Jul 2022 09:01:08 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Tue, 19 Jul 2022 09:02:07 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Tue, 19 Jul 2022 09:02:10 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 19 Jul 2022 09:02:11 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Tue, 19 Jul 2022 09:02:18 GMT
RUN set -eux; 	version='6.0.1'; 	sha1='a1c02b6b754d74c08a70d5a8b604bdb72f1b276a'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 777 wp-content
# Tue, 19 Jul 2022 09:02:22 GMT
VOLUME [/var/www/html]
# Tue, 19 Jul 2022 09:02:23 GMT
COPY --chown=www-data:www-datafile:f95ddeaad9b50ddddf288560052a9de4f33fa6297ea70870e396f6d99c482b7a in /usr/src/wordpress/ 
# Tue, 19 Jul 2022 09:02:23 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Tue, 19 Jul 2022 09:02:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Jul 2022 09:02:24 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5f1840d5bacf4162a87f497e22d94bce946e660bdfce8eeefcbf7bd0beb193f3`  
		Last Modified: Mon, 18 Jul 2022 20:42:36 GMT  
		Size: 2.6 MB (2580798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9842ade5e34b07c420965519970b802ea9e999bc04dc2757c682c4fcdb9a105`  
		Last Modified: Tue, 19 Jul 2022 03:30:23 GMT  
		Size: 1.8 MB (1766739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11189b7b565fb9039d6d93c6badbfaf6890f39532261d177b5352414b76fea65`  
		Last Modified: Tue, 19 Jul 2022 03:30:23 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36504c72275c98013fb2457e15e8efe23a0692912549611f4b044d0fcd9aec06`  
		Last Modified: Tue, 19 Jul 2022 03:30:23 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61af1dcb5b0ad8565d35413fb3f97c95c75b67934201b433d2ece265ac23c5b6`  
		Last Modified: Tue, 19 Jul 2022 03:36:06 GMT  
		Size: 10.4 MB (10439084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d078cf61f851e7dad3504dd4c6611f767118886201cbbfb81e05b4d0d9edf884`  
		Last Modified: Tue, 19 Jul 2022 03:36:06 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:780ebe36ebbc45dc46a570bd2f1c3ece332374d21725f8ec82674edadf05325f`  
		Last Modified: Tue, 19 Jul 2022 03:36:40 GMT  
		Size: 11.0 MB (11049781 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:683cd09cc7cbc09540d86becb0f62e1b7caaf0b8953743cb3a42cb76fc4c999b`  
		Last Modified: Tue, 19 Jul 2022 03:36:39 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e875885614cd1b42588318ca786ed582d1ebd9ad038e5b7c68f9a7133474ac62`  
		Last Modified: Tue, 19 Jul 2022 03:36:38 GMT  
		Size: 18.4 KB (18392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78c6e49538cc62c1a38dc0095fe810008f870c9e8401a6d993d690828abfc71c`  
		Last Modified: Tue, 19 Jul 2022 03:36:38 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:842f81a7c98521832df491a8a545eb7469b94f60e0f42a9594f2f8efbebe7927`  
		Last Modified: Tue, 19 Jul 2022 09:14:59 GMT  
		Size: 38.0 MB (37981347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10fd9668d96ad517a9c3683b88f805e318fbd9e3f6fe2b645a9ae55e4236c0b6`  
		Last Modified: Tue, 19 Jul 2022 09:14:55 GMT  
		Size: 4.4 MB (4357534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f34f8b99b63dad65a9373c79964027140d63467c1f1c0181ebaa70c0da943dd`  
		Last Modified: Tue, 19 Jul 2022 09:14:53 GMT  
		Size: 59.4 KB (59376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:760e128ceca09af7803e3db9e6fab4ef268501eb93ec048ad8d1b97aececba54`  
		Last Modified: Tue, 19 Jul 2022 09:14:53 GMT  
		Size: 387.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a98dd41df9cca5dcebaddb6282e2d3080cc0d7a0d5435da79eba4a5bc3b7a882`  
		Last Modified: Tue, 19 Jul 2022 09:14:55 GMT  
		Size: 21.0 MB (20994684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcd64a9b60cdb5b6472798f770795006a3b221ae156c256a5156ae82ff0466d4`  
		Last Modified: Tue, 19 Jul 2022 09:14:53 GMT  
		Size: 2.3 KB (2339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f32488e8686b553a55716a9bc664f38d65d017d6e8bd293e93ccf1c7ee8fe699`  
		Last Modified: Tue, 19 Jul 2022 09:14:53 GMT  
		Size: 1.7 KB (1728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
