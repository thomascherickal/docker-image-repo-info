<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `adminer`

-	[`adminer:4`](#adminer4)
-	[`adminer:4-fastcgi`](#adminer4-fastcgi)
-	[`adminer:4-standalone`](#adminer4-standalone)
-	[`adminer:4.8.0`](#adminer480)
-	[`adminer:4.8.0-fastcgi`](#adminer480-fastcgi)
-	[`adminer:4.8.0-standalone`](#adminer480-standalone)
-	[`adminer:fastcgi`](#adminerfastcgi)
-	[`adminer:latest`](#adminerlatest)
-	[`adminer:standalone`](#adminerstandalone)

## `adminer:4`

```console
$ docker pull adminer@sha256:a3e73e13e4f3f1bd1007d7a5d75a6bd23846c3252b71ab7a5817de9ffec04826
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

### `adminer:4` - linux; amd64

```console
$ docker pull adminer@sha256:12d118ebf5a210b26b665b62af21041766a04d73fbbc63c1b116ad6dc0387b26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.6 MB (33647506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7707fd9b142f208f18d4e495601ad485b68f5dfdd2e4cb904d253f5974ff47dc`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:39:20 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 04:03:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 04:03:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 04:08:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 04:08:27 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 04:08:28 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 04:08:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 04:08:29 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 05:51:26 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:51:26 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 05:51:27 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:51:27 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 05:51:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:51:50 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:51:53 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:51:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:51:53 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:51:53 GMT
USER adminer
# Sat, 01 May 2021 05:51:53 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 05:51:54 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39378a44d29a4d45755bbbc75353969a68f030d8c0cec90ad7f9878f59ea3f5`  
		Last Modified: Sat, 01 May 2021 04:38:19 GMT  
		Size: 10.4 MB (10360243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417049c4f35584148dfd47d28edf662385807b7efa745d4f434ba03de07494b`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21742283d02f6f9451092c008c910a3909a41e37355848483d58e4dff63faffe`  
		Last Modified: Sat, 01 May 2021 04:38:26 GMT  
		Size: 14.3 MB (14256660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50815441106c8e704643e5f718299730f3cb96b03b9214c4f32385a7d2fef9f3`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a20d3bc0470221193d84e1e28160e63d41220d5efea36e336c064fdadbfc34`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 17.5 KB (17529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a75094b0a27256eb69095e9efefc4482cf91c15bd0c82b92934ec41abb83b19`  
		Last Modified: Sat, 01 May 2021 05:52:54 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4ac41937dc4363c09566855d60c909b65e892af0706e331ccceef9ff6033bc`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85ce354c2194e2f1001e52a8c9b13058f0b5b0911d87aa541c50c18fa9d883c`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 3.9 MB (3908144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b65d1b74856e3ed0629fc712e36cf1448d5796212d5b538e77f9e08e03cb77a`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828b20dbe6f1b761839e4e1d7eaa5cf689f716af52c6e1879c7b2cd798c822fb`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 582.8 KB (582804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7b7f0dab3313363e1281a6bfe913030c6c4168beda748d4350e16880480323`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v6

```console
$ docker pull adminer@sha256:16b56985dc271840e1e8164d283af7b63b6b0e96870a3f87c2ebb6e305cb7b1c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32131886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dbef13bdb0432e75de02942ac821772395bbc7e5042fd3b5cde516593dd3f3b`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:06:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:07:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:07:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:07:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:07:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:07:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:29:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:07:41 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:07:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:07:42 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:07:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:07:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:12:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:12:47 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:12:52 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:12:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:12:54 GMT
CMD ["php" "-a"]
# Fri, 30 Apr 2021 23:14:36 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Fri, 30 Apr 2021 23:14:36 GMT
STOPSIGNAL SIGINT
# Fri, 30 Apr 2021 23:14:39 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 30 Apr 2021 23:14:41 GMT
WORKDIR /var/www/html
# Fri, 30 Apr 2021 23:15:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Fri, 30 Apr 2021 23:15:38 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Fri, 30 Apr 2021 23:15:40 GMT
ENV ADMINER_VERSION=4.8.0
# Fri, 30 Apr 2021 23:15:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Fri, 30 Apr 2021 23:15:42 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Fri, 30 Apr 2021 23:15:46 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Fri, 30 Apr 2021 23:15:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 30 Apr 2021 23:15:47 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Fri, 30 Apr 2021 23:15:48 GMT
USER adminer
# Fri, 30 Apr 2021 23:15:49 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Fri, 30 Apr 2021 23:15:49 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726cd3e9e578579e631e21133870b656f3938f6a87797a842254b274d8b76e8`  
		Last Modified: Thu, 15 Apr 2021 02:33:02 GMT  
		Size: 1.7 MB (1690998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db188e87a6ea4fd0959949208b039a0d9facc96183df8dc346c6d0d3368b77e`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73dce0ed56811623cd40b786e95b951ce9d6341d9bfefded4f8aa12574283`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7272eaae063c5d7f7a55cddcfd266b2249c9c29941e2a74712e8ef4847e31dc`  
		Last Modified: Fri, 30 Apr 2021 22:39:32 GMT  
		Size: 10.4 MB (10360229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b3ded6063933c78570fc225ff275611490972800db3a316c9c2bc7846fd31c`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2454cd2b5598ce6dd8ff8f0a593ec04bc91fe623f385a270e5fcd23a9efe837f`  
		Last Modified: Fri, 30 Apr 2021 22:39:33 GMT  
		Size: 13.2 MB (13245293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c3b006179364603a89e8662502d244437ead12db6fd3367949fcc3e72ad3dc`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1974a1d957df5934ade9796f0fa21cad68c36cf7ddee2fd124e430a2f2e159c`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 17.6 KB (17551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163da5758d6703ae0d3c6ab673fc9c00e778461230ff5aff7163baffcd7f6361`  
		Last Modified: Fri, 30 Apr 2021 23:18:35 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73f8523f7b76c4f107a5fdde83c2eed8ef45b6f265432293af6d78b772149e7`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca9f9202fb99ea8d097d90a5bb62979fbc35544da64a8a677da4b8bbf420f96`  
		Last Modified: Fri, 30 Apr 2021 23:18:35 GMT  
		Size: 3.6 MB (3604909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebdcc1e39d88d3548486b0b94fd4925deda0fd89552ec953ec45103639056e3`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634b5387043b43b3105ba37b43d31e1bf5a1ad5c5a63ee766b5c6aa198d6a2f`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 582.8 KB (582802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b737b034949aeddb4bd174c7f33742314e10f2db3cbe879b3507c0f2b2faf7`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm variant v7

```console
$ docker pull adminer@sha256:f1cd758c5bcbe78188b5766221c37d6041a5c8d727af64e9a49b277e09e80ce1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30938697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99e81544e5622446ab0920052f90534d15fe52866ccfddc0d883edcada095a7f`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:08:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:08:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:08:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:08:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:08:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:08:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:35:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:09:59 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:10:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:10:02 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:10:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:10:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:13:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:13:14 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 02:13:17 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:13:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:13:19 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 03:51:49 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 03:51:50 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 03:51:54 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 03:51:55 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 03:52:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 03:52:48 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 03:52:49 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 03:52:50 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 03:52:51 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 03:52:57 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 03:52:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 03:52:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 03:53:02 GMT
USER adminer
# Sat, 01 May 2021 03:53:05 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 03:53:07 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc6d3f07b2e440bf9a8e52a0a5bba0f27637990ee4976424cef6aae97e169f`  
		Last Modified: Thu, 15 Apr 2021 03:38:53 GMT  
		Size: 1.6 MB (1559061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9000ca9dcd92a2066a3a2c4031e677c3998cd82a3ecbc68468d11255ecbdb62`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d102949f174ecad1044574e45dded8368eb7451bf66b3bdac6e367c7f415d3`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5dab41947ddc5db66501a8111f7ef729f521e11ca3ad87ecf37bd79eac6ef3`  
		Last Modified: Sat, 01 May 2021 02:35:25 GMT  
		Size: 10.4 MB (10360231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2700665f109862388a4e0ed21b2fd335c4d89050efbad76af079999dfd9a4b68`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7aabe4a04c27ab686de62e8f214ca07e6d03fe93c6d40ade09bced2eab56901`  
		Last Modified: Sat, 01 May 2021 02:35:28 GMT  
		Size: 12.4 MB (12407150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebda42f2c319f9f89154be7b8165960eccb3900eb3f5b9e2857420d88f5ca575`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f9f67e3447fb75cf1724c1d4b7d53b8b1de00a8ec05d4aba9f7d8c09a9035`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 17.5 KB (17540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677aab5c428da05844e96dc166beb86af6dc68f33a93546bbbefed7d3839112c`  
		Last Modified: Sat, 01 May 2021 03:55:43 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2789eb966365d0da44c2eb6fce9e8d6b0b0b0640c29214cc9a6407267f9b4`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da46a02e36d762092675c2d38e18ca37e2e0163b58bf248c621b0a9dc8866d8e`  
		Last Modified: Sat, 01 May 2021 03:55:43 GMT  
		Size: 3.6 MB (3579788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841c453f4c80b715d2c60cdeb21facc849ad7ea141aef125bcdfff3fc87ea2e6`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 1.5 KB (1472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052526ae6f5bb73b64438863414d320716ac83cd7542b7db8216dba070bc9f72`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cde09e1b359229258d6f040ec2f23d5b10a5b6b50cc84580a40aaf5fa55556`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:2995c05337d98dd62225e6d58c6c551940eb5d2314ee022551a359c2edfdbb95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33288719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e49d6a5068aff4b8f7d53e5ca53084149e52a21716008685d3634f152a93cc82`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:27:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:28:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:28:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:28:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:28:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:53:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 01:51:16 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 01:51:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 01:51:18 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 01:51:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 01:51:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 01:55:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 01:55:39 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 01:55:43 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 01:55:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 01:55:46 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 04:07:49 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 04:07:50 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 04:07:54 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 04:07:55 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 04:08:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 04:08:56 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 04:08:57 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 04:08:58 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 04:08:59 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 04:09:03 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 04:09:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 04:09:05 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 04:09:06 GMT
USER adminer
# Sat, 01 May 2021 04:09:07 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 04:09:08 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea792edc0a65854bc13c90079b9e33a399c351b73e194d9df4f2cf5a0efeb2`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 1.7 MB (1700262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31bbfcb500579a0c450809a6b082c564c3ce4873732c1b62d8dab52ed0a11ac`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22841fe152c1fe4ec2048ebca3b9c0db9d29773b0d0670167a848d87fcfe83f3`  
		Last Modified: Thu, 15 Apr 2021 01:59:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86a2990f157991d12ee804183f42ab624a7af15605920e9c12adce886783bd9`  
		Last Modified: Sat, 01 May 2021 02:24:37 GMT  
		Size: 10.4 MB (10360252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717c7ad0a34fca1bd9fe22eb98d3abc226862c3a4875c05fec802e7c66425afe`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec40f0928e2ca1518729b1c63da742a00d1df98e4861f80d6e8f4019fbde9f26`  
		Last Modified: Sat, 01 May 2021 02:24:40 GMT  
		Size: 14.0 MB (14028751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d802fc3cc61952c8e0f43df7f44975e487e3d138bacfdc9c2daeca67d47cd976`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f89f4b8ccd74e3d8337940607bb14e9230a6ca849950ded149286a4b79e268a`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9208e6df146eb023a8d9b5260435c9cbd6f67b60dfb46766c5841339f85f8ec0`  
		Last Modified: Sat, 01 May 2021 04:11:07 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b108d0b6a7ff2b8cf63b53bbe86fd0454a91008e3714557e80df86a09cda0abf`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273c8a35b22772c8535453bfe942ed895b853bfabedfce587de72643c2ca6aaa`  
		Last Modified: Sat, 01 May 2021 04:11:07 GMT  
		Size: 3.9 MB (3879098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df87fa0c04f21673d85d974891030708b890f98615a245ac79d220ecf1378f7`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb52da6ce3c536b5587683997df91e97198a9ed221fd6df0b6b7d49f57717d3`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 582.8 KB (582804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4830f1e50425a8f4fc4e1236b44d93d5b39a716f837b8d921c8afb2fd5be92e`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; 386

```console
$ docker pull adminer@sha256:19d6d656da0acd11da3961bef1d4d85e7a41e7467f127e7989d0db6f8a342a95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34231434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcfa500fd2970be787667cf0eae0f3db72409b63b7d985f6402ec9b2667b013a`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 04:15:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:24:22 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:24:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:24:23 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:24:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:24:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:33:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:33:53 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:33:56 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:33:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:33:58 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 00:17:31 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 00:17:31 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 00:17:33 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 00:17:34 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 00:18:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 00:18:54 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 00:18:54 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 00:18:55 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 00:18:55 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 00:18:58 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 00:18:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 00:18:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 00:18:59 GMT
USER adminer
# Sat, 01 May 2021 00:18:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 00:19:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f032c69e4d0122e069320b9680ef26b8bb3c430278739a6fea12af3a4f96e134`  
		Last Modified: Fri, 30 Apr 2021 23:40:49 GMT  
		Size: 10.4 MB (10360220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c9984d072093737e593d0ef515c92f288b39d14aabf7a7d51b86898bc1aef7`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5e9496813676c2e99e74df895938ef33a8cf138c5a38a3e73968cc1b2fa932`  
		Last Modified: Fri, 30 Apr 2021 23:40:54 GMT  
		Size: 14.6 MB (14632431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d376f079b3a59dc3fc16b3017ea542c2ea92a6de4dcdb3aa927c19364e1df5`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df9b26593ad898c78d3de9232c23626d904c18e6b24f18767a144a5536e73e1`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 17.5 KB (17541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40300d5ae7ee86745631c5498bfc7757e4ac4bf3eacda6a10991b2a38dbcecf7`  
		Last Modified: Sat, 01 May 2021 00:21:38 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e1a92ccdfda888c1542ec341a96c423af53a5f232f654b95e5436b7256fd7b`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e200018a310c11b06c52afa2eb578aed71d2fcff109735fac4a4224a2d99198`  
		Last Modified: Sat, 01 May 2021 00:21:36 GMT  
		Size: 4.0 MB (4012274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5d7bd779781644a969c9a0c3214e5b34c562367de371486d6d908161ee3bee`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69a63a5467a891b0c71e5954c34e2275c605b8fddd9bc7856ec4442ae2a1c0d`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 582.8 KB (582810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3637c8ae22706fe31d88cd4487ddc444d18f7b005442b713e7594c150a8aa5e8`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; ppc64le

```console
$ docker pull adminer@sha256:dbb3b10c00dc1f3ece08df27b44d79f66f959aedc9d4680e63052716fda1881e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34733557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea9e143138a6e56e3f5db1c7fd10a20e080c0b8a996439d5b1e154c009c52c5`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:16:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:46:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 03:42:52 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 03:42:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 03:43:08 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 03:43:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 03:43:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 03:48:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 03:48:36 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 03:48:53 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 03:49:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 03:49:13 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 07:05:31 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 07:05:43 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 07:06:08 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 07:06:19 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 07:07:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 07:07:46 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 07:07:56 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 07:08:03 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 07:08:22 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 07:08:57 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 07:09:05 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 07:09:11 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 07:09:22 GMT
USER adminer
# Sat, 01 May 2021 07:09:31 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 07:09:38 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d82dc7c3129f9f8efe068b46b7988252e5911a9bf70f2f3ec970ed7382d8f92`  
		Last Modified: Sat, 01 May 2021 04:28:17 GMT  
		Size: 10.4 MB (10360240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f5852448efedd86253d2f693d58031fd8707b7fd4983e4b0453351d357f118`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89a34f310b9721f0ab0de62088a7d630d699d7cf59fbb7957542afbc7659f3`  
		Last Modified: Sat, 01 May 2021 04:28:19 GMT  
		Size: 15.3 MB (15282748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a34edc1036d80f0acbe7cd46a9c1bad8d141654a25252318a3457a14311dfe`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587df26cc194e45cf1f6e3bd6b2e3f0bfae286ca1ae26b98b457b556d7427303`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 17.6 KB (17562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a4991a1eff14856b0308c117ac5c87d74aac4a2c00dfc3fc38e69846bdca8e`  
		Last Modified: Sat, 01 May 2021 07:13:15 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbfbca1bede0192cfb0c862f0077baa98e4dbcd683d0682b3c04a4467ec3f67`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e078202145e09994bf4c091f95f65084e2d380b192e68fa3055f4c8da3c0f1a`  
		Last Modified: Sat, 01 May 2021 07:13:14 GMT  
		Size: 3.9 MB (3920436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a08531336bb96df3ee7311a11f8c8f5f78b27fd27f2e1e8cebe3aaebefc0cf6`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4129c43164fd79c0ea01d2c1d993a469846ebb51d831de0d08dc6fe5390ca1d`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 582.8 KB (582809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea793cb13300c9b023cc7deccce5ce057f8611b196da7f5747c42494fa1aa1f5`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4` - linux; s390x

```console
$ docker pull adminer@sha256:be29af6c13419aaaf011ebb117d07f34d74dfd3d51a4657fb92ec7e8a5a3e992
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32536231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e3b6e5f32c6c450164b419f6108097b7765a448b2965197e82c4a7be358dc10`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:18:59 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:54:37 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:54:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:54:38 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:54:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:54:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:58:16 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 02:58:18 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:58:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:58:18 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 05:16:12 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:16:12 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 05:16:14 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:16:15 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 05:16:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:16:55 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:16:58 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:16:59 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:16:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:17:00 GMT
USER adminer
# Sat, 01 May 2021 05:17:00 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 05:17:01 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b7aa20ee47cf4d85a8a033023b14b1948153a005c710022465266b1676ff00`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 10.4 MB (10360232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c09e3c51bdc12e3dac46e704947a4207380cc86861118e2ba93827f09a479b`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c57065802a25a7373daa5d63b66c55320e705d6ef8e47055d2ba2997ac4ac1f`  
		Last Modified: Sat, 01 May 2021 03:23:19 GMT  
		Size: 13.6 MB (13616029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa2ed8a45355ef77a61d2740ffedf281c9079db17e02fcd213477f4c8bd2f4`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d549711db456f1993f2dd16932c69755412329900032bc3250bfff994fd9d43`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa60d82d0a8b59fda860a56dae19ab654de0f1368014f447b7f9c53d96c5584`  
		Last Modified: Sat, 01 May 2021 05:18:16 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d3ea1b608b879ac7c8354ab621b511601a964e24706c82764e975896ec2d4`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1128a53bb989ba9202c67883e70c3aa25bfbc7a44e36360de37f23e678dab0`  
		Last Modified: Sat, 01 May 2021 05:18:15 GMT  
		Size: 3.6 MB (3588293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6ac88d341f35d6278d87a43b3998caa46d2a2d7515df5446755a418c22fb4f`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 1.5 KB (1474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46932d8f58943aa96cffad8c4b13a779eb592deacb98d058e46236c40479d28`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32bae7fbe947016896c76b4d5aea4dbb1dd2feb86f7062de658448beb0f326a`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-fastcgi`

```console
$ docker pull adminer@sha256:cfe2c1bc146279d78623f5af2f516740b209ade304d736bac5412a5125a3b44a
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

### `adminer:4-fastcgi` - linux; amd64

```console
$ docker pull adminer@sha256:bb85a1cd6d92b3ea47ec7f571c8818ef52cda3f87d39c19dd29b9c47b3975bd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33722644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1d5ea625ff4a1425ff14ce42137483342a8fda023b21d49bde2e7bcb9c429`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:08:32 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 00:08:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:08:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:08:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:50:04 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 04:08:45 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 04:08:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 04:08:45 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 04:08:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 04:08:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 04:13:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 04:13:42 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 01 May 2021 04:13:43 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 04:13:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 04:13:44 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 04:13:45 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 May 2021 04:13:45 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 May 2021 04:13:45 GMT
EXPOSE 9000
# Sat, 01 May 2021 04:13:45 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 05:52:02 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:52:03 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:52:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:52:26 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:52:26 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:52:26 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:52:26 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:52:28 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:52:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:52:28 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:52:28 GMT
USER adminer
# Sat, 01 May 2021 05:52:29 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587aa49073cc5bc626d9fa9b5db597ee0494aaabf607c40d47e86b173c352d79`  
		Last Modified: Sat, 01 May 2021 04:39:11 GMT  
		Size: 10.4 MB (10360247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edad11da1d8c5f96cb5180aafd60278895778d981d0858d1f9e8ae7f24e11ef`  
		Last Modified: Sat, 01 May 2021 04:39:07 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9160174d0ea73d3c2daffba80a6bc8fc007e25d4c53af8d79a0e3332ff64d4`  
		Last Modified: Sat, 01 May 2021 04:39:10 GMT  
		Size: 14.3 MB (14323327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588936efd0d0c4bf919d61f6b295adaff847bf6dbb177623e3be3f8ccaa80b7f`  
		Last Modified: Sat, 01 May 2021 04:39:07 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b469d4db80f6beee3277841548290c07a1cd623de057c1696c80f3ea7e25ac8d`  
		Last Modified: Sat, 01 May 2021 04:39:07 GMT  
		Size: 17.5 KB (17536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac3f8b0d122db4cd151c5c8705b9a837b7d07b59767b58b66ac8616fb1994a4`  
		Last Modified: Sat, 01 May 2021 04:39:07 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d6cfa9c78d4431301157113d599e7bfeb7d855f0b61af91a636cc10c643ba4`  
		Last Modified: Sat, 01 May 2021 05:53:22 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb776c1598fd8aa829f31f030b9c4fd717a6d114722e4ac3795df7de20c696eb`  
		Last Modified: Sat, 01 May 2021 05:53:19 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f83a3812371d1b1cf2b689b6c5aa4a3640fc411b48b54e0556bb6cb359763e`  
		Last Modified: Sat, 01 May 2021 05:53:20 GMT  
		Size: 3.9 MB (3908157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b28ebf88514becd53fe7f6e9c186269f708e0a2195c3f0cc241537c1892c36`  
		Last Modified: Sat, 01 May 2021 05:53:19 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70abec07bbc3849eaa135a1e7713d13da566d86471dc5897d07f5e7e7ccbefac`  
		Last Modified: Sat, 01 May 2021 05:53:19 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ae34fdb3b204f750ec26b75040af24cf16b32a6acc688cf3671c2dda0d8325`  
		Last Modified: Sat, 01 May 2021 05:53:19 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v6

```console
$ docker pull adminer@sha256:e7ec089a434466e6ff6988df7d109293e8bea1eaa3a677ecdb3c4f9c20881b58
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32209577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68e7a7c7afa79f110ddb25704d600a79bfe3df1e7267666840f9cf475324c9e7`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:06:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:07:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:07:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:07:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:07:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:13:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 01:13:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:13:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:13:37 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:34:04 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:13:04 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:13:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:13:06 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:13:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:13:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:16:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:16:30 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:16:33 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:16:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:16:35 GMT
WORKDIR /var/www/html
# Fri, 30 Apr 2021 22:16:38 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 30 Apr 2021 22:16:39 GMT
STOPSIGNAL SIGQUIT
# Fri, 30 Apr 2021 22:16:39 GMT
EXPOSE 9000
# Fri, 30 Apr 2021 22:16:40 GMT
CMD ["php-fpm"]
# Fri, 30 Apr 2021 23:16:09 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Fri, 30 Apr 2021 23:16:12 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 30 Apr 2021 23:17:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Fri, 30 Apr 2021 23:17:11 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Fri, 30 Apr 2021 23:17:13 GMT
ENV ADMINER_VERSION=4.8.0
# Fri, 30 Apr 2021 23:17:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Fri, 30 Apr 2021 23:17:18 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Fri, 30 Apr 2021 23:17:26 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Fri, 30 Apr 2021 23:17:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 30 Apr 2021 23:17:39 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Fri, 30 Apr 2021 23:17:44 GMT
USER adminer
# Fri, 30 Apr 2021 23:17:53 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726cd3e9e578579e631e21133870b656f3938f6a87797a842254b274d8b76e8`  
		Last Modified: Thu, 15 Apr 2021 02:33:02 GMT  
		Size: 1.7 MB (1690998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db188e87a6ea4fd0959949208b039a0d9facc96183df8dc346c6d0d3368b77e`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73dce0ed56811623cd40b786e95b951ce9d6341d9bfefded4f8aa12574283`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326d5d407c34c562acf233ba0465a9ca076c4995ea374f4935ee9a50de14304a`  
		Last Modified: Fri, 30 Apr 2021 22:40:09 GMT  
		Size: 10.4 MB (10360233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dbf5ff406dc346ecb05d404dc4cf123d1baed0540ad1fd2ba6dd768aacc0a4`  
		Last Modified: Fri, 30 Apr 2021 22:40:05 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245d552a4da6d15321f0d2b4018fbc871b3d1b71a961f1fbe4cd4f0a987d9f6a`  
		Last Modified: Fri, 30 Apr 2021 22:40:12 GMT  
		Size: 13.3 MB (13314549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa562b1287875972988fafb6ff0daf10a74db6645e30e73c5454dec085afac5`  
		Last Modified: Fri, 30 Apr 2021 22:40:05 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db31be4473204baf475d4f61f078539da6aa94516bdbf657220a83f11ee4398b`  
		Last Modified: Fri, 30 Apr 2021 22:40:05 GMT  
		Size: 17.5 KB (17544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb05aabc72b85e6abe53738ccffde33589c881cb0fa7f48491cc4ed2727590e`  
		Last Modified: Fri, 30 Apr 2021 22:40:05 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b621752cb9db17f7a3c88e8c9740607ac521657f6b04da8c78f1c7d39a9b4717`  
		Last Modified: Fri, 30 Apr 2021 23:18:56 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb194faf95e5814784905c60640a5a3896728c32016fc639e739f69e9712ef5`  
		Last Modified: Fri, 30 Apr 2021 23:18:54 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be1dacf810d372eadb5ced9f960535843b764651e0811627b788a8464fd2563`  
		Last Modified: Fri, 30 Apr 2021 23:18:55 GMT  
		Size: 3.6 MB (3604906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfc52d55996257921b21a1ad3526d2ef315ab03a1952a730d578fb08d9dd00f`  
		Last Modified: Fri, 30 Apr 2021 23:18:54 GMT  
		Size: 1.5 KB (1474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e704e7b03cf4efc6a7d79dc1c2cf6ab9cae0e9b1cf155ab25526600202c304ac`  
		Last Modified: Fri, 30 Apr 2021 23:18:54 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357d24cb511a94dc36a682ffe261d6997ea85814130bbd95f17d62662abbb40`  
		Last Modified: Fri, 30 Apr 2021 23:18:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:3c3debd1bc71b455e1d828fb1f612c8841e46a45a49ad0b873f90e303e1c3294
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31013421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3afc0fd4429ee14929b3d58c7d8dd88d25fa11c07ed4a57544d80b6b462c170c`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:08:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:08:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:08:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:08:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:08:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:16:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 02:16:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:16:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:16:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:39:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:13:34 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:13:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:13:36 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:13:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:13:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:16:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:16:50 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 01 May 2021 02:16:53 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:16:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:16:55 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 02:16:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 May 2021 02:16:57 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 May 2021 02:16:58 GMT
EXPOSE 9000
# Sat, 01 May 2021 02:16:59 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 03:53:31 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 03:53:38 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 03:54:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 03:54:47 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 03:54:49 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 03:54:51 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 03:54:54 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 03:55:07 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 03:55:09 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 03:55:10 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 03:55:16 GMT
USER adminer
# Sat, 01 May 2021 03:55:17 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc6d3f07b2e440bf9a8e52a0a5bba0f27637990ee4976424cef6aae97e169f`  
		Last Modified: Thu, 15 Apr 2021 03:38:53 GMT  
		Size: 1.6 MB (1559061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9000ca9dcd92a2066a3a2c4031e677c3998cd82a3ecbc68468d11255ecbdb62`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d102949f174ecad1044574e45dded8368eb7451bf66b3bdac6e367c7f415d3`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a887d4c3f8fab0b8a41f2e15f80000594b1db228b9a1d1068315132400a18dee`  
		Last Modified: Sat, 01 May 2021 02:35:58 GMT  
		Size: 10.4 MB (10360228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e0919fd704aa13a8b60f3a3d1e2beb99969ca0340f005b60c5ba8972a863b7`  
		Last Modified: Sat, 01 May 2021 02:35:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285eb6e1ce27fc069915bbd5b8f5b0a25a164b9c730ceea9b5d31fc4b366e173`  
		Last Modified: Sat, 01 May 2021 02:35:58 GMT  
		Size: 12.5 MB (12473434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fe9e780825250d91c98ce931c8c5b40b0840a3be7271c0da68cb91a2c363b4`  
		Last Modified: Sat, 01 May 2021 02:35:54 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8242f69b6d1406a05b5c09d0558be9cd86b94bc543392550e695d7918d12253f`  
		Last Modified: Sat, 01 May 2021 02:35:54 GMT  
		Size: 17.5 KB (17541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7df415ac941092e1076f45c06471de55333fcf15a6d6b62be12fca1d54aed65`  
		Last Modified: Sat, 01 May 2021 02:35:54 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08419d195bbd19dbc53bcfe26f58d991296299dc73e4e2f3366d05e064a172dd`  
		Last Modified: Sat, 01 May 2021 03:56:01 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547f32cf92bcb6638a56acb652022d7e025980febbd89a6da7cc430b0f80d7d5`  
		Last Modified: Sat, 01 May 2021 03:55:59 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16180895a27991a5eb67173e12509076698a8f69cacbec4bf312cd6cf98b9c6f`  
		Last Modified: Sat, 01 May 2021 03:56:00 GMT  
		Size: 3.6 MB (3579791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241656f2ebfb873a2577639b2a666b7477a81bf98d78befedb3fade16e603dd6`  
		Last Modified: Sat, 01 May 2021 03:55:59 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da4900892195d60e34c3e22c18d49ae7579a878b90638cab2b95b42d09f8c63`  
		Last Modified: Sat, 01 May 2021 03:55:59 GMT  
		Size: 582.8 KB (582802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e71054e8d8f0c9daf0a9ac9d0a7d9f0dd1dfea2c96c39e188d5c45909cee55`  
		Last Modified: Sat, 01 May 2021 03:55:59 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:5bdcde869d50b9c00ab27beb39d281ad22bed1f5ec63798d5987ec3f22a0e714
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33365959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41e197d619b95eba3b7f74b12406fe8d9f7736033704a608fc6fd23c59eb45c9`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:27:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:28:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:28:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:28:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:35:04 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 00:35:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:35:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:35:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:59:03 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 01:55:56 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 01:55:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 01:55:58 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 01:56:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 01:56:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:00:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:00:30 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 01 May 2021 02:00:36 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:00:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:00:39 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 02:00:42 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 May 2021 02:00:43 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 May 2021 02:00:44 GMT
EXPOSE 9000
# Sat, 01 May 2021 02:00:45 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 04:09:26 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 04:09:30 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 04:10:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 04:10:32 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 04:10:32 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 04:10:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 04:10:36 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 04:10:39 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 04:10:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 04:10:41 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 04:10:42 GMT
USER adminer
# Sat, 01 May 2021 04:10:43 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea792edc0a65854bc13c90079b9e33a399c351b73e194d9df4f2cf5a0efeb2`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 1.7 MB (1700262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31bbfcb500579a0c450809a6b082c564c3ce4873732c1b62d8dab52ed0a11ac`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22841fe152c1fe4ec2048ebca3b9c0db9d29773b0d0670167a848d87fcfe83f3`  
		Last Modified: Thu, 15 Apr 2021 01:59:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f8d535e8cad7ccb6f9170d7f17ed57c87e17bf74a6a9b889ee0c5d6f7a1ea0`  
		Last Modified: Sat, 01 May 2021 02:25:10 GMT  
		Size: 10.4 MB (10360253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1179292319d52c55b46cc86f4fa096f9eedb627658fb3128a302aaabeb59e9ac`  
		Last Modified: Sat, 01 May 2021 02:25:07 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e8f6926f90333ec21d01591e3d561257958f646ff18d4378f3e221e855d44`  
		Last Modified: Sat, 01 May 2021 02:25:12 GMT  
		Size: 14.1 MB (14097538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98f02f5190a9daeedd8a8c4a41aaf6272b146159c0558fbd85fdc58314469fa`  
		Last Modified: Sat, 01 May 2021 02:25:07 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e04d4e8e1659348f3dc256da300f9af8dd465317b5d4942e1c2f21bea7de34`  
		Last Modified: Sat, 01 May 2021 02:25:07 GMT  
		Size: 17.6 KB (17552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa6a64b7ec15a2645b5a6ea3a024de9f48b106bfbf5f750258505a213fe9839`  
		Last Modified: Sat, 01 May 2021 02:25:07 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb774aca288aac911b70975bfc2ffeb5316320c6f4fe13e7f6f19a2f3f5f36a`  
		Last Modified: Sat, 01 May 2021 04:11:26 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7cc42da3fb11d474881ed09adfe71ae03b2f6c2bbc3acbbd1b02c4a6529ee2`  
		Last Modified: Sat, 01 May 2021 04:11:25 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb23dde682fc45d4ad40ae4e219fd928a6e22e7c5d8c2761b45b9d1967c1969`  
		Last Modified: Sat, 01 May 2021 04:11:25 GMT  
		Size: 3.9 MB (3879097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc216bf5d605cb3e2f408d6377ef069a318da1a977f494b0e160853d2260413`  
		Last Modified: Sat, 01 May 2021 04:11:25 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9704d03344ddee4c9f158745ce184c23e8a21070c215ef5aa391af1f0d4b8b37`  
		Last Modified: Sat, 01 May 2021 04:11:25 GMT  
		Size: 582.8 KB (582799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645e8857d1e4befaa7629398c8b40cdf458341fc6ec1d9eeed6500ec44fd95fc`  
		Last Modified: Sat, 01 May 2021 04:11:24 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:d74304e9ccb1c9a94feceab9fe4fc5a2b314a0279e5144bedf39b69b2d1fb252
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34313904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c714a94da17e01e0a403f19139167a764ce92e01f46e26555b63db0bf988e2d5`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:45:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 03:45:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:45:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:45:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 04:23:18 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:34:17 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:34:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:34:18 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:34:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:34:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:47:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:47:32 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:47:35 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:47:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:47:36 GMT
WORKDIR /var/www/html
# Fri, 30 Apr 2021 22:47:38 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 30 Apr 2021 22:47:38 GMT
STOPSIGNAL SIGQUIT
# Fri, 30 Apr 2021 22:47:39 GMT
EXPOSE 9000
# Fri, 30 Apr 2021 22:47:39 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 00:19:14 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 00:19:16 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 00:20:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 00:20:34 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 00:20:35 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 00:20:35 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 00:20:36 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 00:20:39 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 00:20:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 00:20:39 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 00:20:40 GMT
USER adminer
# Sat, 01 May 2021 00:20:40 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0588acad61f86a7af9aa7d5fb5aa2b86975cc43ff9ed779a12e1f5bc055cc13d`  
		Last Modified: Fri, 30 Apr 2021 23:42:01 GMT  
		Size: 10.4 MB (10360228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9da74d5ef034b8e3d1c1843ff0f1fb32729355a09cdd37d2bb85ac0f9c84132`  
		Last Modified: Fri, 30 Apr 2021 23:41:56 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e70ffc5cc286556f65655c714c9e36bab6e3b905642fec24ea7004f7810023`  
		Last Modified: Fri, 30 Apr 2021 23:42:03 GMT  
		Size: 14.7 MB (14706461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319f59bb7b102d3532483b7815c4fd4d1a6341eb830a003ce3f5939f0735c34b`  
		Last Modified: Fri, 30 Apr 2021 23:41:56 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cc3ec3ce916d4202109b5982a0edf7f286de88ae1d7f509478b88f670b386f`  
		Last Modified: Fri, 30 Apr 2021 23:41:56 GMT  
		Size: 17.5 KB (17534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768af260a05ac95876aedc485d9ca861bddfc8bdeaeb068ef75c470344c0cd32`  
		Last Modified: Fri, 30 Apr 2021 23:41:57 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cbd27b9cc3599d28a895b6058ea82cef72905afaf0386353e458dfc656db66`  
		Last Modified: Sat, 01 May 2021 00:22:18 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339416d12f4664d3a58d59d73f746f6bfce7b9f5c1e785a4e57c2fe22c6fd030`  
		Last Modified: Sat, 01 May 2021 00:22:15 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94963c2504ced8e6b9acea28bbb4631103f18e02c9bb19b69cf856cb55b03c33`  
		Last Modified: Sat, 01 May 2021 00:22:16 GMT  
		Size: 4.0 MB (4012274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ed1d23c56aa78752221c9bb10a79ea56488d9a5761eafeaf1de7fbe5bf1843`  
		Last Modified: Sat, 01 May 2021 00:22:15 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f38dd8765af05bb660549a816d1668249fad78c5c130c5621c9f4372ad8dc7`  
		Last Modified: Sat, 01 May 2021 00:22:15 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0092d5b2329fcb1ab536ec27da58c7f4dc463cd60ed2549af3b5d324d95e57`  
		Last Modified: Sat, 01 May 2021 00:22:15 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:c9b9eb9d5f0ed98f1ef38090d1f43c75ef5aa7dc0f8f38177997929c1985fc06
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34818570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3edf620a1c345fc880bc58c5a4b925e3db5e6b2c5ea1de288f6a55c880bb08b5`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:24:29 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 14 Apr 2021 20:24:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:24:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:24:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:52:31 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 03:49:49 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 03:50:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 03:50:09 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 03:50:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 03:50:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 03:55:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 03:56:03 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 01 May 2021 03:56:22 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 03:56:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 03:56:37 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 03:56:58 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 May 2021 03:57:01 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 May 2021 03:57:05 GMT
EXPOSE 9000
# Sat, 01 May 2021 03:57:11 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 07:10:09 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 07:10:25 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 07:11:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 07:11:51 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 07:12:03 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 07:12:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 07:12:21 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 07:12:37 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 07:12:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 07:12:42 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 07:12:47 GMT
USER adminer
# Sat, 01 May 2021 07:12:49 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a25b688370820b31acaf43fe6aad086a49129e7f4cd65fe66400802f6ff46dc`  
		Last Modified: Sat, 01 May 2021 04:29:07 GMT  
		Size: 10.4 MB (10360238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a19c6448c2799fe4c148db7f3ff08fdd52be33aef25d7c62e5221f55ad41e9`  
		Last Modified: Sat, 01 May 2021 04:28:55 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfb1afb48a1979b4b32e84e66970768c28e3dc95e39a00636047349d2cab46e`  
		Last Modified: Sat, 01 May 2021 04:28:58 GMT  
		Size: 15.4 MB (15359291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72318803e295efc133889dde8281f0732d6579873ca2b88745cc3bad1e1edf0`  
		Last Modified: Sat, 01 May 2021 04:28:55 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1938d024d250ee9fd0ab42de3b74cfa6a509927a3d2bd7048e641c436827170a`  
		Last Modified: Sat, 01 May 2021 04:28:55 GMT  
		Size: 17.6 KB (17564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d534f17e924b8e0071bef66f86c1f585f78114defb32745c3bd09d1c171d72`  
		Last Modified: Sat, 01 May 2021 04:28:55 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afaad7c43a999235106d692ee7f57f72669564f26e13cbe066930abb3593cbef`  
		Last Modified: Sat, 01 May 2021 07:13:45 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee73d8b50916c3f6360690a67b457bb80dd0274af5a974e9162d23b7ab46440`  
		Last Modified: Sat, 01 May 2021 07:13:41 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475c2ec11a2c27fca9e40ee49d0e3eff6179b202dfd129dbd1983b0d0190daa4`  
		Last Modified: Sat, 01 May 2021 07:13:42 GMT  
		Size: 3.9 MB (3920457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978fe06073ae7b42ab9a1e5da4b4b12f7c546a458c491008ee3dd48a3df25efb`  
		Last Modified: Sat, 01 May 2021 07:13:42 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee616b65b8bc2e4c94a9c18aa115a754d3d5f9d882651bc410de09e18b8d07b`  
		Last Modified: Sat, 01 May 2021 07:13:42 GMT  
		Size: 582.8 KB (582806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be7c2a12b8d7973076f32cfb95817188412322c36bd0f584187df322a9ab65d`  
		Last Modified: Sat, 01 May 2021 07:13:42 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:37a6de47cf6b7daf309c4f3c01c65814a6047edc67e1ed4069c29882f12eac31
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32611287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfc0fe17d5a4a91c650323f38dc9900f70d4cba8abb1be23add218b42310390`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:06:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 14 Apr 2021 19:06:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:06:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:06:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:23:06 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:58:28 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:58:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:58:29 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:58:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:58:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 03:02:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 03:02:38 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 01 May 2021 03:02:40 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 03:02:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 03:02:41 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 03:02:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 May 2021 03:02:43 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 May 2021 03:02:44 GMT
EXPOSE 9000
# Sat, 01 May 2021 03:02:44 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 05:17:09 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:17:10 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:17:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:17:53 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:17:54 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:17:54 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:17:55 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:17:56 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:17:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:17:57 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:17:58 GMT
USER adminer
# Sat, 01 May 2021 05:17:58 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b18d4d900c0b380efa64da748d0c37984ab724c0562146008bd0a83426bdf32`  
		Last Modified: Sat, 01 May 2021 03:23:42 GMT  
		Size: 10.4 MB (10360230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2b51626ff6ef4a34223c4702434966b98229831f9c66530be32ca820415023`  
		Last Modified: Sat, 01 May 2021 03:23:39 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b865e0a6889c0902c9c9a9c2532251cf3cb0ec10684bfced428e30ed7b5e31`  
		Last Modified: Sat, 01 May 2021 03:23:42 GMT  
		Size: 13.7 MB (13682636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5714ded1c7464453f58c2d56cd5f421e11279ff4c93260a83bac5d650209ac78`  
		Last Modified: Sat, 01 May 2021 03:23:40 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652b954cfcf9d2518ff31f7e4e148840c6d2c9e092061adef93c360036077073`  
		Last Modified: Sat, 01 May 2021 03:23:39 GMT  
		Size: 17.5 KB (17547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6835da2d9378e6d9f357627a1635841f878d84d98dd7a4ac573adf0350115f66`  
		Last Modified: Sat, 01 May 2021 03:23:40 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f286878d9ffd08b9406bd8a90c540439d3f13469d7718e4f3299d0203dad5741`  
		Last Modified: Sat, 01 May 2021 05:18:31 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c5a297c12725cfbb9204865f3624d699f7aeeef484e04c6aab1055336f45c7`  
		Last Modified: Sat, 01 May 2021 05:18:29 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67496f3d3bb2e7009814fbcbc8d05eff8a850133c52638dab840493f46139417`  
		Last Modified: Sat, 01 May 2021 05:18:30 GMT  
		Size: 3.6 MB (3588283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5f14dd8fdf5f2a7efcaabae07705db96f36ffc04ec4c9057e2e5e82aa2f403`  
		Last Modified: Sat, 01 May 2021 05:18:29 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c775b338acd3d66cd584bf6bb9fc2df1adcda0aee42be49a8f390d2ebac16e3d`  
		Last Modified: Sat, 01 May 2021 05:18:29 GMT  
		Size: 582.8 KB (582811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c433f73919fc4940a0f062f4bd12ced604d485430d8bf0a3a51448794accbe3f`  
		Last Modified: Sat, 01 May 2021 05:18:30 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4-standalone`

```console
$ docker pull adminer@sha256:a3e73e13e4f3f1bd1007d7a5d75a6bd23846c3252b71ab7a5817de9ffec04826
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
$ docker pull adminer@sha256:12d118ebf5a210b26b665b62af21041766a04d73fbbc63c1b116ad6dc0387b26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.6 MB (33647506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7707fd9b142f208f18d4e495601ad485b68f5dfdd2e4cb904d253f5974ff47dc`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:39:20 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 04:03:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 04:03:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 04:08:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 04:08:27 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 04:08:28 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 04:08:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 04:08:29 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 05:51:26 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:51:26 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 05:51:27 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:51:27 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 05:51:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:51:50 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:51:53 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:51:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:51:53 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:51:53 GMT
USER adminer
# Sat, 01 May 2021 05:51:53 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 05:51:54 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39378a44d29a4d45755bbbc75353969a68f030d8c0cec90ad7f9878f59ea3f5`  
		Last Modified: Sat, 01 May 2021 04:38:19 GMT  
		Size: 10.4 MB (10360243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417049c4f35584148dfd47d28edf662385807b7efa745d4f434ba03de07494b`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21742283d02f6f9451092c008c910a3909a41e37355848483d58e4dff63faffe`  
		Last Modified: Sat, 01 May 2021 04:38:26 GMT  
		Size: 14.3 MB (14256660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50815441106c8e704643e5f718299730f3cb96b03b9214c4f32385a7d2fef9f3`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a20d3bc0470221193d84e1e28160e63d41220d5efea36e336c064fdadbfc34`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 17.5 KB (17529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a75094b0a27256eb69095e9efefc4482cf91c15bd0c82b92934ec41abb83b19`  
		Last Modified: Sat, 01 May 2021 05:52:54 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4ac41937dc4363c09566855d60c909b65e892af0706e331ccceef9ff6033bc`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85ce354c2194e2f1001e52a8c9b13058f0b5b0911d87aa541c50c18fa9d883c`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 3.9 MB (3908144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b65d1b74856e3ed0629fc712e36cf1448d5796212d5b538e77f9e08e03cb77a`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828b20dbe6f1b761839e4e1d7eaa5cf689f716af52c6e1879c7b2cd798c822fb`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 582.8 KB (582804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7b7f0dab3313363e1281a6bfe913030c6c4168beda748d4350e16880480323`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v6

```console
$ docker pull adminer@sha256:16b56985dc271840e1e8164d283af7b63b6b0e96870a3f87c2ebb6e305cb7b1c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32131886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dbef13bdb0432e75de02942ac821772395bbc7e5042fd3b5cde516593dd3f3b`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:06:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:07:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:07:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:07:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:07:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:07:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:29:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:07:41 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:07:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:07:42 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:07:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:07:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:12:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:12:47 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:12:52 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:12:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:12:54 GMT
CMD ["php" "-a"]
# Fri, 30 Apr 2021 23:14:36 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Fri, 30 Apr 2021 23:14:36 GMT
STOPSIGNAL SIGINT
# Fri, 30 Apr 2021 23:14:39 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 30 Apr 2021 23:14:41 GMT
WORKDIR /var/www/html
# Fri, 30 Apr 2021 23:15:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Fri, 30 Apr 2021 23:15:38 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Fri, 30 Apr 2021 23:15:40 GMT
ENV ADMINER_VERSION=4.8.0
# Fri, 30 Apr 2021 23:15:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Fri, 30 Apr 2021 23:15:42 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Fri, 30 Apr 2021 23:15:46 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Fri, 30 Apr 2021 23:15:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 30 Apr 2021 23:15:47 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Fri, 30 Apr 2021 23:15:48 GMT
USER adminer
# Fri, 30 Apr 2021 23:15:49 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Fri, 30 Apr 2021 23:15:49 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726cd3e9e578579e631e21133870b656f3938f6a87797a842254b274d8b76e8`  
		Last Modified: Thu, 15 Apr 2021 02:33:02 GMT  
		Size: 1.7 MB (1690998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db188e87a6ea4fd0959949208b039a0d9facc96183df8dc346c6d0d3368b77e`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73dce0ed56811623cd40b786e95b951ce9d6341d9bfefded4f8aa12574283`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7272eaae063c5d7f7a55cddcfd266b2249c9c29941e2a74712e8ef4847e31dc`  
		Last Modified: Fri, 30 Apr 2021 22:39:32 GMT  
		Size: 10.4 MB (10360229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b3ded6063933c78570fc225ff275611490972800db3a316c9c2bc7846fd31c`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2454cd2b5598ce6dd8ff8f0a593ec04bc91fe623f385a270e5fcd23a9efe837f`  
		Last Modified: Fri, 30 Apr 2021 22:39:33 GMT  
		Size: 13.2 MB (13245293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c3b006179364603a89e8662502d244437ead12db6fd3367949fcc3e72ad3dc`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1974a1d957df5934ade9796f0fa21cad68c36cf7ddee2fd124e430a2f2e159c`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 17.6 KB (17551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163da5758d6703ae0d3c6ab673fc9c00e778461230ff5aff7163baffcd7f6361`  
		Last Modified: Fri, 30 Apr 2021 23:18:35 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73f8523f7b76c4f107a5fdde83c2eed8ef45b6f265432293af6d78b772149e7`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca9f9202fb99ea8d097d90a5bb62979fbc35544da64a8a677da4b8bbf420f96`  
		Last Modified: Fri, 30 Apr 2021 23:18:35 GMT  
		Size: 3.6 MB (3604909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebdcc1e39d88d3548486b0b94fd4925deda0fd89552ec953ec45103639056e3`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634b5387043b43b3105ba37b43d31e1bf5a1ad5c5a63ee766b5c6aa198d6a2f`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 582.8 KB (582802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b737b034949aeddb4bd174c7f33742314e10f2db3cbe879b3507c0f2b2faf7`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:f1cd758c5bcbe78188b5766221c37d6041a5c8d727af64e9a49b277e09e80ce1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30938697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99e81544e5622446ab0920052f90534d15fe52866ccfddc0d883edcada095a7f`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:08:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:08:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:08:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:08:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:08:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:08:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:35:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:09:59 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:10:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:10:02 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:10:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:10:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:13:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:13:14 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 02:13:17 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:13:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:13:19 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 03:51:49 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 03:51:50 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 03:51:54 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 03:51:55 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 03:52:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 03:52:48 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 03:52:49 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 03:52:50 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 03:52:51 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 03:52:57 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 03:52:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 03:52:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 03:53:02 GMT
USER adminer
# Sat, 01 May 2021 03:53:05 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 03:53:07 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc6d3f07b2e440bf9a8e52a0a5bba0f27637990ee4976424cef6aae97e169f`  
		Last Modified: Thu, 15 Apr 2021 03:38:53 GMT  
		Size: 1.6 MB (1559061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9000ca9dcd92a2066a3a2c4031e677c3998cd82a3ecbc68468d11255ecbdb62`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d102949f174ecad1044574e45dded8368eb7451bf66b3bdac6e367c7f415d3`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5dab41947ddc5db66501a8111f7ef729f521e11ca3ad87ecf37bd79eac6ef3`  
		Last Modified: Sat, 01 May 2021 02:35:25 GMT  
		Size: 10.4 MB (10360231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2700665f109862388a4e0ed21b2fd335c4d89050efbad76af079999dfd9a4b68`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7aabe4a04c27ab686de62e8f214ca07e6d03fe93c6d40ade09bced2eab56901`  
		Last Modified: Sat, 01 May 2021 02:35:28 GMT  
		Size: 12.4 MB (12407150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebda42f2c319f9f89154be7b8165960eccb3900eb3f5b9e2857420d88f5ca575`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f9f67e3447fb75cf1724c1d4b7d53b8b1de00a8ec05d4aba9f7d8c09a9035`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 17.5 KB (17540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677aab5c428da05844e96dc166beb86af6dc68f33a93546bbbefed7d3839112c`  
		Last Modified: Sat, 01 May 2021 03:55:43 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2789eb966365d0da44c2eb6fce9e8d6b0b0b0640c29214cc9a6407267f9b4`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da46a02e36d762092675c2d38e18ca37e2e0163b58bf248c621b0a9dc8866d8e`  
		Last Modified: Sat, 01 May 2021 03:55:43 GMT  
		Size: 3.6 MB (3579788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841c453f4c80b715d2c60cdeb21facc849ad7ea141aef125bcdfff3fc87ea2e6`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 1.5 KB (1472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052526ae6f5bb73b64438863414d320716ac83cd7542b7db8216dba070bc9f72`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cde09e1b359229258d6f040ec2f23d5b10a5b6b50cc84580a40aaf5fa55556`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:2995c05337d98dd62225e6d58c6c551940eb5d2314ee022551a359c2edfdbb95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33288719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e49d6a5068aff4b8f7d53e5ca53084149e52a21716008685d3634f152a93cc82`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:27:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:28:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:28:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:28:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:28:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:53:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 01:51:16 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 01:51:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 01:51:18 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 01:51:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 01:51:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 01:55:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 01:55:39 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 01:55:43 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 01:55:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 01:55:46 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 04:07:49 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 04:07:50 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 04:07:54 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 04:07:55 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 04:08:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 04:08:56 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 04:08:57 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 04:08:58 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 04:08:59 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 04:09:03 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 04:09:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 04:09:05 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 04:09:06 GMT
USER adminer
# Sat, 01 May 2021 04:09:07 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 04:09:08 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea792edc0a65854bc13c90079b9e33a399c351b73e194d9df4f2cf5a0efeb2`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 1.7 MB (1700262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31bbfcb500579a0c450809a6b082c564c3ce4873732c1b62d8dab52ed0a11ac`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22841fe152c1fe4ec2048ebca3b9c0db9d29773b0d0670167a848d87fcfe83f3`  
		Last Modified: Thu, 15 Apr 2021 01:59:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86a2990f157991d12ee804183f42ab624a7af15605920e9c12adce886783bd9`  
		Last Modified: Sat, 01 May 2021 02:24:37 GMT  
		Size: 10.4 MB (10360252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717c7ad0a34fca1bd9fe22eb98d3abc226862c3a4875c05fec802e7c66425afe`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec40f0928e2ca1518729b1c63da742a00d1df98e4861f80d6e8f4019fbde9f26`  
		Last Modified: Sat, 01 May 2021 02:24:40 GMT  
		Size: 14.0 MB (14028751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d802fc3cc61952c8e0f43df7f44975e487e3d138bacfdc9c2daeca67d47cd976`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f89f4b8ccd74e3d8337940607bb14e9230a6ca849950ded149286a4b79e268a`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9208e6df146eb023a8d9b5260435c9cbd6f67b60dfb46766c5841339f85f8ec0`  
		Last Modified: Sat, 01 May 2021 04:11:07 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b108d0b6a7ff2b8cf63b53bbe86fd0454a91008e3714557e80df86a09cda0abf`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273c8a35b22772c8535453bfe942ed895b853bfabedfce587de72643c2ca6aaa`  
		Last Modified: Sat, 01 May 2021 04:11:07 GMT  
		Size: 3.9 MB (3879098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df87fa0c04f21673d85d974891030708b890f98615a245ac79d220ecf1378f7`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb52da6ce3c536b5587683997df91e97198a9ed221fd6df0b6b7d49f57717d3`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 582.8 KB (582804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4830f1e50425a8f4fc4e1236b44d93d5b39a716f837b8d921c8afb2fd5be92e`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; 386

```console
$ docker pull adminer@sha256:19d6d656da0acd11da3961bef1d4d85e7a41e7467f127e7989d0db6f8a342a95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34231434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcfa500fd2970be787667cf0eae0f3db72409b63b7d985f6402ec9b2667b013a`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 04:15:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:24:22 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:24:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:24:23 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:24:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:24:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:33:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:33:53 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:33:56 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:33:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:33:58 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 00:17:31 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 00:17:31 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 00:17:33 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 00:17:34 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 00:18:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 00:18:54 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 00:18:54 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 00:18:55 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 00:18:55 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 00:18:58 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 00:18:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 00:18:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 00:18:59 GMT
USER adminer
# Sat, 01 May 2021 00:18:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 00:19:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f032c69e4d0122e069320b9680ef26b8bb3c430278739a6fea12af3a4f96e134`  
		Last Modified: Fri, 30 Apr 2021 23:40:49 GMT  
		Size: 10.4 MB (10360220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c9984d072093737e593d0ef515c92f288b39d14aabf7a7d51b86898bc1aef7`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5e9496813676c2e99e74df895938ef33a8cf138c5a38a3e73968cc1b2fa932`  
		Last Modified: Fri, 30 Apr 2021 23:40:54 GMT  
		Size: 14.6 MB (14632431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d376f079b3a59dc3fc16b3017ea542c2ea92a6de4dcdb3aa927c19364e1df5`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df9b26593ad898c78d3de9232c23626d904c18e6b24f18767a144a5536e73e1`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 17.5 KB (17541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40300d5ae7ee86745631c5498bfc7757e4ac4bf3eacda6a10991b2a38dbcecf7`  
		Last Modified: Sat, 01 May 2021 00:21:38 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e1a92ccdfda888c1542ec341a96c423af53a5f232f654b95e5436b7256fd7b`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e200018a310c11b06c52afa2eb578aed71d2fcff109735fac4a4224a2d99198`  
		Last Modified: Sat, 01 May 2021 00:21:36 GMT  
		Size: 4.0 MB (4012274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5d7bd779781644a969c9a0c3214e5b34c562367de371486d6d908161ee3bee`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69a63a5467a891b0c71e5954c34e2275c605b8fddd9bc7856ec4442ae2a1c0d`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 582.8 KB (582810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3637c8ae22706fe31d88cd4487ddc444d18f7b005442b713e7594c150a8aa5e8`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:dbb3b10c00dc1f3ece08df27b44d79f66f959aedc9d4680e63052716fda1881e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34733557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea9e143138a6e56e3f5db1c7fd10a20e080c0b8a996439d5b1e154c009c52c5`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:16:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:46:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 03:42:52 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 03:42:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 03:43:08 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 03:43:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 03:43:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 03:48:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 03:48:36 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 03:48:53 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 03:49:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 03:49:13 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 07:05:31 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 07:05:43 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 07:06:08 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 07:06:19 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 07:07:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 07:07:46 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 07:07:56 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 07:08:03 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 07:08:22 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 07:08:57 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 07:09:05 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 07:09:11 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 07:09:22 GMT
USER adminer
# Sat, 01 May 2021 07:09:31 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 07:09:38 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d82dc7c3129f9f8efe068b46b7988252e5911a9bf70f2f3ec970ed7382d8f92`  
		Last Modified: Sat, 01 May 2021 04:28:17 GMT  
		Size: 10.4 MB (10360240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f5852448efedd86253d2f693d58031fd8707b7fd4983e4b0453351d357f118`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89a34f310b9721f0ab0de62088a7d630d699d7cf59fbb7957542afbc7659f3`  
		Last Modified: Sat, 01 May 2021 04:28:19 GMT  
		Size: 15.3 MB (15282748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a34edc1036d80f0acbe7cd46a9c1bad8d141654a25252318a3457a14311dfe`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587df26cc194e45cf1f6e3bd6b2e3f0bfae286ca1ae26b98b457b556d7427303`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 17.6 KB (17562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a4991a1eff14856b0308c117ac5c87d74aac4a2c00dfc3fc38e69846bdca8e`  
		Last Modified: Sat, 01 May 2021 07:13:15 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbfbca1bede0192cfb0c862f0077baa98e4dbcd683d0682b3c04a4467ec3f67`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e078202145e09994bf4c091f95f65084e2d380b192e68fa3055f4c8da3c0f1a`  
		Last Modified: Sat, 01 May 2021 07:13:14 GMT  
		Size: 3.9 MB (3920436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a08531336bb96df3ee7311a11f8c8f5f78b27fd27f2e1e8cebe3aaebefc0cf6`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4129c43164fd79c0ea01d2c1d993a469846ebb51d831de0d08dc6fe5390ca1d`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 582.8 KB (582809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea793cb13300c9b023cc7deccce5ce057f8611b196da7f5747c42494fa1aa1f5`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:be29af6c13419aaaf011ebb117d07f34d74dfd3d51a4657fb92ec7e8a5a3e992
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32536231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e3b6e5f32c6c450164b419f6108097b7765a448b2965197e82c4a7be358dc10`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:18:59 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:54:37 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:54:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:54:38 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:54:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:54:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:58:16 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 02:58:18 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:58:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:58:18 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 05:16:12 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:16:12 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 05:16:14 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:16:15 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 05:16:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:16:55 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:16:58 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:16:59 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:16:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:17:00 GMT
USER adminer
# Sat, 01 May 2021 05:17:00 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 05:17:01 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b7aa20ee47cf4d85a8a033023b14b1948153a005c710022465266b1676ff00`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 10.4 MB (10360232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c09e3c51bdc12e3dac46e704947a4207380cc86861118e2ba93827f09a479b`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c57065802a25a7373daa5d63b66c55320e705d6ef8e47055d2ba2997ac4ac1f`  
		Last Modified: Sat, 01 May 2021 03:23:19 GMT  
		Size: 13.6 MB (13616029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa2ed8a45355ef77a61d2740ffedf281c9079db17e02fcd213477f4c8bd2f4`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d549711db456f1993f2dd16932c69755412329900032bc3250bfff994fd9d43`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa60d82d0a8b59fda860a56dae19ab654de0f1368014f447b7f9c53d96c5584`  
		Last Modified: Sat, 01 May 2021 05:18:16 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d3ea1b608b879ac7c8354ab621b511601a964e24706c82764e975896ec2d4`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1128a53bb989ba9202c67883e70c3aa25bfbc7a44e36360de37f23e678dab0`  
		Last Modified: Sat, 01 May 2021 05:18:15 GMT  
		Size: 3.6 MB (3588293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6ac88d341f35d6278d87a43b3998caa46d2a2d7515df5446755a418c22fb4f`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 1.5 KB (1474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46932d8f58943aa96cffad8c4b13a779eb592deacb98d058e46236c40479d28`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32bae7fbe947016896c76b4d5aea4dbb1dd2feb86f7062de658448beb0f326a`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.0`

```console
$ docker pull adminer@sha256:a3e73e13e4f3f1bd1007d7a5d75a6bd23846c3252b71ab7a5817de9ffec04826
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

### `adminer:4.8.0` - linux; amd64

```console
$ docker pull adminer@sha256:12d118ebf5a210b26b665b62af21041766a04d73fbbc63c1b116ad6dc0387b26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.6 MB (33647506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7707fd9b142f208f18d4e495601ad485b68f5dfdd2e4cb904d253f5974ff47dc`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:39:20 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 04:03:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 04:03:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 04:08:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 04:08:27 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 04:08:28 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 04:08:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 04:08:29 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 05:51:26 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:51:26 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 05:51:27 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:51:27 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 05:51:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:51:50 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:51:53 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:51:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:51:53 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:51:53 GMT
USER adminer
# Sat, 01 May 2021 05:51:53 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 05:51:54 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39378a44d29a4d45755bbbc75353969a68f030d8c0cec90ad7f9878f59ea3f5`  
		Last Modified: Sat, 01 May 2021 04:38:19 GMT  
		Size: 10.4 MB (10360243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417049c4f35584148dfd47d28edf662385807b7efa745d4f434ba03de07494b`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21742283d02f6f9451092c008c910a3909a41e37355848483d58e4dff63faffe`  
		Last Modified: Sat, 01 May 2021 04:38:26 GMT  
		Size: 14.3 MB (14256660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50815441106c8e704643e5f718299730f3cb96b03b9214c4f32385a7d2fef9f3`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a20d3bc0470221193d84e1e28160e63d41220d5efea36e336c064fdadbfc34`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 17.5 KB (17529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a75094b0a27256eb69095e9efefc4482cf91c15bd0c82b92934ec41abb83b19`  
		Last Modified: Sat, 01 May 2021 05:52:54 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4ac41937dc4363c09566855d60c909b65e892af0706e331ccceef9ff6033bc`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85ce354c2194e2f1001e52a8c9b13058f0b5b0911d87aa541c50c18fa9d883c`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 3.9 MB (3908144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b65d1b74856e3ed0629fc712e36cf1448d5796212d5b538e77f9e08e03cb77a`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828b20dbe6f1b761839e4e1d7eaa5cf689f716af52c6e1879c7b2cd798c822fb`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 582.8 KB (582804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7b7f0dab3313363e1281a6bfe913030c6c4168beda748d4350e16880480323`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0` - linux; arm variant v6

```console
$ docker pull adminer@sha256:16b56985dc271840e1e8164d283af7b63b6b0e96870a3f87c2ebb6e305cb7b1c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32131886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dbef13bdb0432e75de02942ac821772395bbc7e5042fd3b5cde516593dd3f3b`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:06:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:07:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:07:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:07:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:07:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:07:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:29:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:07:41 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:07:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:07:42 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:07:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:07:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:12:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:12:47 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:12:52 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:12:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:12:54 GMT
CMD ["php" "-a"]
# Fri, 30 Apr 2021 23:14:36 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Fri, 30 Apr 2021 23:14:36 GMT
STOPSIGNAL SIGINT
# Fri, 30 Apr 2021 23:14:39 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 30 Apr 2021 23:14:41 GMT
WORKDIR /var/www/html
# Fri, 30 Apr 2021 23:15:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Fri, 30 Apr 2021 23:15:38 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Fri, 30 Apr 2021 23:15:40 GMT
ENV ADMINER_VERSION=4.8.0
# Fri, 30 Apr 2021 23:15:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Fri, 30 Apr 2021 23:15:42 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Fri, 30 Apr 2021 23:15:46 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Fri, 30 Apr 2021 23:15:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 30 Apr 2021 23:15:47 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Fri, 30 Apr 2021 23:15:48 GMT
USER adminer
# Fri, 30 Apr 2021 23:15:49 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Fri, 30 Apr 2021 23:15:49 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726cd3e9e578579e631e21133870b656f3938f6a87797a842254b274d8b76e8`  
		Last Modified: Thu, 15 Apr 2021 02:33:02 GMT  
		Size: 1.7 MB (1690998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db188e87a6ea4fd0959949208b039a0d9facc96183df8dc346c6d0d3368b77e`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73dce0ed56811623cd40b786e95b951ce9d6341d9bfefded4f8aa12574283`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7272eaae063c5d7f7a55cddcfd266b2249c9c29941e2a74712e8ef4847e31dc`  
		Last Modified: Fri, 30 Apr 2021 22:39:32 GMT  
		Size: 10.4 MB (10360229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b3ded6063933c78570fc225ff275611490972800db3a316c9c2bc7846fd31c`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2454cd2b5598ce6dd8ff8f0a593ec04bc91fe623f385a270e5fcd23a9efe837f`  
		Last Modified: Fri, 30 Apr 2021 22:39:33 GMT  
		Size: 13.2 MB (13245293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c3b006179364603a89e8662502d244437ead12db6fd3367949fcc3e72ad3dc`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1974a1d957df5934ade9796f0fa21cad68c36cf7ddee2fd124e430a2f2e159c`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 17.6 KB (17551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163da5758d6703ae0d3c6ab673fc9c00e778461230ff5aff7163baffcd7f6361`  
		Last Modified: Fri, 30 Apr 2021 23:18:35 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73f8523f7b76c4f107a5fdde83c2eed8ef45b6f265432293af6d78b772149e7`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca9f9202fb99ea8d097d90a5bb62979fbc35544da64a8a677da4b8bbf420f96`  
		Last Modified: Fri, 30 Apr 2021 23:18:35 GMT  
		Size: 3.6 MB (3604909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebdcc1e39d88d3548486b0b94fd4925deda0fd89552ec953ec45103639056e3`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634b5387043b43b3105ba37b43d31e1bf5a1ad5c5a63ee766b5c6aa198d6a2f`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 582.8 KB (582802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b737b034949aeddb4bd174c7f33742314e10f2db3cbe879b3507c0f2b2faf7`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0` - linux; arm variant v7

```console
$ docker pull adminer@sha256:f1cd758c5bcbe78188b5766221c37d6041a5c8d727af64e9a49b277e09e80ce1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30938697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99e81544e5622446ab0920052f90534d15fe52866ccfddc0d883edcada095a7f`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:08:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:08:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:08:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:08:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:08:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:08:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:35:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:09:59 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:10:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:10:02 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:10:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:10:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:13:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:13:14 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 02:13:17 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:13:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:13:19 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 03:51:49 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 03:51:50 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 03:51:54 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 03:51:55 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 03:52:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 03:52:48 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 03:52:49 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 03:52:50 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 03:52:51 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 03:52:57 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 03:52:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 03:52:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 03:53:02 GMT
USER adminer
# Sat, 01 May 2021 03:53:05 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 03:53:07 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc6d3f07b2e440bf9a8e52a0a5bba0f27637990ee4976424cef6aae97e169f`  
		Last Modified: Thu, 15 Apr 2021 03:38:53 GMT  
		Size: 1.6 MB (1559061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9000ca9dcd92a2066a3a2c4031e677c3998cd82a3ecbc68468d11255ecbdb62`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d102949f174ecad1044574e45dded8368eb7451bf66b3bdac6e367c7f415d3`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5dab41947ddc5db66501a8111f7ef729f521e11ca3ad87ecf37bd79eac6ef3`  
		Last Modified: Sat, 01 May 2021 02:35:25 GMT  
		Size: 10.4 MB (10360231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2700665f109862388a4e0ed21b2fd335c4d89050efbad76af079999dfd9a4b68`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7aabe4a04c27ab686de62e8f214ca07e6d03fe93c6d40ade09bced2eab56901`  
		Last Modified: Sat, 01 May 2021 02:35:28 GMT  
		Size: 12.4 MB (12407150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebda42f2c319f9f89154be7b8165960eccb3900eb3f5b9e2857420d88f5ca575`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f9f67e3447fb75cf1724c1d4b7d53b8b1de00a8ec05d4aba9f7d8c09a9035`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 17.5 KB (17540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677aab5c428da05844e96dc166beb86af6dc68f33a93546bbbefed7d3839112c`  
		Last Modified: Sat, 01 May 2021 03:55:43 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2789eb966365d0da44c2eb6fce9e8d6b0b0b0640c29214cc9a6407267f9b4`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da46a02e36d762092675c2d38e18ca37e2e0163b58bf248c621b0a9dc8866d8e`  
		Last Modified: Sat, 01 May 2021 03:55:43 GMT  
		Size: 3.6 MB (3579788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841c453f4c80b715d2c60cdeb21facc849ad7ea141aef125bcdfff3fc87ea2e6`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 1.5 KB (1472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052526ae6f5bb73b64438863414d320716ac83cd7542b7db8216dba070bc9f72`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cde09e1b359229258d6f040ec2f23d5b10a5b6b50cc84580a40aaf5fa55556`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:2995c05337d98dd62225e6d58c6c551940eb5d2314ee022551a359c2edfdbb95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33288719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e49d6a5068aff4b8f7d53e5ca53084149e52a21716008685d3634f152a93cc82`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:27:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:28:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:28:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:28:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:28:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:53:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 01:51:16 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 01:51:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 01:51:18 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 01:51:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 01:51:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 01:55:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 01:55:39 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 01:55:43 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 01:55:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 01:55:46 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 04:07:49 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 04:07:50 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 04:07:54 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 04:07:55 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 04:08:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 04:08:56 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 04:08:57 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 04:08:58 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 04:08:59 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 04:09:03 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 04:09:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 04:09:05 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 04:09:06 GMT
USER adminer
# Sat, 01 May 2021 04:09:07 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 04:09:08 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea792edc0a65854bc13c90079b9e33a399c351b73e194d9df4f2cf5a0efeb2`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 1.7 MB (1700262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31bbfcb500579a0c450809a6b082c564c3ce4873732c1b62d8dab52ed0a11ac`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22841fe152c1fe4ec2048ebca3b9c0db9d29773b0d0670167a848d87fcfe83f3`  
		Last Modified: Thu, 15 Apr 2021 01:59:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86a2990f157991d12ee804183f42ab624a7af15605920e9c12adce886783bd9`  
		Last Modified: Sat, 01 May 2021 02:24:37 GMT  
		Size: 10.4 MB (10360252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717c7ad0a34fca1bd9fe22eb98d3abc226862c3a4875c05fec802e7c66425afe`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec40f0928e2ca1518729b1c63da742a00d1df98e4861f80d6e8f4019fbde9f26`  
		Last Modified: Sat, 01 May 2021 02:24:40 GMT  
		Size: 14.0 MB (14028751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d802fc3cc61952c8e0f43df7f44975e487e3d138bacfdc9c2daeca67d47cd976`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f89f4b8ccd74e3d8337940607bb14e9230a6ca849950ded149286a4b79e268a`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9208e6df146eb023a8d9b5260435c9cbd6f67b60dfb46766c5841339f85f8ec0`  
		Last Modified: Sat, 01 May 2021 04:11:07 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b108d0b6a7ff2b8cf63b53bbe86fd0454a91008e3714557e80df86a09cda0abf`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273c8a35b22772c8535453bfe942ed895b853bfabedfce587de72643c2ca6aaa`  
		Last Modified: Sat, 01 May 2021 04:11:07 GMT  
		Size: 3.9 MB (3879098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df87fa0c04f21673d85d974891030708b890f98615a245ac79d220ecf1378f7`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb52da6ce3c536b5587683997df91e97198a9ed221fd6df0b6b7d49f57717d3`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 582.8 KB (582804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4830f1e50425a8f4fc4e1236b44d93d5b39a716f837b8d921c8afb2fd5be92e`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0` - linux; 386

```console
$ docker pull adminer@sha256:19d6d656da0acd11da3961bef1d4d85e7a41e7467f127e7989d0db6f8a342a95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34231434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcfa500fd2970be787667cf0eae0f3db72409b63b7d985f6402ec9b2667b013a`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 04:15:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:24:22 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:24:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:24:23 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:24:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:24:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:33:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:33:53 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:33:56 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:33:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:33:58 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 00:17:31 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 00:17:31 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 00:17:33 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 00:17:34 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 00:18:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 00:18:54 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 00:18:54 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 00:18:55 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 00:18:55 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 00:18:58 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 00:18:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 00:18:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 00:18:59 GMT
USER adminer
# Sat, 01 May 2021 00:18:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 00:19:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f032c69e4d0122e069320b9680ef26b8bb3c430278739a6fea12af3a4f96e134`  
		Last Modified: Fri, 30 Apr 2021 23:40:49 GMT  
		Size: 10.4 MB (10360220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c9984d072093737e593d0ef515c92f288b39d14aabf7a7d51b86898bc1aef7`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5e9496813676c2e99e74df895938ef33a8cf138c5a38a3e73968cc1b2fa932`  
		Last Modified: Fri, 30 Apr 2021 23:40:54 GMT  
		Size: 14.6 MB (14632431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d376f079b3a59dc3fc16b3017ea542c2ea92a6de4dcdb3aa927c19364e1df5`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df9b26593ad898c78d3de9232c23626d904c18e6b24f18767a144a5536e73e1`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 17.5 KB (17541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40300d5ae7ee86745631c5498bfc7757e4ac4bf3eacda6a10991b2a38dbcecf7`  
		Last Modified: Sat, 01 May 2021 00:21:38 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e1a92ccdfda888c1542ec341a96c423af53a5f232f654b95e5436b7256fd7b`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e200018a310c11b06c52afa2eb578aed71d2fcff109735fac4a4224a2d99198`  
		Last Modified: Sat, 01 May 2021 00:21:36 GMT  
		Size: 4.0 MB (4012274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5d7bd779781644a969c9a0c3214e5b34c562367de371486d6d908161ee3bee`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69a63a5467a891b0c71e5954c34e2275c605b8fddd9bc7856ec4442ae2a1c0d`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 582.8 KB (582810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3637c8ae22706fe31d88cd4487ddc444d18f7b005442b713e7594c150a8aa5e8`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0` - linux; ppc64le

```console
$ docker pull adminer@sha256:dbb3b10c00dc1f3ece08df27b44d79f66f959aedc9d4680e63052716fda1881e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34733557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea9e143138a6e56e3f5db1c7fd10a20e080c0b8a996439d5b1e154c009c52c5`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:16:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:46:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 03:42:52 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 03:42:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 03:43:08 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 03:43:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 03:43:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 03:48:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 03:48:36 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 03:48:53 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 03:49:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 03:49:13 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 07:05:31 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 07:05:43 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 07:06:08 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 07:06:19 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 07:07:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 07:07:46 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 07:07:56 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 07:08:03 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 07:08:22 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 07:08:57 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 07:09:05 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 07:09:11 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 07:09:22 GMT
USER adminer
# Sat, 01 May 2021 07:09:31 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 07:09:38 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d82dc7c3129f9f8efe068b46b7988252e5911a9bf70f2f3ec970ed7382d8f92`  
		Last Modified: Sat, 01 May 2021 04:28:17 GMT  
		Size: 10.4 MB (10360240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f5852448efedd86253d2f693d58031fd8707b7fd4983e4b0453351d357f118`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89a34f310b9721f0ab0de62088a7d630d699d7cf59fbb7957542afbc7659f3`  
		Last Modified: Sat, 01 May 2021 04:28:19 GMT  
		Size: 15.3 MB (15282748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a34edc1036d80f0acbe7cd46a9c1bad8d141654a25252318a3457a14311dfe`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587df26cc194e45cf1f6e3bd6b2e3f0bfae286ca1ae26b98b457b556d7427303`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 17.6 KB (17562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a4991a1eff14856b0308c117ac5c87d74aac4a2c00dfc3fc38e69846bdca8e`  
		Last Modified: Sat, 01 May 2021 07:13:15 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbfbca1bede0192cfb0c862f0077baa98e4dbcd683d0682b3c04a4467ec3f67`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e078202145e09994bf4c091f95f65084e2d380b192e68fa3055f4c8da3c0f1a`  
		Last Modified: Sat, 01 May 2021 07:13:14 GMT  
		Size: 3.9 MB (3920436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a08531336bb96df3ee7311a11f8c8f5f78b27fd27f2e1e8cebe3aaebefc0cf6`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4129c43164fd79c0ea01d2c1d993a469846ebb51d831de0d08dc6fe5390ca1d`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 582.8 KB (582809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea793cb13300c9b023cc7deccce5ce057f8611b196da7f5747c42494fa1aa1f5`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0` - linux; s390x

```console
$ docker pull adminer@sha256:be29af6c13419aaaf011ebb117d07f34d74dfd3d51a4657fb92ec7e8a5a3e992
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32536231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e3b6e5f32c6c450164b419f6108097b7765a448b2965197e82c4a7be358dc10`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:18:59 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:54:37 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:54:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:54:38 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:54:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:54:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:58:16 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 02:58:18 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:58:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:58:18 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 05:16:12 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:16:12 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 05:16:14 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:16:15 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 05:16:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:16:55 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:16:58 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:16:59 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:16:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:17:00 GMT
USER adminer
# Sat, 01 May 2021 05:17:00 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 05:17:01 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b7aa20ee47cf4d85a8a033023b14b1948153a005c710022465266b1676ff00`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 10.4 MB (10360232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c09e3c51bdc12e3dac46e704947a4207380cc86861118e2ba93827f09a479b`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c57065802a25a7373daa5d63b66c55320e705d6ef8e47055d2ba2997ac4ac1f`  
		Last Modified: Sat, 01 May 2021 03:23:19 GMT  
		Size: 13.6 MB (13616029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa2ed8a45355ef77a61d2740ffedf281c9079db17e02fcd213477f4c8bd2f4`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d549711db456f1993f2dd16932c69755412329900032bc3250bfff994fd9d43`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa60d82d0a8b59fda860a56dae19ab654de0f1368014f447b7f9c53d96c5584`  
		Last Modified: Sat, 01 May 2021 05:18:16 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d3ea1b608b879ac7c8354ab621b511601a964e24706c82764e975896ec2d4`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1128a53bb989ba9202c67883e70c3aa25bfbc7a44e36360de37f23e678dab0`  
		Last Modified: Sat, 01 May 2021 05:18:15 GMT  
		Size: 3.6 MB (3588293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6ac88d341f35d6278d87a43b3998caa46d2a2d7515df5446755a418c22fb4f`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 1.5 KB (1474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46932d8f58943aa96cffad8c4b13a779eb592deacb98d058e46236c40479d28`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32bae7fbe947016896c76b4d5aea4dbb1dd2feb86f7062de658448beb0f326a`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.0-fastcgi`

```console
$ docker pull adminer@sha256:cfe2c1bc146279d78623f5af2f516740b209ade304d736bac5412a5125a3b44a
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

### `adminer:4.8.0-fastcgi` - linux; amd64

```console
$ docker pull adminer@sha256:bb85a1cd6d92b3ea47ec7f571c8818ef52cda3f87d39c19dd29b9c47b3975bd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33722644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1d5ea625ff4a1425ff14ce42137483342a8fda023b21d49bde2e7bcb9c429`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:08:32 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 00:08:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:08:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:08:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:50:04 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 04:08:45 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 04:08:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 04:08:45 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 04:08:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 04:08:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 04:13:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 04:13:42 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 01 May 2021 04:13:43 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 04:13:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 04:13:44 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 04:13:45 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 May 2021 04:13:45 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 May 2021 04:13:45 GMT
EXPOSE 9000
# Sat, 01 May 2021 04:13:45 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 05:52:02 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:52:03 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:52:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:52:26 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:52:26 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:52:26 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:52:26 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:52:28 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:52:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:52:28 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:52:28 GMT
USER adminer
# Sat, 01 May 2021 05:52:29 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587aa49073cc5bc626d9fa9b5db597ee0494aaabf607c40d47e86b173c352d79`  
		Last Modified: Sat, 01 May 2021 04:39:11 GMT  
		Size: 10.4 MB (10360247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edad11da1d8c5f96cb5180aafd60278895778d981d0858d1f9e8ae7f24e11ef`  
		Last Modified: Sat, 01 May 2021 04:39:07 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9160174d0ea73d3c2daffba80a6bc8fc007e25d4c53af8d79a0e3332ff64d4`  
		Last Modified: Sat, 01 May 2021 04:39:10 GMT  
		Size: 14.3 MB (14323327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588936efd0d0c4bf919d61f6b295adaff847bf6dbb177623e3be3f8ccaa80b7f`  
		Last Modified: Sat, 01 May 2021 04:39:07 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b469d4db80f6beee3277841548290c07a1cd623de057c1696c80f3ea7e25ac8d`  
		Last Modified: Sat, 01 May 2021 04:39:07 GMT  
		Size: 17.5 KB (17536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac3f8b0d122db4cd151c5c8705b9a837b7d07b59767b58b66ac8616fb1994a4`  
		Last Modified: Sat, 01 May 2021 04:39:07 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d6cfa9c78d4431301157113d599e7bfeb7d855f0b61af91a636cc10c643ba4`  
		Last Modified: Sat, 01 May 2021 05:53:22 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb776c1598fd8aa829f31f030b9c4fd717a6d114722e4ac3795df7de20c696eb`  
		Last Modified: Sat, 01 May 2021 05:53:19 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f83a3812371d1b1cf2b689b6c5aa4a3640fc411b48b54e0556bb6cb359763e`  
		Last Modified: Sat, 01 May 2021 05:53:20 GMT  
		Size: 3.9 MB (3908157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b28ebf88514becd53fe7f6e9c186269f708e0a2195c3f0cc241537c1892c36`  
		Last Modified: Sat, 01 May 2021 05:53:19 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70abec07bbc3849eaa135a1e7713d13da566d86471dc5897d07f5e7e7ccbefac`  
		Last Modified: Sat, 01 May 2021 05:53:19 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ae34fdb3b204f750ec26b75040af24cf16b32a6acc688cf3671c2dda0d8325`  
		Last Modified: Sat, 01 May 2021 05:53:19 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0-fastcgi` - linux; arm variant v6

```console
$ docker pull adminer@sha256:e7ec089a434466e6ff6988df7d109293e8bea1eaa3a677ecdb3c4f9c20881b58
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32209577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68e7a7c7afa79f110ddb25704d600a79bfe3df1e7267666840f9cf475324c9e7`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:06:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:07:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:07:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:07:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:07:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:13:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 01:13:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:13:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:13:37 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:34:04 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:13:04 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:13:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:13:06 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:13:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:13:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:16:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:16:30 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:16:33 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:16:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:16:35 GMT
WORKDIR /var/www/html
# Fri, 30 Apr 2021 22:16:38 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 30 Apr 2021 22:16:39 GMT
STOPSIGNAL SIGQUIT
# Fri, 30 Apr 2021 22:16:39 GMT
EXPOSE 9000
# Fri, 30 Apr 2021 22:16:40 GMT
CMD ["php-fpm"]
# Fri, 30 Apr 2021 23:16:09 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Fri, 30 Apr 2021 23:16:12 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 30 Apr 2021 23:17:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Fri, 30 Apr 2021 23:17:11 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Fri, 30 Apr 2021 23:17:13 GMT
ENV ADMINER_VERSION=4.8.0
# Fri, 30 Apr 2021 23:17:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Fri, 30 Apr 2021 23:17:18 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Fri, 30 Apr 2021 23:17:26 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Fri, 30 Apr 2021 23:17:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 30 Apr 2021 23:17:39 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Fri, 30 Apr 2021 23:17:44 GMT
USER adminer
# Fri, 30 Apr 2021 23:17:53 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726cd3e9e578579e631e21133870b656f3938f6a87797a842254b274d8b76e8`  
		Last Modified: Thu, 15 Apr 2021 02:33:02 GMT  
		Size: 1.7 MB (1690998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db188e87a6ea4fd0959949208b039a0d9facc96183df8dc346c6d0d3368b77e`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73dce0ed56811623cd40b786e95b951ce9d6341d9bfefded4f8aa12574283`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326d5d407c34c562acf233ba0465a9ca076c4995ea374f4935ee9a50de14304a`  
		Last Modified: Fri, 30 Apr 2021 22:40:09 GMT  
		Size: 10.4 MB (10360233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dbf5ff406dc346ecb05d404dc4cf123d1baed0540ad1fd2ba6dd768aacc0a4`  
		Last Modified: Fri, 30 Apr 2021 22:40:05 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245d552a4da6d15321f0d2b4018fbc871b3d1b71a961f1fbe4cd4f0a987d9f6a`  
		Last Modified: Fri, 30 Apr 2021 22:40:12 GMT  
		Size: 13.3 MB (13314549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa562b1287875972988fafb6ff0daf10a74db6645e30e73c5454dec085afac5`  
		Last Modified: Fri, 30 Apr 2021 22:40:05 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db31be4473204baf475d4f61f078539da6aa94516bdbf657220a83f11ee4398b`  
		Last Modified: Fri, 30 Apr 2021 22:40:05 GMT  
		Size: 17.5 KB (17544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb05aabc72b85e6abe53738ccffde33589c881cb0fa7f48491cc4ed2727590e`  
		Last Modified: Fri, 30 Apr 2021 22:40:05 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b621752cb9db17f7a3c88e8c9740607ac521657f6b04da8c78f1c7d39a9b4717`  
		Last Modified: Fri, 30 Apr 2021 23:18:56 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb194faf95e5814784905c60640a5a3896728c32016fc639e739f69e9712ef5`  
		Last Modified: Fri, 30 Apr 2021 23:18:54 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be1dacf810d372eadb5ced9f960535843b764651e0811627b788a8464fd2563`  
		Last Modified: Fri, 30 Apr 2021 23:18:55 GMT  
		Size: 3.6 MB (3604906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfc52d55996257921b21a1ad3526d2ef315ab03a1952a730d578fb08d9dd00f`  
		Last Modified: Fri, 30 Apr 2021 23:18:54 GMT  
		Size: 1.5 KB (1474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e704e7b03cf4efc6a7d79dc1c2cf6ab9cae0e9b1cf155ab25526600202c304ac`  
		Last Modified: Fri, 30 Apr 2021 23:18:54 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357d24cb511a94dc36a682ffe261d6997ea85814130bbd95f17d62662abbb40`  
		Last Modified: Fri, 30 Apr 2021 23:18:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0-fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:3c3debd1bc71b455e1d828fb1f612c8841e46a45a49ad0b873f90e303e1c3294
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31013421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3afc0fd4429ee14929b3d58c7d8dd88d25fa11c07ed4a57544d80b6b462c170c`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:08:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:08:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:08:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:08:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:08:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:16:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 02:16:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:16:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:16:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:39:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:13:34 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:13:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:13:36 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:13:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:13:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:16:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:16:50 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 01 May 2021 02:16:53 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:16:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:16:55 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 02:16:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 May 2021 02:16:57 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 May 2021 02:16:58 GMT
EXPOSE 9000
# Sat, 01 May 2021 02:16:59 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 03:53:31 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 03:53:38 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 03:54:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 03:54:47 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 03:54:49 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 03:54:51 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 03:54:54 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 03:55:07 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 03:55:09 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 03:55:10 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 03:55:16 GMT
USER adminer
# Sat, 01 May 2021 03:55:17 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc6d3f07b2e440bf9a8e52a0a5bba0f27637990ee4976424cef6aae97e169f`  
		Last Modified: Thu, 15 Apr 2021 03:38:53 GMT  
		Size: 1.6 MB (1559061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9000ca9dcd92a2066a3a2c4031e677c3998cd82a3ecbc68468d11255ecbdb62`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d102949f174ecad1044574e45dded8368eb7451bf66b3bdac6e367c7f415d3`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a887d4c3f8fab0b8a41f2e15f80000594b1db228b9a1d1068315132400a18dee`  
		Last Modified: Sat, 01 May 2021 02:35:58 GMT  
		Size: 10.4 MB (10360228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e0919fd704aa13a8b60f3a3d1e2beb99969ca0340f005b60c5ba8972a863b7`  
		Last Modified: Sat, 01 May 2021 02:35:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285eb6e1ce27fc069915bbd5b8f5b0a25a164b9c730ceea9b5d31fc4b366e173`  
		Last Modified: Sat, 01 May 2021 02:35:58 GMT  
		Size: 12.5 MB (12473434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fe9e780825250d91c98ce931c8c5b40b0840a3be7271c0da68cb91a2c363b4`  
		Last Modified: Sat, 01 May 2021 02:35:54 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8242f69b6d1406a05b5c09d0558be9cd86b94bc543392550e695d7918d12253f`  
		Last Modified: Sat, 01 May 2021 02:35:54 GMT  
		Size: 17.5 KB (17541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7df415ac941092e1076f45c06471de55333fcf15a6d6b62be12fca1d54aed65`  
		Last Modified: Sat, 01 May 2021 02:35:54 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08419d195bbd19dbc53bcfe26f58d991296299dc73e4e2f3366d05e064a172dd`  
		Last Modified: Sat, 01 May 2021 03:56:01 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547f32cf92bcb6638a56acb652022d7e025980febbd89a6da7cc430b0f80d7d5`  
		Last Modified: Sat, 01 May 2021 03:55:59 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16180895a27991a5eb67173e12509076698a8f69cacbec4bf312cd6cf98b9c6f`  
		Last Modified: Sat, 01 May 2021 03:56:00 GMT  
		Size: 3.6 MB (3579791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241656f2ebfb873a2577639b2a666b7477a81bf98d78befedb3fade16e603dd6`  
		Last Modified: Sat, 01 May 2021 03:55:59 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da4900892195d60e34c3e22c18d49ae7579a878b90638cab2b95b42d09f8c63`  
		Last Modified: Sat, 01 May 2021 03:55:59 GMT  
		Size: 582.8 KB (582802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e71054e8d8f0c9daf0a9ac9d0a7d9f0dd1dfea2c96c39e188d5c45909cee55`  
		Last Modified: Sat, 01 May 2021 03:55:59 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0-fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:5bdcde869d50b9c00ab27beb39d281ad22bed1f5ec63798d5987ec3f22a0e714
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33365959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41e197d619b95eba3b7f74b12406fe8d9f7736033704a608fc6fd23c59eb45c9`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:27:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:28:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:28:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:28:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:35:04 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 00:35:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:35:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:35:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:59:03 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 01:55:56 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 01:55:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 01:55:58 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 01:56:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 01:56:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:00:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:00:30 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 01 May 2021 02:00:36 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:00:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:00:39 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 02:00:42 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 May 2021 02:00:43 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 May 2021 02:00:44 GMT
EXPOSE 9000
# Sat, 01 May 2021 02:00:45 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 04:09:26 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 04:09:30 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 04:10:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 04:10:32 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 04:10:32 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 04:10:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 04:10:36 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 04:10:39 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 04:10:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 04:10:41 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 04:10:42 GMT
USER adminer
# Sat, 01 May 2021 04:10:43 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea792edc0a65854bc13c90079b9e33a399c351b73e194d9df4f2cf5a0efeb2`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 1.7 MB (1700262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31bbfcb500579a0c450809a6b082c564c3ce4873732c1b62d8dab52ed0a11ac`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22841fe152c1fe4ec2048ebca3b9c0db9d29773b0d0670167a848d87fcfe83f3`  
		Last Modified: Thu, 15 Apr 2021 01:59:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f8d535e8cad7ccb6f9170d7f17ed57c87e17bf74a6a9b889ee0c5d6f7a1ea0`  
		Last Modified: Sat, 01 May 2021 02:25:10 GMT  
		Size: 10.4 MB (10360253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1179292319d52c55b46cc86f4fa096f9eedb627658fb3128a302aaabeb59e9ac`  
		Last Modified: Sat, 01 May 2021 02:25:07 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e8f6926f90333ec21d01591e3d561257958f646ff18d4378f3e221e855d44`  
		Last Modified: Sat, 01 May 2021 02:25:12 GMT  
		Size: 14.1 MB (14097538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98f02f5190a9daeedd8a8c4a41aaf6272b146159c0558fbd85fdc58314469fa`  
		Last Modified: Sat, 01 May 2021 02:25:07 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e04d4e8e1659348f3dc256da300f9af8dd465317b5d4942e1c2f21bea7de34`  
		Last Modified: Sat, 01 May 2021 02:25:07 GMT  
		Size: 17.6 KB (17552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa6a64b7ec15a2645b5a6ea3a024de9f48b106bfbf5f750258505a213fe9839`  
		Last Modified: Sat, 01 May 2021 02:25:07 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb774aca288aac911b70975bfc2ffeb5316320c6f4fe13e7f6f19a2f3f5f36a`  
		Last Modified: Sat, 01 May 2021 04:11:26 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7cc42da3fb11d474881ed09adfe71ae03b2f6c2bbc3acbbd1b02c4a6529ee2`  
		Last Modified: Sat, 01 May 2021 04:11:25 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb23dde682fc45d4ad40ae4e219fd928a6e22e7c5d8c2761b45b9d1967c1969`  
		Last Modified: Sat, 01 May 2021 04:11:25 GMT  
		Size: 3.9 MB (3879097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc216bf5d605cb3e2f408d6377ef069a318da1a977f494b0e160853d2260413`  
		Last Modified: Sat, 01 May 2021 04:11:25 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9704d03344ddee4c9f158745ce184c23e8a21070c215ef5aa391af1f0d4b8b37`  
		Last Modified: Sat, 01 May 2021 04:11:25 GMT  
		Size: 582.8 KB (582799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645e8857d1e4befaa7629398c8b40cdf458341fc6ec1d9eeed6500ec44fd95fc`  
		Last Modified: Sat, 01 May 2021 04:11:24 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0-fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:d74304e9ccb1c9a94feceab9fe4fc5a2b314a0279e5144bedf39b69b2d1fb252
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34313904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c714a94da17e01e0a403f19139167a764ce92e01f46e26555b63db0bf988e2d5`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:45:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 03:45:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:45:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:45:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 04:23:18 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:34:17 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:34:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:34:18 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:34:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:34:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:47:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:47:32 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:47:35 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:47:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:47:36 GMT
WORKDIR /var/www/html
# Fri, 30 Apr 2021 22:47:38 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 30 Apr 2021 22:47:38 GMT
STOPSIGNAL SIGQUIT
# Fri, 30 Apr 2021 22:47:39 GMT
EXPOSE 9000
# Fri, 30 Apr 2021 22:47:39 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 00:19:14 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 00:19:16 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 00:20:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 00:20:34 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 00:20:35 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 00:20:35 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 00:20:36 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 00:20:39 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 00:20:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 00:20:39 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 00:20:40 GMT
USER adminer
# Sat, 01 May 2021 00:20:40 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0588acad61f86a7af9aa7d5fb5aa2b86975cc43ff9ed779a12e1f5bc055cc13d`  
		Last Modified: Fri, 30 Apr 2021 23:42:01 GMT  
		Size: 10.4 MB (10360228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9da74d5ef034b8e3d1c1843ff0f1fb32729355a09cdd37d2bb85ac0f9c84132`  
		Last Modified: Fri, 30 Apr 2021 23:41:56 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e70ffc5cc286556f65655c714c9e36bab6e3b905642fec24ea7004f7810023`  
		Last Modified: Fri, 30 Apr 2021 23:42:03 GMT  
		Size: 14.7 MB (14706461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319f59bb7b102d3532483b7815c4fd4d1a6341eb830a003ce3f5939f0735c34b`  
		Last Modified: Fri, 30 Apr 2021 23:41:56 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cc3ec3ce916d4202109b5982a0edf7f286de88ae1d7f509478b88f670b386f`  
		Last Modified: Fri, 30 Apr 2021 23:41:56 GMT  
		Size: 17.5 KB (17534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768af260a05ac95876aedc485d9ca861bddfc8bdeaeb068ef75c470344c0cd32`  
		Last Modified: Fri, 30 Apr 2021 23:41:57 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cbd27b9cc3599d28a895b6058ea82cef72905afaf0386353e458dfc656db66`  
		Last Modified: Sat, 01 May 2021 00:22:18 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339416d12f4664d3a58d59d73f746f6bfce7b9f5c1e785a4e57c2fe22c6fd030`  
		Last Modified: Sat, 01 May 2021 00:22:15 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94963c2504ced8e6b9acea28bbb4631103f18e02c9bb19b69cf856cb55b03c33`  
		Last Modified: Sat, 01 May 2021 00:22:16 GMT  
		Size: 4.0 MB (4012274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ed1d23c56aa78752221c9bb10a79ea56488d9a5761eafeaf1de7fbe5bf1843`  
		Last Modified: Sat, 01 May 2021 00:22:15 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f38dd8765af05bb660549a816d1668249fad78c5c130c5621c9f4372ad8dc7`  
		Last Modified: Sat, 01 May 2021 00:22:15 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0092d5b2329fcb1ab536ec27da58c7f4dc463cd60ed2549af3b5d324d95e57`  
		Last Modified: Sat, 01 May 2021 00:22:15 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0-fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:c9b9eb9d5f0ed98f1ef38090d1f43c75ef5aa7dc0f8f38177997929c1985fc06
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34818570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3edf620a1c345fc880bc58c5a4b925e3db5e6b2c5ea1de288f6a55c880bb08b5`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:24:29 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 14 Apr 2021 20:24:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:24:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:24:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:52:31 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 03:49:49 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 03:50:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 03:50:09 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 03:50:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 03:50:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 03:55:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 03:56:03 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 01 May 2021 03:56:22 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 03:56:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 03:56:37 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 03:56:58 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 May 2021 03:57:01 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 May 2021 03:57:05 GMT
EXPOSE 9000
# Sat, 01 May 2021 03:57:11 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 07:10:09 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 07:10:25 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 07:11:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 07:11:51 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 07:12:03 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 07:12:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 07:12:21 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 07:12:37 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 07:12:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 07:12:42 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 07:12:47 GMT
USER adminer
# Sat, 01 May 2021 07:12:49 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a25b688370820b31acaf43fe6aad086a49129e7f4cd65fe66400802f6ff46dc`  
		Last Modified: Sat, 01 May 2021 04:29:07 GMT  
		Size: 10.4 MB (10360238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a19c6448c2799fe4c148db7f3ff08fdd52be33aef25d7c62e5221f55ad41e9`  
		Last Modified: Sat, 01 May 2021 04:28:55 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfb1afb48a1979b4b32e84e66970768c28e3dc95e39a00636047349d2cab46e`  
		Last Modified: Sat, 01 May 2021 04:28:58 GMT  
		Size: 15.4 MB (15359291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72318803e295efc133889dde8281f0732d6579873ca2b88745cc3bad1e1edf0`  
		Last Modified: Sat, 01 May 2021 04:28:55 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1938d024d250ee9fd0ab42de3b74cfa6a509927a3d2bd7048e641c436827170a`  
		Last Modified: Sat, 01 May 2021 04:28:55 GMT  
		Size: 17.6 KB (17564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d534f17e924b8e0071bef66f86c1f585f78114defb32745c3bd09d1c171d72`  
		Last Modified: Sat, 01 May 2021 04:28:55 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afaad7c43a999235106d692ee7f57f72669564f26e13cbe066930abb3593cbef`  
		Last Modified: Sat, 01 May 2021 07:13:45 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee73d8b50916c3f6360690a67b457bb80dd0274af5a974e9162d23b7ab46440`  
		Last Modified: Sat, 01 May 2021 07:13:41 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475c2ec11a2c27fca9e40ee49d0e3eff6179b202dfd129dbd1983b0d0190daa4`  
		Last Modified: Sat, 01 May 2021 07:13:42 GMT  
		Size: 3.9 MB (3920457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978fe06073ae7b42ab9a1e5da4b4b12f7c546a458c491008ee3dd48a3df25efb`  
		Last Modified: Sat, 01 May 2021 07:13:42 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee616b65b8bc2e4c94a9c18aa115a754d3d5f9d882651bc410de09e18b8d07b`  
		Last Modified: Sat, 01 May 2021 07:13:42 GMT  
		Size: 582.8 KB (582806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be7c2a12b8d7973076f32cfb95817188412322c36bd0f584187df322a9ab65d`  
		Last Modified: Sat, 01 May 2021 07:13:42 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0-fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:37a6de47cf6b7daf309c4f3c01c65814a6047edc67e1ed4069c29882f12eac31
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32611287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfc0fe17d5a4a91c650323f38dc9900f70d4cba8abb1be23add218b42310390`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:06:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 14 Apr 2021 19:06:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:06:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:06:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:23:06 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:58:28 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:58:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:58:29 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:58:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:58:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 03:02:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 03:02:38 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 01 May 2021 03:02:40 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 03:02:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 03:02:41 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 03:02:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 May 2021 03:02:43 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 May 2021 03:02:44 GMT
EXPOSE 9000
# Sat, 01 May 2021 03:02:44 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 05:17:09 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:17:10 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:17:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:17:53 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:17:54 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:17:54 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:17:55 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:17:56 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:17:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:17:57 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:17:58 GMT
USER adminer
# Sat, 01 May 2021 05:17:58 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b18d4d900c0b380efa64da748d0c37984ab724c0562146008bd0a83426bdf32`  
		Last Modified: Sat, 01 May 2021 03:23:42 GMT  
		Size: 10.4 MB (10360230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2b51626ff6ef4a34223c4702434966b98229831f9c66530be32ca820415023`  
		Last Modified: Sat, 01 May 2021 03:23:39 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b865e0a6889c0902c9c9a9c2532251cf3cb0ec10684bfced428e30ed7b5e31`  
		Last Modified: Sat, 01 May 2021 03:23:42 GMT  
		Size: 13.7 MB (13682636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5714ded1c7464453f58c2d56cd5f421e11279ff4c93260a83bac5d650209ac78`  
		Last Modified: Sat, 01 May 2021 03:23:40 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652b954cfcf9d2518ff31f7e4e148840c6d2c9e092061adef93c360036077073`  
		Last Modified: Sat, 01 May 2021 03:23:39 GMT  
		Size: 17.5 KB (17547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6835da2d9378e6d9f357627a1635841f878d84d98dd7a4ac573adf0350115f66`  
		Last Modified: Sat, 01 May 2021 03:23:40 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f286878d9ffd08b9406bd8a90c540439d3f13469d7718e4f3299d0203dad5741`  
		Last Modified: Sat, 01 May 2021 05:18:31 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c5a297c12725cfbb9204865f3624d699f7aeeef484e04c6aab1055336f45c7`  
		Last Modified: Sat, 01 May 2021 05:18:29 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67496f3d3bb2e7009814fbcbc8d05eff8a850133c52638dab840493f46139417`  
		Last Modified: Sat, 01 May 2021 05:18:30 GMT  
		Size: 3.6 MB (3588283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5f14dd8fdf5f2a7efcaabae07705db96f36ffc04ec4c9057e2e5e82aa2f403`  
		Last Modified: Sat, 01 May 2021 05:18:29 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c775b338acd3d66cd584bf6bb9fc2df1adcda0aee42be49a8f390d2ebac16e3d`  
		Last Modified: Sat, 01 May 2021 05:18:29 GMT  
		Size: 582.8 KB (582811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c433f73919fc4940a0f062f4bd12ced604d485430d8bf0a3a51448794accbe3f`  
		Last Modified: Sat, 01 May 2021 05:18:30 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:4.8.0-standalone`

```console
$ docker pull adminer@sha256:a3e73e13e4f3f1bd1007d7a5d75a6bd23846c3252b71ab7a5817de9ffec04826
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

### `adminer:4.8.0-standalone` - linux; amd64

```console
$ docker pull adminer@sha256:12d118ebf5a210b26b665b62af21041766a04d73fbbc63c1b116ad6dc0387b26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.6 MB (33647506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7707fd9b142f208f18d4e495601ad485b68f5dfdd2e4cb904d253f5974ff47dc`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:39:20 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 04:03:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 04:03:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 04:08:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 04:08:27 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 04:08:28 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 04:08:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 04:08:29 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 05:51:26 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:51:26 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 05:51:27 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:51:27 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 05:51:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:51:50 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:51:53 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:51:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:51:53 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:51:53 GMT
USER adminer
# Sat, 01 May 2021 05:51:53 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 05:51:54 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39378a44d29a4d45755bbbc75353969a68f030d8c0cec90ad7f9878f59ea3f5`  
		Last Modified: Sat, 01 May 2021 04:38:19 GMT  
		Size: 10.4 MB (10360243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417049c4f35584148dfd47d28edf662385807b7efa745d4f434ba03de07494b`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21742283d02f6f9451092c008c910a3909a41e37355848483d58e4dff63faffe`  
		Last Modified: Sat, 01 May 2021 04:38:26 GMT  
		Size: 14.3 MB (14256660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50815441106c8e704643e5f718299730f3cb96b03b9214c4f32385a7d2fef9f3`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a20d3bc0470221193d84e1e28160e63d41220d5efea36e336c064fdadbfc34`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 17.5 KB (17529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a75094b0a27256eb69095e9efefc4482cf91c15bd0c82b92934ec41abb83b19`  
		Last Modified: Sat, 01 May 2021 05:52:54 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4ac41937dc4363c09566855d60c909b65e892af0706e331ccceef9ff6033bc`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85ce354c2194e2f1001e52a8c9b13058f0b5b0911d87aa541c50c18fa9d883c`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 3.9 MB (3908144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b65d1b74856e3ed0629fc712e36cf1448d5796212d5b538e77f9e08e03cb77a`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828b20dbe6f1b761839e4e1d7eaa5cf689f716af52c6e1879c7b2cd798c822fb`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 582.8 KB (582804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7b7f0dab3313363e1281a6bfe913030c6c4168beda748d4350e16880480323`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0-standalone` - linux; arm variant v6

```console
$ docker pull adminer@sha256:16b56985dc271840e1e8164d283af7b63b6b0e96870a3f87c2ebb6e305cb7b1c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32131886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dbef13bdb0432e75de02942ac821772395bbc7e5042fd3b5cde516593dd3f3b`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:06:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:07:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:07:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:07:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:07:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:07:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:29:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:07:41 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:07:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:07:42 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:07:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:07:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:12:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:12:47 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:12:52 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:12:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:12:54 GMT
CMD ["php" "-a"]
# Fri, 30 Apr 2021 23:14:36 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Fri, 30 Apr 2021 23:14:36 GMT
STOPSIGNAL SIGINT
# Fri, 30 Apr 2021 23:14:39 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 30 Apr 2021 23:14:41 GMT
WORKDIR /var/www/html
# Fri, 30 Apr 2021 23:15:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Fri, 30 Apr 2021 23:15:38 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Fri, 30 Apr 2021 23:15:40 GMT
ENV ADMINER_VERSION=4.8.0
# Fri, 30 Apr 2021 23:15:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Fri, 30 Apr 2021 23:15:42 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Fri, 30 Apr 2021 23:15:46 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Fri, 30 Apr 2021 23:15:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 30 Apr 2021 23:15:47 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Fri, 30 Apr 2021 23:15:48 GMT
USER adminer
# Fri, 30 Apr 2021 23:15:49 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Fri, 30 Apr 2021 23:15:49 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726cd3e9e578579e631e21133870b656f3938f6a87797a842254b274d8b76e8`  
		Last Modified: Thu, 15 Apr 2021 02:33:02 GMT  
		Size: 1.7 MB (1690998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db188e87a6ea4fd0959949208b039a0d9facc96183df8dc346c6d0d3368b77e`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73dce0ed56811623cd40b786e95b951ce9d6341d9bfefded4f8aa12574283`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7272eaae063c5d7f7a55cddcfd266b2249c9c29941e2a74712e8ef4847e31dc`  
		Last Modified: Fri, 30 Apr 2021 22:39:32 GMT  
		Size: 10.4 MB (10360229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b3ded6063933c78570fc225ff275611490972800db3a316c9c2bc7846fd31c`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2454cd2b5598ce6dd8ff8f0a593ec04bc91fe623f385a270e5fcd23a9efe837f`  
		Last Modified: Fri, 30 Apr 2021 22:39:33 GMT  
		Size: 13.2 MB (13245293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c3b006179364603a89e8662502d244437ead12db6fd3367949fcc3e72ad3dc`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1974a1d957df5934ade9796f0fa21cad68c36cf7ddee2fd124e430a2f2e159c`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 17.6 KB (17551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163da5758d6703ae0d3c6ab673fc9c00e778461230ff5aff7163baffcd7f6361`  
		Last Modified: Fri, 30 Apr 2021 23:18:35 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73f8523f7b76c4f107a5fdde83c2eed8ef45b6f265432293af6d78b772149e7`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca9f9202fb99ea8d097d90a5bb62979fbc35544da64a8a677da4b8bbf420f96`  
		Last Modified: Fri, 30 Apr 2021 23:18:35 GMT  
		Size: 3.6 MB (3604909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebdcc1e39d88d3548486b0b94fd4925deda0fd89552ec953ec45103639056e3`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634b5387043b43b3105ba37b43d31e1bf5a1ad5c5a63ee766b5c6aa198d6a2f`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 582.8 KB (582802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b737b034949aeddb4bd174c7f33742314e10f2db3cbe879b3507c0f2b2faf7`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0-standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:f1cd758c5bcbe78188b5766221c37d6041a5c8d727af64e9a49b277e09e80ce1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30938697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99e81544e5622446ab0920052f90534d15fe52866ccfddc0d883edcada095a7f`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:08:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:08:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:08:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:08:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:08:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:08:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:35:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:09:59 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:10:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:10:02 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:10:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:10:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:13:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:13:14 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 02:13:17 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:13:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:13:19 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 03:51:49 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 03:51:50 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 03:51:54 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 03:51:55 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 03:52:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 03:52:48 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 03:52:49 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 03:52:50 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 03:52:51 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 03:52:57 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 03:52:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 03:52:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 03:53:02 GMT
USER adminer
# Sat, 01 May 2021 03:53:05 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 03:53:07 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc6d3f07b2e440bf9a8e52a0a5bba0f27637990ee4976424cef6aae97e169f`  
		Last Modified: Thu, 15 Apr 2021 03:38:53 GMT  
		Size: 1.6 MB (1559061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9000ca9dcd92a2066a3a2c4031e677c3998cd82a3ecbc68468d11255ecbdb62`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d102949f174ecad1044574e45dded8368eb7451bf66b3bdac6e367c7f415d3`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5dab41947ddc5db66501a8111f7ef729f521e11ca3ad87ecf37bd79eac6ef3`  
		Last Modified: Sat, 01 May 2021 02:35:25 GMT  
		Size: 10.4 MB (10360231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2700665f109862388a4e0ed21b2fd335c4d89050efbad76af079999dfd9a4b68`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7aabe4a04c27ab686de62e8f214ca07e6d03fe93c6d40ade09bced2eab56901`  
		Last Modified: Sat, 01 May 2021 02:35:28 GMT  
		Size: 12.4 MB (12407150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebda42f2c319f9f89154be7b8165960eccb3900eb3f5b9e2857420d88f5ca575`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f9f67e3447fb75cf1724c1d4b7d53b8b1de00a8ec05d4aba9f7d8c09a9035`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 17.5 KB (17540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677aab5c428da05844e96dc166beb86af6dc68f33a93546bbbefed7d3839112c`  
		Last Modified: Sat, 01 May 2021 03:55:43 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2789eb966365d0da44c2eb6fce9e8d6b0b0b0640c29214cc9a6407267f9b4`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da46a02e36d762092675c2d38e18ca37e2e0163b58bf248c621b0a9dc8866d8e`  
		Last Modified: Sat, 01 May 2021 03:55:43 GMT  
		Size: 3.6 MB (3579788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841c453f4c80b715d2c60cdeb21facc849ad7ea141aef125bcdfff3fc87ea2e6`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 1.5 KB (1472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052526ae6f5bb73b64438863414d320716ac83cd7542b7db8216dba070bc9f72`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cde09e1b359229258d6f040ec2f23d5b10a5b6b50cc84580a40aaf5fa55556`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0-standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:2995c05337d98dd62225e6d58c6c551940eb5d2314ee022551a359c2edfdbb95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33288719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e49d6a5068aff4b8f7d53e5ca53084149e52a21716008685d3634f152a93cc82`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:27:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:28:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:28:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:28:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:28:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:53:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 01:51:16 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 01:51:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 01:51:18 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 01:51:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 01:51:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 01:55:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 01:55:39 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 01:55:43 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 01:55:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 01:55:46 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 04:07:49 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 04:07:50 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 04:07:54 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 04:07:55 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 04:08:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 04:08:56 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 04:08:57 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 04:08:58 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 04:08:59 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 04:09:03 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 04:09:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 04:09:05 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 04:09:06 GMT
USER adminer
# Sat, 01 May 2021 04:09:07 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 04:09:08 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea792edc0a65854bc13c90079b9e33a399c351b73e194d9df4f2cf5a0efeb2`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 1.7 MB (1700262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31bbfcb500579a0c450809a6b082c564c3ce4873732c1b62d8dab52ed0a11ac`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22841fe152c1fe4ec2048ebca3b9c0db9d29773b0d0670167a848d87fcfe83f3`  
		Last Modified: Thu, 15 Apr 2021 01:59:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86a2990f157991d12ee804183f42ab624a7af15605920e9c12adce886783bd9`  
		Last Modified: Sat, 01 May 2021 02:24:37 GMT  
		Size: 10.4 MB (10360252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717c7ad0a34fca1bd9fe22eb98d3abc226862c3a4875c05fec802e7c66425afe`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec40f0928e2ca1518729b1c63da742a00d1df98e4861f80d6e8f4019fbde9f26`  
		Last Modified: Sat, 01 May 2021 02:24:40 GMT  
		Size: 14.0 MB (14028751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d802fc3cc61952c8e0f43df7f44975e487e3d138bacfdc9c2daeca67d47cd976`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f89f4b8ccd74e3d8337940607bb14e9230a6ca849950ded149286a4b79e268a`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9208e6df146eb023a8d9b5260435c9cbd6f67b60dfb46766c5841339f85f8ec0`  
		Last Modified: Sat, 01 May 2021 04:11:07 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b108d0b6a7ff2b8cf63b53bbe86fd0454a91008e3714557e80df86a09cda0abf`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273c8a35b22772c8535453bfe942ed895b853bfabedfce587de72643c2ca6aaa`  
		Last Modified: Sat, 01 May 2021 04:11:07 GMT  
		Size: 3.9 MB (3879098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df87fa0c04f21673d85d974891030708b890f98615a245ac79d220ecf1378f7`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb52da6ce3c536b5587683997df91e97198a9ed221fd6df0b6b7d49f57717d3`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 582.8 KB (582804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4830f1e50425a8f4fc4e1236b44d93d5b39a716f837b8d921c8afb2fd5be92e`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0-standalone` - linux; 386

```console
$ docker pull adminer@sha256:19d6d656da0acd11da3961bef1d4d85e7a41e7467f127e7989d0db6f8a342a95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34231434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcfa500fd2970be787667cf0eae0f3db72409b63b7d985f6402ec9b2667b013a`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 04:15:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:24:22 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:24:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:24:23 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:24:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:24:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:33:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:33:53 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:33:56 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:33:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:33:58 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 00:17:31 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 00:17:31 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 00:17:33 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 00:17:34 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 00:18:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 00:18:54 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 00:18:54 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 00:18:55 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 00:18:55 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 00:18:58 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 00:18:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 00:18:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 00:18:59 GMT
USER adminer
# Sat, 01 May 2021 00:18:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 00:19:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f032c69e4d0122e069320b9680ef26b8bb3c430278739a6fea12af3a4f96e134`  
		Last Modified: Fri, 30 Apr 2021 23:40:49 GMT  
		Size: 10.4 MB (10360220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c9984d072093737e593d0ef515c92f288b39d14aabf7a7d51b86898bc1aef7`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5e9496813676c2e99e74df895938ef33a8cf138c5a38a3e73968cc1b2fa932`  
		Last Modified: Fri, 30 Apr 2021 23:40:54 GMT  
		Size: 14.6 MB (14632431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d376f079b3a59dc3fc16b3017ea542c2ea92a6de4dcdb3aa927c19364e1df5`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df9b26593ad898c78d3de9232c23626d904c18e6b24f18767a144a5536e73e1`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 17.5 KB (17541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40300d5ae7ee86745631c5498bfc7757e4ac4bf3eacda6a10991b2a38dbcecf7`  
		Last Modified: Sat, 01 May 2021 00:21:38 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e1a92ccdfda888c1542ec341a96c423af53a5f232f654b95e5436b7256fd7b`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e200018a310c11b06c52afa2eb578aed71d2fcff109735fac4a4224a2d99198`  
		Last Modified: Sat, 01 May 2021 00:21:36 GMT  
		Size: 4.0 MB (4012274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5d7bd779781644a969c9a0c3214e5b34c562367de371486d6d908161ee3bee`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69a63a5467a891b0c71e5954c34e2275c605b8fddd9bc7856ec4442ae2a1c0d`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 582.8 KB (582810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3637c8ae22706fe31d88cd4487ddc444d18f7b005442b713e7594c150a8aa5e8`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0-standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:dbb3b10c00dc1f3ece08df27b44d79f66f959aedc9d4680e63052716fda1881e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34733557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea9e143138a6e56e3f5db1c7fd10a20e080c0b8a996439d5b1e154c009c52c5`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:16:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:46:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 03:42:52 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 03:42:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 03:43:08 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 03:43:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 03:43:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 03:48:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 03:48:36 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 03:48:53 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 03:49:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 03:49:13 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 07:05:31 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 07:05:43 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 07:06:08 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 07:06:19 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 07:07:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 07:07:46 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 07:07:56 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 07:08:03 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 07:08:22 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 07:08:57 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 07:09:05 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 07:09:11 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 07:09:22 GMT
USER adminer
# Sat, 01 May 2021 07:09:31 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 07:09:38 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d82dc7c3129f9f8efe068b46b7988252e5911a9bf70f2f3ec970ed7382d8f92`  
		Last Modified: Sat, 01 May 2021 04:28:17 GMT  
		Size: 10.4 MB (10360240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f5852448efedd86253d2f693d58031fd8707b7fd4983e4b0453351d357f118`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89a34f310b9721f0ab0de62088a7d630d699d7cf59fbb7957542afbc7659f3`  
		Last Modified: Sat, 01 May 2021 04:28:19 GMT  
		Size: 15.3 MB (15282748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a34edc1036d80f0acbe7cd46a9c1bad8d141654a25252318a3457a14311dfe`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587df26cc194e45cf1f6e3bd6b2e3f0bfae286ca1ae26b98b457b556d7427303`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 17.6 KB (17562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a4991a1eff14856b0308c117ac5c87d74aac4a2c00dfc3fc38e69846bdca8e`  
		Last Modified: Sat, 01 May 2021 07:13:15 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbfbca1bede0192cfb0c862f0077baa98e4dbcd683d0682b3c04a4467ec3f67`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e078202145e09994bf4c091f95f65084e2d380b192e68fa3055f4c8da3c0f1a`  
		Last Modified: Sat, 01 May 2021 07:13:14 GMT  
		Size: 3.9 MB (3920436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a08531336bb96df3ee7311a11f8c8f5f78b27fd27f2e1e8cebe3aaebefc0cf6`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4129c43164fd79c0ea01d2c1d993a469846ebb51d831de0d08dc6fe5390ca1d`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 582.8 KB (582809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea793cb13300c9b023cc7deccce5ce057f8611b196da7f5747c42494fa1aa1f5`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:4.8.0-standalone` - linux; s390x

```console
$ docker pull adminer@sha256:be29af6c13419aaaf011ebb117d07f34d74dfd3d51a4657fb92ec7e8a5a3e992
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32536231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e3b6e5f32c6c450164b419f6108097b7765a448b2965197e82c4a7be358dc10`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:18:59 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:54:37 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:54:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:54:38 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:54:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:54:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:58:16 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 02:58:18 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:58:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:58:18 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 05:16:12 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:16:12 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 05:16:14 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:16:15 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 05:16:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:16:55 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:16:58 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:16:59 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:16:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:17:00 GMT
USER adminer
# Sat, 01 May 2021 05:17:00 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 05:17:01 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b7aa20ee47cf4d85a8a033023b14b1948153a005c710022465266b1676ff00`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 10.4 MB (10360232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c09e3c51bdc12e3dac46e704947a4207380cc86861118e2ba93827f09a479b`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c57065802a25a7373daa5d63b66c55320e705d6ef8e47055d2ba2997ac4ac1f`  
		Last Modified: Sat, 01 May 2021 03:23:19 GMT  
		Size: 13.6 MB (13616029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa2ed8a45355ef77a61d2740ffedf281c9079db17e02fcd213477f4c8bd2f4`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d549711db456f1993f2dd16932c69755412329900032bc3250bfff994fd9d43`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa60d82d0a8b59fda860a56dae19ab654de0f1368014f447b7f9c53d96c5584`  
		Last Modified: Sat, 01 May 2021 05:18:16 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d3ea1b608b879ac7c8354ab621b511601a964e24706c82764e975896ec2d4`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1128a53bb989ba9202c67883e70c3aa25bfbc7a44e36360de37f23e678dab0`  
		Last Modified: Sat, 01 May 2021 05:18:15 GMT  
		Size: 3.6 MB (3588293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6ac88d341f35d6278d87a43b3998caa46d2a2d7515df5446755a418c22fb4f`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 1.5 KB (1474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46932d8f58943aa96cffad8c4b13a779eb592deacb98d058e46236c40479d28`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32bae7fbe947016896c76b4d5aea4dbb1dd2feb86f7062de658448beb0f326a`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:fastcgi`

```console
$ docker pull adminer@sha256:cfe2c1bc146279d78623f5af2f516740b209ade304d736bac5412a5125a3b44a
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

### `adminer:fastcgi` - linux; amd64

```console
$ docker pull adminer@sha256:bb85a1cd6d92b3ea47ec7f571c8818ef52cda3f87d39c19dd29b9c47b3975bd1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33722644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35f1d5ea625ff4a1425ff14ce42137483342a8fda023b21d49bde2e7bcb9c429`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:08:32 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 00:08:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:08:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:08:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:50:04 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 04:08:45 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 04:08:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 04:08:45 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 04:08:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 04:08:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 04:13:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 04:13:42 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 01 May 2021 04:13:43 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 04:13:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 04:13:44 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 04:13:45 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 May 2021 04:13:45 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 May 2021 04:13:45 GMT
EXPOSE 9000
# Sat, 01 May 2021 04:13:45 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 05:52:02 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:52:03 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:52:26 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:52:26 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:52:26 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:52:26 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:52:26 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:52:28 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:52:28 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:52:28 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:52:28 GMT
USER adminer
# Sat, 01 May 2021 05:52:29 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587aa49073cc5bc626d9fa9b5db597ee0494aaabf607c40d47e86b173c352d79`  
		Last Modified: Sat, 01 May 2021 04:39:11 GMT  
		Size: 10.4 MB (10360247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1edad11da1d8c5f96cb5180aafd60278895778d981d0858d1f9e8ae7f24e11ef`  
		Last Modified: Sat, 01 May 2021 04:39:07 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9160174d0ea73d3c2daffba80a6bc8fc007e25d4c53af8d79a0e3332ff64d4`  
		Last Modified: Sat, 01 May 2021 04:39:10 GMT  
		Size: 14.3 MB (14323327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:588936efd0d0c4bf919d61f6b295adaff847bf6dbb177623e3be3f8ccaa80b7f`  
		Last Modified: Sat, 01 May 2021 04:39:07 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b469d4db80f6beee3277841548290c07a1cd623de057c1696c80f3ea7e25ac8d`  
		Last Modified: Sat, 01 May 2021 04:39:07 GMT  
		Size: 17.5 KB (17536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac3f8b0d122db4cd151c5c8705b9a837b7d07b59767b58b66ac8616fb1994a4`  
		Last Modified: Sat, 01 May 2021 04:39:07 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d6cfa9c78d4431301157113d599e7bfeb7d855f0b61af91a636cc10c643ba4`  
		Last Modified: Sat, 01 May 2021 05:53:22 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb776c1598fd8aa829f31f030b9c4fd717a6d114722e4ac3795df7de20c696eb`  
		Last Modified: Sat, 01 May 2021 05:53:19 GMT  
		Size: 1.4 KB (1404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0f83a3812371d1b1cf2b689b6c5aa4a3640fc411b48b54e0556bb6cb359763e`  
		Last Modified: Sat, 01 May 2021 05:53:20 GMT  
		Size: 3.9 MB (3908157 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25b28ebf88514becd53fe7f6e9c186269f708e0a2195c3f0cc241537c1892c36`  
		Last Modified: Sat, 01 May 2021 05:53:19 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70abec07bbc3849eaa135a1e7713d13da566d86471dc5897d07f5e7e7ccbefac`  
		Last Modified: Sat, 01 May 2021 05:53:19 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4ae34fdb3b204f750ec26b75040af24cf16b32a6acc688cf3671c2dda0d8325`  
		Last Modified: Sat, 01 May 2021 05:53:19 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v6

```console
$ docker pull adminer@sha256:e7ec089a434466e6ff6988df7d109293e8bea1eaa3a677ecdb3c4f9c20881b58
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32209577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68e7a7c7afa79f110ddb25704d600a79bfe3df1e7267666840f9cf475324c9e7`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:06:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:07:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:07:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:07:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:07:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:13:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 01:13:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:13:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:13:37 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:34:04 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:13:04 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:13:05 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:13:06 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:13:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:13:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:16:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:16:30 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:16:33 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:16:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:16:35 GMT
WORKDIR /var/www/html
# Fri, 30 Apr 2021 22:16:38 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 30 Apr 2021 22:16:39 GMT
STOPSIGNAL SIGQUIT
# Fri, 30 Apr 2021 22:16:39 GMT
EXPOSE 9000
# Fri, 30 Apr 2021 22:16:40 GMT
CMD ["php-fpm"]
# Fri, 30 Apr 2021 23:16:09 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Fri, 30 Apr 2021 23:16:12 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 30 Apr 2021 23:17:09 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Fri, 30 Apr 2021 23:17:11 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Fri, 30 Apr 2021 23:17:13 GMT
ENV ADMINER_VERSION=4.8.0
# Fri, 30 Apr 2021 23:17:16 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Fri, 30 Apr 2021 23:17:18 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Fri, 30 Apr 2021 23:17:26 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Fri, 30 Apr 2021 23:17:33 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 30 Apr 2021 23:17:39 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Fri, 30 Apr 2021 23:17:44 GMT
USER adminer
# Fri, 30 Apr 2021 23:17:53 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726cd3e9e578579e631e21133870b656f3938f6a87797a842254b274d8b76e8`  
		Last Modified: Thu, 15 Apr 2021 02:33:02 GMT  
		Size: 1.7 MB (1690998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db188e87a6ea4fd0959949208b039a0d9facc96183df8dc346c6d0d3368b77e`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73dce0ed56811623cd40b786e95b951ce9d6341d9bfefded4f8aa12574283`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:326d5d407c34c562acf233ba0465a9ca076c4995ea374f4935ee9a50de14304a`  
		Last Modified: Fri, 30 Apr 2021 22:40:09 GMT  
		Size: 10.4 MB (10360233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4dbf5ff406dc346ecb05d404dc4cf123d1baed0540ad1fd2ba6dd768aacc0a4`  
		Last Modified: Fri, 30 Apr 2021 22:40:05 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:245d552a4da6d15321f0d2b4018fbc871b3d1b71a961f1fbe4cd4f0a987d9f6a`  
		Last Modified: Fri, 30 Apr 2021 22:40:12 GMT  
		Size: 13.3 MB (13314549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aa562b1287875972988fafb6ff0daf10a74db6645e30e73c5454dec085afac5`  
		Last Modified: Fri, 30 Apr 2021 22:40:05 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db31be4473204baf475d4f61f078539da6aa94516bdbf657220a83f11ee4398b`  
		Last Modified: Fri, 30 Apr 2021 22:40:05 GMT  
		Size: 17.5 KB (17544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8cb05aabc72b85e6abe53738ccffde33589c881cb0fa7f48491cc4ed2727590e`  
		Last Modified: Fri, 30 Apr 2021 22:40:05 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b621752cb9db17f7a3c88e8c9740607ac521657f6b04da8c78f1c7d39a9b4717`  
		Last Modified: Fri, 30 Apr 2021 23:18:56 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cb194faf95e5814784905c60640a5a3896728c32016fc639e739f69e9712ef5`  
		Last Modified: Fri, 30 Apr 2021 23:18:54 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4be1dacf810d372eadb5ced9f960535843b764651e0811627b788a8464fd2563`  
		Last Modified: Fri, 30 Apr 2021 23:18:55 GMT  
		Size: 3.6 MB (3604906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:adfc52d55996257921b21a1ad3526d2ef315ab03a1952a730d578fb08d9dd00f`  
		Last Modified: Fri, 30 Apr 2021 23:18:54 GMT  
		Size: 1.5 KB (1474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e704e7b03cf4efc6a7d79dc1c2cf6ab9cae0e9b1cf155ab25526600202c304ac`  
		Last Modified: Fri, 30 Apr 2021 23:18:54 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5357d24cb511a94dc36a682ffe261d6997ea85814130bbd95f17d62662abbb40`  
		Last Modified: Fri, 30 Apr 2021 23:18:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm variant v7

```console
$ docker pull adminer@sha256:3c3debd1bc71b455e1d828fb1f612c8841e46a45a49ad0b873f90e303e1c3294
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.0 MB (31013421 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3afc0fd4429ee14929b3d58c7d8dd88d25fa11c07ed4a57544d80b6b462c170c`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:08:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:08:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:08:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:08:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:08:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:16:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 02:16:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:16:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:16:30 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:39:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:13:34 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:13:35 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:13:36 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:13:42 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:13:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:16:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:16:50 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 01 May 2021 02:16:53 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:16:54 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:16:55 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 02:16:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 May 2021 02:16:57 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 May 2021 02:16:58 GMT
EXPOSE 9000
# Sat, 01 May 2021 02:16:59 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 03:53:31 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 03:53:38 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 03:54:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 03:54:47 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 03:54:49 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 03:54:51 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 03:54:54 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 03:55:07 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 03:55:09 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 03:55:10 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 03:55:16 GMT
USER adminer
# Sat, 01 May 2021 03:55:17 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc6d3f07b2e440bf9a8e52a0a5bba0f27637990ee4976424cef6aae97e169f`  
		Last Modified: Thu, 15 Apr 2021 03:38:53 GMT  
		Size: 1.6 MB (1559061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9000ca9dcd92a2066a3a2c4031e677c3998cd82a3ecbc68468d11255ecbdb62`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d102949f174ecad1044574e45dded8368eb7451bf66b3bdac6e367c7f415d3`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a887d4c3f8fab0b8a41f2e15f80000594b1db228b9a1d1068315132400a18dee`  
		Last Modified: Sat, 01 May 2021 02:35:58 GMT  
		Size: 10.4 MB (10360228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8e0919fd704aa13a8b60f3a3d1e2beb99969ca0340f005b60c5ba8972a863b7`  
		Last Modified: Sat, 01 May 2021 02:35:54 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:285eb6e1ce27fc069915bbd5b8f5b0a25a164b9c730ceea9b5d31fc4b366e173`  
		Last Modified: Sat, 01 May 2021 02:35:58 GMT  
		Size: 12.5 MB (12473434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3fe9e780825250d91c98ce931c8c5b40b0840a3be7271c0da68cb91a2c363b4`  
		Last Modified: Sat, 01 May 2021 02:35:54 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8242f69b6d1406a05b5c09d0558be9cd86b94bc543392550e695d7918d12253f`  
		Last Modified: Sat, 01 May 2021 02:35:54 GMT  
		Size: 17.5 KB (17541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7df415ac941092e1076f45c06471de55333fcf15a6d6b62be12fca1d54aed65`  
		Last Modified: Sat, 01 May 2021 02:35:54 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08419d195bbd19dbc53bcfe26f58d991296299dc73e4e2f3366d05e064a172dd`  
		Last Modified: Sat, 01 May 2021 03:56:01 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:547f32cf92bcb6638a56acb652022d7e025980febbd89a6da7cc430b0f80d7d5`  
		Last Modified: Sat, 01 May 2021 03:55:59 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16180895a27991a5eb67173e12509076698a8f69cacbec4bf312cd6cf98b9c6f`  
		Last Modified: Sat, 01 May 2021 03:56:00 GMT  
		Size: 3.6 MB (3579791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241656f2ebfb873a2577639b2a666b7477a81bf98d78befedb3fade16e603dd6`  
		Last Modified: Sat, 01 May 2021 03:55:59 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da4900892195d60e34c3e22c18d49ae7579a878b90638cab2b95b42d09f8c63`  
		Last Modified: Sat, 01 May 2021 03:55:59 GMT  
		Size: 582.8 KB (582802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47e71054e8d8f0c9daf0a9ac9d0a7d9f0dd1dfea2c96c39e188d5c45909cee55`  
		Last Modified: Sat, 01 May 2021 03:55:59 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:5bdcde869d50b9c00ab27beb39d281ad22bed1f5ec63798d5987ec3f22a0e714
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.4 MB (33365959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41e197d619b95eba3b7f74b12406fe8d9f7736033704a608fc6fd23c59eb45c9`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:27:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:28:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:28:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:28:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:35:04 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 00:35:06 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:35:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:35:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:59:03 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 01:55:56 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 01:55:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 01:55:58 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 01:56:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 01:56:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:00:27 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:00:30 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 01 May 2021 02:00:36 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:00:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:00:39 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 02:00:42 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 May 2021 02:00:43 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 May 2021 02:00:44 GMT
EXPOSE 9000
# Sat, 01 May 2021 02:00:45 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 04:09:26 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 04:09:30 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 04:10:29 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 04:10:32 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 04:10:32 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 04:10:34 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 04:10:36 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 04:10:39 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 04:10:40 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 04:10:41 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 04:10:42 GMT
USER adminer
# Sat, 01 May 2021 04:10:43 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea792edc0a65854bc13c90079b9e33a399c351b73e194d9df4f2cf5a0efeb2`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 1.7 MB (1700262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31bbfcb500579a0c450809a6b082c564c3ce4873732c1b62d8dab52ed0a11ac`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22841fe152c1fe4ec2048ebca3b9c0db9d29773b0d0670167a848d87fcfe83f3`  
		Last Modified: Thu, 15 Apr 2021 01:59:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5f8d535e8cad7ccb6f9170d7f17ed57c87e17bf74a6a9b889ee0c5d6f7a1ea0`  
		Last Modified: Sat, 01 May 2021 02:25:10 GMT  
		Size: 10.4 MB (10360253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1179292319d52c55b46cc86f4fa096f9eedb627658fb3128a302aaabeb59e9ac`  
		Last Modified: Sat, 01 May 2021 02:25:07 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:599e8f6926f90333ec21d01591e3d561257958f646ff18d4378f3e221e855d44`  
		Last Modified: Sat, 01 May 2021 02:25:12 GMT  
		Size: 14.1 MB (14097538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98f02f5190a9daeedd8a8c4a41aaf6272b146159c0558fbd85fdc58314469fa`  
		Last Modified: Sat, 01 May 2021 02:25:07 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70e04d4e8e1659348f3dc256da300f9af8dd465317b5d4942e1c2f21bea7de34`  
		Last Modified: Sat, 01 May 2021 02:25:07 GMT  
		Size: 17.6 KB (17552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5aa6a64b7ec15a2645b5a6ea3a024de9f48b106bfbf5f750258505a213fe9839`  
		Last Modified: Sat, 01 May 2021 02:25:07 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb774aca288aac911b70975bfc2ffeb5316320c6f4fe13e7f6f19a2f3f5f36a`  
		Last Modified: Sat, 01 May 2021 04:11:26 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc7cc42da3fb11d474881ed09adfe71ae03b2f6c2bbc3acbbd1b02c4a6529ee2`  
		Last Modified: Sat, 01 May 2021 04:11:25 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb23dde682fc45d4ad40ae4e219fd928a6e22e7c5d8c2761b45b9d1967c1969`  
		Last Modified: Sat, 01 May 2021 04:11:25 GMT  
		Size: 3.9 MB (3879097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc216bf5d605cb3e2f408d6377ef069a318da1a977f494b0e160853d2260413`  
		Last Modified: Sat, 01 May 2021 04:11:25 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9704d03344ddee4c9f158745ce184c23e8a21070c215ef5aa391af1f0d4b8b37`  
		Last Modified: Sat, 01 May 2021 04:11:25 GMT  
		Size: 582.8 KB (582799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645e8857d1e4befaa7629398c8b40cdf458341fc6ec1d9eeed6500ec44fd95fc`  
		Last Modified: Sat, 01 May 2021 04:11:24 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; 386

```console
$ docker pull adminer@sha256:d74304e9ccb1c9a94feceab9fe4fc5a2b314a0279e5144bedf39b69b2d1fb252
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34313904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c714a94da17e01e0a403f19139167a764ce92e01f46e26555b63db0bf988e2d5`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:45:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 15 Apr 2021 03:45:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:45:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:45:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 04:23:18 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:34:17 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:34:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:34:18 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:34:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:34:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:47:30 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:47:32 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:47:35 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:47:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:47:36 GMT
WORKDIR /var/www/html
# Fri, 30 Apr 2021 22:47:38 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 30 Apr 2021 22:47:38 GMT
STOPSIGNAL SIGQUIT
# Fri, 30 Apr 2021 22:47:39 GMT
EXPOSE 9000
# Fri, 30 Apr 2021 22:47:39 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 00:19:14 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 00:19:16 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 00:20:34 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 00:20:34 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 00:20:35 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 00:20:35 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 00:20:36 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 00:20:39 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 00:20:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 00:20:39 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 00:20:40 GMT
USER adminer
# Sat, 01 May 2021 00:20:40 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0588acad61f86a7af9aa7d5fb5aa2b86975cc43ff9ed779a12e1f5bc055cc13d`  
		Last Modified: Fri, 30 Apr 2021 23:42:01 GMT  
		Size: 10.4 MB (10360228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9da74d5ef034b8e3d1c1843ff0f1fb32729355a09cdd37d2bb85ac0f9c84132`  
		Last Modified: Fri, 30 Apr 2021 23:41:56 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96e70ffc5cc286556f65655c714c9e36bab6e3b905642fec24ea7004f7810023`  
		Last Modified: Fri, 30 Apr 2021 23:42:03 GMT  
		Size: 14.7 MB (14706461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319f59bb7b102d3532483b7815c4fd4d1a6341eb830a003ce3f5939f0735c34b`  
		Last Modified: Fri, 30 Apr 2021 23:41:56 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84cc3ec3ce916d4202109b5982a0edf7f286de88ae1d7f509478b88f670b386f`  
		Last Modified: Fri, 30 Apr 2021 23:41:56 GMT  
		Size: 17.5 KB (17534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:768af260a05ac95876aedc485d9ca861bddfc8bdeaeb068ef75c470344c0cd32`  
		Last Modified: Fri, 30 Apr 2021 23:41:57 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92cbd27b9cc3599d28a895b6058ea82cef72905afaf0386353e458dfc656db66`  
		Last Modified: Sat, 01 May 2021 00:22:18 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:339416d12f4664d3a58d59d73f746f6bfce7b9f5c1e785a4e57c2fe22c6fd030`  
		Last Modified: Sat, 01 May 2021 00:22:15 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94963c2504ced8e6b9acea28bbb4631103f18e02c9bb19b69cf856cb55b03c33`  
		Last Modified: Sat, 01 May 2021 00:22:16 GMT  
		Size: 4.0 MB (4012274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ed1d23c56aa78752221c9bb10a79ea56488d9a5761eafeaf1de7fbe5bf1843`  
		Last Modified: Sat, 01 May 2021 00:22:15 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02f38dd8765af05bb660549a816d1668249fad78c5c130c5621c9f4372ad8dc7`  
		Last Modified: Sat, 01 May 2021 00:22:15 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e0092d5b2329fcb1ab536ec27da58c7f4dc463cd60ed2549af3b5d324d95e57`  
		Last Modified: Sat, 01 May 2021 00:22:15 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; ppc64le

```console
$ docker pull adminer@sha256:c9b9eb9d5f0ed98f1ef38090d1f43c75ef5aa7dc0f8f38177997929c1985fc06
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34818570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3edf620a1c345fc880bc58c5a4b925e3db5e6b2c5ea1de288f6a55c880bb08b5`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:24:29 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 14 Apr 2021 20:24:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:24:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:24:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:52:31 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 03:49:49 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 03:50:02 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 03:50:09 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 03:50:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 03:50:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 03:55:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 03:56:03 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 01 May 2021 03:56:22 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 03:56:33 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 03:56:37 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 03:56:58 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 May 2021 03:57:01 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 May 2021 03:57:05 GMT
EXPOSE 9000
# Sat, 01 May 2021 03:57:11 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 07:10:09 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 07:10:25 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 07:11:42 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 07:11:51 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 07:12:03 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 07:12:14 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 07:12:21 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 07:12:37 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 07:12:39 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 07:12:42 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 07:12:47 GMT
USER adminer
# Sat, 01 May 2021 07:12:49 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a25b688370820b31acaf43fe6aad086a49129e7f4cd65fe66400802f6ff46dc`  
		Last Modified: Sat, 01 May 2021 04:29:07 GMT  
		Size: 10.4 MB (10360238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87a19c6448c2799fe4c148db7f3ff08fdd52be33aef25d7c62e5221f55ad41e9`  
		Last Modified: Sat, 01 May 2021 04:28:55 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bfb1afb48a1979b4b32e84e66970768c28e3dc95e39a00636047349d2cab46e`  
		Last Modified: Sat, 01 May 2021 04:28:58 GMT  
		Size: 15.4 MB (15359291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e72318803e295efc133889dde8281f0732d6579873ca2b88745cc3bad1e1edf0`  
		Last Modified: Sat, 01 May 2021 04:28:55 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1938d024d250ee9fd0ab42de3b74cfa6a509927a3d2bd7048e641c436827170a`  
		Last Modified: Sat, 01 May 2021 04:28:55 GMT  
		Size: 17.6 KB (17564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82d534f17e924b8e0071bef66f86c1f585f78114defb32745c3bd09d1c171d72`  
		Last Modified: Sat, 01 May 2021 04:28:55 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afaad7c43a999235106d692ee7f57f72669564f26e13cbe066930abb3593cbef`  
		Last Modified: Sat, 01 May 2021 07:13:45 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee73d8b50916c3f6360690a67b457bb80dd0274af5a974e9162d23b7ab46440`  
		Last Modified: Sat, 01 May 2021 07:13:41 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:475c2ec11a2c27fca9e40ee49d0e3eff6179b202dfd129dbd1983b0d0190daa4`  
		Last Modified: Sat, 01 May 2021 07:13:42 GMT  
		Size: 3.9 MB (3920457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:978fe06073ae7b42ab9a1e5da4b4b12f7c546a458c491008ee3dd48a3df25efb`  
		Last Modified: Sat, 01 May 2021 07:13:42 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ee616b65b8bc2e4c94a9c18aa115a754d3d5f9d882651bc410de09e18b8d07b`  
		Last Modified: Sat, 01 May 2021 07:13:42 GMT  
		Size: 582.8 KB (582806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9be7c2a12b8d7973076f32cfb95817188412322c36bd0f584187df322a9ab65d`  
		Last Modified: Sat, 01 May 2021 07:13:42 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:fastcgi` - linux; s390x

```console
$ docker pull adminer@sha256:37a6de47cf6b7daf309c4f3c01c65814a6047edc67e1ed4069c29882f12eac31
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32611287 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dbfc0fe17d5a4a91c650323f38dc9900f70d4cba8abb1be23add218b42310390`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:06:46 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 14 Apr 2021 19:06:46 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:06:47 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:06:47 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:23:06 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:58:28 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:58:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:58:29 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:58:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:58:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 03:02:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 03:02:38 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Sat, 01 May 2021 03:02:40 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 03:02:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 03:02:41 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 03:02:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 01 May 2021 03:02:43 GMT
STOPSIGNAL SIGQUIT
# Sat, 01 May 2021 03:02:44 GMT
EXPOSE 9000
# Sat, 01 May 2021 03:02:44 GMT
CMD ["php-fpm"]
# Sat, 01 May 2021 05:17:09 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:17:10 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:17:52 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:17:53 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:17:54 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:17:54 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:17:55 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:17:56 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:17:57 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:17:57 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:17:58 GMT
USER adminer
# Sat, 01 May 2021 05:17:58 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b18d4d900c0b380efa64da748d0c37984ab724c0562146008bd0a83426bdf32`  
		Last Modified: Sat, 01 May 2021 03:23:42 GMT  
		Size: 10.4 MB (10360230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d2b51626ff6ef4a34223c4702434966b98229831f9c66530be32ca820415023`  
		Last Modified: Sat, 01 May 2021 03:23:39 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80b865e0a6889c0902c9c9a9c2532251cf3cb0ec10684bfced428e30ed7b5e31`  
		Last Modified: Sat, 01 May 2021 03:23:42 GMT  
		Size: 13.7 MB (13682636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5714ded1c7464453f58c2d56cd5f421e11279ff4c93260a83bac5d650209ac78`  
		Last Modified: Sat, 01 May 2021 03:23:40 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:652b954cfcf9d2518ff31f7e4e148840c6d2c9e092061adef93c360036077073`  
		Last Modified: Sat, 01 May 2021 03:23:39 GMT  
		Size: 17.5 KB (17547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6835da2d9378e6d9f357627a1635841f878d84d98dd7a4ac573adf0350115f66`  
		Last Modified: Sat, 01 May 2021 03:23:40 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f286878d9ffd08b9406bd8a90c540439d3f13469d7718e4f3299d0203dad5741`  
		Last Modified: Sat, 01 May 2021 05:18:31 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43c5a297c12725cfbb9204865f3624d699f7aeeef484e04c6aab1055336f45c7`  
		Last Modified: Sat, 01 May 2021 05:18:29 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67496f3d3bb2e7009814fbcbc8d05eff8a850133c52638dab840493f46139417`  
		Last Modified: Sat, 01 May 2021 05:18:30 GMT  
		Size: 3.6 MB (3588283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c5f14dd8fdf5f2a7efcaabae07705db96f36ffc04ec4c9057e2e5e82aa2f403`  
		Last Modified: Sat, 01 May 2021 05:18:29 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c775b338acd3d66cd584bf6bb9fc2df1adcda0aee42be49a8f390d2ebac16e3d`  
		Last Modified: Sat, 01 May 2021 05:18:29 GMT  
		Size: 582.8 KB (582811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c433f73919fc4940a0f062f4bd12ced604d485430d8bf0a3a51448794accbe3f`  
		Last Modified: Sat, 01 May 2021 05:18:30 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:latest`

```console
$ docker pull adminer@sha256:a3e73e13e4f3f1bd1007d7a5d75a6bd23846c3252b71ab7a5817de9ffec04826
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

### `adminer:latest` - linux; amd64

```console
$ docker pull adminer@sha256:12d118ebf5a210b26b665b62af21041766a04d73fbbc63c1b116ad6dc0387b26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.6 MB (33647506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7707fd9b142f208f18d4e495601ad485b68f5dfdd2e4cb904d253f5974ff47dc`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:39:20 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 04:03:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 04:03:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 04:08:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 04:08:27 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 04:08:28 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 04:08:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 04:08:29 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 05:51:26 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:51:26 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 05:51:27 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:51:27 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 05:51:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:51:50 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:51:53 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:51:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:51:53 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:51:53 GMT
USER adminer
# Sat, 01 May 2021 05:51:53 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 05:51:54 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39378a44d29a4d45755bbbc75353969a68f030d8c0cec90ad7f9878f59ea3f5`  
		Last Modified: Sat, 01 May 2021 04:38:19 GMT  
		Size: 10.4 MB (10360243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417049c4f35584148dfd47d28edf662385807b7efa745d4f434ba03de07494b`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21742283d02f6f9451092c008c910a3909a41e37355848483d58e4dff63faffe`  
		Last Modified: Sat, 01 May 2021 04:38:26 GMT  
		Size: 14.3 MB (14256660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50815441106c8e704643e5f718299730f3cb96b03b9214c4f32385a7d2fef9f3`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a20d3bc0470221193d84e1e28160e63d41220d5efea36e336c064fdadbfc34`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 17.5 KB (17529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a75094b0a27256eb69095e9efefc4482cf91c15bd0c82b92934ec41abb83b19`  
		Last Modified: Sat, 01 May 2021 05:52:54 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4ac41937dc4363c09566855d60c909b65e892af0706e331ccceef9ff6033bc`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85ce354c2194e2f1001e52a8c9b13058f0b5b0911d87aa541c50c18fa9d883c`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 3.9 MB (3908144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b65d1b74856e3ed0629fc712e36cf1448d5796212d5b538e77f9e08e03cb77a`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828b20dbe6f1b761839e4e1d7eaa5cf689f716af52c6e1879c7b2cd798c822fb`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 582.8 KB (582804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7b7f0dab3313363e1281a6bfe913030c6c4168beda748d4350e16880480323`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v6

```console
$ docker pull adminer@sha256:16b56985dc271840e1e8164d283af7b63b6b0e96870a3f87c2ebb6e305cb7b1c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32131886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dbef13bdb0432e75de02942ac821772395bbc7e5042fd3b5cde516593dd3f3b`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:06:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:07:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:07:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:07:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:07:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:07:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:29:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:07:41 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:07:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:07:42 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:07:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:07:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:12:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:12:47 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:12:52 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:12:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:12:54 GMT
CMD ["php" "-a"]
# Fri, 30 Apr 2021 23:14:36 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Fri, 30 Apr 2021 23:14:36 GMT
STOPSIGNAL SIGINT
# Fri, 30 Apr 2021 23:14:39 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 30 Apr 2021 23:14:41 GMT
WORKDIR /var/www/html
# Fri, 30 Apr 2021 23:15:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Fri, 30 Apr 2021 23:15:38 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Fri, 30 Apr 2021 23:15:40 GMT
ENV ADMINER_VERSION=4.8.0
# Fri, 30 Apr 2021 23:15:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Fri, 30 Apr 2021 23:15:42 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Fri, 30 Apr 2021 23:15:46 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Fri, 30 Apr 2021 23:15:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 30 Apr 2021 23:15:47 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Fri, 30 Apr 2021 23:15:48 GMT
USER adminer
# Fri, 30 Apr 2021 23:15:49 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Fri, 30 Apr 2021 23:15:49 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726cd3e9e578579e631e21133870b656f3938f6a87797a842254b274d8b76e8`  
		Last Modified: Thu, 15 Apr 2021 02:33:02 GMT  
		Size: 1.7 MB (1690998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db188e87a6ea4fd0959949208b039a0d9facc96183df8dc346c6d0d3368b77e`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73dce0ed56811623cd40b786e95b951ce9d6341d9bfefded4f8aa12574283`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7272eaae063c5d7f7a55cddcfd266b2249c9c29941e2a74712e8ef4847e31dc`  
		Last Modified: Fri, 30 Apr 2021 22:39:32 GMT  
		Size: 10.4 MB (10360229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b3ded6063933c78570fc225ff275611490972800db3a316c9c2bc7846fd31c`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2454cd2b5598ce6dd8ff8f0a593ec04bc91fe623f385a270e5fcd23a9efe837f`  
		Last Modified: Fri, 30 Apr 2021 22:39:33 GMT  
		Size: 13.2 MB (13245293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c3b006179364603a89e8662502d244437ead12db6fd3367949fcc3e72ad3dc`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1974a1d957df5934ade9796f0fa21cad68c36cf7ddee2fd124e430a2f2e159c`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 17.6 KB (17551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163da5758d6703ae0d3c6ab673fc9c00e778461230ff5aff7163baffcd7f6361`  
		Last Modified: Fri, 30 Apr 2021 23:18:35 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73f8523f7b76c4f107a5fdde83c2eed8ef45b6f265432293af6d78b772149e7`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca9f9202fb99ea8d097d90a5bb62979fbc35544da64a8a677da4b8bbf420f96`  
		Last Modified: Fri, 30 Apr 2021 23:18:35 GMT  
		Size: 3.6 MB (3604909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebdcc1e39d88d3548486b0b94fd4925deda0fd89552ec953ec45103639056e3`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634b5387043b43b3105ba37b43d31e1bf5a1ad5c5a63ee766b5c6aa198d6a2f`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 582.8 KB (582802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b737b034949aeddb4bd174c7f33742314e10f2db3cbe879b3507c0f2b2faf7`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm variant v7

```console
$ docker pull adminer@sha256:f1cd758c5bcbe78188b5766221c37d6041a5c8d727af64e9a49b277e09e80ce1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30938697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99e81544e5622446ab0920052f90534d15fe52866ccfddc0d883edcada095a7f`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:08:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:08:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:08:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:08:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:08:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:08:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:35:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:09:59 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:10:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:10:02 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:10:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:10:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:13:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:13:14 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 02:13:17 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:13:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:13:19 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 03:51:49 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 03:51:50 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 03:51:54 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 03:51:55 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 03:52:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 03:52:48 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 03:52:49 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 03:52:50 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 03:52:51 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 03:52:57 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 03:52:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 03:52:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 03:53:02 GMT
USER adminer
# Sat, 01 May 2021 03:53:05 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 03:53:07 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc6d3f07b2e440bf9a8e52a0a5bba0f27637990ee4976424cef6aae97e169f`  
		Last Modified: Thu, 15 Apr 2021 03:38:53 GMT  
		Size: 1.6 MB (1559061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9000ca9dcd92a2066a3a2c4031e677c3998cd82a3ecbc68468d11255ecbdb62`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d102949f174ecad1044574e45dded8368eb7451bf66b3bdac6e367c7f415d3`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5dab41947ddc5db66501a8111f7ef729f521e11ca3ad87ecf37bd79eac6ef3`  
		Last Modified: Sat, 01 May 2021 02:35:25 GMT  
		Size: 10.4 MB (10360231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2700665f109862388a4e0ed21b2fd335c4d89050efbad76af079999dfd9a4b68`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7aabe4a04c27ab686de62e8f214ca07e6d03fe93c6d40ade09bced2eab56901`  
		Last Modified: Sat, 01 May 2021 02:35:28 GMT  
		Size: 12.4 MB (12407150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebda42f2c319f9f89154be7b8165960eccb3900eb3f5b9e2857420d88f5ca575`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f9f67e3447fb75cf1724c1d4b7d53b8b1de00a8ec05d4aba9f7d8c09a9035`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 17.5 KB (17540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677aab5c428da05844e96dc166beb86af6dc68f33a93546bbbefed7d3839112c`  
		Last Modified: Sat, 01 May 2021 03:55:43 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2789eb966365d0da44c2eb6fce9e8d6b0b0b0640c29214cc9a6407267f9b4`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da46a02e36d762092675c2d38e18ca37e2e0163b58bf248c621b0a9dc8866d8e`  
		Last Modified: Sat, 01 May 2021 03:55:43 GMT  
		Size: 3.6 MB (3579788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841c453f4c80b715d2c60cdeb21facc849ad7ea141aef125bcdfff3fc87ea2e6`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 1.5 KB (1472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052526ae6f5bb73b64438863414d320716ac83cd7542b7db8216dba070bc9f72`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cde09e1b359229258d6f040ec2f23d5b10a5b6b50cc84580a40aaf5fa55556`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:2995c05337d98dd62225e6d58c6c551940eb5d2314ee022551a359c2edfdbb95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33288719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e49d6a5068aff4b8f7d53e5ca53084149e52a21716008685d3634f152a93cc82`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:27:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:28:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:28:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:28:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:28:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:53:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 01:51:16 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 01:51:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 01:51:18 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 01:51:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 01:51:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 01:55:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 01:55:39 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 01:55:43 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 01:55:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 01:55:46 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 04:07:49 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 04:07:50 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 04:07:54 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 04:07:55 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 04:08:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 04:08:56 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 04:08:57 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 04:08:58 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 04:08:59 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 04:09:03 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 04:09:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 04:09:05 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 04:09:06 GMT
USER adminer
# Sat, 01 May 2021 04:09:07 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 04:09:08 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea792edc0a65854bc13c90079b9e33a399c351b73e194d9df4f2cf5a0efeb2`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 1.7 MB (1700262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31bbfcb500579a0c450809a6b082c564c3ce4873732c1b62d8dab52ed0a11ac`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22841fe152c1fe4ec2048ebca3b9c0db9d29773b0d0670167a848d87fcfe83f3`  
		Last Modified: Thu, 15 Apr 2021 01:59:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86a2990f157991d12ee804183f42ab624a7af15605920e9c12adce886783bd9`  
		Last Modified: Sat, 01 May 2021 02:24:37 GMT  
		Size: 10.4 MB (10360252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717c7ad0a34fca1bd9fe22eb98d3abc226862c3a4875c05fec802e7c66425afe`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec40f0928e2ca1518729b1c63da742a00d1df98e4861f80d6e8f4019fbde9f26`  
		Last Modified: Sat, 01 May 2021 02:24:40 GMT  
		Size: 14.0 MB (14028751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d802fc3cc61952c8e0f43df7f44975e487e3d138bacfdc9c2daeca67d47cd976`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f89f4b8ccd74e3d8337940607bb14e9230a6ca849950ded149286a4b79e268a`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9208e6df146eb023a8d9b5260435c9cbd6f67b60dfb46766c5841339f85f8ec0`  
		Last Modified: Sat, 01 May 2021 04:11:07 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b108d0b6a7ff2b8cf63b53bbe86fd0454a91008e3714557e80df86a09cda0abf`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273c8a35b22772c8535453bfe942ed895b853bfabedfce587de72643c2ca6aaa`  
		Last Modified: Sat, 01 May 2021 04:11:07 GMT  
		Size: 3.9 MB (3879098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df87fa0c04f21673d85d974891030708b890f98615a245ac79d220ecf1378f7`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb52da6ce3c536b5587683997df91e97198a9ed221fd6df0b6b7d49f57717d3`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 582.8 KB (582804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4830f1e50425a8f4fc4e1236b44d93d5b39a716f837b8d921c8afb2fd5be92e`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; 386

```console
$ docker pull adminer@sha256:19d6d656da0acd11da3961bef1d4d85e7a41e7467f127e7989d0db6f8a342a95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34231434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcfa500fd2970be787667cf0eae0f3db72409b63b7d985f6402ec9b2667b013a`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 04:15:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:24:22 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:24:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:24:23 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:24:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:24:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:33:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:33:53 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:33:56 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:33:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:33:58 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 00:17:31 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 00:17:31 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 00:17:33 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 00:17:34 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 00:18:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 00:18:54 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 00:18:54 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 00:18:55 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 00:18:55 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 00:18:58 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 00:18:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 00:18:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 00:18:59 GMT
USER adminer
# Sat, 01 May 2021 00:18:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 00:19:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f032c69e4d0122e069320b9680ef26b8bb3c430278739a6fea12af3a4f96e134`  
		Last Modified: Fri, 30 Apr 2021 23:40:49 GMT  
		Size: 10.4 MB (10360220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c9984d072093737e593d0ef515c92f288b39d14aabf7a7d51b86898bc1aef7`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5e9496813676c2e99e74df895938ef33a8cf138c5a38a3e73968cc1b2fa932`  
		Last Modified: Fri, 30 Apr 2021 23:40:54 GMT  
		Size: 14.6 MB (14632431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d376f079b3a59dc3fc16b3017ea542c2ea92a6de4dcdb3aa927c19364e1df5`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df9b26593ad898c78d3de9232c23626d904c18e6b24f18767a144a5536e73e1`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 17.5 KB (17541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40300d5ae7ee86745631c5498bfc7757e4ac4bf3eacda6a10991b2a38dbcecf7`  
		Last Modified: Sat, 01 May 2021 00:21:38 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e1a92ccdfda888c1542ec341a96c423af53a5f232f654b95e5436b7256fd7b`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e200018a310c11b06c52afa2eb578aed71d2fcff109735fac4a4224a2d99198`  
		Last Modified: Sat, 01 May 2021 00:21:36 GMT  
		Size: 4.0 MB (4012274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5d7bd779781644a969c9a0c3214e5b34c562367de371486d6d908161ee3bee`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69a63a5467a891b0c71e5954c34e2275c605b8fddd9bc7856ec4442ae2a1c0d`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 582.8 KB (582810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3637c8ae22706fe31d88cd4487ddc444d18f7b005442b713e7594c150a8aa5e8`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; ppc64le

```console
$ docker pull adminer@sha256:dbb3b10c00dc1f3ece08df27b44d79f66f959aedc9d4680e63052716fda1881e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34733557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea9e143138a6e56e3f5db1c7fd10a20e080c0b8a996439d5b1e154c009c52c5`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:16:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:46:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 03:42:52 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 03:42:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 03:43:08 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 03:43:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 03:43:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 03:48:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 03:48:36 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 03:48:53 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 03:49:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 03:49:13 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 07:05:31 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 07:05:43 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 07:06:08 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 07:06:19 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 07:07:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 07:07:46 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 07:07:56 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 07:08:03 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 07:08:22 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 07:08:57 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 07:09:05 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 07:09:11 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 07:09:22 GMT
USER adminer
# Sat, 01 May 2021 07:09:31 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 07:09:38 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d82dc7c3129f9f8efe068b46b7988252e5911a9bf70f2f3ec970ed7382d8f92`  
		Last Modified: Sat, 01 May 2021 04:28:17 GMT  
		Size: 10.4 MB (10360240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f5852448efedd86253d2f693d58031fd8707b7fd4983e4b0453351d357f118`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89a34f310b9721f0ab0de62088a7d630d699d7cf59fbb7957542afbc7659f3`  
		Last Modified: Sat, 01 May 2021 04:28:19 GMT  
		Size: 15.3 MB (15282748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a34edc1036d80f0acbe7cd46a9c1bad8d141654a25252318a3457a14311dfe`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587df26cc194e45cf1f6e3bd6b2e3f0bfae286ca1ae26b98b457b556d7427303`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 17.6 KB (17562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a4991a1eff14856b0308c117ac5c87d74aac4a2c00dfc3fc38e69846bdca8e`  
		Last Modified: Sat, 01 May 2021 07:13:15 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbfbca1bede0192cfb0c862f0077baa98e4dbcd683d0682b3c04a4467ec3f67`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e078202145e09994bf4c091f95f65084e2d380b192e68fa3055f4c8da3c0f1a`  
		Last Modified: Sat, 01 May 2021 07:13:14 GMT  
		Size: 3.9 MB (3920436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a08531336bb96df3ee7311a11f8c8f5f78b27fd27f2e1e8cebe3aaebefc0cf6`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4129c43164fd79c0ea01d2c1d993a469846ebb51d831de0d08dc6fe5390ca1d`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 582.8 KB (582809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea793cb13300c9b023cc7deccce5ce057f8611b196da7f5747c42494fa1aa1f5`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:latest` - linux; s390x

```console
$ docker pull adminer@sha256:be29af6c13419aaaf011ebb117d07f34d74dfd3d51a4657fb92ec7e8a5a3e992
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32536231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e3b6e5f32c6c450164b419f6108097b7765a448b2965197e82c4a7be358dc10`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:18:59 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:54:37 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:54:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:54:38 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:54:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:54:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:58:16 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 02:58:18 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:58:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:58:18 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 05:16:12 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:16:12 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 05:16:14 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:16:15 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 05:16:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:16:55 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:16:58 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:16:59 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:16:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:17:00 GMT
USER adminer
# Sat, 01 May 2021 05:17:00 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 05:17:01 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b7aa20ee47cf4d85a8a033023b14b1948153a005c710022465266b1676ff00`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 10.4 MB (10360232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c09e3c51bdc12e3dac46e704947a4207380cc86861118e2ba93827f09a479b`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c57065802a25a7373daa5d63b66c55320e705d6ef8e47055d2ba2997ac4ac1f`  
		Last Modified: Sat, 01 May 2021 03:23:19 GMT  
		Size: 13.6 MB (13616029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa2ed8a45355ef77a61d2740ffedf281c9079db17e02fcd213477f4c8bd2f4`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d549711db456f1993f2dd16932c69755412329900032bc3250bfff994fd9d43`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa60d82d0a8b59fda860a56dae19ab654de0f1368014f447b7f9c53d96c5584`  
		Last Modified: Sat, 01 May 2021 05:18:16 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d3ea1b608b879ac7c8354ab621b511601a964e24706c82764e975896ec2d4`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1128a53bb989ba9202c67883e70c3aa25bfbc7a44e36360de37f23e678dab0`  
		Last Modified: Sat, 01 May 2021 05:18:15 GMT  
		Size: 3.6 MB (3588293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6ac88d341f35d6278d87a43b3998caa46d2a2d7515df5446755a418c22fb4f`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 1.5 KB (1474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46932d8f58943aa96cffad8c4b13a779eb592deacb98d058e46236c40479d28`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32bae7fbe947016896c76b4d5aea4dbb1dd2feb86f7062de658448beb0f326a`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `adminer:standalone`

```console
$ docker pull adminer@sha256:a3e73e13e4f3f1bd1007d7a5d75a6bd23846c3252b71ab7a5817de9ffec04826
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

### `adminer:standalone` - linux; amd64

```console
$ docker pull adminer@sha256:12d118ebf5a210b26b665b62af21041766a04d73fbbc63c1b116ad6dc0387b26
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.6 MB (33647506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7707fd9b142f208f18d4e495601ad485b68f5dfdd2e4cb904d253f5974ff47dc`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:39 GMT
ADD file:8ec69d882e7f29f0652d537557160e638168550f738d0d49f90a7ef96bf31787 in / 
# Wed, 14 Apr 2021 19:19:39 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:59:18 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 23:59:20 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 23:59:22 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 23:59:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 23:59:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 23:59:24 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:39:20 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 04:03:33 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 04:03:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 04:03:39 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 04:08:26 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 04:08:27 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 04:08:28 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 04:08:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 04:08:29 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 05:51:26 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:51:26 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 05:51:27 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:51:27 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 05:51:50 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:51:50 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:51:51 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:51:53 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:51:53 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:51:53 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:51:53 GMT
USER adminer
# Sat, 01 May 2021 05:51:53 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 05:51:54 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:540db60ca9383eac9e418f78490994d0af424aab7bf6d0e47ac8ed4e2e9bcbba`  
		Last Modified: Wed, 14 Apr 2021 17:59:29 GMT  
		Size: 2.8 MB (2811969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:933cf2f4a68ffb603d67468c6e390ce893a1410ea927dc00e8faabfd01032afa`  
		Last Modified: Thu, 15 Apr 2021 02:15:25 GMT  
		Size: 1.7 MB (1702188 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c5cc202a60c205410f5462131556b8ecfba3092bceab1bf75723d1a356c7fb`  
		Last Modified: Thu, 15 Apr 2021 02:15:23 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74403c16157d84037726eebe566275f9e5fdb3f301ce6c101eeb3fb37b8914ef`  
		Last Modified: Thu, 15 Apr 2021 02:15:22 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f39378a44d29a4d45755bbbc75353969a68f030d8c0cec90ad7f9878f59ea3f5`  
		Last Modified: Sat, 01 May 2021 04:38:19 GMT  
		Size: 10.4 MB (10360243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9417049c4f35584148dfd47d28edf662385807b7efa745d4f434ba03de07494b`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21742283d02f6f9451092c008c910a3909a41e37355848483d58e4dff63faffe`  
		Last Modified: Sat, 01 May 2021 04:38:26 GMT  
		Size: 14.3 MB (14256660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50815441106c8e704643e5f718299730f3cb96b03b9214c4f32385a7d2fef9f3`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 2.3 KB (2266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13a20d3bc0470221193d84e1e28160e63d41220d5efea36e336c064fdadbfc34`  
		Last Modified: Sat, 01 May 2021 04:38:18 GMT  
		Size: 17.5 KB (17529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a75094b0a27256eb69095e9efefc4482cf91c15bd0c82b92934ec41abb83b19`  
		Last Modified: Sat, 01 May 2021 05:52:54 GMT  
		Size: 304.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4ac41937dc4363c09566855d60c909b65e892af0706e331ccceef9ff6033bc`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85ce354c2194e2f1001e52a8c9b13058f0b5b0911d87aa541c50c18fa9d883c`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 3.9 MB (3908144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b65d1b74856e3ed0629fc712e36cf1448d5796212d5b538e77f9e08e03cb77a`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 1.5 KB (1473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:828b20dbe6f1b761839e4e1d7eaa5cf689f716af52c6e1879c7b2cd798c822fb`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 582.8 KB (582804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7b7f0dab3313363e1281a6bfe913030c6c4168beda748d4350e16880480323`  
		Last Modified: Sat, 01 May 2021 05:52:51 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v6

```console
$ docker pull adminer@sha256:16b56985dc271840e1e8164d283af7b63b6b0e96870a3f87c2ebb6e305cb7b1c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32131886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3dbef13bdb0432e75de02942ac821772395bbc7e5042fd3b5cde516593dd3f3b`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:49:39 GMT
ADD file:4479f0a51530e039edf231d87201896dcff908aa542a613cdccb015f93dda8a3 in / 
# Wed, 14 Apr 2021 18:49:40 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 01:06:58 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 01:07:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 01:07:14 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 01:07:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 01:07:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 01:07:25 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:27 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 01:07:29 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 01:29:48 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:07:41 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:07:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:07:42 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:07:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:07:51 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:12:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:12:47 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:12:52 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:12:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:12:54 GMT
CMD ["php" "-a"]
# Fri, 30 Apr 2021 23:14:36 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Fri, 30 Apr 2021 23:14:36 GMT
STOPSIGNAL SIGINT
# Fri, 30 Apr 2021 23:14:39 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Fri, 30 Apr 2021 23:14:41 GMT
WORKDIR /var/www/html
# Fri, 30 Apr 2021 23:15:37 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Fri, 30 Apr 2021 23:15:38 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Fri, 30 Apr 2021 23:15:40 GMT
ENV ADMINER_VERSION=4.8.0
# Fri, 30 Apr 2021 23:15:41 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Fri, 30 Apr 2021 23:15:42 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Fri, 30 Apr 2021 23:15:46 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Fri, 30 Apr 2021 23:15:46 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Fri, 30 Apr 2021 23:15:47 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Fri, 30 Apr 2021 23:15:48 GMT
USER adminer
# Fri, 30 Apr 2021 23:15:49 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Fri, 30 Apr 2021 23:15:49 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:740c950346cf39c85b52576998695c9b909c24a58a8bb1b64cce91fda3ef1d3a`  
		Last Modified: Wed, 14 Apr 2021 18:50:30 GMT  
		Size: 2.6 MB (2622131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4726cd3e9e578579e631e21133870b656f3938f6a87797a842254b274d8b76e8`  
		Last Modified: Thu, 15 Apr 2021 02:33:02 GMT  
		Size: 1.7 MB (1690998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0db188e87a6ea4fd0959949208b039a0d9facc96183df8dc346c6d0d3368b77e`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9a73dce0ed56811623cd40b786e95b951ce9d6341d9bfefded4f8aa12574283`  
		Last Modified: Thu, 15 Apr 2021 02:33:01 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7272eaae063c5d7f7a55cddcfd266b2249c9c29941e2a74712e8ef4847e31dc`  
		Last Modified: Fri, 30 Apr 2021 22:39:32 GMT  
		Size: 10.4 MB (10360229 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b3ded6063933c78570fc225ff275611490972800db3a316c9c2bc7846fd31c`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2454cd2b5598ce6dd8ff8f0a593ec04bc91fe623f385a270e5fcd23a9efe837f`  
		Last Modified: Fri, 30 Apr 2021 22:39:33 GMT  
		Size: 13.2 MB (13245293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1c3b006179364603a89e8662502d244437ead12db6fd3367949fcc3e72ad3dc`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 2.3 KB (2271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1974a1d957df5934ade9796f0fa21cad68c36cf7ddee2fd124e430a2f2e159c`  
		Last Modified: Fri, 30 Apr 2021 22:39:25 GMT  
		Size: 17.6 KB (17551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:163da5758d6703ae0d3c6ab673fc9c00e778461230ff5aff7163baffcd7f6361`  
		Last Modified: Fri, 30 Apr 2021 23:18:35 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f73f8523f7b76c4f107a5fdde83c2eed8ef45b6f265432293af6d78b772149e7`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca9f9202fb99ea8d097d90a5bb62979fbc35544da64a8a677da4b8bbf420f96`  
		Last Modified: Fri, 30 Apr 2021 23:18:35 GMT  
		Size: 3.6 MB (3604909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebdcc1e39d88d3548486b0b94fd4925deda0fd89552ec953ec45103639056e3`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a634b5387043b43b3105ba37b43d31e1bf5a1ad5c5a63ee766b5c6aa198d6a2f`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 582.8 KB (582802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6b737b034949aeddb4bd174c7f33742314e10f2db3cbe879b3507c0f2b2faf7`  
		Last Modified: Fri, 30 Apr 2021 23:18:34 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm variant v7

```console
$ docker pull adminer@sha256:f1cd758c5bcbe78188b5766221c37d6041a5c8d727af64e9a49b277e09e80ce1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30938697 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99e81544e5622446ab0920052f90534d15fe52866ccfddc0d883edcada095a7f`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:57:39 GMT
ADD file:028c5b473d862250586e174c5dd19b37f8fc3bffbc02d888e72df30f32fd6129 in / 
# Wed, 14 Apr 2021 18:57:39 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 02:08:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 02:08:23 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 02:08:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 02:08:27 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 02:08:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 02:08:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 02:08:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 02:35:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:09:59 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:10:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:10:02 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:10:09 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:10:09 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:13:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:13:14 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 02:13:17 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:13:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:13:19 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 03:51:49 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 03:51:50 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 03:51:54 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 03:51:55 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 03:52:47 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 03:52:48 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 03:52:49 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 03:52:50 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 03:52:51 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 03:52:57 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 03:52:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 03:52:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 03:53:02 GMT
USER adminer
# Sat, 01 May 2021 03:53:05 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 03:53:07 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:e160e00eb35d5bc2373770873fbc9c8f5706045b0b06bfd1c364fcf69f02e9fe`  
		Last Modified: Wed, 14 Apr 2021 18:58:36 GMT  
		Size: 2.4 MB (2424145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bc6d3f07b2e440bf9a8e52a0a5bba0f27637990ee4976424cef6aae97e169f`  
		Last Modified: Thu, 15 Apr 2021 03:38:53 GMT  
		Size: 1.6 MB (1559061 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9000ca9dcd92a2066a3a2c4031e677c3998cd82a3ecbc68468d11255ecbdb62`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09d102949f174ecad1044574e45dded8368eb7451bf66b3bdac6e367c7f415d3`  
		Last Modified: Thu, 15 Apr 2021 03:38:49 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5dab41947ddc5db66501a8111f7ef729f521e11ca3ad87ecf37bd79eac6ef3`  
		Last Modified: Sat, 01 May 2021 02:35:25 GMT  
		Size: 10.4 MB (10360231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2700665f109862388a4e0ed21b2fd335c4d89050efbad76af079999dfd9a4b68`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7aabe4a04c27ab686de62e8f214ca07e6d03fe93c6d40ade09bced2eab56901`  
		Last Modified: Sat, 01 May 2021 02:35:28 GMT  
		Size: 12.4 MB (12407150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebda42f2c319f9f89154be7b8165960eccb3900eb3f5b9e2857420d88f5ca575`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f9f67e3447fb75cf1724c1d4b7d53b8b1de00a8ec05d4aba9f7d8c09a9035`  
		Last Modified: Sat, 01 May 2021 02:35:24 GMT  
		Size: 17.5 KB (17540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:677aab5c428da05844e96dc166beb86af6dc68f33a93546bbbefed7d3839112c`  
		Last Modified: Sat, 01 May 2021 03:55:43 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cd2789eb966365d0da44c2eb6fce9e8d6b0b0b0640c29214cc9a6407267f9b4`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da46a02e36d762092675c2d38e18ca37e2e0163b58bf248c621b0a9dc8866d8e`  
		Last Modified: Sat, 01 May 2021 03:55:43 GMT  
		Size: 3.6 MB (3579788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:841c453f4c80b715d2c60cdeb21facc849ad7ea141aef125bcdfff3fc87ea2e6`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 1.5 KB (1472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:052526ae6f5bb73b64438863414d320716ac83cd7542b7db8216dba070bc9f72`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cde09e1b359229258d6f040ec2f23d5b10a5b6b50cc84580a40aaf5fa55556`  
		Last Modified: Sat, 01 May 2021 03:55:42 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; arm64 variant v8

```console
$ docker pull adminer@sha256:2995c05337d98dd62225e6d58c6c551940eb5d2314ee022551a359c2edfdbb95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.3 MB (33288719 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e49d6a5068aff4b8f7d53e5ca53084149e52a21716008685d3634f152a93cc82`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:42:37 GMT
ADD file:ca9d8b5d1cc2f2186983fc6b9507da6ada5eb92f2b518c06af1128d5396c6f34 in / 
# Wed, 14 Apr 2021 18:42:38 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 00:27:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 00:28:02 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 00:28:11 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 00:28:13 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 00:28:21 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 00:28:23 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:24 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 00:28:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 00:53:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 01:51:16 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 01:51:17 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 01:51:18 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 01:51:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 01:51:26 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 01:55:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 01:55:39 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 01:55:43 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 01:55:45 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 01:55:46 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 04:07:49 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 04:07:50 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 04:07:54 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 04:07:55 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 04:08:54 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 04:08:56 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 04:08:57 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 04:08:58 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 04:08:59 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 04:09:03 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 04:09:04 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 04:09:05 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 04:09:06 GMT
USER adminer
# Sat, 01 May 2021 04:09:07 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 04:09:08 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:595b0fe564bb9444ebfe78288079a01ee6d7f666544028d5e96ba610f909ee43`  
		Last Modified: Wed, 14 Apr 2021 18:43:41 GMT  
		Size: 2.7 MB (2712026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bea792edc0a65854bc13c90079b9e33a399c351b73e194d9df4f2cf5a0efeb2`  
		Last Modified: Thu, 15 Apr 2021 01:59:52 GMT  
		Size: 1.7 MB (1700262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e31bbfcb500579a0c450809a6b082c564c3ce4873732c1b62d8dab52ed0a11ac`  
		Last Modified: Thu, 15 Apr 2021 01:59:50 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22841fe152c1fe4ec2048ebca3b9c0db9d29773b0d0670167a848d87fcfe83f3`  
		Last Modified: Thu, 15 Apr 2021 01:59:51 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f86a2990f157991d12ee804183f42ab624a7af15605920e9c12adce886783bd9`  
		Last Modified: Sat, 01 May 2021 02:24:37 GMT  
		Size: 10.4 MB (10360252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:717c7ad0a34fca1bd9fe22eb98d3abc226862c3a4875c05fec802e7c66425afe`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec40f0928e2ca1518729b1c63da742a00d1df98e4861f80d6e8f4019fbde9f26`  
		Last Modified: Sat, 01 May 2021 02:24:40 GMT  
		Size: 14.0 MB (14028751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d802fc3cc61952c8e0f43df7f44975e487e3d138bacfdc9c2daeca67d47cd976`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 2.3 KB (2267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f89f4b8ccd74e3d8337940607bb14e9230a6ca849950ded149286a4b79e268a`  
		Last Modified: Sat, 01 May 2021 02:24:36 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9208e6df146eb023a8d9b5260435c9cbd6f67b60dfb46766c5841339f85f8ec0`  
		Last Modified: Sat, 01 May 2021 04:11:07 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b108d0b6a7ff2b8cf63b53bbe86fd0454a91008e3714557e80df86a09cda0abf`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:273c8a35b22772c8535453bfe942ed895b853bfabedfce587de72643c2ca6aaa`  
		Last Modified: Sat, 01 May 2021 04:11:07 GMT  
		Size: 3.9 MB (3879098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7df87fa0c04f21673d85d974891030708b890f98615a245ac79d220ecf1378f7`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0fb52da6ce3c536b5587683997df91e97198a9ed221fd6df0b6b7d49f57717d3`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 582.8 KB (582804 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4830f1e50425a8f4fc4e1236b44d93d5b39a716f837b8d921c8afb2fd5be92e`  
		Last Modified: Sat, 01 May 2021 04:11:06 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; 386

```console
$ docker pull adminer@sha256:19d6d656da0acd11da3961bef1d4d85e7a41e7467f127e7989d0db6f8a342a95
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.2 MB (34231434 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dcfa500fd2970be787667cf0eae0f3db72409b63b7d985f6402ec9b2667b013a`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:29 GMT
ADD file:36634145ad6ec95a6b1a4f8d875f48719357c7a90f9b4906f8ce74f71b28c19d in / 
# Wed, 14 Apr 2021 18:38:29 GMT
CMD ["/bin/sh"]
# Thu, 15 Apr 2021 03:38:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 15 Apr 2021 03:38:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 15 Apr 2021 03:38:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 15 Apr 2021 03:38:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 15 Apr 2021 03:38:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 15 Apr 2021 03:38:48 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 15 Apr 2021 04:15:19 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 30 Apr 2021 22:24:22 GMT
ENV PHP_VERSION=7.4.18
# Fri, 30 Apr 2021 22:24:23 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Fri, 30 Apr 2021 22:24:23 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Fri, 30 Apr 2021 22:24:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 30 Apr 2021 22:24:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:33:52 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 30 Apr 2021 22:33:53 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Fri, 30 Apr 2021 22:33:56 GMT
RUN docker-php-ext-enable sodium
# Fri, 30 Apr 2021 22:33:58 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 30 Apr 2021 22:33:58 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 00:17:31 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 00:17:31 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 00:17:33 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 00:17:34 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 00:18:53 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 00:18:54 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 00:18:54 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 00:18:55 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 00:18:55 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 00:18:58 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 00:18:58 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 00:18:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 00:18:59 GMT
USER adminer
# Sat, 01 May 2021 00:18:59 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 00:19:00 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:31b7e7ccca9e17fd08b39c9a4ffd3ded380b62816c489d6c3758c9bb5a632430`  
		Last Modified: Wed, 14 Apr 2021 18:39:24 GMT  
		Size: 2.8 MB (2818900 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3818e7e8eb8d9c0ab0e377e89ed7df3037ec2c0d4c4c89bd3a2abedc459366c`  
		Last Modified: Thu, 15 Apr 2021 05:57:45 GMT  
		Size: 1.8 MB (1799274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274cbc3732aca6ca32c0ba51f7504eb2d19d4fd52d0f89f9ff2597a673484be8`  
		Last Modified: Thu, 15 Apr 2021 05:57:43 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32aa0b7923dc47bd54c1e8cc895686f0638c3a28a9a40f8ed831545df00ce891`  
		Last Modified: Thu, 15 Apr 2021 05:57:46 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f032c69e4d0122e069320b9680ef26b8bb3c430278739a6fea12af3a4f96e134`  
		Last Modified: Fri, 30 Apr 2021 23:40:49 GMT  
		Size: 10.4 MB (10360220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c9984d072093737e593d0ef515c92f288b39d14aabf7a7d51b86898bc1aef7`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b5e9496813676c2e99e74df895938ef33a8cf138c5a38a3e73968cc1b2fa932`  
		Last Modified: Fri, 30 Apr 2021 23:40:54 GMT  
		Size: 14.6 MB (14632431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9d376f079b3a59dc3fc16b3017ea542c2ea92a6de4dcdb3aa927c19364e1df5`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 2.3 KB (2268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df9b26593ad898c78d3de9232c23626d904c18e6b24f18767a144a5536e73e1`  
		Last Modified: Fri, 30 Apr 2021 23:40:47 GMT  
		Size: 17.5 KB (17541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40300d5ae7ee86745631c5498bfc7757e4ac4bf3eacda6a10991b2a38dbcecf7`  
		Last Modified: Sat, 01 May 2021 00:21:38 GMT  
		Size: 309.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e1a92ccdfda888c1542ec341a96c423af53a5f232f654b95e5436b7256fd7b`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 1.4 KB (1408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e200018a310c11b06c52afa2eb578aed71d2fcff109735fac4a4224a2d99198`  
		Last Modified: Sat, 01 May 2021 00:21:36 GMT  
		Size: 4.0 MB (4012274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5d7bd779781644a969c9a0c3214e5b34c562367de371486d6d908161ee3bee`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 1.5 KB (1476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d69a63a5467a891b0c71e5954c34e2275c605b8fddd9bc7856ec4442ae2a1c0d`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 582.8 KB (582810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3637c8ae22706fe31d88cd4487ddc444d18f7b005442b713e7594c150a8aa5e8`  
		Last Modified: Sat, 01 May 2021 00:21:35 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; ppc64le

```console
$ docker pull adminer@sha256:dbb3b10c00dc1f3ece08df27b44d79f66f959aedc9d4680e63052716fda1881e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34733557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dea9e143138a6e56e3f5db1c7fd10a20e080c0b8a996439d5b1e154c009c52c5`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 19:30:57 GMT
ADD file:52162c4413e3597dad4ccb790c379b67ef40d50c0d0659e8b6c65d833886b3af in / 
# Wed, 14 Apr 2021 19:31:02 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:15:47 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 20:15:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 20:16:09 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 20:16:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 20:16:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 20:16:29 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 20:16:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 20:46:01 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 03:42:52 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 03:42:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 03:43:08 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 03:43:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 03:43:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 03:48:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 03:48:36 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 03:48:53 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 03:49:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 03:49:13 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 07:05:31 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 07:05:43 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 07:06:08 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 07:06:19 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 07:07:43 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 07:07:46 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 07:07:56 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 07:08:03 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 07:08:22 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 07:08:57 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 07:09:05 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 07:09:11 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 07:09:22 GMT
USER adminer
# Sat, 01 May 2021 07:09:31 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 07:09:38 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:771d2590aa602a0d4a922e322f02b22cc9d193f8cd159d9d1a140cadf1f8b4d4`  
		Last Modified: Wed, 14 Apr 2021 19:32:33 GMT  
		Size: 2.8 MB (2813141 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b18b4999d98214ab55ea75ff5caca694bebb5bb07f5c23e9a6f4ce900ce4c2c6`  
		Last Modified: Wed, 14 Apr 2021 22:01:00 GMT  
		Size: 1.7 MB (1748637 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8118faf424e03fa2a7d0df76aa1813928f5598c3bdd1b390629452fd95766a66`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc86fc5a1b429a1fd2c88a0a1f7506b2543ae32ff0ba83f0ba697a84dafa2ded`  
		Last Modified: Wed, 14 Apr 2021 22:00:59 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d82dc7c3129f9f8efe068b46b7988252e5911a9bf70f2f3ec970ed7382d8f92`  
		Last Modified: Sat, 01 May 2021 04:28:17 GMT  
		Size: 10.4 MB (10360240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15f5852448efedd86253d2f693d58031fd8707b7fd4983e4b0453351d357f118`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e89a34f310b9721f0ab0de62088a7d630d699d7cf59fbb7957542afbc7659f3`  
		Last Modified: Sat, 01 May 2021 04:28:19 GMT  
		Size: 15.3 MB (15282748 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93a34edc1036d80f0acbe7cd46a9c1bad8d141654a25252318a3457a14311dfe`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:587df26cc194e45cf1f6e3bd6b2e3f0bfae286ca1ae26b98b457b556d7427303`  
		Last Modified: Sat, 01 May 2021 04:28:16 GMT  
		Size: 17.6 KB (17562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a4991a1eff14856b0308c117ac5c87d74aac4a2c00dfc3fc38e69846bdca8e`  
		Last Modified: Sat, 01 May 2021 07:13:15 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fbfbca1bede0192cfb0c862f0077baa98e4dbcd683d0682b3c04a4467ec3f67`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e078202145e09994bf4c091f95f65084e2d380b192e68fa3055f4c8da3c0f1a`  
		Last Modified: Sat, 01 May 2021 07:13:14 GMT  
		Size: 3.9 MB (3920436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a08531336bb96df3ee7311a11f8c8f5f78b27fd27f2e1e8cebe3aaebefc0cf6`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 1.5 KB (1475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4129c43164fd79c0ea01d2c1d993a469846ebb51d831de0d08dc6fe5390ca1d`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 582.8 KB (582809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea793cb13300c9b023cc7deccce5ce057f8611b196da7f5747c42494fa1aa1f5`  
		Last Modified: Sat, 01 May 2021 07:13:13 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `adminer:standalone` - linux; s390x

```console
$ docker pull adminer@sha256:be29af6c13419aaaf011ebb117d07f34d74dfd3d51a4657fb92ec7e8a5a3e992
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32536231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e3b6e5f32c6c450164b419f6108097b7765a448b2965197e82c4a7be358dc10`
-	Entrypoint: `["entrypoint.sh","docker-php-entrypoint"]`
-	Default Command: `["php","-S","[::]:8080","-t","\/var\/www\/html"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:35 GMT
ADD file:c715fef757fe2b022ae1bbff71dbc58bddf5a858deb0aac5a6fbcf10d5f3111c in / 
# Wed, 14 Apr 2021 18:41:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 19:00:51 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Wed, 14 Apr 2021 19:00:54 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Wed, 14 Apr 2021 19:00:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Wed, 14 Apr 2021 19:00:56 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 14 Apr 2021 19:00:57 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 14 Apr 2021 19:00:59 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 14 Apr 2021 19:18:59 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 01 May 2021 02:54:37 GMT
ENV PHP_VERSION=7.4.18
# Sat, 01 May 2021 02:54:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.18.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.18.tar.xz.asc
# Sat, 01 May 2021 02:54:38 GMT
ENV PHP_SHA256=ab97f22b128d21dcbc009b50a37aaea0051b2721cbcd122d9e00e6ffc3c4b7e1
# Sat, 01 May 2021 02:54:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 01 May 2021 02:54:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 01 May 2021 02:58:15 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Sat, 01 May 2021 02:58:16 GMT
COPY multi:efd917b98407edb5d558edb0edbd8e63c9318f701892aaa449794d019a092f37 in /usr/local/bin/ 
# Sat, 01 May 2021 02:58:18 GMT
RUN docker-php-ext-enable sodium
# Sat, 01 May 2021 02:58:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 01 May 2021 02:58:18 GMT
CMD ["php" "-a"]
# Sat, 01 May 2021 05:16:12 GMT
RUN echo "upload_max_filesize = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "post_max_size = 128M" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "memory_limit = 1G" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_execution_time = 600" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini &&	echo "max_input_vars = 5000" >> /usr/local/etc/php/conf.d/0-upload_large_dumps.ini
# Sat, 01 May 2021 05:16:12 GMT
STOPSIGNAL SIGINT
# Sat, 01 May 2021 05:16:14 GMT
RUN addgroup -S adminer &&	adduser -S -G adminer adminer &&	mkdir -p /var/www/html &&	mkdir -p /var/www/html/plugins-enabled &&	chown -R adminer:adminer /var/www/html
# Sat, 01 May 2021 05:16:15 GMT
WORKDIR /var/www/html
# Sat, 01 May 2021 05:16:55 GMT
RUN set -x &&	apk add --no-cache --virtual .build-deps 	postgresql-dev 	sqlite-dev 	unixodbc-dev 	freetds-dev &&	docker-php-ext-configure pdo_odbc --with-pdo-odbc=unixODBC,/usr &&	docker-php-ext-install 	pdo_mysql 	pdo_pgsql 	pdo_sqlite 	pdo_odbc 	pdo_dblib &&	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" &&	apk add --virtual .phpexts-rundeps $runDeps &&	apk del .build-deps
# Sat, 01 May 2021 05:16:55 GMT
COPY multi:3020a2cf8da93deb4663b2b608f3156b5f8da81b19c0fa615f495168d48abf9c in /var/www/html/ 
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_VERSION=4.8.0
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_DOWNLOAD_SHA256=e274268e0e0f2a6b8040c000a969889062904ae7a5ccbaf013dc890e12e32eaa
# Sat, 01 May 2021 05:16:56 GMT
ENV ADMINER_SRC_DOWNLOAD_SHA256=55b52851faa5661667edb003b00cf520ebeb1e41cfcea4a7fc028ed0f55ff557
# Sat, 01 May 2021 05:16:58 GMT
RUN set -x &&	curl -fsSL https://github.com/vrana/adminer/releases/download/v$ADMINER_VERSION/adminer-$ADMINER_VERSION.php -o adminer.php &&	echo "$ADMINER_DOWNLOAD_SHA256  adminer.php" |sha256sum -c - &&	curl -fsSL https://github.com/vrana/adminer/archive/v$ADMINER_VERSION.tar.gz -o source.tar.gz &&	echo "$ADMINER_SRC_DOWNLOAD_SHA256  source.tar.gz" |sha256sum -c - &&	tar xzf source.tar.gz --strip-components=1 "adminer-$ADMINER_VERSION/designs/" "adminer-$ADMINER_VERSION/plugins/" &&	rm source.tar.gz
# Sat, 01 May 2021 05:16:59 GMT
COPY file:5ff0be587f5dd9166f7a558457b0e656c889de46d3bb2afd41f1714ab2c02ceb in /usr/local/bin/ 
# Sat, 01 May 2021 05:16:59 GMT
ENTRYPOINT ["entrypoint.sh" "docker-php-entrypoint"]
# Sat, 01 May 2021 05:17:00 GMT
USER adminer
# Sat, 01 May 2021 05:17:00 GMT
CMD ["php" "-S" "[::]:8080" "-t" "/var/www/html"]
# Sat, 01 May 2021 05:17:01 GMT
EXPOSE 8080
```

-	Layers:
	-	`sha256:afadee6ad6a38d3172beeeca818219604c782efbe93201ef4d39512f289b05ae`  
		Last Modified: Wed, 14 Apr 2021 18:42:16 GMT  
		Size: 2.6 MB (2602650 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d300c94e92b07eb0727117362a4c02c33a3af45a2c84e27e191b18fd64537ff2`  
		Last Modified: Wed, 14 Apr 2021 20:01:05 GMT  
		Size: 1.8 MB (1760701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21c222b785aeace308f4ae843bd963ab89b5e43b40c39e44819a79a97ab65ffd`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abdca579f326f21cb64727b7a043ef139e61e18d78e009c7aaa0d00c8787d500`  
		Last Modified: Wed, 14 Apr 2021 20:01:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08b7aa20ee47cf4d85a8a033023b14b1948153a005c710022465266b1676ff00`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 10.4 MB (10360232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8c09e3c51bdc12e3dac46e704947a4207380cc86861118e2ba93827f09a479b`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c57065802a25a7373daa5d63b66c55320e705d6ef8e47055d2ba2997ac4ac1f`  
		Last Modified: Sat, 01 May 2021 03:23:19 GMT  
		Size: 13.6 MB (13616029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:08fa2ed8a45355ef77a61d2740ffedf281c9079db17e02fcd213477f4c8bd2f4`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 2.3 KB (2263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d549711db456f1993f2dd16932c69755412329900032bc3250bfff994fd9d43`  
		Last Modified: Sat, 01 May 2021 03:23:17 GMT  
		Size: 17.5 KB (17549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8aa60d82d0a8b59fda860a56dae19ab654de0f1368014f447b7f9c53d96c5584`  
		Last Modified: Sat, 01 May 2021 05:18:16 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e07d3ea1b608b879ac7c8354ab621b511601a964e24706c82764e975896ec2d4`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 1.4 KB (1407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f1128a53bb989ba9202c67883e70c3aa25bfbc7a44e36360de37f23e678dab0`  
		Last Modified: Sat, 01 May 2021 05:18:15 GMT  
		Size: 3.6 MB (3588293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e6ac88d341f35d6278d87a43b3998caa46d2a2d7515df5446755a418c22fb4f`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 1.5 KB (1474 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f46932d8f58943aa96cffad8c4b13a779eb592deacb98d058e46236c40479d28`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 582.8 KB (582808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b32bae7fbe947016896c76b4d5aea4dbb1dd2feb86f7062de658448beb0f326a`  
		Last Modified: Sat, 01 May 2021 05:18:14 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
