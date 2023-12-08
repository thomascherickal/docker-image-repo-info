## `wordpress:php8.3-fpm-alpine`

```console
$ docker pull wordpress@sha256:de660bb2505879dcaa4422d6ac2c855176745a8ddf6669572e7da22a31564399
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

### `wordpress:php8.3-fpm-alpine` - linux; amd64

```console
$ docker pull wordpress@sha256:47bd6f68510bf165b47ca4fdce6e7d06b59e39aa52434915c7c0376487f96b69
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105284843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db1bf1684660c705e531fc08f478fb0ac1faf42b0c3a4572c892c082cf5211e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Thu, 30 Nov 2023 23:32:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 30 Nov 2023 23:32:53 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 30 Nov 2023 23:32:53 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 30 Nov 2023 23:32:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 30 Nov 2023 23:32:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 30 Nov 2023 23:32:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 30 Nov 2023 23:32:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 30 Nov 2023 23:32:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 30 Nov 2023 23:32:54 GMT
ENV GPG_KEYS=1198C0117593497A5EC5C199286AF1F9897469DC C28D937575603EB4ABB725861C0779DC5C0A9DE4 AFD8691FDAEDF03BDF6E460563F15A9B715376CA
# Thu, 30 Nov 2023 23:32:54 GMT
ENV PHP_VERSION=8.3.0
# Thu, 30 Nov 2023 23:32:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.3.0.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.3.0.tar.xz.asc
# Thu, 30 Nov 2023 23:32:55 GMT
ENV PHP_SHA256=1db84fec57125aa93638b51bb2b15103e12ac196e2f960f0d124275b2687ea54
# Thu, 30 Nov 2023 23:33:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 30 Nov 2023 23:33:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 30 Nov 2023 23:40:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 30 Nov 2023 23:40:16 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 30 Nov 2023 23:40:17 GMT
RUN docker-php-ext-enable sodium
# Thu, 30 Nov 2023 23:40:17 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 30 Nov 2023 23:40:17 GMT
WORKDIR /var/www/html
# Thu, 30 Nov 2023 23:40:17 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 30 Nov 2023 23:40:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Nov 2023 23:40:18 GMT
EXPOSE 9000
# Thu, 30 Nov 2023 23:40:18 GMT
CMD ["php-fpm"]
# Fri, 01 Dec 2023 02:51:13 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 01 Dec 2023 02:52:59 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 01 Dec 2023 02:53:01 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 01 Dec 2023 02:53:01 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Dec 2023 22:28:06 GMT
RUN set -eux; 	version='6.4.2'; 	sha1='d1aedbfea77b243b09e0ab05b100b782497406dd'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 07 Dec 2023 22:28:06 GMT
VOLUME [/var/www/html]
# Thu, 07 Dec 2023 22:28:07 GMT
COPY --chown=www-data:www-datafile:428b392bbc74b7aa0266d0b70812aab289561b5840fddd951986ac44165a331d in /usr/src/wordpress/ 
# Thu, 07 Dec 2023 22:28:07 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Dec 2023 22:28:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:28:07 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8e26b626c27026d1938a0b6bd77e36b4113da4b7a1134df8d1aa9f49658b25f`  
		Last Modified: Fri, 01 Dec 2023 00:42:07 GMT  
		Size: 2.7 MB (2679359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23427f6f19cc27aa3496173559d7fc30c2501d1d179a15b52ac1758cc1667d37`  
		Last Modified: Fri, 01 Dec 2023 00:42:07 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938ee652f0dd66c081c31e773163d4c3d8ec979f9ced384ed270cdc5fbcbe657`  
		Last Modified: Fri, 01 Dec 2023 00:42:07 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8abe2aaf4047e9984223c8d63be88c09b7d447f8c9f77851aa06771c52bba05b`  
		Last Modified: Fri, 01 Dec 2023 00:42:04 GMT  
		Size: 12.5 MB (12452105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e06ec6f102433dfe7410990547f8d059d4c3e56455e35d7b4dfbfb96784486e1`  
		Last Modified: Fri, 01 Dec 2023 00:42:04 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:412745adb586396a351d94331d2ebad683acb437e24d8a56293ecbd1cbe51b67`  
		Last Modified: Fri, 01 Dec 2023 00:42:47 GMT  
		Size: 12.9 MB (12924042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9e550534acfa15f459cf9f1e2483785ab59569e89f61a59cef618fd951cdaf8`  
		Last Modified: Fri, 01 Dec 2023 00:42:45 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4976c3e028d8a74493ea1bf801742f3a8941af58d12f1ef3f400ef918a7d0ac1`  
		Last Modified: Fri, 01 Dec 2023 00:42:45 GMT  
		Size: 19.0 KB (18951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd54681fabf784342374885c09181f306c26d2a2be3ee0328588c720ce5e0fb6`  
		Last Modified: Fri, 01 Dec 2023 00:42:45 GMT  
		Size: 9.2 KB (9178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9ceca3d52f135b83f8ece2d794c89d7a89faede432b996672297f682a8006c`  
		Last Modified: Fri, 01 Dec 2023 02:59:34 GMT  
		Size: 45.1 MB (45053506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067f7df83c31a0b27e735e80ee0db168fb616f8e65d446dc261dde0616f3a76a`  
		Last Modified: Fri, 01 Dec 2023 02:59:29 GMT  
		Size: 4.4 MB (4360334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a975675946149e50dd34c7ced48a16f7d36be8d926dc7c6a85f2212388ba209`  
		Last Modified: Fri, 01 Dec 2023 02:59:26 GMT  
		Size: 66.2 KB (66224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b9322d26b59f55c44aa198b776c994f13e1adf897cb9bbeff46bfa445b7020f`  
		Last Modified: Fri, 01 Dec 2023 02:59:26 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c39582c0be73176410373fb69a3af55f366b04c0d47194dbc0870616f9b1943`  
		Last Modified: Thu, 07 Dec 2023 22:32:39 GMT  
		Size: 24.3 MB (24309779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fc3cf56fa406b1873f2c462d580f779aba02f0c50363ae3fa6f8975d6c0545`  
		Last Modified: Thu, 07 Dec 2023 22:32:35 GMT  
		Size: 2.3 KB (2348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fba8dec8eb78081358fca7944d152153570af5af20e2da5e973be9cd52594db2`  
		Last Modified: Thu, 07 Dec 2023 22:32:36 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.3-fpm-alpine` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:6558989fafc09e5826dd969cebdbd970ff42d322c762dccfc5c56ecf794a87f9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.6 MB (99550104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fccbd4cd5bebad330148ae038dae9345e5d7ad27d081bc7b055361b3a6bc43a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:18 GMT
ADD file:dbf65487d049081dc2d39b3d99d2c64b6c89754e7e2996a46169d3512e59f32a in / 
# Thu, 30 Nov 2023 22:49:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Nov 2023 23:15:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 30 Nov 2023 23:15:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 30 Nov 2023 23:15:35 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 30 Nov 2023 23:15:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 30 Nov 2023 23:15:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 30 Nov 2023 23:15:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 30 Nov 2023 23:15:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 30 Nov 2023 23:15:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 30 Nov 2023 23:15:36 GMT
ENV GPG_KEYS=1198C0117593497A5EC5C199286AF1F9897469DC C28D937575603EB4ABB725861C0779DC5C0A9DE4 AFD8691FDAEDF03BDF6E460563F15A9B715376CA
# Thu, 30 Nov 2023 23:15:36 GMT
ENV PHP_VERSION=8.3.0
# Thu, 30 Nov 2023 23:15:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.3.0.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.3.0.tar.xz.asc
# Thu, 30 Nov 2023 23:15:36 GMT
ENV PHP_SHA256=1db84fec57125aa93638b51bb2b15103e12ac196e2f960f0d124275b2687ea54
# Thu, 30 Nov 2023 23:15:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 30 Nov 2023 23:15:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 30 Nov 2023 23:22:58 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 30 Nov 2023 23:22:58 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 30 Nov 2023 23:22:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 30 Nov 2023 23:22:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 30 Nov 2023 23:23:00 GMT
WORKDIR /var/www/html
# Thu, 30 Nov 2023 23:23:00 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 30 Nov 2023 23:23:00 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Nov 2023 23:23:00 GMT
EXPOSE 9000
# Thu, 30 Nov 2023 23:23:00 GMT
CMD ["php-fpm"]
# Fri, 01 Dec 2023 12:16:06 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 01 Dec 2023 12:17:00 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 01 Dec 2023 12:17:01 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 01 Dec 2023 12:17:02 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Dec 2023 21:51:56 GMT
RUN set -eux; 	version='6.4.2'; 	sha1='d1aedbfea77b243b09e0ab05b100b782497406dd'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 07 Dec 2023 21:51:56 GMT
VOLUME [/var/www/html]
# Thu, 07 Dec 2023 21:51:56 GMT
COPY --chown=www-data:www-datafile:428b392bbc74b7aa0266d0b70812aab289561b5840fddd951986ac44165a331d in /usr/src/wordpress/ 
# Thu, 07 Dec 2023 21:51:56 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:51:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:51:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:85ae953f9e6740471d4e1440b27721679dc7a511e112eb73df467a4cde26e421`  
		Last Modified: Thu, 30 Nov 2023 22:49:40 GMT  
		Size: 3.1 MB (3146870 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad3f4bb45cafc3a0c4349f9564390ff0fe5c2a3dc4287f0ddf3de8a86dcbb66`  
		Last Modified: Fri, 01 Dec 2023 00:15:00 GMT  
		Size: 2.7 MB (2685809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a06cb8c5272936441cf9c53173eed2af740b588b3a9d8bbbb0b6565f38005e36`  
		Last Modified: Fri, 01 Dec 2023 00:14:59 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6156dbc484960b6656a156d5d82d973371555039e45046b37e9af1cbfec8569`  
		Last Modified: Fri, 01 Dec 2023 00:14:59 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66811c19a32e40a429b8ba817b3ceb6493496ebd20655f68d5a7ca3844b6c96c`  
		Last Modified: Fri, 01 Dec 2023 00:14:59 GMT  
		Size: 12.5 MB (12452097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4954b5c64e0b15f09646882302df3b0ee246ee32b00519bd4e89f052587d473a`  
		Last Modified: Fri, 01 Dec 2023 00:14:57 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae54c46f81d563a28091f46a5723e8e9842c1f18c210b5c28f1c518ef67b30e9`  
		Last Modified: Fri, 01 Dec 2023 00:15:44 GMT  
		Size: 11.8 MB (11827883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b09b0d9432e283cf429d9a1ded0687c696c0d79b84dc8427596d4c9b84907bc`  
		Last Modified: Fri, 01 Dec 2023 00:15:41 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1833febc5b4fdab8914dd12872231a796572e5f4c32f533610921e74da2aa85a`  
		Last Modified: Fri, 01 Dec 2023 00:15:41 GMT  
		Size: 18.8 KB (18768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4cf5ea31d2b2a3f1c3cf4a6c58af49886d0f1fc444284563521f66b7a7615d5`  
		Last Modified: Fri, 01 Dec 2023 00:15:41 GMT  
		Size: 9.2 KB (9179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed39a82ce81b64b99865f89c44164c3367f601067f1c6d7d2aa87887c615be3`  
		Last Modified: Fri, 01 Dec 2023 12:21:47 GMT  
		Size: 40.9 MB (40855571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28fb2389fda801be9ef7af397e8cb7ef73511af84c042177cbd3a640cce658f6`  
		Last Modified: Fri, 01 Dec 2023 12:21:42 GMT  
		Size: 4.2 MB (4168976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91dcea41089d93afe2e43e8d4cad913aca9eabe66f70fde4aac39b127dc27b6f`  
		Last Modified: Fri, 01 Dec 2023 12:21:39 GMT  
		Size: 66.2 KB (66239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c018c1eec3e69e0eb7730d916847d4e171b64d7619543880ff0eedb7f9cc4c9`  
		Last Modified: Fri, 01 Dec 2023 12:21:39 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d268a4666f6afe6a079819776bfb92ccd98da0964577332214d2ac998e5b2d8b`  
		Last Modified: Thu, 07 Dec 2023 21:53:16 GMT  
		Size: 24.3 MB (24309764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b63c54957d66df63b4af14372baa7d85383235676dbcd240715cbdaa2ee0db3`  
		Last Modified: Thu, 07 Dec 2023 21:53:12 GMT  
		Size: 2.4 KB (2351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a6a2dec95fe7d5cbdfe82a8d2859fe5f3b8f224900bf3dd0cf46689ac73eaf9`  
		Last Modified: Thu, 07 Dec 2023 21:53:12 GMT  
		Size: 1.7 KB (1735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.3-fpm-alpine` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:a8d49cb8a62c0d29c5fa63b6277169006f7093a82782601732dd292ec8be7c10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **96.2 MB (96232382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:884a023bc1b3d671b9a2a1b211abbcfd7437ecffe6994a141891cd2f7d624615`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 30 Nov 2023 22:49:28 GMT
ADD file:dcb85d43d1fb96861612c42288878b13debfa9d0b956adea1f2472d0c50f0144 in / 
# Thu, 30 Nov 2023 22:49:29 GMT
CMD ["/bin/sh"]
# Thu, 30 Nov 2023 22:58:53 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 30 Nov 2023 22:58:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 30 Nov 2023 22:58:55 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 30 Nov 2023 22:58:55 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 30 Nov 2023 22:58:56 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 30 Nov 2023 22:58:56 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 30 Nov 2023 22:58:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 30 Nov 2023 22:58:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 30 Nov 2023 22:58:56 GMT
ENV GPG_KEYS=1198C0117593497A5EC5C199286AF1F9897469DC C28D937575603EB4ABB725861C0779DC5C0A9DE4 AFD8691FDAEDF03BDF6E460563F15A9B715376CA
# Thu, 30 Nov 2023 22:58:56 GMT
ENV PHP_VERSION=8.3.0
# Thu, 30 Nov 2023 22:58:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.3.0.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.3.0.tar.xz.asc
# Thu, 30 Nov 2023 22:58:56 GMT
ENV PHP_SHA256=1db84fec57125aa93638b51bb2b15103e12ac196e2f960f0d124275b2687ea54
# Thu, 30 Nov 2023 22:59:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 30 Nov 2023 22:59:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 30 Nov 2023 23:03:50 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 30 Nov 2023 23:03:51 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 30 Nov 2023 23:03:52 GMT
RUN docker-php-ext-enable sodium
# Thu, 30 Nov 2023 23:03:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 30 Nov 2023 23:03:52 GMT
WORKDIR /var/www/html
# Thu, 30 Nov 2023 23:03:52 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 30 Nov 2023 23:03:52 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Nov 2023 23:03:52 GMT
EXPOSE 9000
# Thu, 30 Nov 2023 23:03:52 GMT
CMD ["php-fpm"]
# Fri, 01 Dec 2023 02:46:07 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 01 Dec 2023 02:48:03 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 01 Dec 2023 02:48:06 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 01 Dec 2023 02:48:07 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Dec 2023 22:03:00 GMT
RUN set -eux; 	version='6.4.2'; 	sha1='d1aedbfea77b243b09e0ab05b100b782497406dd'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 07 Dec 2023 22:03:00 GMT
VOLUME [/var/www/html]
# Thu, 07 Dec 2023 22:03:00 GMT
COPY --chown=www-data:www-datafile:428b392bbc74b7aa0266d0b70812aab289561b5840fddd951986ac44165a331d in /usr/src/wordpress/ 
# Thu, 07 Dec 2023 22:03:00 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Dec 2023 22:03:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:03:01 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:2387a44129d2147bd4e806bf369f3db92eb3ad3b6b8825c739db364b8baa4e26`  
		Last Modified: Thu, 30 Nov 2023 22:49:56 GMT  
		Size: 2.9 MB (2901006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:463dfc43b4287670c76354cf1d002e077c0a4b8f41207fdbd96316d0f649fdd5`  
		Last Modified: Thu, 30 Nov 2023 23:58:02 GMT  
		Size: 2.5 MB (2524902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab8445d08981ee2b82e7069c3bf290f41039993039dd9740da05b6c962c368ea`  
		Last Modified: Thu, 30 Nov 2023 23:58:01 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8472c3889e6c64cf9e26fe36cc30bf9e211560aea77f82e97443348cb5956b88`  
		Last Modified: Thu, 30 Nov 2023 23:58:00 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e1a31c7a08192627a7e02da4b1d5ea494d5c25269ca986f8d2e7a8ae2d9365d`  
		Last Modified: Thu, 30 Nov 2023 23:58:00 GMT  
		Size: 12.5 MB (12452107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b3a23b2108bae03e59ed5e203dc9570b4d69cb6e8636a1f35e442846def57e`  
		Last Modified: Thu, 30 Nov 2023 23:57:59 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118444cd820bd6e50fbbdbc9e2ed47b9f4e2002f4c99f71de4ea78b37f3e0e3`  
		Last Modified: Thu, 30 Nov 2023 23:58:43 GMT  
		Size: 11.1 MB (11065349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c70a8c933c74a44b79288d9138990e29a695de52c46de08adfbe6b02eb5487`  
		Last Modified: Thu, 30 Nov 2023 23:58:40 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82133102a57e8f23f9f46c8569a880589aaff3e6f18918b587a89ee87089347b`  
		Last Modified: Thu, 30 Nov 2023 23:58:40 GMT  
		Size: 18.8 KB (18772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72d93b121acdd5c10e9fb769b5590812bc59328fa5bb8a6d9510c4b35208858b`  
		Last Modified: Thu, 30 Nov 2023 23:58:40 GMT  
		Size: 9.2 KB (9177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eecf3e32fbf2638632ff2567ad10a92410f2c732eda30c5cb86042b075f3749f`  
		Last Modified: Fri, 01 Dec 2023 02:55:53 GMT  
		Size: 38.7 MB (38664958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4209cc1cf6c977ff0fededbfa770d646314ce9b370a5699e9685ca7e93f9272`  
		Last Modified: Fri, 01 Dec 2023 02:55:48 GMT  
		Size: 4.2 MB (4211173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f76375e04dbd55ebca5b09b4114af10768e917710c42772e7a663b7de8ac832`  
		Last Modified: Fri, 01 Dec 2023 02:55:45 GMT  
		Size: 66.2 KB (66239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae3ba119aaf8d84a7628524930d89721084f7e16c85c72e5e6c00b3604f1ef13`  
		Last Modified: Fri, 01 Dec 2023 02:55:46 GMT  
		Size: 393.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52745f212f284845937677b3d20a42aa5ad0e3c653f01ab85ce6497adb4707bf`  
		Last Modified: Thu, 07 Dec 2023 22:07:45 GMT  
		Size: 24.3 MB (24309759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3655c96f3d0f84e52bc0b159d3402899e69b1678198a42f73a7de6511aeadd9`  
		Last Modified: Thu, 07 Dec 2023 22:07:41 GMT  
		Size: 2.3 KB (2349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31d43c364301e11184c7ffbadfc1114c7c3a0fa5350149b504fdbbb2fce2ac72`  
		Last Modified: Thu, 07 Dec 2023 22:07:41 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.3-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:c123d857e4610e02ace2c4023c566afcf52bab1126a40ccf3340ddc6f564d4c8
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.5 MB (104547056 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88bc8430741939abece3a694139a1cc960552ff49b17f3f9dc435107cc3bae5b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Thu, 30 Nov 2023 23:28:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 30 Nov 2023 23:29:00 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 30 Nov 2023 23:29:00 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 30 Nov 2023 23:29:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 30 Nov 2023 23:29:01 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 30 Nov 2023 23:29:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 30 Nov 2023 23:29:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 30 Nov 2023 23:29:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 30 Nov 2023 23:29:01 GMT
ENV GPG_KEYS=1198C0117593497A5EC5C199286AF1F9897469DC C28D937575603EB4ABB725861C0779DC5C0A9DE4 AFD8691FDAEDF03BDF6E460563F15A9B715376CA
# Thu, 30 Nov 2023 23:29:01 GMT
ENV PHP_VERSION=8.3.0
# Thu, 30 Nov 2023 23:29:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.3.0.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.3.0.tar.xz.asc
# Thu, 30 Nov 2023 23:29:02 GMT
ENV PHP_SHA256=1db84fec57125aa93638b51bb2b15103e12ac196e2f960f0d124275b2687ea54
# Thu, 30 Nov 2023 23:29:07 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 30 Nov 2023 23:29:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 30 Nov 2023 23:36:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 30 Nov 2023 23:36:55 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 30 Nov 2023 23:36:56 GMT
RUN docker-php-ext-enable sodium
# Thu, 30 Nov 2023 23:36:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 30 Nov 2023 23:36:57 GMT
WORKDIR /var/www/html
# Thu, 30 Nov 2023 23:36:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 30 Nov 2023 23:36:57 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Nov 2023 23:36:57 GMT
EXPOSE 9000
# Thu, 30 Nov 2023 23:36:57 GMT
CMD ["php-fpm"]
# Fri, 01 Dec 2023 00:52:37 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 01 Dec 2023 00:55:17 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 01 Dec 2023 00:55:18 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 01 Dec 2023 00:55:18 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Dec 2023 21:57:30 GMT
RUN set -eux; 	version='6.4.2'; 	sha1='d1aedbfea77b243b09e0ab05b100b782497406dd'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 07 Dec 2023 21:57:30 GMT
VOLUME [/var/www/html]
# Thu, 07 Dec 2023 21:57:30 GMT
COPY --chown=www-data:www-datafile:428b392bbc74b7aa0266d0b70812aab289561b5840fddd951986ac44165a331d in /usr/src/wordpress/ 
# Thu, 07 Dec 2023 21:57:31 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:57:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:57:31 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec91cb5b5977bc2c77c932761c9cd04eda4b0df9636a46228a4c0af65ad1b4f3`  
		Last Modified: Fri, 01 Dec 2023 00:40:05 GMT  
		Size: 2.7 MB (2717190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1563f945b2330cf35b9fc87a3f6456664dde2d6c4b6739047a9dd457f4a3d681`  
		Last Modified: Fri, 01 Dec 2023 00:40:04 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2549a9ef4a38d3afd713cc21e4de8fdf9a61d4d4f5b2897c0de403ec047f69a`  
		Last Modified: Fri, 01 Dec 2023 00:40:03 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285b1cbb8a2c86c2e2959b55b31fa9ac7abd053db302a937ce14d713aeaf8f44`  
		Last Modified: Fri, 01 Dec 2023 00:40:03 GMT  
		Size: 12.5 MB (12452091 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42ac31d6bb70b19a698a7b74ae40261071bc6f22d09403fea931a7923ca8af18`  
		Last Modified: Fri, 01 Dec 2023 00:40:02 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55eb051a38ab3ff5e0e4f55492b0cca01db3eb62985cd1cc0adf4ed9aebf964e`  
		Last Modified: Fri, 01 Dec 2023 00:40:44 GMT  
		Size: 13.0 MB (12994610 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19d9ac40d151bb59b4d87cadd39ca7e017d93f4b9f5076385d250c543878393a`  
		Last Modified: Fri, 01 Dec 2023 00:40:43 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0648d6f680a695029e48f25f688ec7f4a3fe69db085ba374dec32f8be413747c`  
		Last Modified: Fri, 01 Dec 2023 00:40:42 GMT  
		Size: 18.7 KB (18731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cce20cb644d2bd75c18a6fa5d0817faf1ed41c32323801bc659554d878a0ef6`  
		Last Modified: Fri, 01 Dec 2023 00:40:42 GMT  
		Size: 9.2 KB (9179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8b8a41b4e9432ab0881eb2a193a716fcd08805abdb4f62421e09c76f2036aa8`  
		Last Modified: Fri, 01 Dec 2023 01:01:20 GMT  
		Size: 44.3 MB (44253064 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b129210b5abfc47158109d99e94f6553183cccd998ef3c2b64886169b625c7a5`  
		Last Modified: Fri, 01 Dec 2023 01:01:16 GMT  
		Size: 4.4 MB (4384260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42198dc3f0a7eb84ceeac265fbf774c594f680073d23d3c7416b141a8a10a52a`  
		Last Modified: Fri, 01 Dec 2023 01:01:13 GMT  
		Size: 66.2 KB (66192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0ac9e6ae79047e305bbfbf98318d2a4bf85cd94a19ea954bba5f55ec566f18`  
		Last Modified: Fri, 01 Dec 2023 01:01:13 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd68154ba62f36d0407d7f68487be4877cb52bd92cddfc5c6f36d6047fde0b24`  
		Last Modified: Thu, 07 Dec 2023 22:02:04 GMT  
		Size: 24.3 MB (24309761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a359403f56f0b4bcea2d1eacf9fe425a0e07ba8b4e8c27cc87f2be7ae440c9`  
		Last Modified: Thu, 07 Dec 2023 22:02:01 GMT  
		Size: 2.4 KB (2351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b974ac631aebcd71d75726f059475e6baa2680d4c7e4188eb735760ba36564b8`  
		Last Modified: Thu, 07 Dec 2023 22:02:01 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.3-fpm-alpine` - linux; 386

```console
$ docker pull wordpress@sha256:bac797d6d121325476ad4c669e34ae907b089eff87175ca3e3ac0c7749309f3a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.3 MB (102264949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48e2bb46d5c7eb5cc2ad295a5c0ddb58ef0fd39575ff8c4d5389732ed85077d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 01 Dec 2023 02:03:44 GMT
ADD file:92902088cd15ed8f5dca2f7fc6570fb4e4824fac8b09e091c88e96bbd0ca814b in / 
# Fri, 01 Dec 2023 02:03:44 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:05:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 01 Dec 2023 02:05:21 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 01 Dec 2023 02:05:21 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 01 Dec 2023 02:05:21 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 01 Dec 2023 02:05:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Fri, 01 Dec 2023 02:05:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 01 Dec 2023 02:05:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 01 Dec 2023 02:05:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 01 Dec 2023 02:05:22 GMT
ENV GPG_KEYS=1198C0117593497A5EC5C199286AF1F9897469DC C28D937575603EB4ABB725861C0779DC5C0A9DE4 AFD8691FDAEDF03BDF6E460563F15A9B715376CA
# Fri, 01 Dec 2023 02:05:22 GMT
ENV PHP_VERSION=8.3.0
# Fri, 01 Dec 2023 02:05:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.3.0.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.3.0.tar.xz.asc
# Fri, 01 Dec 2023 02:05:23 GMT
ENV PHP_SHA256=1db84fec57125aa93638b51bb2b15103e12ac196e2f960f0d124275b2687ea54
# Fri, 01 Dec 2023 02:05:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 01 Dec 2023 02:05:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 01 Dec 2023 02:18:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 01 Dec 2023 02:18:36 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 01 Dec 2023 02:18:38 GMT
RUN docker-php-ext-enable sodium
# Fri, 01 Dec 2023 02:18:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 01 Dec 2023 02:18:38 GMT
WORKDIR /var/www/html
# Fri, 01 Dec 2023 02:18:39 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 01 Dec 2023 02:18:39 GMT
STOPSIGNAL SIGQUIT
# Fri, 01 Dec 2023 02:18:39 GMT
EXPOSE 9000
# Fri, 01 Dec 2023 02:18:39 GMT
CMD ["php-fpm"]
# Fri, 01 Dec 2023 11:00:23 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 01 Dec 2023 11:01:42 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 01 Dec 2023 11:01:44 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 01 Dec 2023 11:01:44 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Dec 2023 21:47:09 GMT
RUN set -eux; 	version='6.4.2'; 	sha1='d1aedbfea77b243b09e0ab05b100b782497406dd'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 07 Dec 2023 21:47:09 GMT
VOLUME [/var/www/html]
# Thu, 07 Dec 2023 21:47:09 GMT
COPY --chown=www-data:www-datafile:428b392bbc74b7aa0266d0b70812aab289561b5840fddd951986ac44165a331d in /usr/src/wordpress/ 
# Thu, 07 Dec 2023 21:47:10 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:47:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:47:10 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:4966a8bd129b0a6adf93dc295a8fbe8f665d3194a684a5ce199c1c3596dbf3d9`  
		Last Modified: Fri, 01 Dec 2023 02:04:18 GMT  
		Size: 3.2 MB (3238831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786b6949c7da1fc85a439f51aa05ace6592ed6759802ad370ed74bc4f479828b`  
		Last Modified: Fri, 01 Dec 2023 04:07:07 GMT  
		Size: 2.7 MB (2723376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27aec508afba473c67b8d2ad4216ba2489f0e9f08768454183b11877384d8139`  
		Last Modified: Fri, 01 Dec 2023 04:07:05 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a55ae0822cb02fa8febaedc0ea40b1c5b2823b47b9e9f3dc9436f506df98f121`  
		Last Modified: Fri, 01 Dec 2023 04:07:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d34e95bca488cede02955576432a46cb1462e07cc769b9eb29f6fb2bf7dcbf`  
		Last Modified: Fri, 01 Dec 2023 04:07:05 GMT  
		Size: 12.5 MB (12452099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03e703b9b578d877bbb5bb3e7217c5b01c4bd415d52c238a814d769297fe5970`  
		Last Modified: Fri, 01 Dec 2023 04:07:03 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:016b3a5a75f3f11395a78dbbf1f49dbe6ecb803f9eac315dd7da6af6a4d80c8c`  
		Last Modified: Fri, 01 Dec 2023 04:07:51 GMT  
		Size: 13.1 MB (13105402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9e9b14301cd9981c0ad78083860c8869baa0a4ae48393497fc05c39cfd6917e`  
		Last Modified: Fri, 01 Dec 2023 04:07:48 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23a1ed0d7573a27866eb418eab2fb8dc98f0784df01cab0e52c2b6a3ffad3fcf`  
		Last Modified: Fri, 01 Dec 2023 04:07:48 GMT  
		Size: 18.9 KB (18927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d37266210038b9998e59d2b36a74ae6d6c1ec0fd07bf9c05d4fc991bb2403ed`  
		Last Modified: Fri, 01 Dec 2023 04:07:48 GMT  
		Size: 9.2 KB (9175 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4b74cf44f173864d93e5040ff70cd97471e51e43c882d694edd151b42f9481d`  
		Last Modified: Fri, 01 Dec 2023 11:10:07 GMT  
		Size: 41.8 MB (41839890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb36326c393f0f92787f9e75c775aa20e84db1b0f60cbb44896867ae7170890`  
		Last Modified: Fri, 01 Dec 2023 11:09:59 GMT  
		Size: 4.5 MB (4492319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:822b30bb9a4845569f9c379da4615098414a2efcad0646d6c717d533e0c7da79`  
		Last Modified: Fri, 01 Dec 2023 11:09:56 GMT  
		Size: 66.2 KB (66225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415c9b5b94e3b74143da131bb9783f95fc4f56e124ba10bded4fc0e2264fc3ee`  
		Last Modified: Fri, 01 Dec 2023 11:09:56 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ef55989fe42b8bbee43af4705f7324271a8c804fcf1e3b43e1568a1eeb88abd`  
		Last Modified: Thu, 07 Dec 2023 21:52:16 GMT  
		Size: 24.3 MB (24309767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc503ea8661ddeb55e2c16e4f094447a960758c9cec8f54ebfd832e22d623e8e`  
		Last Modified: Thu, 07 Dec 2023 21:52:11 GMT  
		Size: 2.4 KB (2350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbcab2e37fb4d930454612acc6afd21a00a9b48d1065f0f7cf20e955f9431645`  
		Last Modified: Thu, 07 Dec 2023 21:52:11 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.3-fpm-alpine` - linux; ppc64le

```console
$ docker pull wordpress@sha256:ba99f3dbfaee447969d53d0dd453402d8797549d71756660b9175912da645482
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.8 MB (110823098 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f4993a4ccbb9f66afcd5a262b7cc5b422e0744bc0b3cafb84207f768eff98202`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 30 Nov 2023 23:19:04 GMT
ADD file:3450a1687b552498a987f87cb844b7f597c7181d7c3d31943d7b3036d5300d5e in / 
# Thu, 30 Nov 2023 23:19:05 GMT
CMD ["/bin/sh"]
# Thu, 30 Nov 2023 23:37:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 30 Nov 2023 23:37:41 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 30 Nov 2023 23:37:46 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 30 Nov 2023 23:37:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 30 Nov 2023 23:37:53 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 30 Nov 2023 23:37:54 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 30 Nov 2023 23:37:56 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 30 Nov 2023 23:37:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 30 Nov 2023 23:37:58 GMT
ENV GPG_KEYS=1198C0117593497A5EC5C199286AF1F9897469DC C28D937575603EB4ABB725861C0779DC5C0A9DE4 AFD8691FDAEDF03BDF6E460563F15A9B715376CA
# Thu, 30 Nov 2023 23:37:59 GMT
ENV PHP_VERSION=8.3.0
# Thu, 30 Nov 2023 23:37:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.3.0.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.3.0.tar.xz.asc
# Thu, 30 Nov 2023 23:38:00 GMT
ENV PHP_SHA256=1db84fec57125aa93638b51bb2b15103e12ac196e2f960f0d124275b2687ea54
# Thu, 30 Nov 2023 23:38:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 30 Nov 2023 23:38:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 30 Nov 2023 23:45:53 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 30 Nov 2023 23:45:56 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 30 Nov 2023 23:46:01 GMT
RUN docker-php-ext-enable sodium
# Thu, 30 Nov 2023 23:46:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 30 Nov 2023 23:46:07 GMT
WORKDIR /var/www/html
# Thu, 30 Nov 2023 23:46:09 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 30 Nov 2023 23:46:14 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Nov 2023 23:46:18 GMT
EXPOSE 9000
# Thu, 30 Nov 2023 23:46:20 GMT
CMD ["php-fpm"]
# Fri, 01 Dec 2023 04:32:40 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 01 Dec 2023 04:34:36 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 01 Dec 2023 04:34:40 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 01 Dec 2023 04:34:45 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Dec 2023 22:26:24 GMT
RUN set -eux; 	version='6.4.2'; 	sha1='d1aedbfea77b243b09e0ab05b100b782497406dd'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 07 Dec 2023 22:26:26 GMT
VOLUME [/var/www/html]
# Thu, 07 Dec 2023 22:26:27 GMT
COPY --chown=www-data:www-datafile:428b392bbc74b7aa0266d0b70812aab289561b5840fddd951986ac44165a331d in /usr/src/wordpress/ 
# Thu, 07 Dec 2023 22:26:28 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Dec 2023 22:26:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:26:29 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:4e13780adf2776477b14ef9c0f4f563f820a2fde166d472218037b979e84d31a`  
		Last Modified: Thu, 30 Nov 2023 23:20:01 GMT  
		Size: 3.3 MB (3348322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f8cb9b4da64e0956e297ed583f04085128cdc4a68dcffa3a41c639319245c27`  
		Last Modified: Fri, 01 Dec 2023 00:53:04 GMT  
		Size: 2.8 MB (2766423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89e2afe36ae984e44fa290115e1355ddb9ba0833dc70a7e3e1f1ed384492c3ec`  
		Last Modified: Fri, 01 Dec 2023 00:53:04 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:233860698dd8a6e8c7a48373c7cb0a908fc5e1ad61c7ba6c0606e54226ed4c5d`  
		Last Modified: Fri, 01 Dec 2023 00:53:03 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8fb69ca1d3e6a6c70e5d15e8c0a1588f2b439de9683f4874bd1b2f921e4232a`  
		Last Modified: Fri, 01 Dec 2023 00:53:02 GMT  
		Size: 12.5 MB (12452085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab6815e64bb3220dda4d71f42ca13e00d8da619677251611904fb38d6e6eb671`  
		Last Modified: Fri, 01 Dec 2023 00:53:02 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d0c005bb10932c903a8030c3f29461da46076871fb7cc3bff7dfe6de7c41b7f`  
		Last Modified: Fri, 01 Dec 2023 00:53:50 GMT  
		Size: 13.3 MB (13345262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9082204217abdb97bf124122c8689cf41c5218a5d7f617b4c7d36c9d4bffcd54`  
		Last Modified: Fri, 01 Dec 2023 00:53:48 GMT  
		Size: 2.5 KB (2451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4dc0e2524e916e0ef213b709ec999edd07409ff347a303a771bb69527643929`  
		Last Modified: Fri, 01 Dec 2023 00:53:48 GMT  
		Size: 18.7 KB (18730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eb7eb574c1f341a34ce77fe3938ca9e8e185683c5083a67dc084ab3384cb5a0`  
		Last Modified: Fri, 01 Dec 2023 00:53:48 GMT  
		Size: 9.2 KB (9183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553beab4a943faaaab12948a8258755dbadeaa95f9ee12d6c92b32ef7a0e4806`  
		Last Modified: Fri, 01 Dec 2023 04:48:47 GMT  
		Size: 50.0 MB (49963652 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1423244af3f30d402dc1b630c8798956b01ebb3edda94d0a5dce272ed931c59f`  
		Last Modified: Fri, 01 Dec 2023 04:48:40 GMT  
		Size: 4.5 MB (4534522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:376044e525409cd27da1e8adde1dea5e5eb7f39bd1d90001b93ed9929ba5151d`  
		Last Modified: Fri, 01 Dec 2023 04:48:37 GMT  
		Size: 66.2 KB (66212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e266d516fdbc499174ea7f0f154cbd74cd90ff8f6928530b2580d69b759c20`  
		Last Modified: Fri, 01 Dec 2023 04:48:37 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ede02029d4e84c1f8282e9089abf5f5d64e6583e867723bf266a0d639c8f9fe8`  
		Last Modified: Thu, 07 Dec 2023 22:31:43 GMT  
		Size: 24.3 MB (24309760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2e7d50e664be37a52b5b7b90347319fa2fd36c6205738e16446bf10abb7cb42`  
		Last Modified: Thu, 07 Dec 2023 22:31:39 GMT  
		Size: 2.3 KB (2347 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931833e4f5e268e35d929e8093a513e1138b4e6bf0ffafcdcb8dce6f6db8d6c9`  
		Last Modified: Thu, 07 Dec 2023 22:31:39 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:php8.3-fpm-alpine` - linux; s390x

```console
$ docker pull wordpress@sha256:388318123cdf2d4b6e914f1661a4d9ff04c70fca22e4b35a8d88dccc8a3d3fae
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.2 MB (104215879 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5953a8ff764445ba074aff283025cfaa614703c4b934b277e141207c45c6f654`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 30 Nov 2023 22:42:08 GMT
ADD file:50d6643abf7df167a927decd69d193b980557ff73cca48dce86d57e2ff25ad45 in / 
# Thu, 30 Nov 2023 22:42:09 GMT
CMD ["/bin/sh"]
# Thu, 30 Nov 2023 22:45:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 30 Nov 2023 22:45:07 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 30 Nov 2023 22:45:08 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 30 Nov 2023 22:45:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 30 Nov 2023 22:45:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Thu, 30 Nov 2023 22:45:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 30 Nov 2023 22:45:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 30 Nov 2023 22:45:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 30 Nov 2023 22:45:09 GMT
ENV GPG_KEYS=1198C0117593497A5EC5C199286AF1F9897469DC C28D937575603EB4ABB725861C0779DC5C0A9DE4 AFD8691FDAEDF03BDF6E460563F15A9B715376CA
# Thu, 30 Nov 2023 22:45:09 GMT
ENV PHP_VERSION=8.3.0
# Thu, 30 Nov 2023 22:45:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.3.0.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.3.0.tar.xz.asc
# Thu, 30 Nov 2023 22:45:09 GMT
ENV PHP_SHA256=1db84fec57125aa93638b51bb2b15103e12ac196e2f960f0d124275b2687ea54
# Thu, 30 Nov 2023 22:45:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 30 Nov 2023 22:45:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 30 Nov 2023 22:51:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 30 Nov 2023 22:51:20 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 30 Nov 2023 22:51:21 GMT
RUN docker-php-ext-enable sodium
# Thu, 30 Nov 2023 22:51:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 30 Nov 2023 22:51:22 GMT
WORKDIR /var/www/html
# Thu, 30 Nov 2023 22:51:22 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 30 Nov 2023 22:51:22 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Nov 2023 22:51:22 GMT
EXPOSE 9000
# Thu, 30 Nov 2023 22:51:22 GMT
CMD ["php-fpm"]
# Fri, 01 Dec 2023 02:21:13 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 01 Dec 2023 02:22:02 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 01 Dec 2023 02:22:04 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 01 Dec 2023 02:22:04 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Dec 2023 21:51:21 GMT
RUN set -eux; 	version='6.4.2'; 	sha1='d1aedbfea77b243b09e0ab05b100b782497406dd'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 07 Dec 2023 21:51:24 GMT
VOLUME [/var/www/html]
# Thu, 07 Dec 2023 21:51:24 GMT
COPY --chown=www-data:www-datafile:428b392bbc74b7aa0266d0b70812aab289561b5840fddd951986ac44165a331d in /usr/src/wordpress/ 
# Thu, 07 Dec 2023 21:51:24 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:51:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:51:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:2ea477e1c0c3db3337ee1d7c659f8c465021a65c036998ed3fa3b667d4b30153`  
		Last Modified: Thu, 30 Nov 2023 22:42:52 GMT  
		Size: 3.2 MB (3217454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aa5313d02d4fcc59703ea6bd09df7b0df122fc73121b0954b541c214229202e`  
		Last Modified: Thu, 30 Nov 2023 23:47:29 GMT  
		Size: 2.8 MB (2789878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f082f983656d312447043a024c0fa5528e4055dbd73f4101ac38d1d2d3158ea`  
		Last Modified: Thu, 30 Nov 2023 23:47:28 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35feaf89a3d400114f4864637453e2e21cd9e7cb6a859699bd6272483f3a56ee`  
		Last Modified: Thu, 30 Nov 2023 23:47:28 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b59844514cd33789360a3e46dbaff2cdae06b8cd8d18ee9449808c168be15f9`  
		Last Modified: Thu, 30 Nov 2023 23:47:27 GMT  
		Size: 12.5 MB (12452093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:090f8111976872dd0d1fdf290acf04666250d582cbba875706f055725bc42aff`  
		Last Modified: Thu, 30 Nov 2023 23:47:27 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c1abfd1d114600af550c034a5d2e58fcc0cd8278add135099a72b947b27221b`  
		Last Modified: Thu, 30 Nov 2023 23:47:52 GMT  
		Size: 12.1 MB (12074915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e510a785c0a9c5de3fd045d0fe1d0b9aa18618094c25dda6001959bfdf9b61e4`  
		Last Modified: Thu, 30 Nov 2023 23:47:50 GMT  
		Size: 2.4 KB (2446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5b351665435cb92be92f42a18274e11675c5b13253795e4081ba4709d0441f`  
		Last Modified: Thu, 30 Nov 2023 23:47:50 GMT  
		Size: 18.8 KB (18762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61ac11eedcd85ac5d34c151aff99a30d17fdf0217be3f2864d0390e958c1123b`  
		Last Modified: Thu, 30 Nov 2023 23:47:50 GMT  
		Size: 9.2 KB (9179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319f9fa5eb2e18f7132e8f6ba9be11893615619c98420b096b9f1a0313928787`  
		Last Modified: Fri, 01 Dec 2023 02:28:28 GMT  
		Size: 44.8 MB (44799290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66afcdccba11f73836cec36213fc2eebd4e88725c705c4eeaf06d8dd6dcdc11`  
		Last Modified: Fri, 01 Dec 2023 02:28:22 GMT  
		Size: 4.5 MB (4469850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5728f7527c86bcb76516ccc2dab0b9e6f6855800a29ceb10605168f76f0067d4`  
		Last Modified: Fri, 01 Dec 2023 02:28:20 GMT  
		Size: 65.8 KB (65755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de48680aded2227703a506367505b8d4640a5b691d5837af26846da700fe5a0`  
		Last Modified: Fri, 01 Dec 2023 02:28:20 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41144483ae738542047b4e7454b6575ef0b53621c15488d53e484e90be1a59e8`  
		Last Modified: Thu, 07 Dec 2023 21:55:16 GMT  
		Size: 24.3 MB (24309763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd4fdfb9617bd6d14e8cd4062f2ebe633106c93fd715c391494c4c245e74f29`  
		Last Modified: Thu, 07 Dec 2023 21:55:12 GMT  
		Size: 2.3 KB (2348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b1702053d4f1f673e70218356f990b052f2786d3c381e86f5acbdba656b497d`  
		Last Modified: Thu, 07 Dec 2023 21:55:13 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
