## `wordpress:6-php8.2-fpm-alpine`

```console
$ docker pull wordpress@sha256:0170fa720ce33ec17640f204920c6d4f9aa05f04bc68dc5ffb0e3a58029f3854
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

### `wordpress:6-php8.2-fpm-alpine` - linux; amd64

```console
$ docker pull wordpress@sha256:e853d0d370733e9697aae9b535794e531f0b6fc6fa87af657dce8a2de707429a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.7 MB (104694505 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d361810b2ae7f41938581825b21f996322e00e62373ddc43c9677fce16b1e4c0`
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
# Thu, 30 Nov 2023 23:55:47 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 30 Nov 2023 23:55:47 GMT
ENV PHP_VERSION=8.2.13
# Thu, 30 Nov 2023 23:55:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Thu, 30 Nov 2023 23:55:48 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Thu, 30 Nov 2023 23:55:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 30 Nov 2023 23:55:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 01 Dec 2023 00:02:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 01 Dec 2023 00:02:52 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 01 Dec 2023 00:02:53 GMT
RUN docker-php-ext-enable sodium
# Fri, 01 Dec 2023 00:02:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 01 Dec 2023 00:02:53 GMT
WORKDIR /var/www/html
# Fri, 01 Dec 2023 00:02:53 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 01 Dec 2023 00:02:53 GMT
STOPSIGNAL SIGQUIT
# Fri, 01 Dec 2023 00:02:53 GMT
EXPOSE 9000
# Fri, 01 Dec 2023 00:02:54 GMT
CMD ["php-fpm"]
# Fri, 01 Dec 2023 02:46:28 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 01 Dec 2023 02:47:20 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 01 Dec 2023 02:47:21 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 01 Dec 2023 02:47:21 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Dec 2023 22:27:43 GMT
RUN set -eux; 	version='6.4.2'; 	sha1='d1aedbfea77b243b09e0ab05b100b782497406dd'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 07 Dec 2023 22:27:44 GMT
VOLUME [/var/www/html]
# Thu, 07 Dec 2023 22:27:44 GMT
COPY --chown=www-data:www-datafile:428b392bbc74b7aa0266d0b70812aab289561b5840fddd951986ac44165a331d in /usr/src/wordpress/ 
# Thu, 07 Dec 2023 22:27:44 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Dec 2023 22:27:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:27:44 GMT
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
	-	`sha256:3732066280a1d3be2cd3e77503f8cfb033ee0755d8816e760a51936bba17155a`  
		Last Modified: Fri, 01 Dec 2023 00:44:34 GMT  
		Size: 12.1 MB (12089953 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23dfeb871e9d19024739cc1ba273b5deb5226d70751fc2fbbca35f5a97391f84`  
		Last Modified: Fri, 01 Dec 2023 00:44:33 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71442a0585dd1ee4d10a9ff3f0779cf26419a5654f140c1c25964c670a978a63`  
		Last Modified: Fri, 01 Dec 2023 00:44:59 GMT  
		Size: 12.7 MB (12700949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930182f44a1638a1ad6803eb827f3c8eb5f46ce7f9e7a3807ce447345a156784`  
		Last Modified: Fri, 01 Dec 2023 00:44:57 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100698e2eb12f67829157faa8db930b7228dd3e2b8fe16b5708efb3ffe68df8f`  
		Last Modified: Fri, 01 Dec 2023 00:44:57 GMT  
		Size: 18.9 KB (18946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1b065e10a0356a81b5686e39dfc358758275095be21fedd4499b6885c8a460f`  
		Last Modified: Fri, 01 Dec 2023 00:44:56 GMT  
		Size: 9.2 KB (9177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23d2de5ab7ffd9928b8ddab1752018bdf3b583a6f7492d79daa7db6127a76a0a`  
		Last Modified: Fri, 01 Dec 2023 02:58:10 GMT  
		Size: 45.1 MB (45053566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38db6f95fab8bcd929c7b8ca545aa43805203ad0bdedf926a382f506467ae675`  
		Last Modified: Fri, 01 Dec 2023 02:58:03 GMT  
		Size: 4.4 MB (4355189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78316dbb2edb14939b07a903c828f498ba2f8d5fd7b5bd4a893ac1fd09c47889`  
		Last Modified: Fri, 01 Dec 2023 02:58:01 GMT  
		Size: 66.2 KB (66226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4924211168b57a22805bba91c00ef2ab0b767b74ddff8537f3c20c5aeb534b45`  
		Last Modified: Fri, 01 Dec 2023 02:58:01 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9885459c3969d67cd4297789745c3af125c92cd8c64e660cf95bce3df3c48723`  
		Last Modified: Thu, 07 Dec 2023 22:31:25 GMT  
		Size: 24.3 MB (24309766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:778f9d4bedbac07526fe351d84a036b8fbf30ac08e4723b286576a4c0d5006f9`  
		Last Modified: Thu, 07 Dec 2023 22:31:21 GMT  
		Size: 2.3 KB (2348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b860699b7ffc4651cb58e1a6ced4fb590acf563664e7325d0576e29867d10be1`  
		Last Modified: Thu, 07 Dec 2023 22:31:21 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:6-php8.2-fpm-alpine` - linux; arm variant v6

```console
$ docker pull wordpress@sha256:05eb748e2277b79a9cf5fbc3ca410b826b3e22ccd2cd0cd6ea31f8b1952afc66
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **99.0 MB (98971649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:130ce11ae16a64c510e9db861bec2af35d34525be1748ea703f2bf2e0bed1857`
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
# Thu, 30 Nov 2023 23:38:20 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 30 Nov 2023 23:38:21 GMT
ENV PHP_VERSION=8.2.13
# Thu, 30 Nov 2023 23:38:21 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Thu, 30 Nov 2023 23:38:21 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Thu, 30 Nov 2023 23:38:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 30 Nov 2023 23:38:29 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 30 Nov 2023 23:45:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 30 Nov 2023 23:45:04 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 30 Nov 2023 23:45:05 GMT
RUN docker-php-ext-enable sodium
# Thu, 30 Nov 2023 23:45:05 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 30 Nov 2023 23:45:06 GMT
WORKDIR /var/www/html
# Thu, 30 Nov 2023 23:45:06 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 30 Nov 2023 23:45:07 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Nov 2023 23:45:07 GMT
EXPOSE 9000
# Thu, 30 Nov 2023 23:45:07 GMT
CMD ["php-fpm"]
# Fri, 01 Dec 2023 12:14:57 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 01 Dec 2023 12:15:50 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 01 Dec 2023 12:15:51 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 01 Dec 2023 12:15:52 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Dec 2023 21:51:49 GMT
RUN set -eux; 	version='6.4.2'; 	sha1='d1aedbfea77b243b09e0ab05b100b782497406dd'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 07 Dec 2023 21:51:49 GMT
VOLUME [/var/www/html]
# Thu, 07 Dec 2023 21:51:49 GMT
COPY --chown=www-data:www-datafile:428b392bbc74b7aa0266d0b70812aab289561b5840fddd951986ac44165a331d in /usr/src/wordpress/ 
# Thu, 07 Dec 2023 21:51:50 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:51:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:51:50 GMT
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
	-	`sha256:3498e93a2d588ae5e9d1202e761cf3d82a0a05227537d661e99568fcdce2c0b3`  
		Last Modified: Fri, 01 Dec 2023 00:17:29 GMT  
		Size: 12.1 MB (12089948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52ab06cb30eb31e97cd9c2cadf68eac361eb4ecbb9cdbf49cd06ae51bf86ec4`  
		Last Modified: Fri, 01 Dec 2023 00:17:27 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e640b0bcfa2c27d9a665e6f0cd8e9e9f4a140109b5e19f28df6a2e3dff4c2c5`  
		Last Modified: Fri, 01 Dec 2023 00:17:57 GMT  
		Size: 11.6 MB (11615160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:693114fa70745217c8b5f7220ada3b431986ca334fcadf200fc02aedff526530`  
		Last Modified: Fri, 01 Dec 2023 00:17:55 GMT  
		Size: 2.4 KB (2448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1034373d111bce254afa2bd1dd1d456bb6c445e2bbcd4d53a2f9e6d55bf5047b`  
		Last Modified: Fri, 01 Dec 2023 00:17:55 GMT  
		Size: 18.8 KB (18768 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f119b39dc2fb3942df617cd21ea8fc62bc3fcdd8eda4726e4eed193fa35254a5`  
		Last Modified: Fri, 01 Dec 2023 00:17:55 GMT  
		Size: 9.2 KB (9180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f9f4050d7d35f5577c2f3069cf5ceba2e3ccec3b03a3bf940a82ed990647695`  
		Last Modified: Fri, 01 Dec 2023 12:21:22 GMT  
		Size: 40.9 MB (40855631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be4cd9873e33eed28f4a387bd79ce500bbb153f61b98d905f9b78550f24a4cc`  
		Last Modified: Fri, 01 Dec 2023 12:21:17 GMT  
		Size: 4.2 MB (4165333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58d18d48f8bf73daefb68cb78d639acdcc43722a5262d0b31a1639e47c2c60b8`  
		Last Modified: Fri, 01 Dec 2023 12:21:14 GMT  
		Size: 66.2 KB (66239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0352ec8226cc8fcbc8249d7e29a6f40f60e2dc80a1e212fa9f280f02b06f750e`  
		Last Modified: Fri, 01 Dec 2023 12:21:14 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14e61048bb6755e2c9846fab65b678f34bf9bdca21aed334ca4bbdea2e7f748c`  
		Last Modified: Thu, 07 Dec 2023 21:52:43 GMT  
		Size: 24.3 MB (24309764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a56c1bf1e298b842939d2f013daa27ead1a67792982b2cd7c4f497bb07189d4`  
		Last Modified: Thu, 07 Dec 2023 21:52:39 GMT  
		Size: 2.4 KB (2350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd39b64e04c820fdae77904d464e971d43ae0f4915d4306e61b98483258fe038`  
		Last Modified: Thu, 07 Dec 2023 21:52:40 GMT  
		Size: 1.7 KB (1734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:6-php8.2-fpm-alpine` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:82db5ee782df83bbeb7f6912bb31e63b866e0d542b83bf6462c473f0972a2ffd
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **95.7 MB (95655401 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3282749b436e8fa42e94c81d979758638a42af463f2f58cc7de083fdb211a92b`
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
# Thu, 30 Nov 2023 23:15:37 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 30 Nov 2023 23:15:37 GMT
ENV PHP_VERSION=8.2.13
# Thu, 30 Nov 2023 23:15:37 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Thu, 30 Nov 2023 23:15:37 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Thu, 30 Nov 2023 23:15:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 30 Nov 2023 23:15:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 30 Nov 2023 23:23:03 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 30 Nov 2023 23:23:03 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 30 Nov 2023 23:23:04 GMT
RUN docker-php-ext-enable sodium
# Thu, 30 Nov 2023 23:23:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 30 Nov 2023 23:23:05 GMT
WORKDIR /var/www/html
# Thu, 30 Nov 2023 23:23:05 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 30 Nov 2023 23:23:05 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Nov 2023 23:23:06 GMT
EXPOSE 9000
# Thu, 30 Nov 2023 23:23:06 GMT
CMD ["php-fpm"]
# Fri, 01 Dec 2023 02:36:10 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 01 Dec 2023 02:38:01 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 01 Dec 2023 02:38:03 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 01 Dec 2023 02:38:04 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Dec 2023 22:02:40 GMT
RUN set -eux; 	version='6.4.2'; 	sha1='d1aedbfea77b243b09e0ab05b100b782497406dd'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 07 Dec 2023 22:02:40 GMT
VOLUME [/var/www/html]
# Thu, 07 Dec 2023 22:02:40 GMT
COPY --chown=www-data:www-datafile:428b392bbc74b7aa0266d0b70812aab289561b5840fddd951986ac44165a331d in /usr/src/wordpress/ 
# Thu, 07 Dec 2023 22:02:40 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Dec 2023 22:02:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:02:41 GMT
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
	-	`sha256:a1f550c3297ee4c4dbdb04e414d483c78d57e76a36003ef752fb45b5b40c2cb2`  
		Last Modified: Fri, 01 Dec 2023 00:00:46 GMT  
		Size: 12.1 MB (12089958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:367f4dbf5ca7bd8551d02f1f9e270b5296620206a1266a6c6200f77635191fb4`  
		Last Modified: Fri, 01 Dec 2023 00:00:44 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdd6045d176d2f9813632989830d19ff10a29a5927cdb3403539112e6e10622a`  
		Last Modified: Fri, 01 Dec 2023 00:01:13 GMT  
		Size: 10.9 MB (10854530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0eecda280b58dd3dcd642a9c91b41ee08230b7a73ac164241579937c5c0825`  
		Last Modified: Fri, 01 Dec 2023 00:01:11 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84066c6b03c9a192241b52134d30c653bba5479dd6106dc0678356ce3fa3e86d`  
		Last Modified: Fri, 01 Dec 2023 00:01:11 GMT  
		Size: 18.8 KB (18777 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb0701bbad5f46e1ccc38f84a96cf3a1940e1febba06692665a2d6d9873bac0`  
		Last Modified: Fri, 01 Dec 2023 00:01:11 GMT  
		Size: 9.2 KB (9178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9c7f804a076d20bcaa04402e2dc71cdd00033d3f31099d32c0e0a59417e20d`  
		Last Modified: Fri, 01 Dec 2023 02:54:27 GMT  
		Size: 38.7 MB (38664918 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35148c7225629c4719ff2385693c9b98a87c6f0879c296bfcae9feb01d3d9ffa`  
		Last Modified: Fri, 01 Dec 2023 02:54:21 GMT  
		Size: 4.2 MB (4207191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff748f626b27e1e76691e404f126c61c0e46c504c9def89a63416e470610747d`  
		Last Modified: Fri, 01 Dec 2023 02:54:18 GMT  
		Size: 66.2 KB (66239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:343d6cf0f09829daff9f42799ef9345b75c6f8c6590c25c6ff11d0c0037ac652`  
		Last Modified: Fri, 01 Dec 2023 02:54:18 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:767261ff3d53dc16ceae6db676084d2f30daf508f56da23ca2f534fe0c1d9f97`  
		Last Modified: Thu, 07 Dec 2023 22:06:23 GMT  
		Size: 24.3 MB (24309760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:802b2364f138e664a1ff8f1c89efe49e12a6db4134e992a7e923e2e917d92f30`  
		Last Modified: Thu, 07 Dec 2023 22:06:20 GMT  
		Size: 2.3 KB (2348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a0c0c8a9d2d8ec5245f084c44bec6a82040406e9514ebe0e91dc1f77d9163d6`  
		Last Modified: Thu, 07 Dec 2023 22:06:19 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:6-php8.2-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:f67f1e64da4d5ce6b405da0d203b6f11f350e28f87ea025bbb826209f6c13a7a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.0 MB (103969095 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d1e2b5c3035a0467a68b7df49b7bc15d8f70df4102da5aaa4996c94415abb1d`
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
# Thu, 30 Nov 2023 23:53:27 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 30 Nov 2023 23:53:27 GMT
ENV PHP_VERSION=8.2.13
# Thu, 30 Nov 2023 23:53:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Thu, 30 Nov 2023 23:53:28 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Thu, 30 Nov 2023 23:53:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 30 Nov 2023 23:53:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 01 Dec 2023 00:00:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 01 Dec 2023 00:00:33 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 01 Dec 2023 00:00:34 GMT
RUN docker-php-ext-enable sodium
# Fri, 01 Dec 2023 00:00:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 01 Dec 2023 00:00:34 GMT
WORKDIR /var/www/html
# Fri, 01 Dec 2023 00:00:34 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 01 Dec 2023 00:00:34 GMT
STOPSIGNAL SIGQUIT
# Fri, 01 Dec 2023 00:00:34 GMT
EXPOSE 9000
# Fri, 01 Dec 2023 00:00:35 GMT
CMD ["php-fpm"]
# Fri, 01 Dec 2023 00:47:02 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 01 Dec 2023 00:47:49 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 01 Dec 2023 00:47:50 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 01 Dec 2023 00:47:50 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Dec 2023 21:57:13 GMT
RUN set -eux; 	version='6.4.2'; 	sha1='d1aedbfea77b243b09e0ab05b100b782497406dd'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 07 Dec 2023 21:57:13 GMT
VOLUME [/var/www/html]
# Thu, 07 Dec 2023 21:57:14 GMT
COPY --chown=www-data:www-datafile:428b392bbc74b7aa0266d0b70812aab289561b5840fddd951986ac44165a331d in /usr/src/wordpress/ 
# Thu, 07 Dec 2023 21:57:14 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:57:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:57:14 GMT
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
	-	`sha256:3d643308102462794542b16b45c2b3ae7f784b8913540e0fc7b3a2cdf29f1578`  
		Last Modified: Fri, 01 Dec 2023 00:42:30 GMT  
		Size: 12.1 MB (12089938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c2a46c10b471f515c34030e1bd5a7b52530fcbf397833257cefbe7807f332dd`  
		Last Modified: Fri, 01 Dec 2023 00:42:29 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c5443af992de1598fc85d8e7cfae65fea9bb369a8411463443bf83115d7512e`  
		Last Modified: Fri, 01 Dec 2023 00:42:54 GMT  
		Size: 12.8 MB (12783401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ce6c0e2e61fcafebbaaa8e81164ff2d176ccaae1194aad85b79d58076cb79cd`  
		Last Modified: Fri, 01 Dec 2023 00:42:52 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b663d25c7104c9ff139fc9a72f0e4bca351f241d743f299c1913ede4230e9719`  
		Last Modified: Fri, 01 Dec 2023 00:42:52 GMT  
		Size: 18.7 KB (18720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:843f48704249537998e7dad0015b35005a7b3790a5039ffab11812e9617a1097`  
		Last Modified: Fri, 01 Dec 2023 00:42:52 GMT  
		Size: 9.2 KB (9176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb0b398f3e85abe3f4b56394c8a653b9655370a5833626ff6f23c3fe451ed0fb`  
		Last Modified: Fri, 01 Dec 2023 00:59:59 GMT  
		Size: 44.3 MB (44253093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ddf3f5981b5df960f6f7788c2217cdac57ddf5dc13eabd6c34eedf8519c56151`  
		Last Modified: Fri, 01 Dec 2023 00:59:55 GMT  
		Size: 4.4 MB (4379646 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41065e1c6b2920d6cf2f5676e8e80eba70608e599f646d680fb2bca35305e36f`  
		Last Modified: Fri, 01 Dec 2023 00:59:53 GMT  
		Size: 66.2 KB (66193 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c46ca3526a75f25449fbaf1d8889727e90e3ab6b5cf08e6126c78e143c5530a6`  
		Last Modified: Fri, 01 Dec 2023 00:59:53 GMT  
		Size: 386.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ef0fa0662b448d2227a6c3b0f05659c8bbfa30830b82725c9184b33b4c2074`  
		Last Modified: Thu, 07 Dec 2023 22:00:44 GMT  
		Size: 24.3 MB (24309767 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bddefcab88770c862331d927443aac4b832f4dc28b90cf41a07fe7f9e728620`  
		Last Modified: Thu, 07 Dec 2023 22:00:41 GMT  
		Size: 2.3 KB (2348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:034cf648050698eec3305ca84a5c63200607d1fcc31619cc1f42e46be433835f`  
		Last Modified: Thu, 07 Dec 2023 22:00:41 GMT  
		Size: 1.7 KB (1731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:6-php8.2-fpm-alpine` - linux; 386

```console
$ docker pull wordpress@sha256:e01500216f9ee4b01b97a013a00ac0481da8f23f94e0dbf0e8f01fe2893b1d57
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.7 MB (101693214 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f3393945fe200d25b903002dc57722523ef28962d027dcf1fd624070e6c5d85`
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
# Fri, 01 Dec 2023 02:46:05 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 01 Dec 2023 02:46:05 GMT
ENV PHP_VERSION=8.2.13
# Fri, 01 Dec 2023 02:46:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Fri, 01 Dec 2023 02:46:05 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Fri, 01 Dec 2023 02:46:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 01 Dec 2023 02:46:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 01 Dec 2023 02:58:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 01 Dec 2023 02:58:57 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 01 Dec 2023 02:58:58 GMT
RUN docker-php-ext-enable sodium
# Fri, 01 Dec 2023 02:58:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 01 Dec 2023 02:58:59 GMT
WORKDIR /var/www/html
# Fri, 01 Dec 2023 02:58:59 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 01 Dec 2023 02:58:59 GMT
STOPSIGNAL SIGQUIT
# Fri, 01 Dec 2023 02:58:59 GMT
EXPOSE 9000
# Fri, 01 Dec 2023 02:58:59 GMT
CMD ["php-fpm"]
# Fri, 01 Dec 2023 10:50:32 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 01 Dec 2023 10:51:46 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 01 Dec 2023 10:51:47 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 01 Dec 2023 10:51:48 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Dec 2023 21:46:47 GMT
RUN set -eux; 	version='6.4.2'; 	sha1='d1aedbfea77b243b09e0ab05b100b782497406dd'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 07 Dec 2023 21:46:48 GMT
VOLUME [/var/www/html]
# Thu, 07 Dec 2023 21:46:48 GMT
COPY --chown=www-data:www-datafile:428b392bbc74b7aa0266d0b70812aab289561b5840fddd951986ac44165a331d in /usr/src/wordpress/ 
# Thu, 07 Dec 2023 21:46:48 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:46:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:46:48 GMT
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
	-	`sha256:75e15122d4b0622d0eeaa9c6d86620f623e55a81bdd65449a84d67ae055f9c2d`  
		Last Modified: Fri, 01 Dec 2023 04:09:56 GMT  
		Size: 12.1 MB (12089949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c83768c66a55023cba77c892eeaf9b5bf98c37210cf2deb3894f76d2cccfd506`  
		Last Modified: Fri, 01 Dec 2023 04:09:54 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841648ba2e7795fc2dca8bfbedc06a8837f18f3fbee12af4658d88e85bad7d97`  
		Last Modified: Fri, 01 Dec 2023 04:10:25 GMT  
		Size: 12.9 MB (12898920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44dd31eea04bcd5b23292df68d206d17d558c394e8f1963ae3af34f04d8354ad`  
		Last Modified: Fri, 01 Dec 2023 04:10:22 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6409a0df8bcce0e6c6bf4fa9533f7ca13bac7e2b0f824ba331e2cc6a158709a5`  
		Last Modified: Fri, 01 Dec 2023 04:10:22 GMT  
		Size: 18.9 KB (18927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81d1dbc4cee1ba305600a63ae74b399329430abf20dc780e4976837026938d4b`  
		Last Modified: Fri, 01 Dec 2023 04:10:22 GMT  
		Size: 9.2 KB (9179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04a9575d228521d0a2878b1de45525f65f03adf323ad7cf27bdde46615bc2aeb`  
		Last Modified: Fri, 01 Dec 2023 11:08:35 GMT  
		Size: 41.8 MB (41839916 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a47a8170f78e2d18b9a0a00d84ff340bd179ee30aba7efc1cd1cb125607752`  
		Last Modified: Fri, 01 Dec 2023 11:08:27 GMT  
		Size: 4.5 MB (4489169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:047d97634fc2f8447034204ab492c21749666aafca17029468ce5facc0be0934`  
		Last Modified: Fri, 01 Dec 2023 11:08:23 GMT  
		Size: 66.2 KB (66223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d37091728a322603fe5e86c24a107a41918ad69300ba25bce529957e524b0d93`  
		Last Modified: Fri, 01 Dec 2023 11:08:23 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9717d08b2908513d861990911369bb54c5a35f788257b1f59ad619c55ae0137`  
		Last Modified: Thu, 07 Dec 2023 21:50:52 GMT  
		Size: 24.3 MB (24309779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:067195c8ac7382cfc00e1baeb593f9d889db1444f3b11d2841de574427faff11`  
		Last Modified: Thu, 07 Dec 2023 21:50:46 GMT  
		Size: 2.3 KB (2349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:010f868ada6b944617bc984bdc81ac3993f1001e90f13c04318895d4d2e9cde0`  
		Last Modified: Thu, 07 Dec 2023 21:50:47 GMT  
		Size: 1.7 KB (1733 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:6-php8.2-fpm-alpine` - linux; ppc64le

```console
$ docker pull wordpress@sha256:fff4f71e61a840141a182503d07556e0d7df92b0c9a50031dae37332714cee84
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.2 MB (110227589 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e56d459b017899f710a256f534470987c2f0aae71abc0f3cda142d9929510a0`
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
# Fri, 01 Dec 2023 00:03:05 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Fri, 01 Dec 2023 00:03:09 GMT
ENV PHP_VERSION=8.2.13
# Fri, 01 Dec 2023 00:03:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Fri, 01 Dec 2023 00:03:14 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Fri, 01 Dec 2023 00:03:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 01 Dec 2023 00:03:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 01 Dec 2023 00:10:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 01 Dec 2023 00:10:33 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 01 Dec 2023 00:10:35 GMT
RUN docker-php-ext-enable sodium
# Fri, 01 Dec 2023 00:10:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 01 Dec 2023 00:10:39 GMT
WORKDIR /var/www/html
# Fri, 01 Dec 2023 00:10:47 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Fri, 01 Dec 2023 00:10:48 GMT
STOPSIGNAL SIGQUIT
# Fri, 01 Dec 2023 00:10:49 GMT
EXPOSE 9000
# Fri, 01 Dec 2023 00:10:49 GMT
CMD ["php-fpm"]
# Fri, 01 Dec 2023 03:50:44 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 01 Dec 2023 03:52:21 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 01 Dec 2023 03:52:24 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 01 Dec 2023 03:52:26 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Dec 2023 22:25:52 GMT
RUN set -eux; 	version='6.4.2'; 	sha1='d1aedbfea77b243b09e0ab05b100b782497406dd'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 07 Dec 2023 22:25:54 GMT
VOLUME [/var/www/html]
# Thu, 07 Dec 2023 22:25:54 GMT
COPY --chown=www-data:www-datafile:428b392bbc74b7aa0266d0b70812aab289561b5840fddd951986ac44165a331d in /usr/src/wordpress/ 
# Thu, 07 Dec 2023 22:25:54 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Dec 2023 22:25:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:25:55 GMT
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
	-	`sha256:bed9c8962a6b1061db6c45dcec8c8afcfa270d0d88920f8559a8c1b10518bda1`  
		Last Modified: Fri, 01 Dec 2023 00:55:58 GMT  
		Size: 12.1 MB (12089942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4adcb4960a3c972b2f4a61dc635dd020155c541b604d7ad67c02d1126aa22e44`  
		Last Modified: Fri, 01 Dec 2023 00:55:58 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d66109ee3fc1826e8d7ea66465a5101a25ba7a9f8ba69f43a1cd4d143d7ec8e8`  
		Last Modified: Fri, 01 Dec 2023 00:56:26 GMT  
		Size: 13.1 MB (13115978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6f62bd268e48f69ea9cec2efd6e504f49a299d75061e632a9d62332ae5ae94`  
		Last Modified: Fri, 01 Dec 2023 00:56:23 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93b0e1aeb6e86a69e188acaf2e3269b8a79a7cfc8beb8e33151286851f6bfeb5`  
		Last Modified: Fri, 01 Dec 2023 00:56:23 GMT  
		Size: 18.7 KB (18730 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6224767926b8a269da5fe6c5dd37801af594450357f6270dd7aeab92620bcd2`  
		Last Modified: Fri, 01 Dec 2023 00:56:24 GMT  
		Size: 9.2 KB (9180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:149a436d679cb2cfa1447080d3503bf7378750f905847fc765a308fb546d7921`  
		Last Modified: Fri, 01 Dec 2023 04:47:52 GMT  
		Size: 50.0 MB (49963623 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dafd87e7905658dfd6847d2a7867895c0931556174501c60911bd2ef72f19757`  
		Last Modified: Fri, 01 Dec 2023 04:47:44 GMT  
		Size: 4.5 MB (4530463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bd472ef7b007f3a5deb28a50c5bc34f9ddfa0bf7ed5addef71182bff36161fe`  
		Last Modified: Fri, 01 Dec 2023 04:47:41 GMT  
		Size: 66.2 KB (66212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd800c96f57c6c56c4105c530d7a6ea444be4126ef98ac6ba3b6f1d4cf7e680`  
		Last Modified: Fri, 01 Dec 2023 04:47:41 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e16a1c2ec2bf3442b425ef13a146d0f0a6b3d09e6ba6600c9b7018a8b0a9547`  
		Last Modified: Thu, 07 Dec 2023 22:30:12 GMT  
		Size: 24.3 MB (24309764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:102b557b9590e79527e69787cb9947ed8b36149dd0a2af3777d078ed961bc1ab`  
		Last Modified: Thu, 07 Dec 2023 22:30:08 GMT  
		Size: 2.3 KB (2349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c4145dfdf3541194825ea3de09d8811f01b24d2303a9908d13a38295410f6d4`  
		Last Modified: Thu, 07 Dec 2023 22:30:08 GMT  
		Size: 1.7 KB (1732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:6-php8.2-fpm-alpine` - linux; s390x

```console
$ docker pull wordpress@sha256:e9c5929226ac65c72916047cb692a77e6d3e1b01d7f270487f112d3139285327
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **103.6 MB (103637881 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:449c68565979a3228b5c9efb52cbb0dd28f5f664f9174c98ee9368e262aa58c3`
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
# Thu, 30 Nov 2023 23:06:49 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Thu, 30 Nov 2023 23:06:49 GMT
ENV PHP_VERSION=8.2.13
# Thu, 30 Nov 2023 23:06:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.13.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.13.tar.xz.asc
# Thu, 30 Nov 2023 23:06:49 GMT
ENV PHP_SHA256=2629bba10117bf78912068a230c68a8fd09b7740267bd8ebd3cfce91515d454b
# Thu, 30 Nov 2023 23:06:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 30 Nov 2023 23:06:53 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 30 Nov 2023 23:12:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 30 Nov 2023 23:12:19 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 30 Nov 2023 23:12:20 GMT
RUN docker-php-ext-enable sodium
# Thu, 30 Nov 2023 23:12:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 30 Nov 2023 23:12:20 GMT
WORKDIR /var/www/html
# Thu, 30 Nov 2023 23:12:21 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 30 Nov 2023 23:12:21 GMT
STOPSIGNAL SIGQUIT
# Thu, 30 Nov 2023 23:12:21 GMT
EXPOSE 9000
# Thu, 30 Nov 2023 23:12:21 GMT
CMD ["php-fpm"]
# Fri, 01 Dec 2023 02:14:55 GMT
RUN set -eux; 	apk add --no-cache 		bash 		ghostscript 		imagemagick 	;
# Fri, 01 Dec 2023 02:15:44 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		freetype-dev 		icu-dev 		imagemagick-dev 		libjpeg-turbo-dev 		libpng-dev 		libwebp-dev 		libzip-dev 	; 		docker-php-ext-configure gd 		--with-freetype 		--with-jpeg 		--with-webp 	; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		intl 		mysqli 		zip 	; 	pecl install imagick-3.6.0; 	docker-php-ext-enable imagick; 	rm -r /tmp/pear; 		out="$(php -r 'exit(0);')"; 	[ -z "$out" ]; 	err="$(php -r 'exit(0);' 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]; 		extDir="$(php -r 'echo ini_get("extension_dir");')"; 	[ -d "$extDir" ]; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive "$extDir" 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .wordpress-phpexts-rundeps $runDeps; 	apk del --no-network .build-deps; 		! { ldd "$extDir"/*.so | grep 'not found'; }; 	err="$(php --version 3>&1 1>&2 2>&3)"; 	[ -z "$err" ]
# Fri, 01 Dec 2023 02:15:46 GMT
RUN set -eux; 	docker-php-ext-enable opcache; 	{ 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 01 Dec 2023 02:15:46 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Thu, 07 Dec 2023 21:50:42 GMT
RUN set -eux; 	version='6.4.2'; 	sha1='d1aedbfea77b243b09e0ab05b100b782497406dd'; 		curl -o wordpress.tar.gz -fL "https://wordpress.org/wordpress-$version.tar.gz"; 	echo "$sha1 *wordpress.tar.gz" | sha1sum -c -; 		tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 		[ ! -e /usr/src/wordpress/.htaccess ]; 	{ 		echo '# BEGIN WordPress'; 		echo ''; 		echo 'RewriteEngine On'; 		echo 'RewriteRule .* - [E=HTTP_AUTHORIZATION:%{HTTP:Authorization}]'; 		echo 'RewriteBase /'; 		echo 'RewriteRule ^index\.php$ - [L]'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-f'; 		echo 'RewriteCond %{REQUEST_FILENAME} !-d'; 		echo 'RewriteRule . /index.php [L]'; 		echo ''; 		echo '# END WordPress'; 	} > /usr/src/wordpress/.htaccess; 		chown -R www-data:www-data /usr/src/wordpress; 	mkdir wp-content; 	for dir in /usr/src/wordpress/wp-content/*/ cache; do 		dir="$(basename "${dir%/}")"; 		mkdir "wp-content/$dir"; 	done; 	chown -R www-data:www-data wp-content; 	chmod -R 1777 wp-content
# Thu, 07 Dec 2023 21:50:44 GMT
VOLUME [/var/www/html]
# Thu, 07 Dec 2023 21:50:44 GMT
COPY --chown=www-data:www-datafile:428b392bbc74b7aa0266d0b70812aab289561b5840fddd951986ac44165a331d in /usr/src/wordpress/ 
# Thu, 07 Dec 2023 21:50:44 GMT
COPY file:5be6bcc31206cb827f037769d89fd092037ed61a1e10d6cae7939a37055beb4c in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:50:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:50:44 GMT
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
	-	`sha256:a639bb74c8bc3bb0e993f8be2ff5fbc4e8a44b22c7e9438db204d77471f9954e`  
		Last Modified: Thu, 30 Nov 2023 23:49:17 GMT  
		Size: 12.1 MB (12089942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939f3beba64a47c9389e55c1fa3dfea2bc04780e13a3a78404f505d98153d5c2`  
		Last Modified: Thu, 30 Nov 2023 23:49:17 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871a04924538931cf94ef8acf4886aea1410a32d9a52b16242e5736bff4eb108`  
		Last Modified: Thu, 30 Nov 2023 23:49:32 GMT  
		Size: 11.9 MB (11861249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea71f3db8cdb85d8129506ee3c7b14274cce3cf20f353be7147c9eecab45bb7a`  
		Last Modified: Thu, 30 Nov 2023 23:49:30 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e0f733773ac893bf16c99b89e9a98391cadec7da41d106c8838c2db43cc91a`  
		Last Modified: Thu, 30 Nov 2023 23:49:31 GMT  
		Size: 18.8 KB (18771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da14478326d758bad6aa82b0e327f1bdf7854757a9e0f3b2e476869d3d1735a5`  
		Last Modified: Thu, 30 Nov 2023 23:49:30 GMT  
		Size: 9.2 KB (9178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a29056feccc8835a0c17c1f17ddbe08729c5ae0bb56b3d92e9595a6a95d849e`  
		Last Modified: Fri, 01 Dec 2023 02:27:36 GMT  
		Size: 44.8 MB (44799249 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07b8d816173e32d012411871f10815cb8c14859bb759181ceff1c8ef4ea56fcb`  
		Last Modified: Fri, 01 Dec 2023 02:27:31 GMT  
		Size: 4.5 MB (4467683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8579bd1d18255bf1628c2366f4561d9e7a16a41d81d8b46686de3626e42bdfdf`  
		Last Modified: Fri, 01 Dec 2023 02:27:28 GMT  
		Size: 65.8 KB (65758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51a7e1a3b4b7143603edd3bcdf29867ab65ddc60c8087f31093669b4811d5bb`  
		Last Modified: Fri, 01 Dec 2023 02:27:29 GMT  
		Size: 391.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e72fae3f7ad09841d18c69694fcbe77204eae55b938da0dacb1ba95dba34843`  
		Last Modified: Thu, 07 Dec 2023 21:54:23 GMT  
		Size: 24.3 MB (24309770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9bb752272bd53197240777674de6534dfd3fc75d3f2e2d1211959efab7db314`  
		Last Modified: Thu, 07 Dec 2023 21:54:20 GMT  
		Size: 2.3 KB (2349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de22275d7ddb183aee572e0cd1f903fd08aa91f41f3af8763168e79f5ff43733`  
		Last Modified: Thu, 07 Dec 2023 21:54:20 GMT  
		Size: 1.7 KB (1736 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
