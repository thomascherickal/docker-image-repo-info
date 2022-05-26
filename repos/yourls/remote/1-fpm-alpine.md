## `yourls:1-fpm-alpine`

```console
$ docker pull yourls@sha256:e342632fcf02f49dbcc54ec3ef6c4220d1b547fdf1a44c472ebbedd99a12b4c8
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

### `yourls:1-fpm-alpine` - linux; amd64

```console
$ docker pull yourls@sha256:b2622fb68b4c28a117be9b7eaeda96e6cf373e74a93db13f9ce8cef722ce1293
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.6 MB (33574181 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e00f091632791d934f3b255ab0bd25de33f00031ae267143d57e3c67d2aa7f84`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 19:48:06 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 19:48:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 19:48:09 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 19:48:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 19:48:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 19:48:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:48:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:48:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 19:48:10 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 25 May 2022 19:48:10 GMT
ENV PHP_VERSION=8.1.6
# Wed, 25 May 2022 19:48:10 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Wed, 25 May 2022 19:48:10 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Wed, 25 May 2022 19:48:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 25 May 2022 19:48:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 25 May 2022 19:56:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 25 May 2022 19:56:28 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 25 May 2022 19:56:30 GMT
RUN docker-php-ext-enable sodium
# Wed, 25 May 2022 19:56:30 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 25 May 2022 19:56:30 GMT
WORKDIR /var/www/html
# Wed, 25 May 2022 19:56:30 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 25 May 2022 19:56:30 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 May 2022 19:56:31 GMT
EXPOSE 9000
# Wed, 25 May 2022 19:56:31 GMT
CMD ["php-fpm"]
# Thu, 26 May 2022 00:28:56 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 26 May 2022 00:28:57 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 26 May 2022 00:28:57 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 26 May 2022 00:28:57 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 26 May 2022 00:28:57 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 26 May 2022 00:28:57 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 26 May 2022 00:28:57 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 26 May 2022 00:29:51 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 26 May 2022 00:29:52 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 26 May 2022 00:29:53 GMT
RUN apk add --no-cache bash
# Thu, 26 May 2022 00:29:53 GMT
ARG YOURLS_VERSION=1.9
# Thu, 26 May 2022 00:29:53 GMT
ARG YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Thu, 26 May 2022 00:29:53 GMT
LABEL org.opencontainers.image.version=1.9
# Thu, 26 May 2022 00:29:53 GMT
ENV YOURLS_VERSION=1.9
# Thu, 26 May 2022 00:29:53 GMT
ENV YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Thu, 26 May 2022 00:29:55 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 26 May 2022 00:29:56 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 26 May 2022 00:29:56 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 26 May 2022 00:29:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 May 2022 00:29:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fde5ea1cb188409ac6276c7e55f3a6f6b0dfe9e3bd72711881e32183f03e8d99`  
		Last Modified: Wed, 25 May 2022 20:28:12 GMT  
		Size: 1.7 MB (1704858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3935ba60366aecf1bc3d1f0c663cb07711d490232ffa0ddde876eb4ebc40e469`  
		Last Modified: Wed, 25 May 2022 20:28:11 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4712e34f1d293d5afd1871939afc2d84d672bf03d6c4ef9c9558c720f40e5195`  
		Last Modified: Wed, 25 May 2022 20:28:11 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc3d7d2af8f28d51531216a7a44dfdf45f73158bb31093bdb95640f5a4341ea`  
		Last Modified: Wed, 25 May 2022 20:28:09 GMT  
		Size: 11.7 MB (11728849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2370c00e68b7dec0e32d562a3618a78fa9849210ccd45c420190d09209faf67`  
		Last Modified: Wed, 25 May 2022 20:28:09 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8af7b7a3cca411d68c0ebe7cbdc487d608613236700887b0da544eee4ed9c6`  
		Last Modified: Wed, 25 May 2022 20:29:02 GMT  
		Size: 12.4 MB (12361231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dad926bf9ecbc361cf7b02acb1ebc20027444e93f9265911a26033d23eadb010`  
		Last Modified: Wed, 25 May 2022 20:29:00 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1fad0bc29ddb13c4a35b1cf238007e4d361a97785e8f0b66d31c7a41c9e7bd4`  
		Last Modified: Wed, 25 May 2022 20:29:00 GMT  
		Size: 18.6 KB (18553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36ca02b1c80fc8c3ae27d279e505d91dc134fcee840b213ea92e5abb0d4918c3`  
		Last Modified: Wed, 25 May 2022 20:29:00 GMT  
		Size: 8.6 KB (8617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef119162516bdf19637752d6adc946fe43e223ad95819751fb89bf056faa24a`  
		Last Modified: Thu, 26 May 2022 00:30:26 GMT  
		Size: 533.4 KB (533359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aeaee4302da4d7e576224016943fbe6b3d9fe844c83dec5038a9d175774519b`  
		Last Modified: Thu, 26 May 2022 00:30:24 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc3f6fac41c217c50bea5dc5944944a1b5eeb4079c625098a82ff34ca0771e63`  
		Last Modified: Thu, 26 May 2022 00:30:24 GMT  
		Size: 467.0 KB (467042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c132ffd716b911b6751c1cc8cba2fb26ec349c122f2ceadbd67d4230d21830da`  
		Last Modified: Thu, 26 May 2022 00:30:25 GMT  
		Size: 3.9 MB (3944394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfb9825f0a6abd7e4aa5b5bb656036edf92500d60b08a642171058553d7fd6b0`  
		Last Modified: Thu, 26 May 2022 00:30:24 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffedf0bc6cf63474a2dc1d338ae1feded3895c90fc0d8824ef09f17d3430ebce`  
		Last Modified: Thu, 26 May 2022 00:30:24 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; arm variant v6

```console
$ docker pull yourls@sha256:6de4c4b553161daf503453ebc3874ca3d86a000c8ff0c733ae5f0781e18b71a5
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.9 MB (31858699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f80aa8e039bf58636833f4601f21a76dbe16b90781bc7cd631bef2a4bbab998`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 May 2022 19:49:32 GMT
ADD file:f7cee617575b5e5a7672d298a519bb8d8b5098efb90aa2a5d7b0510003457d52 in / 
# Mon, 23 May 2022 19:49:33 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 21:50:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 21:50:07 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 21:50:08 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 21:50:09 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 21:50:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 21:50:11 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 21:50:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 21:50:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 21:50:12 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 25 May 2022 21:50:12 GMT
ENV PHP_VERSION=8.1.6
# Wed, 25 May 2022 21:50:13 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Wed, 25 May 2022 21:50:13 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Wed, 25 May 2022 21:50:22 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 25 May 2022 21:50:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 25 May 2022 22:00:40 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 25 May 2022 22:00:42 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 25 May 2022 22:00:45 GMT
RUN docker-php-ext-enable sodium
# Wed, 25 May 2022 22:00:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 25 May 2022 22:00:46 GMT
WORKDIR /var/www/html
# Wed, 25 May 2022 22:00:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 25 May 2022 22:00:49 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 May 2022 22:00:50 GMT
EXPOSE 9000
# Wed, 25 May 2022 22:00:50 GMT
CMD ["php-fpm"]
# Thu, 26 May 2022 02:43:53 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 26 May 2022 02:43:54 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 26 May 2022 02:43:54 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 26 May 2022 02:43:55 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 26 May 2022 02:43:55 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 26 May 2022 02:43:55 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 26 May 2022 02:43:56 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 26 May 2022 02:44:59 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 26 May 2022 02:45:01 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 26 May 2022 02:45:03 GMT
RUN apk add --no-cache bash
# Thu, 26 May 2022 02:45:04 GMT
ARG YOURLS_VERSION=1.9
# Thu, 26 May 2022 02:45:04 GMT
ARG YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Thu, 26 May 2022 02:45:04 GMT
LABEL org.opencontainers.image.version=1.9
# Thu, 26 May 2022 02:45:05 GMT
ENV YOURLS_VERSION=1.9
# Thu, 26 May 2022 02:45:05 GMT
ENV YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Thu, 26 May 2022 02:45:09 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 26 May 2022 02:45:10 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 26 May 2022 02:45:10 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 26 May 2022 02:45:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 May 2022 02:45:11 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:79a25ccaf940855872635c06e7614d9b27dd38ffb5a8adfdb9274dfdc0ea0d87`  
		Last Modified: Mon, 23 May 2022 19:08:47 GMT  
		Size: 2.6 MB (2606142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39e7eae6d0293087d982d321125f6f132894675f6acb732427528058758d6ae3`  
		Last Modified: Wed, 25 May 2022 22:46:23 GMT  
		Size: 1.7 MB (1693282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad96c7e3fdd13c53c906a10fab89b0dc599bf1746acd163f9648f8f9ec949de`  
		Last Modified: Wed, 25 May 2022 22:46:21 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1acccbd45290b92307c479937198ace1c187e0fd49d5e1ea72c1f5d7d5e1705`  
		Last Modified: Wed, 25 May 2022 22:46:21 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1842ff51cd1241f5cd22b72ce83b11e98d68afdfe3e4ca4fb12d0389822470d2`  
		Last Modified: Wed, 25 May 2022 22:46:22 GMT  
		Size: 11.7 MB (11728842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5dd0b482cb5d553f8f814d7435c7be9c69b3ac1d825cd2298e0e98e6198c6e`  
		Last Modified: Wed, 25 May 2022 22:46:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85f049a690032628c8886843dddfb7ec5b518cd69e66bbbed01c78aa9632b1d1`  
		Last Modified: Wed, 25 May 2022 22:47:46 GMT  
		Size: 11.2 MB (11229078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eb48b70ed3967b153ab36cf94b68b8294ee63f90fd9a6be1205a399f86e892a`  
		Last Modified: Wed, 25 May 2022 22:47:38 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:882db848f544ca2dcc7815c2fa53c336ba273b48d57e1bed088d5e05c3643482`  
		Last Modified: Wed, 25 May 2022 22:47:38 GMT  
		Size: 18.4 KB (18366 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4063d6c0419ad992bef551c93788fea3e7578a568e774a570d99adcc82f85151`  
		Last Modified: Wed, 25 May 2022 22:47:38 GMT  
		Size: 8.6 KB (8619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b79190132d002b3aa2ec7b05c4542f961b4dd5db5403e0634f0f971120131441`  
		Last Modified: Thu, 26 May 2022 02:45:44 GMT  
		Size: 167.3 KB (167310 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02257f0334d3b2222518363f7822e89c96132565ac4835626e6537cb02bbc00f`  
		Last Modified: Thu, 26 May 2022 02:45:42 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afdc29ecc20dae93acd330a2ac14938741743f5eab9f5d6af42dab29bbd7c5b5`  
		Last Modified: Thu, 26 May 2022 02:45:42 GMT  
		Size: 454.3 KB (454279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd0dd22cd65dda6940f7e66a1c3605c4d87679242dc8a4b4e76b06c9d70e46bc`  
		Last Modified: Thu, 26 May 2022 02:45:45 GMT  
		Size: 3.9 MB (3944386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da3494665216128f2fe21cf2ae7d447528445fc31a3e4e1992fe100238a171b7`  
		Last Modified: Thu, 26 May 2022 02:45:42 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bddcc728531a57968535659e232b15e5b7fd8c254f4659148a75df564135a2b2`  
		Last Modified: Thu, 26 May 2022 02:45:42 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; arm variant v7

```console
$ docker pull yourls@sha256:c68d311c3aa040c3895d09dc69c7193f6f4e74e9ccc2975d583613ecde72a01e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32278428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd043ee7afa5a4b678704cb983cbb6a20099d673d7f337dc3444cfca0351ca15`
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
# Fri, 13 May 2022 22:42:30 GMT
ENV PHP_VERSION=8.1.6
# Fri, 13 May 2022 22:42:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Fri, 13 May 2022 22:42:31 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Fri, 13 May 2022 22:42:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 13 May 2022 22:42:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 13 May 2022 22:51:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 13 May 2022 22:51:36 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 13 May 2022 22:51:39 GMT
RUN docker-php-ext-enable sodium
# Fri, 13 May 2022 22:51:39 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 13 May 2022 22:51:40 GMT
WORKDIR /var/www/html
# Fri, 13 May 2022 22:51:42 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 13 May 2022 22:51:43 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 May 2022 22:51:43 GMT
EXPOSE 9000
# Fri, 13 May 2022 22:51:43 GMT
CMD ["php-fpm"]
# Sat, 14 May 2022 01:39:47 GMT
LABEL org.opencontainers.image.title=YOURLS
# Sat, 14 May 2022 01:39:48 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Sat, 14 May 2022 01:39:48 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Sat, 14 May 2022 01:39:48 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Sat, 14 May 2022 01:39:49 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Sat, 14 May 2022 01:39:49 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Sat, 14 May 2022 01:39:50 GMT
LABEL org.opencontainers.image.licenses=MIT
# Sat, 14 May 2022 01:40:48 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 14 May 2022 01:40:49 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 14 May 2022 01:40:51 GMT
RUN apk add --no-cache bash
# Sat, 14 May 2022 01:40:52 GMT
ARG YOURLS_VERSION=1.9
# Sat, 14 May 2022 01:40:52 GMT
ARG YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Sat, 14 May 2022 01:40:53 GMT
LABEL org.opencontainers.image.version=1.9
# Sat, 14 May 2022 01:40:53 GMT
ENV YOURLS_VERSION=1.9
# Sat, 14 May 2022 01:40:53 GMT
ENV YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Sat, 14 May 2022 01:40:57 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 14 May 2022 01:40:58 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Sat, 14 May 2022 01:40:58 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Sat, 14 May 2022 01:40:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 May 2022 01:40:59 GMT
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
	-	`sha256:a7eb30f8e454a086b270e51b3a84e238e34f2376558f0ccb9e8528302e9551e1`  
		Last Modified: Fri, 13 May 2022 23:39:46 GMT  
		Size: 11.7 MB (11728867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456cea678444662ecadb26cdefe80bbb6d812324d004154576daa07d2ff7dd2e`  
		Last Modified: Fri, 13 May 2022 23:39:43 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cce49f440af83c9a78eced4e0f4c6e36c7febca0063171aa376fe59fb00cc24`  
		Last Modified: Fri, 13 May 2022 23:41:08 GMT  
		Size: 12.0 MB (12016802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:406d317e43c0dfbd7103ffb26542f456fdbe21739ef4c12bae2143dd0d5357c6`  
		Last Modified: Fri, 13 May 2022 23:41:01 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d912b8140e615f6e52cb831a2da7ce0bbeb07dde8d009f7369a8307ab7f7f96f`  
		Last Modified: Fri, 13 May 2022 23:41:00 GMT  
		Size: 18.5 KB (18513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0171425e03740f64cc65246e1a1bcf5d3be7a47e8c1827281d0f722a768c570`  
		Last Modified: Fri, 13 May 2022 23:41:01 GMT  
		Size: 8.6 KB (8620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cea44f2b1ab3a4710b6a53af3f2b12406d2a853f093f808577794bd249f6e495`  
		Last Modified: Sat, 14 May 2022 01:43:06 GMT  
		Size: 156.4 KB (156387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d3571ab2b2a74e457fce9e94ffc2c700c671f9699084a0f047a7feac6c3d6c`  
		Last Modified: Sat, 14 May 2022 01:43:04 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12b7f7f512034738d563f763df4ab192a9abe9e1f2cf20dc8ab46a5fb8559437`  
		Last Modified: Sat, 14 May 2022 01:43:05 GMT  
		Size: 415.7 KB (415665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db24225600de6f4e09aafbb6a1c04f073959cca3a099e1a7fc6ba9c3399d1bfa`  
		Last Modified: Sat, 14 May 2022 01:43:07 GMT  
		Size: 3.9 MB (3944387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d97c00c248dfaf75310208715798bf53190c4ec7928bd6533ba9148110fe09`  
		Last Modified: Sat, 14 May 2022 01:43:06 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a0394ca449cc00fa7b1ea5ab5bff8340e6833c29a3ab26eaef2471e1e055e92`  
		Last Modified: Sat, 14 May 2022 01:43:04 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:7883c9930a5310e3aacd49198c3cfee4eeccaf0f5465173798d5bce4917e2015
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.8 MB (33806142 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:97b0d2240665cbcfdd91779b2844bb24a64b56cd03155ebe219b9b1b40ae2a48`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 20:06:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 20:06:19 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 20:06:20 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 20:06:21 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 20:06:22 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 20:06:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 20:06:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 20:06:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 20:06:26 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 25 May 2022 20:06:27 GMT
ENV PHP_VERSION=8.1.6
# Wed, 25 May 2022 20:06:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Wed, 25 May 2022 20:06:29 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Wed, 25 May 2022 20:06:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 25 May 2022 20:06:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 25 May 2022 20:27:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 25 May 2022 20:27:48 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 25 May 2022 20:27:49 GMT
RUN docker-php-ext-enable sodium
# Wed, 25 May 2022 20:27:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 25 May 2022 20:27:51 GMT
WORKDIR /var/www/html
# Wed, 25 May 2022 20:27:52 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 25 May 2022 20:27:53 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 May 2022 20:27:54 GMT
EXPOSE 9000
# Wed, 25 May 2022 20:27:55 GMT
CMD ["php-fpm"]
# Thu, 26 May 2022 01:21:56 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 26 May 2022 01:21:57 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 26 May 2022 01:21:58 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 26 May 2022 01:21:59 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 26 May 2022 01:22:00 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 26 May 2022 01:22:01 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 26 May 2022 01:22:02 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 26 May 2022 01:25:16 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 26 May 2022 01:25:17 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 26 May 2022 01:25:19 GMT
RUN apk add --no-cache bash
# Thu, 26 May 2022 01:25:20 GMT
ARG YOURLS_VERSION=1.9
# Thu, 26 May 2022 01:25:21 GMT
ARG YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Thu, 26 May 2022 01:25:22 GMT
LABEL org.opencontainers.image.version=1.9
# Thu, 26 May 2022 01:25:23 GMT
ENV YOURLS_VERSION=1.9
# Thu, 26 May 2022 01:25:24 GMT
ENV YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Thu, 26 May 2022 01:25:27 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 26 May 2022 01:25:29 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 26 May 2022 01:25:30 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 26 May 2022 01:25:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 May 2022 01:25:31 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6a240d0a51bf6100803c8ce9f1ce769377fd09a2824a580ad991fb1a8a64610`  
		Last Modified: Wed, 25 May 2022 21:26:48 GMT  
		Size: 1.7 MB (1703255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d989eb157716fb2e84408b95764324504b7dd9aac628dd9a66a7f15eeb43a66`  
		Last Modified: Wed, 25 May 2022 21:26:48 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:940028d0e55a77f4d9df2de18c1a76fa1058bdb66dee66fa6309f9337e500d6e`  
		Last Modified: Wed, 25 May 2022 21:26:48 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42f067a62df3579043ff26a92694b04ef25e184d04a5a9b5dd2f910ff0798cc2`  
		Last Modified: Wed, 25 May 2022 21:26:47 GMT  
		Size: 11.7 MB (11728607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeaaef60a8ac82e391742a21b4b071c059ad7017227191e1c5b936051886bc1b`  
		Last Modified: Wed, 25 May 2022 21:26:45 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d023afabb4d3f7acd8aa539577cd88941bfa9f49527b8876a325412b1a786302`  
		Last Modified: Wed, 25 May 2022 21:27:45 GMT  
		Size: 12.4 MB (12415755 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e96613d40681eef5567520e6c77dbafd9c9bb8580043b7c51e03d8aad653a696`  
		Last Modified: Wed, 25 May 2022 21:27:43 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:689813d325d9a2f2f6796715cdb7245eeb615c077f7175d6a4734ff0f05a23f5`  
		Last Modified: Wed, 25 May 2022 21:27:43 GMT  
		Size: 18.3 KB (18255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93d0cc0869f99665a037d34747a0535385fd62bf44ac0fe1fd272cd2f6be3a00`  
		Last Modified: Wed, 25 May 2022 21:27:43 GMT  
		Size: 8.6 KB (8621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:503106cb694067991d868885a63f2b04105e5dbac3165a6280886a3a6cb564a6`  
		Last Modified: Thu, 26 May 2022 01:26:10 GMT  
		Size: 811.0 KB (810997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d772dd0f850913d767d0506af5e03769e8d61b61ae1af023bcc999d9c697e6e1`  
		Last Modified: Thu, 26 May 2022 01:26:08 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fbb71855a0efaa3871ec21ae9623d5bf766c1c2cea874033d556837be6effd1`  
		Last Modified: Thu, 26 May 2022 01:26:11 GMT  
		Size: 473.5 KB (473540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fc864bfb25e4696e02fb1f085d454092b299e7864fd9f84b84f78003bc531b7`  
		Last Modified: Thu, 26 May 2022 01:26:08 GMT  
		Size: 3.9 MB (3944326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff0efa201d23799f6ffe92bb22ccaa1361af415b33bfd888627e6c73ef697c77`  
		Last Modified: Thu, 26 May 2022 01:26:11 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b26bc6fd3905ab97be2eedad25ad5369475fc93814acefeda810d791fc003ef5`  
		Last Modified: Thu, 26 May 2022 01:26:07 GMT  
		Size: 1.6 KB (1550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; 386

```console
$ docker pull yourls@sha256:ffa21621d7d301d27d57a627c3342fe29bd3b60235a8b038b2a69a5b0c65f660
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (33988714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2d97174449525100404d3624bf0de3b35ee050227a5a2392032eab493d718fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 May 2022 19:38:20 GMT
ADD file:1750ccfabfe93636015070d51a6e824cbd738056223421c69d8aaabc38041b18 in / 
# Mon, 23 May 2022 19:38:20 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 19:56:25 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 19:56:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 19:56:28 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 19:56:29 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 19:56:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 19:56:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:56:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 19:56:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 19:56:34 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 25 May 2022 19:56:35 GMT
ENV PHP_VERSION=8.1.6
# Wed, 25 May 2022 19:56:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Wed, 25 May 2022 19:56:37 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Wed, 25 May 2022 19:56:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 25 May 2022 19:56:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 25 May 2022 20:04:51 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 25 May 2022 20:04:52 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 25 May 2022 20:04:52 GMT
RUN docker-php-ext-enable sodium
# Wed, 25 May 2022 20:04:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 25 May 2022 20:04:54 GMT
WORKDIR /var/www/html
# Wed, 25 May 2022 20:04:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 25 May 2022 20:04:56 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 May 2022 20:04:57 GMT
EXPOSE 9000
# Wed, 25 May 2022 20:04:58 GMT
CMD ["php-fpm"]
# Thu, 26 May 2022 00:40:38 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 26 May 2022 00:40:39 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 26 May 2022 00:40:40 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 26 May 2022 00:40:41 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 26 May 2022 00:40:42 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 26 May 2022 00:40:43 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 26 May 2022 00:40:44 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 26 May 2022 00:41:40 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 26 May 2022 00:41:40 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 26 May 2022 00:41:42 GMT
RUN apk add --no-cache bash
# Thu, 26 May 2022 00:41:42 GMT
ARG YOURLS_VERSION=1.9
# Thu, 26 May 2022 00:41:43 GMT
ARG YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Thu, 26 May 2022 00:41:44 GMT
LABEL org.opencontainers.image.version=1.9
# Thu, 26 May 2022 00:41:45 GMT
ENV YOURLS_VERSION=1.9
# Thu, 26 May 2022 00:41:46 GMT
ENV YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Thu, 26 May 2022 00:41:49 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 26 May 2022 00:41:50 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 26 May 2022 00:41:51 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 26 May 2022 00:41:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 May 2022 00:41:52 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:bb638a3869eed698f88775c7a48f36f8e22e7c6bbaa98fa1d5678966b619b859`  
		Last Modified: Mon, 23 May 2022 19:09:25 GMT  
		Size: 2.8 MB (2801887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97eb700ff81c1dbea3f8e204a809be7b7431ba817b16c87c1efe84972e2fe6c1`  
		Last Modified: Wed, 25 May 2022 20:43:18 GMT  
		Size: 1.8 MB (1807504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eaabb95698f746340e8771d50f4e356e03ad67347638c9d30dc7d3d7cdb3359`  
		Last Modified: Wed, 25 May 2022 20:43:18 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f127678bc84e9717b47e929fd82c70e9bc39b96e731eb561d466d4373561cd1`  
		Last Modified: Wed, 25 May 2022 20:43:17 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0a74f89ed523fa6c81a7bd2f7a2f9d56fec9eb5ade225ae27574d601c83b2c6`  
		Last Modified: Wed, 25 May 2022 20:43:17 GMT  
		Size: 11.7 MB (11728596 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26de6301808ce43b4fdde9e7b64c1f4c5404296ebf9c02558edea07dca502f90`  
		Last Modified: Wed, 25 May 2022 20:43:15 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa89c1d454319054d3d5823f06e4e6bc870759ef4d85e0fd32e6787fd9df008c`  
		Last Modified: Wed, 25 May 2022 20:44:19 GMT  
		Size: 12.7 MB (12653017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eae6089d6ed68ded8e0a913d5bf0544de3a5dcdeb8648bafb4c06686b0ae91c9`  
		Last Modified: Wed, 25 May 2022 20:44:17 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1350d4bf4147f136c0a949448eceef442ee7fea9a6e11f00ccb842b79444b0`  
		Last Modified: Wed, 25 May 2022 20:44:17 GMT  
		Size: 18.5 KB (18458 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e7937d70ecb38d06fb8523bbaf73fd292c525bd9ae887056b74dcd3bf373292`  
		Last Modified: Wed, 25 May 2022 20:44:17 GMT  
		Size: 8.6 KB (8619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c94fefe536c5ea9c8315328e5d588ad82ba39af384507f44163291c67c27d8b4`  
		Last Modified: Thu, 26 May 2022 00:42:40 GMT  
		Size: 514.3 KB (514252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335447aafc25f63a888e4191e3c1f0879eea947c217e4c8200a1e17f3f50037c`  
		Last Modified: Thu, 26 May 2022 00:42:37 GMT  
		Size: 322.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:902e92ea4e3504cd76cae9d10b85677e273ef9434ab4a60941a2e4356b13ed5a`  
		Last Modified: Thu, 26 May 2022 00:42:37 GMT  
		Size: 503.8 KB (503751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffbb121f4ff56f1c0e1ef42fae93ad985af40cca08ec0523545674c987424b05`  
		Last Modified: Thu, 26 May 2022 00:42:38 GMT  
		Size: 3.9 MB (3944320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc4ce87cde30f10a0a89b53d1bae7818f17c120df9f9304bb2c7f4e65663cab`  
		Last Modified: Thu, 26 May 2022 00:42:37 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2708fb4a2ef5a9a303d699eff9675bfbe43f6a1e60958be1278dcaabc27bad98`  
		Last Modified: Thu, 26 May 2022 00:42:37 GMT  
		Size: 1.5 KB (1549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; ppc64le

```console
$ docker pull yourls@sha256:4bb9b448dde19c57f82ee92a661393f4e5e97ab1dd5e1e08cb1862a67f1b46ad
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.5 MB (35520264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed9c5bf578628912d75226898e86c2210efa4263b47c8731d036b9fabad8e098`
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
# Fri, 13 May 2022 23:19:04 GMT
ENV PHP_VERSION=8.1.6
# Fri, 13 May 2022 23:19:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Fri, 13 May 2022 23:19:12 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Fri, 13 May 2022 23:19:45 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 13 May 2022 23:19:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 13 May 2022 23:30:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 13 May 2022 23:30:59 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Fri, 13 May 2022 23:31:07 GMT
RUN docker-php-ext-enable sodium
# Fri, 13 May 2022 23:31:11 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 13 May 2022 23:31:14 GMT
WORKDIR /var/www/html
# Fri, 13 May 2022 23:31:20 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 13 May 2022 23:31:24 GMT
STOPSIGNAL SIGQUIT
# Fri, 13 May 2022 23:31:26 GMT
EXPOSE 9000
# Fri, 13 May 2022 23:31:31 GMT
CMD ["php-fpm"]
# Sat, 14 May 2022 04:07:40 GMT
LABEL org.opencontainers.image.title=YOURLS
# Sat, 14 May 2022 04:07:44 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Sat, 14 May 2022 04:07:47 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Sat, 14 May 2022 04:07:51 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Sat, 14 May 2022 04:07:55 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Sat, 14 May 2022 04:07:59 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Sat, 14 May 2022 04:08:01 GMT
LABEL org.opencontainers.image.licenses=MIT
# Sat, 14 May 2022 04:09:01 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Sat, 14 May 2022 04:09:21 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 14 May 2022 04:09:45 GMT
RUN apk add --no-cache bash
# Sat, 14 May 2022 04:10:01 GMT
ARG YOURLS_VERSION=1.9
# Sat, 14 May 2022 04:10:11 GMT
ARG YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Sat, 14 May 2022 04:10:20 GMT
LABEL org.opencontainers.image.version=1.9
# Sat, 14 May 2022 04:10:31 GMT
ENV YOURLS_VERSION=1.9
# Sat, 14 May 2022 04:10:43 GMT
ENV YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Sat, 14 May 2022 04:11:04 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 14 May 2022 04:11:10 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Sat, 14 May 2022 04:11:12 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Sat, 14 May 2022 04:11:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 14 May 2022 04:11:22 GMT
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
	-	`sha256:815dd04a8bcd1b0eb3a2dc1d62eac13ea5fe12bd1250c518230ea035e64b57f0`  
		Last Modified: Sat, 14 May 2022 00:15:56 GMT  
		Size: 11.7 MB (11728887 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9892dc7be9eb13a8eb6af62271dd07fa6a2df09b411794a3120e5107c2fa9fa3`  
		Last Modified: Sat, 14 May 2022 00:15:54 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2dad0369d79cadb91ad115f5c994f3fd56e6ba3df9aa7806ce9a80a96820d82`  
		Last Modified: Sat, 14 May 2022 00:17:15 GMT  
		Size: 14.5 MB (14524298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c512ddd8ac28208aad0b7f26d24c06039387f7edb196cdfab195169f0d9eb4`  
		Last Modified: Sat, 14 May 2022 00:17:12 GMT  
		Size: 2.4 KB (2447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0df393653f865ca4e418cfa34f41e50676d1244e8e109670ed0697ee4ae3d49`  
		Last Modified: Sat, 14 May 2022 00:17:12 GMT  
		Size: 18.5 KB (18527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d9c11960e0e8c031bfe6f66b344e96399977bf25b3dfef2610b8a4be4b1452`  
		Last Modified: Sat, 14 May 2022 00:17:12 GMT  
		Size: 8.6 KB (8624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bad2f9a849ac761c41850dd41dd83a7808b01294c70996be5dd3123e78a578d`  
		Last Modified: Sat, 14 May 2022 04:13:39 GMT  
		Size: 202.5 KB (202540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c103a2144802298c168a214188b24d8abd08afb8e4e4887bfad360fefb7622`  
		Last Modified: Sat, 14 May 2022 04:13:35 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7da8ce65c0defc88c48d788c2dec19f5ea0e130abe9bc43fe19e3affc70e0917`  
		Last Modified: Sat, 14 May 2022 04:13:35 GMT  
		Size: 528.7 KB (528749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e378a1c8389bf77d9338811374444f481aa9038d0923425dda964c1822ee193`  
		Last Modified: Sat, 14 May 2022 04:13:36 GMT  
		Size: 3.9 MB (3944398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdda5a3a61eedd082f55f870a1ca9fc65843b6738c2390b80bb712b79f41f5c6`  
		Last Modified: Sat, 14 May 2022 04:13:35 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15699a261f036218b8ed84b8bd16bfafb4410f2e1f2dafac73499de4f8dbb367`  
		Last Modified: Sat, 14 May 2022 04:13:35 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; s390x

```console
$ docker pull yourls@sha256:aaf1f67707a85c43ec349e6e7344b658fb65d6ffaa95683e498bd0417cda22bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32267205 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e6174d0e85a27a91a17714a4e000ceb76e1e314b14b61d49271a4c94a45d5ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Wed, 25 May 2022 20:06:36 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 25 May 2022 20:06:39 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 25 May 2022 20:06:40 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 25 May 2022 20:06:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 25 May 2022 20:06:42 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 25 May 2022 20:06:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 20:06:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 25 May 2022 20:06:43 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 25 May 2022 20:06:43 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 25 May 2022 20:06:43 GMT
ENV PHP_VERSION=8.1.6
# Wed, 25 May 2022 20:06:43 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.6.tar.xz.asc
# Wed, 25 May 2022 20:06:44 GMT
ENV PHP_SHA256=da38d65bb0d5dd56f711cd478204f2b62a74a2c2b0d2d523a78d6eb865b2364c
# Wed, 25 May 2022 20:06:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 25 May 2022 20:06:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 25 May 2022 20:17:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		gnu-libiconv-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		rm -vf /usr/include/iconv.h; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv=/usr 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 25 May 2022 20:17:39 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 25 May 2022 20:17:42 GMT
RUN docker-php-ext-enable sodium
# Wed, 25 May 2022 20:17:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 25 May 2022 20:17:44 GMT
WORKDIR /var/www/html
# Wed, 25 May 2022 20:17:46 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 25 May 2022 20:17:47 GMT
STOPSIGNAL SIGQUIT
# Wed, 25 May 2022 20:17:48 GMT
EXPOSE 9000
# Wed, 25 May 2022 20:17:48 GMT
CMD ["php-fpm"]
# Thu, 26 May 2022 01:04:04 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 26 May 2022 01:04:05 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 26 May 2022 01:04:05 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 26 May 2022 01:04:05 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 26 May 2022 01:04:05 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 26 May 2022 01:04:06 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 26 May 2022 01:04:06 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 26 May 2022 01:04:31 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 26 May 2022 01:04:32 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 26 May 2022 01:04:33 GMT
RUN apk add --no-cache bash
# Thu, 26 May 2022 01:04:33 GMT
ARG YOURLS_VERSION=1.9
# Thu, 26 May 2022 01:04:34 GMT
ARG YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Thu, 26 May 2022 01:04:34 GMT
LABEL org.opencontainers.image.version=1.9
# Thu, 26 May 2022 01:04:34 GMT
ENV YOURLS_VERSION=1.9
# Thu, 26 May 2022 01:04:34 GMT
ENV YOURLS_SHA256=212c4cd283f0b2b44e07da66a882cca4886e064f642bf4de8ecb8dbfb867e542
# Thu, 26 May 2022 01:04:37 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 26 May 2022 01:04:38 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 26 May 2022 01:04:39 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 26 May 2022 01:04:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 26 May 2022 01:04:40 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ad757c376420c4bd689dd2059809802df6400dc63a1f808ebb6ca69780724e3`  
		Last Modified: Wed, 25 May 2022 21:13:30 GMT  
		Size: 1.8 MB (1765925 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ece50bae8c0ec9d3501fc804150b9b5ad9fe9187347f2304690718df868b540`  
		Last Modified: Wed, 25 May 2022 21:13:29 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:992853a158bd58244683eefc2e1a8c73fa903949f9422c6c9f2d55a4a83fc0f3`  
		Last Modified: Wed, 25 May 2022 21:13:29 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6d8be0c46ec1fd773cae71474e25dd8907cbc886636236c1a67fec6d0e068a3`  
		Last Modified: Wed, 25 May 2022 21:13:28 GMT  
		Size: 11.7 MB (11728846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e7ca0d012e9303da91d38f051e68f41905cae307f757947fa8d8afde0dfbd57`  
		Last Modified: Wed, 25 May 2022 21:13:28 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb2f8bb04925c5aa631cf0cd58360f9bb96bebd96f7a756ca7fa420ab51d6331`  
		Last Modified: Wed, 25 May 2022 21:14:08 GMT  
		Size: 11.6 MB (11552068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09313793ea067697baac0237a8b2ea25eda2c90b9f3710459517f46ea1a02f39`  
		Last Modified: Wed, 25 May 2022 21:14:06 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7249ccf52faa58a2c9cdc63b5cc7c71bf4d7314d9d73c9b32717bebfd6c460ef`  
		Last Modified: Wed, 25 May 2022 21:14:06 GMT  
		Size: 18.4 KB (18375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa10694ceecd5a373c368e44504a6eb6e413fd105be85d27da7c3787f12ecd2d`  
		Last Modified: Wed, 25 May 2022 21:14:07 GMT  
		Size: 8.6 KB (8624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de4f9bafea69e06eab1bbad092649aa6cffa86f4532e68e22fa6bde052538aab`  
		Last Modified: Thu, 26 May 2022 01:05:35 GMT  
		Size: 176.5 KB (176503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:455a7e36ca5236237756ba5f042cfe3d230d06b3cef93c1a60db57d06899e608`  
		Last Modified: Thu, 26 May 2022 01:05:34 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805384ba2e9ca30e67410c221c42e5e968b61f23c34fda6104890393e27640a1`  
		Last Modified: Thu, 26 May 2022 01:05:34 GMT  
		Size: 483.6 KB (483585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15867a9786aa1b4a9364a79a7b6a761201b09866bccd5a27d02bfe8c838d5af6`  
		Last Modified: Thu, 26 May 2022 01:05:34 GMT  
		Size: 3.9 MB (3944391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b6e69f7a6892dadb7fd380afa99da3353c23e80cd05d608f489a8ee5d658aa`  
		Last Modified: Thu, 26 May 2022 01:05:34 GMT  
		Size: 2.0 KB (2045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cec18df103123c0a05caf9cc09725982922237f6291501607ebc04e3863d7e1`  
		Last Modified: Thu, 26 May 2022 01:05:34 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
