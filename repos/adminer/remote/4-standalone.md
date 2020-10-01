## `adminer:4-standalone`

```console
$ docker pull adminer@sha256:99cee46862b08d40d2d22a6e8fe2bce2017cfc951d243303f1ca3fc2b2604516
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

### `adminer:4-standalone` - linux; amd64

```console
$ docker pull adminer@sha256:3e96766afea7075a7a44bd623b15af7c034f4fc985f0ea11d36bab9dfb42ecd0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33933192 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0101225da586db252b29b3ec10c5376f7f68a5e9b317dba96e338a3c69560c6`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:51:57 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:51:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:51:59 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:51:59 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:52:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:52:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:52:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Sep 2020 19:44:30 GMT
ENV PHP_VERSION=7.4.10
# Thu, 03 Sep 2020 19:44:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.10.tar.xz.asc
# Thu, 03 Sep 2020 19:44:31 GMT
ENV PHP_SHA256=c2d90b00b14284588a787b100dee54c2400e7db995b457864d66f00ad64fb010 PHP_MD5=
# Thu, 03 Sep 2020 19:44:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 19:44:35 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 19:52:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 19:52:57 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 03 Sep 2020 19:52:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 19:52:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 19:52:59 GMT
CMD ["php" "-a"]
# Thu, 03 Sep 2020 23:17:54 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Thu, 03 Sep 2020 23:17:54 GMT
STOPSIGNAL SIGINT
# Thu, 03 Sep 2020 23:17:55 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 03 Sep 2020 23:17:55 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 23:18:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Thu, 03 Sep 2020 23:18:21 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Thu, 03 Sep 2020 23:18:21 GMT
ENV ADMINER_VERSION=4.7.7
# Thu, 03 Sep 2020 23:18:21 GMT
ENV ADMINER_DOWNLOAD_SHA256=566152a2d86186dcfb28856b4ed0dfdb60e355d93ab693f7931201f75868fff0
# Thu, 03 Sep 2020 23:18:21 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=5d28c03739ce647a48ebe77e8db247b7f5ec7a2ee66ccabe00743c117d50e319
# Thu, 03 Sep 2020 23:18:23 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Thu, 03 Sep 2020 23:18:23 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 03 Sep 2020 23:18:23 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Thu, 03 Sep 2020 23:18:23 GMT
USER adminer
# Thu, 03 Sep 2020 23:18:23 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 03 Sep 2020 23:18:24 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b358d6dbbdff5c10cbe23c608b7ff9c6d1dd13331dd7dc7644b727ca5ea8e742`  
		Last Modified: Thu, 11 Jun 2020 22:14:55 GMT  
		Size: 1.3 MB (1340817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0232d962484c6b9a1caa33a12f1beed4cb20996085056b4fb1591a9fd1d8c89f`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c1d3ac04d2af7a9f0eee25eccc72e586400051054ffb4aff7cdf2f4ebc993e8`  
		Last Modified: Thu, 11 Jun 2020 22:14:54 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16de917e7920b60bdadfa5483b1d46012306437f7d933277924b973ca75642ad`  
		Last Modified: Thu, 03 Sep 2020 22:51:06 GMT  
		Size: 10.3 MB (10317336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4688fcc9c77366e549b8561f84c417a8d8e7422555a03314ed00a2a6c91cbf1e`  
		Last Modified: Thu, 03 Sep 2020 22:51:04 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9790b0ac94c080930aa74d7f186c2db9335ad17efb7e43ced6627e841bcd07c9`  
		Last Modified: Thu, 03 Sep 2020 22:51:10 GMT  
		Size: 14.6 MB (14560960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d1da0bfefaa219b09bb4232b29508bc5ba3e1890bf4c992a58e23a8c744c65b`  
		Last Modified: Thu, 03 Sep 2020 22:51:04 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510744afa01db1625f6d728ce6ce646cc3e48199b34c02b0435bba8c7b3dc9f5`  
		Last Modified: Thu, 03 Sep 2020 22:51:04 GMT  
		Size: 17.0 KB (17025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0e554a1920fc645697c2beffc03786f21585d26b02b53724cb50d8b31e7cef`  
		Last Modified: Thu, 03 Sep 2020 23:19:21 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0294974f4c4d9012fc8754292584a536363dab66d99c99a429b6946e19b5e821`  
		Last Modified: Thu, 03 Sep 2020 23:19:20 GMT  
		Size: 1.4 KB (1350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e16e700a0ec3ddb8d4df7535a40e133878f0f53b45dee0a0d8a28bcdbb5f2f`  
		Last Modified: Thu, 03 Sep 2020 23:19:20 GMT  
		Size: 4.3 MB (4320976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47a606cc378cb59e0dfe820fa1f7c96ef3eacec35b195c948df059f930d422b3`  
		Last Modified: Thu, 03 Sep 2020 23:19:20 GMT  
		Size: 1.5 KB (1474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a345ba017bdfa1fdcf87243dd6d6c502a2a3ee193b1ec1b2740da5726664ed2`  
		Last Modified: Thu, 03 Sep 2020 23:19:20 GMT  
		Size: 570.7 KB (570687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:007164bfb31a042c75ae4892af39baa2246a435c0177e72b4cd3fd60240b7c1b`  
		Last Modified: Thu, 03 Sep 2020 23:19:20 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v6

```console
$ docker pull adminer@sha256:a8a3a2e80918dabe9e1743ccdc31638a7cd0522bc4ff511d19522c61e5cd22fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.4 MB (32433319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeefcc5ef822336f648711d7f53cd3acd165be3f27f5ebe7b0fa9cf42571bad0`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Fri, 29 May 2020 21:50:55 GMT
ADD file:f46e997a56849423db17e5fc9f0249ab6c73b155245927dba5fcb9dfd65f622f in / 
# Fri, 29 May 2020 21:50:56 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:14:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:14:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:14:52 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:14:53 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:14:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:14:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:14:57 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:14:58 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Sep 2020 19:06:49 GMT
ENV PHP_VERSION=7.4.10
# Thu, 03 Sep 2020 19:06:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.10.tar.xz.asc
# Thu, 03 Sep 2020 19:07:11 GMT
ENV PHP_SHA256=c2d90b00b14284588a787b100dee54c2400e7db995b457864d66f00ad64fb010 PHP_MD5=
# Thu, 03 Sep 2020 19:07:55 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 19:08:10 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 19:12:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 19:13:25 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 03 Sep 2020 19:14:19 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 19:14:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 19:14:46 GMT
CMD ["php" "-a"]
# Thu, 03 Sep 2020 22:04:54 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Thu, 03 Sep 2020 22:05:07 GMT
STOPSIGNAL SIGINT
# Thu, 03 Sep 2020 22:05:46 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 03 Sep 2020 22:06:04 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 22:07:20 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Thu, 03 Sep 2020 22:07:38 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Thu, 03 Sep 2020 22:07:48 GMT
ENV ADMINER_VERSION=4.7.7
# Thu, 03 Sep 2020 22:07:55 GMT
ENV ADMINER_DOWNLOAD_SHA256=566152a2d86186dcfb28856b4ed0dfdb60e355d93ab693f7931201f75868fff0
# Thu, 03 Sep 2020 22:08:02 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=5d28c03739ce647a48ebe77e8db247b7f5ec7a2ee66ccabe00743c117d50e319
# Thu, 03 Sep 2020 22:08:29 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Thu, 03 Sep 2020 22:08:43 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 03 Sep 2020 22:08:50 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Thu, 03 Sep 2020 22:08:56 GMT
USER adminer
# Thu, 03 Sep 2020 22:09:04 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 03 Sep 2020 22:09:11 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:b4b72e716706d29f5d2351709c20bf737b94f876a5472a43ff1b6e203c65d27f`  
		Last Modified: Fri, 29 May 2020 21:51:30 GMT  
		Size: 2.6 MB (2603286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72788d65e292354c2ce4b67441d334d0ba534db5ce71d5b8bf78011a256b566f`  
		Last Modified: Thu, 11 Jun 2020 19:29:37 GMT  
		Size: 1.3 MB (1310273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e32d62de43da999aca07cf15fdbe1cd6b03aebc88c15409c3463daadf13e01`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6701e05673b745147608cd1b6eb47a3fbc35bcfd8a65bc536e5b9f919b3d0e77`  
		Last Modified: Thu, 11 Jun 2020 19:29:36 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcb3879db8978b46a0c8b58a30baee0d9926faf4c176eef17e05b6a9ee1bc8e9`  
		Last Modified: Thu, 03 Sep 2020 20:56:58 GMT  
		Size: 10.3 MB (10317362 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:415e5a9cd24f2f4e4a0a51e22c8cf40b6407263aaf05cef43aaf3aa292dce104`  
		Last Modified: Thu, 03 Sep 2020 20:56:57 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c6bbbc190ab0385a00dbddf0dcbe2df7d4c624497f4864ef72344bffda4d44`  
		Last Modified: Thu, 03 Sep 2020 20:57:03 GMT  
		Size: 13.6 MB (13582383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2700f26e3034155161c7dfe948933c184f28ad925f240b7bbd938ff0a9704a3`  
		Last Modified: Thu, 03 Sep 2020 20:56:57 GMT  
		Size: 2.3 KB (2277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5d2241c7bf55eb571042ec050de4442eb07156fa90d8acd1258847fad650a60`  
		Last Modified: Thu, 03 Sep 2020 20:56:57 GMT  
		Size: 17.0 KB (16973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7143e4570be0839570fa66237c16f9f630fd5938cf593c7d115bc81a2fc38ab`  
		Last Modified: Thu, 03 Sep 2020 22:15:30 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:469ec9b21890289d9e63632e5b47bd7a892af24aae5f0b2c838aacdff6e1f49b`  
		Last Modified: Thu, 03 Sep 2020 22:15:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55a05f1103b683e5d7fa74373396290f7dd3e0713857c53bdb3c5129b083994b`  
		Last Modified: Thu, 03 Sep 2020 22:15:27 GMT  
		Size: 4.0 MB (4024288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8221ceb1b2802bd72f7ad34e54c1bf4ba3715f551364ac6d02f502b8340a9b6`  
		Last Modified: Thu, 03 Sep 2020 22:15:26 GMT  
		Size: 1.5 KB (1477 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:027d1f72122f55b5b41c2325895f88f064c2fea27585d271ba8d80f8eb42e295`  
		Last Modified: Thu, 03 Sep 2020 22:15:27 GMT  
		Size: 570.8 KB (570773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481ad07075488cf150068a32ed82432823e3ea8b051748392d83d58e193a4b33`  
		Last Modified: Thu, 03 Sep 2020 22:15:26 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:1222816e17f846775def287aa67019e79980b8caf462ade3c2f36f78d6204487
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31161716 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2460b64d3243d6340d80112751e1a5dff935491b79ef4393c38b436ec7523a0`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Fri, 29 May 2020 21:02:07 GMT
ADD file:e97bf0d217846312b19a9f7264604851aedd125c23b4d291eed4c69b880dce26 in / 
# Fri, 29 May 2020 21:02:08 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:34:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:35:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:35:07 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:35:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:35:12 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:35:13 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:35:14 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:35:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:35:16 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Sep 2020 20:48:11 GMT
ENV PHP_VERSION=7.4.10
# Thu, 03 Sep 2020 20:48:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.10.tar.xz.asc
# Thu, 03 Sep 2020 20:48:40 GMT
ENV PHP_SHA256=c2d90b00b14284588a787b100dee54c2400e7db995b457864d66f00ad64fb010 PHP_MD5=
# Thu, 03 Sep 2020 20:49:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 20:49:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 20:53:02 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 20:53:48 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 03 Sep 2020 20:54:17 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 20:54:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 20:54:33 GMT
CMD ["php" "-a"]
# Fri, 04 Sep 2020 01:33:22 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Fri, 04 Sep 2020 01:33:30 GMT
STOPSIGNAL SIGINT
# Fri, 04 Sep 2020 01:34:05 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 04 Sep 2020 01:34:14 GMT
WORKDIR /var/www/html
# Fri, 04 Sep 2020 01:35:36 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Fri, 04 Sep 2020 01:35:58 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Fri, 04 Sep 2020 01:36:06 GMT
ENV ADMINER_VERSION=4.7.7
# Fri, 04 Sep 2020 01:36:13 GMT
ENV ADMINER_DOWNLOAD_SHA256=566152a2d86186dcfb28856b4ed0dfdb60e355d93ab693f7931201f75868fff0
# Fri, 04 Sep 2020 01:36:20 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=5d28c03739ce647a48ebe77e8db247b7f5ec7a2ee66ccabe00743c117d50e319
# Fri, 04 Sep 2020 01:36:50 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Fri, 04 Sep 2020 01:37:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 04 Sep 2020 01:37:14 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Fri, 04 Sep 2020 01:37:23 GMT
USER adminer
# Fri, 04 Sep 2020 01:37:32 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Fri, 04 Sep 2020 01:37:49 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:52278dd8e57993669c5b72a9620e89bebdc098f2af2379caaa8945f7403f77a2`  
		Last Modified: Fri, 29 May 2020 21:02:38 GMT  
		Size: 2.4 MB (2406763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d5b4230297ea0028dae43acf7e134a55e11ebc15c53a61a2c0c72935dd0ed35`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.2 MB (1214376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779feafcddcba2692e3d187a609b90060e7deea16e8b629aada3a236e99c40f7`  
		Last Modified: Thu, 11 Jun 2020 20:13:04 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f23b20c0367792ccffce00af872fa2ea0300330509fb8c15fe5c08905d7db739`  
		Last Modified: Thu, 11 Jun 2020 20:13:03 GMT  
		Size: 266.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b08829e67730a957cae19c4530f0e6924a5d6c88f6004032784c56a3a4e4079`  
		Last Modified: Thu, 03 Sep 2020 23:29:03 GMT  
		Size: 10.3 MB (10317359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f58a4ae1bad42e73e2f53150562169ba32a8a3bbc68c9edf5d57d3882455b891`  
		Last Modified: Thu, 03 Sep 2020 23:29:03 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f071ed36128ee64dfef0f062de67201291ad038b1cfdf5021cd1afad4a602be`  
		Last Modified: Thu, 03 Sep 2020 23:29:06 GMT  
		Size: 12.7 MB (12705391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d966f0a67f3c6fd641e02ae2417992de63896f8df65468d35e047635e0746cfc`  
		Last Modified: Thu, 03 Sep 2020 23:29:01 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5e41e761469c901c914e095311dddddb3984671ce3c1d6f7dd35fa1fdd1d708`  
		Last Modified: Thu, 03 Sep 2020 23:29:03 GMT  
		Size: 17.0 KB (16958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66398978ff1673d2592caaa98fc48f0a5b581411eaa7e0b3889cacbaca8c0f28`  
		Last Modified: Fri, 04 Sep 2020 01:43:21 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d8b7800bf9869e169a2d4e481759f454fa4eaf5f6be30402d9012c58284516`  
		Last Modified: Fri, 04 Sep 2020 01:43:17 GMT  
		Size: 1.4 KB (1394 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11a155ab2f5f78394c3859381fa933536817b37f04523b676d228426cc6976b8`  
		Last Modified: Fri, 04 Sep 2020 01:43:17 GMT  
		Size: 3.9 MB (3922117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c2d201e2ab9c7fb051038d527a79b5171d3dc3f83fd48a0bc2a398ed7f80c75`  
		Last Modified: Fri, 04 Sep 2020 01:43:17 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ad2d42f221389df94360ffe98e53452770eedffb781ab0ce7dfa550de8140fd`  
		Last Modified: Fri, 04 Sep 2020 01:43:17 GMT  
		Size: 570.8 KB (570774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:159431d94e1b4b912d6bedbfb13a9c0bf3ecb35c42994d4bb9085d84bdd57f73`  
		Last Modified: Fri, 04 Sep 2020 01:43:17 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:a82eba27d82eaea5df958dbf4818c111dcf830c8a366d1977e0f70751dfec3b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33674714 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b3ccf6d1c53826f7f0ff2e5e91c91df7454d253a3fd1175927ae8e0d7dcffc85`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Fri, 29 May 2020 21:43:19 GMT
ADD file:7574aee4e37a85460ab889212d52912723a9b30dda1c060548f0deb4a05fc398 in / 
# Fri, 29 May 2020 21:43:20 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:40:23 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:40:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:40:31 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:40:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:40:34 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:40:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:40:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:40:36 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:40:37 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Sep 2020 19:49:09 GMT
ENV PHP_VERSION=7.4.10
# Thu, 03 Sep 2020 19:49:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.10.tar.xz.asc
# Thu, 03 Sep 2020 19:49:23 GMT
ENV PHP_SHA256=c2d90b00b14284588a787b100dee54c2400e7db995b457864d66f00ad64fb010 PHP_MD5=
# Thu, 03 Sep 2020 19:49:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 19:50:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 19:53:54 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 19:53:56 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 03 Sep 2020 19:53:59 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 19:54:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 19:54:00 GMT
CMD ["php" "-a"]
# Thu, 03 Sep 2020 22:11:34 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Thu, 03 Sep 2020 22:11:40 GMT
STOPSIGNAL SIGINT
# Thu, 03 Sep 2020 22:12:07 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 03 Sep 2020 22:12:18 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 22:13:28 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Thu, 03 Sep 2020 22:13:37 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Thu, 03 Sep 2020 22:13:48 GMT
ENV ADMINER_VERSION=4.7.7
# Thu, 03 Sep 2020 22:14:00 GMT
ENV ADMINER_DOWNLOAD_SHA256=566152a2d86186dcfb28856b4ed0dfdb60e355d93ab693f7931201f75868fff0
# Thu, 03 Sep 2020 22:14:13 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=5d28c03739ce647a48ebe77e8db247b7f5ec7a2ee66ccabe00743c117d50e319
# Thu, 03 Sep 2020 22:14:42 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Thu, 03 Sep 2020 22:14:49 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 03 Sep 2020 22:14:58 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Thu, 03 Sep 2020 22:15:07 GMT
USER adminer
# Thu, 03 Sep 2020 22:15:14 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 03 Sep 2020 22:15:20 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:b538f80385f9b48122e3da068c932a96ea5018afa3c7be79da00437414bd18cd`  
		Last Modified: Fri, 29 May 2020 21:43:57 GMT  
		Size: 2.7 MB (2707964 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dee09877319de284b8141c396485111447d75eb8cf26c68819f92f85a4de5649`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 MB (1342990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bad472a11fde1c83808bc84cc9c77da0743b9974bb8c51ab25ed0608cbb4558`  
		Last Modified: Thu, 11 Jun 2020 20:30:06 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72fca52dcdf28b691bbc24b2e2aff931667b865a9188287ef18af016712d3a0f`  
		Last Modified: Thu, 11 Jun 2020 20:30:05 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5903c48e790f1ffde5668cd4284685bee30f243e7c7fa1f2f74cbdba25e0578c`  
		Last Modified: Thu, 03 Sep 2020 21:48:25 GMT  
		Size: 10.3 MB (10317378 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf6e666d436f1c85e4575e821d5bebec0d3ddff7ed2c6845ef6463395b8bc313`  
		Last Modified: Thu, 03 Sep 2020 21:48:19 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3fadfe6069b0f5adf3e0302506fc092af1566e680f94669a478d99d2d0834a1`  
		Last Modified: Thu, 03 Sep 2020 21:48:26 GMT  
		Size: 14.4 MB (14380383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0661b3b460e38e7b17bb43ae18694f4d42b756b3e3ee006eaa71b296c10dd67`  
		Last Modified: Thu, 03 Sep 2020 21:48:19 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cae743d597c45150c19cfdba39cea5b3159608b4b955537a863f7d1b6eb6d79`  
		Last Modified: Thu, 03 Sep 2020 21:48:19 GMT  
		Size: 17.0 KB (17024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a07c6900424e7b400ae1979c23b9923be8cefe3a6a3016c04b5ae0ea83b1f25e`  
		Last Modified: Thu, 03 Sep 2020 22:20:00 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9c00efc8694460040830aea784b0d243e6c92ed366085592bf952b31a252fa7`  
		Last Modified: Thu, 03 Sep 2020 22:19:56 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d7c9a04cfbce5b00a9b3d811b092ecb318384719e57feba22139ad94d52fc9`  
		Last Modified: Thu, 03 Sep 2020 22:19:57 GMT  
		Size: 4.3 MB (4330230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2f8599c8cb30ab898449f416aaaebbdf014586917bfe2a0a7bed83711cd4012`  
		Last Modified: Thu, 03 Sep 2020 22:19:56 GMT  
		Size: 1.5 KB (1478 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b7f91846d0eadccd5ae5a728efad536daf9a26bf23464dea4825c0a1f9ac178`  
		Last Modified: Thu, 03 Sep 2020 22:19:58 GMT  
		Size: 570.8 KB (570776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:471b8a4ee309a8d5dff22258f09c0b55ebc514c441ec157a955c9b81ae832f2c`  
		Last Modified: Thu, 03 Sep 2020 22:19:57 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; 386

```console
$ docker pull adminer@sha256:1d93dcb121184d41c96b3ecbdf34bf7095a1aaeeb8e3a8403cfb2c67e7299218
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34609978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cbc50cfde49a1caa9b87425ac8f1904b97e17d57c2261344de8f0e69fd03a5d8`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Fri, 29 May 2020 21:38:33 GMT
ADD file:5624441d97aca5eeb82a582941efc3586397098b8391227a9040ebe434cc1d6b in / 
# Fri, 29 May 2020 21:38:33 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:53:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:53:04 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:53:06 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:53:06 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:53:08 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:53:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:53:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:53:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:53:09 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Sep 2020 20:20:39 GMT
ENV PHP_VERSION=7.4.10
# Thu, 03 Sep 2020 20:20:39 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.10.tar.xz.asc
# Thu, 03 Sep 2020 20:20:39 GMT
ENV PHP_SHA256=c2d90b00b14284588a787b100dee54c2400e7db995b457864d66f00ad64fb010 PHP_MD5=
# Thu, 03 Sep 2020 20:20:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 20:20:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 20:30:48 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 20:30:49 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 03 Sep 2020 20:30:50 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 20:30:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 20:30:51 GMT
CMD ["php" "-a"]
# Thu, 03 Sep 2020 23:51:47 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Thu, 03 Sep 2020 23:51:48 GMT
STOPSIGNAL SIGINT
# Thu, 03 Sep 2020 23:51:48 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 03 Sep 2020 23:51:49 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 23:52:17 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Thu, 03 Sep 2020 23:52:18 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Thu, 03 Sep 2020 23:52:18 GMT
ENV ADMINER_VERSION=4.7.7
# Thu, 03 Sep 2020 23:52:18 GMT
ENV ADMINER_DOWNLOAD_SHA256=566152a2d86186dcfb28856b4ed0dfdb60e355d93ab693f7931201f75868fff0
# Thu, 03 Sep 2020 23:52:18 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=5d28c03739ce647a48ebe77e8db247b7f5ec7a2ee66ccabe00743c117d50e319
# Thu, 03 Sep 2020 23:52:20 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Thu, 03 Sep 2020 23:52:20 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 03 Sep 2020 23:52:20 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Thu, 03 Sep 2020 23:52:20 GMT
USER adminer
# Thu, 03 Sep 2020 23:52:20 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 03 Sep 2020 23:52:21 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:0625b4155e2a59f647ece47c0cd77ed3196b1f84454fa64ce80cad90e2b9b79e`  
		Last Modified: Fri, 29 May 2020 21:38:53 GMT  
		Size: 2.8 MB (2792298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380f9ca051d120d4ed72890904488f0f1e0fd0128cbd1c73adbff366e90bc2aa`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 1.4 MB (1439837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:613b9419908bb5beb7365d9d340ee3071aebf8c7919f5379a7b99221fd74c78f`  
		Last Modified: Thu, 11 Jun 2020 22:28:36 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fd1bd9f7e9212850ee7c4017e1d3e5ec33176a9113258688a743d871983ee8c`  
		Last Modified: Thu, 11 Jun 2020 22:28:37 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29ff9d51de9f04f491705f3a5cb9b15eba0b0216b406feb053f2c43384a3849`  
		Last Modified: Thu, 03 Sep 2020 23:22:54 GMT  
		Size: 10.3 MB (10317338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec134844e56a6b70271755442d04b75c08303c6f4eb911ebbc27d075c9f8b28`  
		Last Modified: Thu, 03 Sep 2020 23:22:53 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f2ecffcd4effa682de2776e258bb2d5625decaebfcb683ff554f119c679dfbb`  
		Last Modified: Thu, 03 Sep 2020 23:22:59 GMT  
		Size: 14.9 MB (14948106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81749ddc1de50db3cb31e9a253e3016caa57bb35e099803c4cd4c176b356fdfc`  
		Last Modified: Thu, 03 Sep 2020 23:22:53 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43779594c6cf7e70ce73ef6c5d4c49ea91b81a1c45f36a46704c9647158262b1`  
		Last Modified: Thu, 03 Sep 2020 23:22:53 GMT  
		Size: 17.0 KB (16980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d111e861d467e450d17c34d4d46abc09bd514116479adf08f9d8f6540891e99e`  
		Last Modified: Thu, 03 Sep 2020 23:53:22 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e14bc95178bc53aaf046f66021956ae2783905fc4f0124642aa620fd4f60efc9`  
		Last Modified: Thu, 03 Sep 2020 23:53:21 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8346ebd91a0a6c4c89cd48f55049822ea1731f6a1a4f7e65dec46d306d7af212`  
		Last Modified: Thu, 03 Sep 2020 23:53:23 GMT  
		Size: 4.5 MB (4516892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4baf1d1a228cab016792da8ec2b9c59b74dca0edd0fae9f3705a731289cdf1e4`  
		Last Modified: Thu, 03 Sep 2020 23:53:21 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f26ecfdc3c5cb0ccb88fa86e6c8a9dcd05075adfd73028f78deac6c880deafe`  
		Last Modified: Thu, 03 Sep 2020 23:53:21 GMT  
		Size: 570.7 KB (570680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caac09de07052197ff5c0010393812e2f0cc69a5c8a4085c3e43145359888503`  
		Last Modified: Thu, 03 Sep 2020 23:53:21 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:368e78f24adab8ca34306ad4f8a18037f83200f5e663d7bda7f25c33b162d7a9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35000759 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4c72886c1b8e0a9dcee67b383390d16ace89597664bf1f9aae6283678f49477e`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Fri, 29 May 2020 21:23:03 GMT
ADD file:8194808a812370fd2202d80d1667f851bd9eac4c560d69d347fe1964f54343de in / 
# Fri, 29 May 2020 21:23:06 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:45:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:45:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:45:29 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:45:31 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:45:39 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:45:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:44 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:45:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 03 Sep 2020 20:11:23 GMT
ENV PHP_VERSION=7.4.10
# Thu, 03 Sep 2020 20:11:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.10.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.10.tar.xz.asc
# Thu, 03 Sep 2020 20:11:40 GMT
ENV PHP_SHA256=c2d90b00b14284588a787b100dee54c2400e7db995b457864d66f00ad64fb010 PHP_MD5=
# Thu, 03 Sep 2020 20:12:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 20:12:17 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 20:16:17 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 20:16:22 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 03 Sep 2020 20:16:36 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 20:16:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 20:16:51 GMT
CMD ["php" "-a"]
# Thu, 03 Sep 2020 23:35:59 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Thu, 03 Sep 2020 23:36:04 GMT
STOPSIGNAL SIGINT
# Thu, 03 Sep 2020 23:36:20 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 03 Sep 2020 23:36:24 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 23:37:18 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Thu, 03 Sep 2020 23:37:21 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Thu, 03 Sep 2020 23:37:27 GMT
ENV ADMINER_VERSION=4.7.7
# Thu, 03 Sep 2020 23:37:30 GMT
ENV ADMINER_DOWNLOAD_SHA256=566152a2d86186dcfb28856b4ed0dfdb60e355d93ab693f7931201f75868fff0
# Thu, 03 Sep 2020 23:37:34 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=5d28c03739ce647a48ebe77e8db247b7f5ec7a2ee66ccabe00743c117d50e319
# Thu, 03 Sep 2020 23:37:44 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Thu, 03 Sep 2020 23:37:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 03 Sep 2020 23:37:51 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Thu, 03 Sep 2020 23:37:57 GMT
USER adminer
# Thu, 03 Sep 2020 23:38:02 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 03 Sep 2020 23:38:08 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:5077f8601dceb5744d875d7740ebc203f674b108a0188f3a31e292b21a4bee64`  
		Last Modified: Fri, 29 May 2020 21:23:37 GMT  
		Size: 2.8 MB (2805199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46f98eb9049c4fcbaa1cf16ddb44aaf910a89a5471dc303198251fa25bc2a1ef`  
		Last Modified: Thu, 11 Jun 2020 20:57:07 GMT  
		Size: 1.4 MB (1383311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e50cdb8e03fc1b19217cd9f80b86142d090ad3e818795b339ea4d9ef9b74555f`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b4466e085b12b265fb47397c7c105fd7d78a5883beef49ab9f386393c4c3dae`  
		Last Modified: Thu, 11 Jun 2020 20:57:06 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4751364c2ff11ca98509d7e1017b0b49d85e8650761520592243ef97dee5eb2f`  
		Last Modified: Thu, 03 Sep 2020 22:19:38 GMT  
		Size: 10.3 MB (10317385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d60b3503347e39963d634851f0e086be74a8a5d3b16d5f7bc6b14cd5b007142d`  
		Last Modified: Thu, 03 Sep 2020 22:19:35 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5295c0b35af78c6060a3d5744e52f53fe2a4624de1e6cc0398f559dc81b53a9e`  
		Last Modified: Thu, 03 Sep 2020 22:19:48 GMT  
		Size: 15.5 MB (15541414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:801b96e678054a34d2dc0d0e3a769fd670c9f4ff5cc543a329f8ee66d5e3d0b7`  
		Last Modified: Thu, 03 Sep 2020 22:19:35 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e36d26cd3e5af600178d3079512cdf76df0433a322e983e16b8007a180c7740`  
		Last Modified: Thu, 03 Sep 2020 22:19:35 GMT  
		Size: 17.0 KB (17026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53853aab5cfe309303edea0354976aaa95aed0897a32316088346fe80f8e551e`  
		Last Modified: Thu, 03 Sep 2020 23:41:32 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:217f65aee5e6e0b6f4d4a1d1a9a1ddec6c07e6e47dbf340ffec666d52b776ac6`  
		Last Modified: Thu, 03 Sep 2020 23:41:28 GMT  
		Size: 1.4 KB (1395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da82220137f9977861f4c2060e908be08df155803f7f58c7c537117b7b074c5`  
		Last Modified: Thu, 03 Sep 2020 23:41:30 GMT  
		Size: 4.4 MB (4357671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfb75e352d53f2a2f89277ab9840a2a0cca241e8f6291d713a9b752049a4bfbe`  
		Last Modified: Thu, 03 Sep 2020 23:41:28 GMT  
		Size: 1.5 KB (1479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb85419a49cfab9c4dd6df85bef4bdead330e317768e2ebff575f740b473d504`  
		Last Modified: Thu, 03 Sep 2020 23:41:28 GMT  
		Size: 570.8 KB (570774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f6e962f8a28975bee5446f4880f1b44716bc66ca4ca1640648d507caba558a1`  
		Last Modified: Thu, 03 Sep 2020 23:41:27 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:706b1a59ba77db832b0fb2bcac33403080cd232c53adc6e28fb24b8f6075a02d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.1 MB (33110263 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:070123ea618f39ec17f378694943e75f03070a66b7e651099ee6638f076f3fa9`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Fri, 29 May 2020 21:41:39 GMT
ADD file:9799ce3b2f782a28e10b1846cd9b3db827fa99c9bc601feb268456195856814e in / 
# Fri, 29 May 2020 21:41:39 GMT
CMD ["/bin/sh"]
# Thu, 11 Jun 2020 18:29:35 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 11 Jun 2020 18:29:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 11 Jun 2020 18:29:38 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 11 Jun 2020 18:29:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:29:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:29:39 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 01 Oct 2020 18:52:41 GMT
ENV PHP_VERSION=7.4.11
# Thu, 01 Oct 2020 18:52:41 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.11.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.11.tar.xz.asc
# Thu, 01 Oct 2020 18:52:41 GMT
ENV PHP_SHA256=5d31675a9b9c21b5bd03389418218c30b26558246870caba8eb54f5856e2d6ce PHP_MD5=
# Thu, 01 Oct 2020 18:52:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 01 Oct 2020 18:52:46 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 01 Oct 2020 18:55:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 01 Oct 2020 18:55:59 GMT
COPY multi:cfe027e655535d9b3eb4b44f84eafb2e1d257620ca628247fe5c1c4fb008a78a in /usr/local/bin/ 
# Thu, 01 Oct 2020 18:56:01 GMT
RUN docker-php-ext-enable sodium
# Thu, 01 Oct 2020 18:56:02 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 01 Oct 2020 18:56:02 GMT
CMD ["php" "-a"]
# Thu, 01 Oct 2020 20:45:29 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Thu, 01 Oct 2020 20:45:30 GMT
STOPSIGNAL SIGINT
# Thu, 01 Oct 2020 20:45:30 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Thu, 01 Oct 2020 20:45:31 GMT
WORKDIR /var/www/html
# Thu, 01 Oct 2020 20:45:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Thu, 01 Oct 2020 20:45:47 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Thu, 01 Oct 2020 20:45:47 GMT
ENV ADMINER_VERSION=4.7.7
# Thu, 01 Oct 2020 20:45:47 GMT
ENV ADMINER_DOWNLOAD_SHA256=566152a2d86186dcfb28856b4ed0dfdb60e355d93ab693f7931201f75868fff0
# Thu, 01 Oct 2020 20:45:48 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=5d28c03739ce647a48ebe77e8db247b7f5ec7a2ee66ccabe00743c117d50e319
# Thu, 01 Oct 2020 20:45:49 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Thu, 01 Oct 2020 20:45:49 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Thu, 01 Oct 2020 20:45:50 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Thu, 01 Oct 2020 20:45:50 GMT
USER adminer
# Thu, 01 Oct 2020 20:45:50 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Thu, 01 Oct 2020 20:45:50 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:8fb3d41b2e9a59630b51745f257cd2561f96bcd15cf309fcc20120d5fcee8c5b`  
		Last Modified: Fri, 29 May 2020 21:42:03 GMT  
		Size: 2.6 MB (2566189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:057c8475c8b5e21c245ff682a57adf8970d16ccbed87694b3ec200c83e17a8fb`  
		Last Modified: Thu, 11 Jun 2020 19:32:19 GMT  
		Size: 1.4 MB (1382745 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad2bbd1ef5644a3638bc6f073de941463cbfceb435ea6d11ce3c7fdb9f8d2539`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b73c5118a1a42bce068c040302cb99d7a26ef9ab76544773e9ba70f28d274d3`  
		Last Modified: Thu, 11 Jun 2020 19:32:18 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bf1750aaf40e10b760944a01628a26128d93951678cb339d707561e17ab2ae`  
		Last Modified: Thu, 01 Oct 2020 20:04:32 GMT  
		Size: 10.3 MB (10320989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5b07eda6143186413ec8b0f692d0862e5431fb2f396c6a5f5600d9671b1f62c`  
		Last Modified: Thu, 01 Oct 2020 20:04:31 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87eda31276ddecc7bde2c7aafc4e6c78e33e2711fc28b0a9b5c20a2d17d8bd7d`  
		Last Modified: Thu, 01 Oct 2020 20:04:34 GMT  
		Size: 14.1 MB (14090545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97e391c5deba650f11785db21a8791ddb6c5bbb198f076356c2282194560ea10`  
		Last Modified: Thu, 01 Oct 2020 20:04:31 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58e6dad0a84d45f82a6b8b5a7aca622525fa7274f480cdb06cd2f90e1b5e51d5`  
		Last Modified: Thu, 01 Oct 2020 20:04:31 GMT  
		Size: 17.0 KB (17048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fb47404505c762d82ba7698c89fc1819ed24024b8061af6cf1d4bfee4ebddd0`  
		Last Modified: Thu, 01 Oct 2020 20:46:37 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbbcf3c8f2b13cbf66ffcf9ae4d75dc8d14c9a6a69e36f63a36063c4b2704b22`  
		Last Modified: Thu, 01 Oct 2020 20:46:31 GMT  
		Size: 1.4 KB (1388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc5f4d27a42b85bec2029cf6379b63d217afc06060375ff96f6c45c98c1b407`  
		Last Modified: Thu, 01 Oct 2020 20:46:31 GMT  
		Size: 4.2 MB (4154012 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e87efb2a2c507a08ee2ef246bae633df1876e099f17ca6de5f35e01e0684a0`  
		Last Modified: Thu, 01 Oct 2020 20:46:31 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eafb5d4cd3f2db6393f8e6ff51dc645351b1882ffdd0f271a9f699a1f06333f9`  
		Last Modified: Thu, 01 Oct 2020 20:46:31 GMT  
		Size: 570.8 KB (570773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b65f8e85ae41080218ef814a66b67e45fb98f08ae59d904e22782d98ace1f3d3`  
		Last Modified: Thu, 01 Oct 2020 20:46:31 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
