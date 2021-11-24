## `mediawiki:stable-fpm-alpine`

```console
$ docker pull mediawiki@sha256:3bfb4df2e68a852272775c2f258169a20a743ea4b5e1b0107825b422ca8812d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `mediawiki:stable-fpm-alpine` - linux; amd64

```console
$ docker pull mediawiki@sha256:8d1431464fc864bc688fc716383516d9f2a3942bd960653ed38588fc8f856359
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.6 MB (156550140 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f33b1df8fb547f2aebe4d1827fa936800614dd2b53ac146d43837b0cae39f51`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 07:48:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 07:48:45 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 07:48:47 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 07:48:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 07:48:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 07:48:49 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 07:48:49 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 07:48:49 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 09:13:39 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Nov 2021 16:53:45 GMT
ENV PHP_VERSION=7.4.26
# Thu, 18 Nov 2021 16:53:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 18 Nov 2021 16:53:46 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 18 Nov 2021 16:54:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Nov 2021 16:54:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 17:12:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 17:12:28 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 18 Nov 2021 17:12:30 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 17:12:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 17:12:31 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 17:12:33 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Nov 2021 17:12:33 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Nov 2021 17:12:34 GMT
EXPOSE 9000
# Thu, 18 Nov 2021 17:12:34 GMT
CMD ["php-fpm"]
# Thu, 18 Nov 2021 23:09:16 GMT
RUN set -eux; 		apk add --no-cache 		git 		imagemagick 		python3 	;
# Thu, 18 Nov 2021 23:10:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		icu-dev 		oniguruma-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install APCu-5.1.20; 	docker-php-ext-enable 		apcu 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .mediawiki-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 18 Nov 2021 23:10:19 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 18 Nov 2021 23:10:20 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Wed, 24 Nov 2021 23:13:31 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.37
# Wed, 24 Nov 2021 23:13:31 GMT
ENV MEDIAWIKI_VERSION=1.37.0
# Wed, 24 Nov 2021 23:13:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps 		bzip2 		gnupg 	; 		curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz.sig" -o mediawiki.tar.gz.sig; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 		D7D6767D135A514BEB86E9BA75682B08E8A3FEC4 		441276E9CCD15F44F6D97D18C119E1A64D70938E 		F7F780D82EBFB8A56556E7EE82403E59F9F8CD79 		1D98867E82982C8FE0ABC25F9B69B3109D3BB7B0 	; 	gpg --batch --verify mediawiki.tar.gz.sig mediawiki.tar.gz; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" mediawiki.tar.gz.sig mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images; 		apk del .fetch-deps
# Wed, 24 Nov 2021 23:13:50 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b67f99012ff9aa7245baebc28963e44f53cc1832fcfaec246f78b5e7e861fbe6`  
		Last Modified: Sat, 13 Nov 2021 10:43:29 GMT  
		Size: 1.7 MB (1712224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db81da314e0b3e7be6d4c80bd6a2cdc1d7f66d6fffc8334a527f6b6e20fca340`  
		Last Modified: Sat, 13 Nov 2021 10:43:29 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5646ac679ebe77089fb6446f9911a66ae64db7d5b774d356b04c1c911ca0a081`  
		Last Modified: Sat, 13 Nov 2021 10:43:29 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0be823f312052566b7ce9a4bd0f842ce5bb4a3eb11a295a0326824ffabb11329`  
		Last Modified: Thu, 18 Nov 2021 19:40:54 GMT  
		Size: 10.4 MB (10440243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2bf6fbeb3f2d33e3045b03de8b00c39540b64ff8ade8bbbceaee342cee8de90`  
		Last Modified: Thu, 18 Nov 2021 19:40:53 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e81a787dbd1e9ce1abbb601e5097839f68fa0872fcf2b20fe9e08d92706cc3f6`  
		Last Modified: Thu, 18 Nov 2021 19:41:36 GMT  
		Size: 14.4 MB (14365377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c60064d1dcd12774fdd35b08d44c9d8d6c36a2d2d22665d0c9aac5122765bae`  
		Last Modified: Thu, 18 Nov 2021 19:41:33 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ad85c2c33f48fea14f6fcc5a45bda37d44c29b176783ba30c4ef8ffaec9579a`  
		Last Modified: Thu, 18 Nov 2021 19:41:33 GMT  
		Size: 18.2 KB (18197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0380c49e03155916174a049701a799d4e3acde985be9ddb835bb401c0c4bc776`  
		Last Modified: Thu, 18 Nov 2021 19:41:33 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e261a7e80f5c38b65dd976ca9988c3f1aac5fecba28f6e028396a38f51c73df`  
		Last Modified: Thu, 18 Nov 2021 23:19:30 GMT  
		Size: 58.8 MB (58788766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cc736023b1f85908d57c2f4150a2a31ae4b94b8c9cea7b9a4e3e19ed3ade3a0`  
		Last Modified: Thu, 18 Nov 2021 23:19:23 GMT  
		Size: 17.3 MB (17306095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d295e942a158b16689adc91bb241bbeeecca4944b19820b8afcd1c084555b0cc`  
		Last Modified: Thu, 18 Nov 2021 23:19:20 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a56912270cff8598a6e64228498e1b3196a8efd246bd558a6f1e52407ea97c`  
		Last Modified: Thu, 18 Nov 2021 23:19:20 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc9d4077da50121e08ec6ffa4ccd0d829bb0f4616f2be0713241aef0749362e9`  
		Last Modified: Wed, 24 Nov 2021 23:16:12 GMT  
		Size: 51.1 MB (51082987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:stable-fpm-alpine` - linux; arm variant v6

```console
$ docker pull mediawiki@sha256:ffaaec0d9e7914fdfcc06538d527b55bd088fb706a655ead77e2cdde7a43d658
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **152.4 MB (152372830 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a3a06bf98b4d67f8dc10237872c57c11e3313778f768207f546339820c73225e`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 01:00:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 01:00:55 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 01:00:57 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 01:00:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 01:00:59 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 01:01:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 01:01:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 01:01:01 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 01:41:14 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Nov 2021 15:54:58 GMT
ENV PHP_VERSION=7.4.26
# Thu, 18 Nov 2021 15:54:59 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 18 Nov 2021 15:54:59 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 18 Nov 2021 15:55:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Nov 2021 15:55:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:04:44 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 16:04:45 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:04:48 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 16:04:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 16:04:49 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 16:04:51 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Nov 2021 16:04:51 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Nov 2021 16:04:52 GMT
EXPOSE 9000
# Thu, 18 Nov 2021 16:04:52 GMT
CMD ["php-fpm"]
# Thu, 18 Nov 2021 18:32:58 GMT
RUN set -eux; 		apk add --no-cache 		git 		imagemagick 		python3 	;
# Thu, 18 Nov 2021 18:35:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		icu-dev 		oniguruma-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install APCu-5.1.20; 	docker-php-ext-enable 		apcu 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .mediawiki-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 18 Nov 2021 18:35:02 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 18 Nov 2021 18:35:03 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Wed, 24 Nov 2021 23:20:59 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.37
# Wed, 24 Nov 2021 23:21:00 GMT
ENV MEDIAWIKI_VERSION=1.37.0
# Wed, 24 Nov 2021 23:21:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps 		bzip2 		gnupg 	; 		curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz.sig" -o mediawiki.tar.gz.sig; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 		D7D6767D135A514BEB86E9BA75682B08E8A3FEC4 		441276E9CCD15F44F6D97D18C119E1A64D70938E 		F7F780D82EBFB8A56556E7EE82403E59F9F8CD79 		1D98867E82982C8FE0ABC25F9B69B3109D3BB7B0 	; 	gpg --batch --verify mediawiki.tar.gz.sig mediawiki.tar.gz; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" mediawiki.tar.gz.sig mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images; 		apk del .fetch-deps
# Wed, 24 Nov 2021 23:21:51 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19fb65eff99d3570be8bbee58e3796b49e0e6fbc64d6c2b55e01eaf1b07709af`  
		Last Modified: Sat, 13 Nov 2021 02:49:22 GMT  
		Size: 1.7 MB (1702248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffe18ffa25cea29b8a20ba6c41b7485fd89e792d6d333919ea738dcff33555f`  
		Last Modified: Sat, 13 Nov 2021 02:49:21 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:215c6f1ae3409a42a8b2531ec3f19b4dddc77724624fdc7fe72175b53fa03ad0`  
		Last Modified: Sat, 13 Nov 2021 02:49:21 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51043c3368ded4fd963ab642ab064049684d3774825d00295f6ca60cfab1f3a0`  
		Last Modified: Thu, 18 Nov 2021 17:04:34 GMT  
		Size: 10.4 MB (10440263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:687f953ec69c43d8ed6b25d8342ad3a9988bfd9ec8b998a3c9150b701281c7e1`  
		Last Modified: Thu, 18 Nov 2021 17:04:32 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5af3d8c14828174afaf52ea2d1687ebcae18f6fdc9347eceaea6729d50dab442`  
		Last Modified: Thu, 18 Nov 2021 17:05:43 GMT  
		Size: 13.4 MB (13355049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f6b8b2d0a6bd485b05c2660f05a72d3a5e2219859149cc907f5fc3286267f0b`  
		Last Modified: Thu, 18 Nov 2021 17:05:37 GMT  
		Size: 2.3 KB (2300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f11a7caf8be03ecdabf9c5e394252e56c2331c1e5fe80678288415d3edabd04`  
		Last Modified: Thu, 18 Nov 2021 17:05:36 GMT  
		Size: 18.2 KB (18205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68b138828e619a0e3c36f93378809eada43426c21ccbad05764660a00bd394ba`  
		Last Modified: Thu, 18 Nov 2021 17:05:36 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67cf370a8ecaa51a406732d527e0c45fec4f0f302ef5742473e3f5343d8487a8`  
		Last Modified: Thu, 18 Nov 2021 18:41:44 GMT  
		Size: 56.3 MB (56321703 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d588d38c3cc66f69904b36f9ab1d04dc42ddf868b99deae21359f736f6e2030`  
		Last Modified: Thu, 18 Nov 2021 18:41:11 GMT  
		Size: 16.8 MB (16804457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:061bbf76d3e3c3ecf9ae61afad08b33625e0fb62df095d09b1c2a0e19b73a724`  
		Last Modified: Thu, 18 Nov 2021 18:41:03 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89a5fdaa9e87e6fc20ae1b4cb17eb558453b8f68ef4ce4602dcd198b3776be0e`  
		Last Modified: Thu, 18 Nov 2021 18:41:03 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5496143cb27250fe23a250996696ee55add8432eb0a60ed916f718e6dada007c`  
		Last Modified: Wed, 24 Nov 2021 23:24:25 GMT  
		Size: 51.1 MB (51082257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:stable-fpm-alpine` - linux; arm variant v7

```console
$ docker pull mediawiki@sha256:35edb568e0372625caad5104c21e32fad821fc6fb4a6935340565b7866d97daa
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **147.1 MB (147110086 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:179ac7e6c0a80703194a3aaaa5d471a50a749d6b5fd1f34398a245b2fc159c31`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 02:20:26 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 02:20:29 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 02:20:30 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 02:20:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 02:20:33 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 02:20:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 02:20:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 02:20:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 03:03:08 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Nov 2021 17:34:29 GMT
ENV PHP_VERSION=7.4.26
# Thu, 18 Nov 2021 17:34:29 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 18 Nov 2021 17:34:30 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 18 Nov 2021 17:34:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Nov 2021 17:34:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 17:43:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 17:43:34 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 18 Nov 2021 17:43:36 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 17:43:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 17:43:37 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 17:43:39 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Nov 2021 17:43:39 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Nov 2021 17:43:40 GMT
EXPOSE 9000
# Thu, 18 Nov 2021 17:43:40 GMT
CMD ["php-fpm"]
# Fri, 19 Nov 2021 00:23:53 GMT
RUN set -eux; 		apk add --no-cache 		git 		imagemagick 		python3 	;
# Fri, 19 Nov 2021 00:25:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		icu-dev 		oniguruma-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install APCu-5.1.20; 	docker-php-ext-enable 		apcu 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .mediawiki-phpext-rundeps $runDeps; 	apk del .build-deps
# Fri, 19 Nov 2021 00:25:49 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 19 Nov 2021 00:25:50 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Fri, 19 Nov 2021 00:25:51 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.36
# Fri, 19 Nov 2021 00:25:51 GMT
ENV MEDIAWIKI_VERSION=1.36.2
# Fri, 19 Nov 2021 00:26:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps 		bzip2 		gnupg 	; 		curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz.sig" -o mediawiki.tar.gz.sig; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 		D7D6767D135A514BEB86E9BA75682B08E8A3FEC4 		441276E9CCD15F44F6D97D18C119E1A64D70938E 		F7F780D82EBFB8A56556E7EE82403E59F9F8CD79 		1D98867E82982C8FE0ABC25F9B69B3109D3BB7B0 	; 	gpg --batch --verify mediawiki.tar.gz.sig mediawiki.tar.gz; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" mediawiki.tar.gz.sig mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images; 		apk del .fetch-deps
# Fri, 19 Nov 2021 00:26:31 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0d591a38553bed13e4644c2ee36cc92a36f4f866265bcec258baef16176c11b`  
		Last Modified: Sat, 13 Nov 2021 04:21:17 GMT  
		Size: 1.6 MB (1571523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a132a38f5266edd87272c20d2129b4448b3dfb530a70424219ddd45fd1d2eb73`  
		Last Modified: Sat, 13 Nov 2021 04:21:16 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a99b8f25382a7fadffc08ae9ebf09b2a2be48a858daf03148035e46335c089a`  
		Last Modified: Sat, 13 Nov 2021 04:21:16 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33572509eb61a00128f39ee9fda81cb699091c67e258241e7006f6a508e94157`  
		Last Modified: Thu, 18 Nov 2021 19:39:10 GMT  
		Size: 10.4 MB (10440242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72afaf8d84251c8c9bb1d3668785c2bce2ef1c270b5f1b16c3fe057f380e8d20`  
		Last Modified: Thu, 18 Nov 2021 19:39:08 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779edc804ece016723b3d8569453951e1eba3770d689a2cbf58191273848167e`  
		Last Modified: Thu, 18 Nov 2021 19:40:20 GMT  
		Size: 12.5 MB (12504986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f7d608b067cd591eeb1aeb25e822c5890e6f0852f8fb1dc5989b5e636ed317a`  
		Last Modified: Thu, 18 Nov 2021 19:40:12 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c49ede17d89f8439fbf9a98b9e5e11eb4ffd92ad07c9add13382718835bbb6a`  
		Last Modified: Thu, 18 Nov 2021 19:40:12 GMT  
		Size: 18.2 KB (18192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29cea458fe8e3a0f91069e42c6056acc7769666ee60cf64ad2dc28a258f740b7`  
		Last Modified: Thu, 18 Nov 2021 19:40:12 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15e34e774b6fb809ea29f40a97c36c5e108756f8d15cd811a6e4bab033b1a9a8`  
		Last Modified: Fri, 19 Nov 2021 00:47:02 GMT  
		Size: 53.3 MB (53343966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f02db13f71377ddf9734c81884ce48de97304518d01391b8ea32a8cfa0d907c`  
		Last Modified: Fri, 19 Nov 2021 00:46:39 GMT  
		Size: 16.8 MB (16830467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1209558ad25d3ed664ba6c8813f33bf435e8ed42c7259bdd38679917112d7d3d`  
		Last Modified: Fri, 19 Nov 2021 00:46:30 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785f1369e88c4b4bfe6d58ef68dc0d2ce4283a08397a42dc8a1a0e482b04e061`  
		Last Modified: Fri, 19 Nov 2021 00:46:30 GMT  
		Size: 168.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c952a3ffa468b2aea2d2db72864c0451d6fb6119a89ce3499f8727da56a72226`  
		Last Modified: Fri, 19 Nov 2021 00:47:24 GMT  
		Size: 49.9 MB (49948825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:stable-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull mediawiki@sha256:ea3423d4bcad849df804f2a4e4a3c206cecb198ed8c19f18acffe25a09f4eb7d
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.8 MB (153765656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6a215f28d939f2c2c4b2c61013ee5cede8544daec6b48bacce9e225472c5d91`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Fri, 12 Nov 2021 19:30:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 12 Nov 2021 19:30:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 12 Nov 2021 19:30:35 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 12 Nov 2021 19:30:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 12 Nov 2021 19:30:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 12 Nov 2021 19:30:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:30:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 12 Nov 2021 19:30:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 12 Nov 2021 20:22:50 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Nov 2021 16:16:44 GMT
ENV PHP_VERSION=7.4.26
# Thu, 18 Nov 2021 16:16:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 18 Nov 2021 16:16:46 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 18 Nov 2021 16:16:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Nov 2021 16:16:57 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:24:16 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 16:24:17 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:24:18 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 16:24:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 16:24:19 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 16:24:20 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Nov 2021 16:24:21 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Nov 2021 16:24:22 GMT
EXPOSE 9000
# Thu, 18 Nov 2021 16:24:23 GMT
CMD ["php-fpm"]
# Sat, 20 Nov 2021 00:47:03 GMT
RUN set -eux; 		apk add --no-cache 		git 		imagemagick 		python3 	;
# Sat, 20 Nov 2021 00:48:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		icu-dev 		oniguruma-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install APCu-5.1.20; 	docker-php-ext-enable 		apcu 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .mediawiki-phpext-rundeps $runDeps; 	apk del .build-deps
# Sat, 20 Nov 2021 00:48:13 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 20 Nov 2021 00:48:14 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sat, 20 Nov 2021 00:48:15 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.36
# Sat, 20 Nov 2021 00:48:16 GMT
ENV MEDIAWIKI_VERSION=1.36.2
# Sat, 20 Nov 2021 00:48:34 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps 		bzip2 		gnupg 	; 		curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz.sig" -o mediawiki.tar.gz.sig; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 		D7D6767D135A514BEB86E9BA75682B08E8A3FEC4 		441276E9CCD15F44F6D97D18C119E1A64D70938E 		F7F780D82EBFB8A56556E7EE82403E59F9F8CD79 		1D98867E82982C8FE0ABC25F9B69B3109D3BB7B0 	; 	gpg --batch --verify mediawiki.tar.gz.sig mediawiki.tar.gz; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" mediawiki.tar.gz.sig mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images; 		apk del .fetch-deps
# Sat, 20 Nov 2021 00:48:36 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9716534ffbe55fb7b1cdc9c51401565113fe78d473379c595bf42e6d05fd5e6e`  
		Last Modified: Fri, 12 Nov 2021 21:25:50 GMT  
		Size: 1.7 MB (1711801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d47cbc9449ef4aab290c562e2d538c1152c89268a02bb026807264d1c3d6da`  
		Last Modified: Fri, 12 Nov 2021 21:25:49 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a654447725655854a94c8af1e17c61ba95c1eb179a627aa323bfd70bfbae408`  
		Last Modified: Fri, 12 Nov 2021 21:25:50 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fe8a5cd6e7b96df864899309b2e8c0fa05b123321e61f6af6cbc7d98ce260c8`  
		Last Modified: Thu, 18 Nov 2021 17:35:10 GMT  
		Size: 10.4 MB (10440015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0d909104778cbfc0311368bde399e8451a0e2a0d149c22eb42fcb1ac70c3cfc`  
		Last Modified: Thu, 18 Nov 2021 17:35:09 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7da90346c6fbfe105ca5ed861a6d771a222ac2c800f62b145cd08fa636b6f51`  
		Last Modified: Thu, 18 Nov 2021 17:35:57 GMT  
		Size: 14.1 MB (14142606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdef70d9f1a8d1a096749e1610f7529ca4c5f58b6ab6a94de1ad3167f860ba69`  
		Last Modified: Thu, 18 Nov 2021 17:35:55 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:59a3657fb4056704509e3c814335d219d1f7ddc4c6df8d32975d2a582a383670`  
		Last Modified: Thu, 18 Nov 2021 17:35:55 GMT  
		Size: 18.1 KB (18109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bee09c074e685d06c59d3db8fc9c241d78fc68e320fea7ab92c8638d4d44b59f`  
		Last Modified: Thu, 18 Nov 2021 17:35:54 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e22bb012e0decd31fc780b3739ab6a0b76e65bcfce8d284235198f4c6e2a5690`  
		Last Modified: Sat, 20 Nov 2021 00:58:44 GMT  
		Size: 57.5 MB (57484538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c35eb188f2425ec63ea060973a4a97b78b8c2b6c8206e23408192868c1f4c84`  
		Last Modified: Sat, 20 Nov 2021 00:58:39 GMT  
		Size: 17.3 MB (17289620 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0f77c25566a4da2aceef614dd4fd96aebda75a38e90a290e94e82adb1657f47`  
		Last Modified: Sat, 20 Nov 2021 00:58:36 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de748e4daf75ba71a64b9d6859893129c4a7f491a1d314f37562cca21c1dad23`  
		Last Modified: Sat, 20 Nov 2021 00:58:36 GMT  
		Size: 136.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:969efac5f41ff8e8abb493502014e704e299eb9a18de5b4ec066b1c12f9fc749`  
		Last Modified: Sat, 20 Nov 2021 00:58:48 GMT  
		Size: 49.9 MB (49948109 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:stable-fpm-alpine` - linux; 386

```console
$ docker pull mediawiki@sha256:ac44a38adc1823d3da939311b823a407a179622afa9cfecd2a97751e96f56005
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **158.4 MB (158397797 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9076902c6c2035a6f3b6d3be3ca0fcfb2e48c3ebf066eb5d2d005c07fea3216d`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 00:47:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 00:47:24 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 00:47:26 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 00:47:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 00:47:27 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 00:47:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 00:47:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 00:47:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 02:05:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Nov 2021 16:36:04 GMT
ENV PHP_VERSION=7.4.26
# Thu, 18 Nov 2021 16:36:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 18 Nov 2021 16:36:05 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 18 Nov 2021 16:36:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Nov 2021 16:36:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:53:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 16:53:53 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 18 Nov 2021 16:53:54 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 16:53:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 16:53:55 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 16:53:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Nov 2021 16:53:56 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Nov 2021 16:53:56 GMT
EXPOSE 9000
# Thu, 18 Nov 2021 16:53:56 GMT
CMD ["php-fpm"]
# Sat, 20 Nov 2021 01:12:47 GMT
RUN set -eux; 		apk add --no-cache 		git 		imagemagick 		python3 	;
# Sat, 20 Nov 2021 01:14:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		icu-dev 		oniguruma-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install APCu-5.1.20; 	docker-php-ext-enable 		apcu 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .mediawiki-phpext-rundeps $runDeps; 	apk del .build-deps
# Sat, 20 Nov 2021 01:14:26 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 20 Nov 2021 01:14:27 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Wed, 24 Nov 2021 22:51:01 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.37
# Wed, 24 Nov 2021 22:51:02 GMT
ENV MEDIAWIKI_VERSION=1.37.0
# Wed, 24 Nov 2021 22:51:22 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps 		bzip2 		gnupg 	; 		curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz.sig" -o mediawiki.tar.gz.sig; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 		D7D6767D135A514BEB86E9BA75682B08E8A3FEC4 		441276E9CCD15F44F6D97D18C119E1A64D70938E 		F7F780D82EBFB8A56556E7EE82403E59F9F8CD79 		1D98867E82982C8FE0ABC25F9B69B3109D3BB7B0 	; 	gpg --batch --verify mediawiki.tar.gz.sig mediawiki.tar.gz; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" mediawiki.tar.gz.sig mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images; 		apk del .fetch-deps
# Wed, 24 Nov 2021 22:51:23 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c05111b719bf0e9c81182879ace55b68244fff3ccaacc6813f9ce740b1adf4d`  
		Last Modified: Sat, 13 Nov 2021 04:00:31 GMT  
		Size: 1.8 MB (1812696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f12e62d2679739a2acadab070b1c7d0f433a8a46d449147d00fa5c4aa0a8753`  
		Last Modified: Sat, 13 Nov 2021 04:00:30 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3e1535943b040497915113f37b46a4ba0dc10f27aabcdb6dbf9d0b594ca8be`  
		Last Modified: Sat, 13 Nov 2021 04:00:30 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e3f24501ef304b64e206982d7aa4664cc7425378028bd85a1d8bec6a61b1fd`  
		Last Modified: Thu, 18 Nov 2021 19:37:10 GMT  
		Size: 10.4 MB (10440236 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cceece03507d726abbafc27867570be8fcec456898af998289ca0a5034a71027`  
		Last Modified: Thu, 18 Nov 2021 19:37:09 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed81a5e471a0fb0ac5db3803906d670ff33f24ce191b6d5503a37b724d753592`  
		Last Modified: Thu, 18 Nov 2021 19:38:05 GMT  
		Size: 14.7 MB (14739579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d34c69be3be4d02cde28162b729b0909898059702aee6a6529b76167bae54c4`  
		Last Modified: Thu, 18 Nov 2021 19:38:00 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a719c36dc46411961b026b86c9b6744fc257a4d971e7637af885757b17898f`  
		Last Modified: Thu, 18 Nov 2021 19:38:00 GMT  
		Size: 18.2 KB (18188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6f545379a5e98d3ea29f36cd127d7f7e95d2f119e73b1f51eb227c6a98185fc`  
		Last Modified: Thu, 18 Nov 2021 19:38:00 GMT  
		Size: 8.4 KB (8438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba8b3340eb701599359227977672182f0b5b40b26602de621e13e49ce0eca67c`  
		Last Modified: Sat, 20 Nov 2021 01:26:42 GMT  
		Size: 60.0 MB (60015304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56db67a87d6c6981433568075a8103d11d80f30015382d40cfcc885b234b8f83`  
		Last Modified: Sat, 20 Nov 2021 01:26:31 GMT  
		Size: 17.4 MB (17445138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30b67c2a8066658ac8480a17522de462799151243ee737252e47b35075875dc6`  
		Last Modified: Sat, 20 Nov 2021 01:26:25 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75916bf5daad300478989ecf17fe45a7a9bcadca1ddf19601b44db8b96d615cc`  
		Last Modified: Sat, 20 Nov 2021 01:26:25 GMT  
		Size: 170.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242541ac538c1c1f85f3bd845bacf07eac241ef574dd0fdde1ad2c0286084438`  
		Last Modified: Wed, 24 Nov 2021 22:55:14 GMT  
		Size: 51.1 MB (51082446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `mediawiki:stable-fpm-alpine` - linux; ppc64le

```console
$ docker pull mediawiki@sha256:13e547ff88496aa13099f005389e27a0b62ac9a6ffe1a58e6af5982fa8407e07
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **157.5 MB (157494642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ccf7bb422cd9eaf28fc187a4fa1886475cb48a93e73cf39c6d212146f379b04`
-	Entrypoint: `["docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 12 Nov 2021 21:18:00 GMT
ADD file:4d45063079cb28a34f1e382fddb22f156ac99d5449aa05ed37cb653c1f7b80f2 in / 
# Fri, 12 Nov 2021 21:18:01 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 11:56:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Sat, 13 Nov 2021 11:56:08 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Sat, 13 Nov 2021 11:56:13 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Sat, 13 Nov 2021 11:56:15 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Sat, 13 Nov 2021 11:56:29 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Sat, 13 Nov 2021 11:56:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 11:56:34 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Sat, 13 Nov 2021 11:56:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 13 Nov 2021 12:51:23 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 18 Nov 2021 17:05:30 GMT
ENV PHP_VERSION=7.4.26
# Thu, 18 Nov 2021 17:05:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.26.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.26.tar.xz.asc
# Thu, 18 Nov 2021 17:05:39 GMT
ENV PHP_SHA256=e305b3aafdc85fa73a81c53d3ce30578bc94d1633ec376add193a1e85e0f0ef8
# Thu, 18 Nov 2021 17:06:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 18 Nov 2021 17:06:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 18 Nov 2021 17:16:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 18 Nov 2021 17:16:35 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 18 Nov 2021 17:16:43 GMT
RUN docker-php-ext-enable sodium
# Thu, 18 Nov 2021 17:16:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 18 Nov 2021 17:16:56 GMT
WORKDIR /var/www/html
# Thu, 18 Nov 2021 17:17:03 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 18 Nov 2021 17:17:08 GMT
STOPSIGNAL SIGQUIT
# Thu, 18 Nov 2021 17:17:12 GMT
EXPOSE 9000
# Thu, 18 Nov 2021 17:17:14 GMT
CMD ["php-fpm"]
# Sat, 20 Nov 2021 01:22:35 GMT
RUN set -eux; 		apk add --no-cache 		git 		imagemagick 		python3 	;
# Sat, 20 Nov 2021 01:23:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		icu-dev 		oniguruma-dev 	; 		docker-php-ext-install -j "$(nproc)" 		intl 		mbstring 		mysqli 		opcache 	; 		pecl install APCu-5.1.20; 	docker-php-ext-enable 		apcu 	; 	rm -r /tmp/pear; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .mediawiki-phpext-rundeps $runDeps; 	apk del .build-deps
# Sat, 20 Nov 2021 01:23:59 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=60'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 20 Nov 2021 01:24:06 GMT
RUN set -eux; 	mkdir -p /var/www/data; 	chown -R www-data:www-data /var/www/data
# Sat, 20 Nov 2021 01:24:07 GMT
ENV MEDIAWIKI_MAJOR_VERSION=1.36
# Sat, 20 Nov 2021 01:24:11 GMT
ENV MEDIAWIKI_VERSION=1.36.2
# Sat, 20 Nov 2021 01:25:08 GMT
RUN set -eux; 	apk add --no-cache --virtual .fetch-deps 		bzip2 		gnupg 	; 		curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz" -o mediawiki.tar.gz; 	curl -fSL "https://releases.wikimedia.org/mediawiki/${MEDIAWIKI_MAJOR_VERSION}/mediawiki-${MEDIAWIKI_VERSION}.tar.gz.sig" -o mediawiki.tar.gz.sig; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys 		D7D6767D135A514BEB86E9BA75682B08E8A3FEC4 		441276E9CCD15F44F6D97D18C119E1A64D70938E 		F7F780D82EBFB8A56556E7EE82403E59F9F8CD79 		1D98867E82982C8FE0ABC25F9B69B3109D3BB7B0 	; 	gpg --batch --verify mediawiki.tar.gz.sig mediawiki.tar.gz; 	tar -x --strip-components=1 -f mediawiki.tar.gz; 	gpgconf --kill all; 	rm -r "$GNUPGHOME" mediawiki.tar.gz.sig mediawiki.tar.gz; 	chown -R www-data:www-data extensions skins cache images; 		apk del .fetch-deps
# Sat, 20 Nov 2021 01:25:12 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:72940440c1ab65eca4d38846164719ffde4b147543cc658d041407a925b13368`  
		Last Modified: Fri, 12 Nov 2021 21:19:32 GMT  
		Size: 2.8 MB (2817467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf526002982778a0157923a6219fbadd645d22999e9251af0db89be07d002272`  
		Last Modified: Sat, 13 Nov 2021 14:08:23 GMT  
		Size: 1.8 MB (1759206 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9b47bb623f5bce1748b7a2c4e16b2726478248c03150000de676a1020aaeada`  
		Last Modified: Sat, 13 Nov 2021 14:08:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f035bbd1b7db7792a68686cccf93b48bd273f6f89375962d7fae46bab690f7ac`  
		Last Modified: Sat, 13 Nov 2021 14:08:23 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2ca048d84a232d0369a78f9f5bf66058a7e1c2a028f54aa283b9890a81d0b2d`  
		Last Modified: Thu, 18 Nov 2021 19:08:44 GMT  
		Size: 10.4 MB (10440243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf4af54fb1c5fa2e7a563486f08bd776a2e77920493432d57cb1fa9e7f3e2221`  
		Last Modified: Thu, 18 Nov 2021 19:08:42 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22abbb1bfdfab112ca8f4555945d8cc158f898ab6c7082672177729f50bdb9f0`  
		Last Modified: Thu, 18 Nov 2021 19:09:45 GMT  
		Size: 15.4 MB (15400958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85829949ff50cbd0cb85470e897b384e4dfd995a8ef131b2aabd503f78ad44c8`  
		Last Modified: Thu, 18 Nov 2021 19:09:34 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bf287c1d47a86d0a2ef12df4a2d3e23355fe12430d14c89bf932720f79f516`  
		Last Modified: Thu, 18 Nov 2021 19:09:34 GMT  
		Size: 18.2 KB (18200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffa20a5b92239e77c1a86c3d4d7fbe9767a0fb8f8393f6c0aad7866bbbc72941`  
		Last Modified: Thu, 18 Nov 2021 19:09:34 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb7047e6ee8624608c63885c55adacd82062d0cfb4974ab6e37394f400cac42e`  
		Last Modified: Sat, 20 Nov 2021 01:54:26 GMT  
		Size: 59.7 MB (59705524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7383a849f6272e64adab52f9e8b1f6b99f476c173fe58429cc0b1bd4404fcb3`  
		Last Modified: Sat, 20 Nov 2021 01:54:04 GMT  
		Size: 17.4 MB (17391348 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5865a24665f897b6235ba1e21e474ec09e133f0e44600a74f508b09300a56730`  
		Last Modified: Sat, 20 Nov 2021 01:53:58 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50d8ea6a81dd83948100ded7a2aab4fd0efd6e19b10afcbc30de0e5c249db50c`  
		Last Modified: Sat, 20 Nov 2021 01:53:58 GMT  
		Size: 169.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca6cdb61969b0500cb8813f2e6a507d38d40b2526d4d4989167b02d1d3f1fc6b`  
		Last Modified: Sat, 20 Nov 2021 01:55:21 GMT  
		Size: 49.9 MB (49948423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
