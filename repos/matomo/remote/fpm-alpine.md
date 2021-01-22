## `matomo:fpm-alpine`

```console
$ docker pull matomo@sha256:c3a7743669636b9d100ff2a3529fc40c84a2a1b633b2f757662139ecdf6e2aee
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

### `matomo:fpm-alpine` - linux; amd64

```console
$ docker pull matomo@sha256:9703d7fdbb7737f83daf4ac8d2ce2c0cb2ffb84b1ce757a5bc21276f9369e421
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.7 MB (49673015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cff9d5ee69dd0cab26312eae3fcec1e3004d1acbe2c687680a8209d7b596480a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 15 Jan 2021 02:23:51 GMT
ADD file:edbe213ae0c825a5bfbe569928cf20f683f334f93a093ccd0a3a014b7428e760 in / 
# Fri, 15 Jan 2021 02:23:51 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 23:43:21 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 23:43:24 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 23:43:26 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 23:43:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 23:43:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 23:52:00 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 15 Jan 2021 23:52:00 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:52:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:52:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Sat, 16 Jan 2021 00:13:03 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Sat, 16 Jan 2021 00:13:03 GMT
ENV PHP_VERSION=7.4.14
# Sat, 16 Jan 2021 00:13:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Sat, 16 Jan 2021 00:13:04 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Sat, 16 Jan 2021 00:13:08 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 16 Jan 2021 00:13:08 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 16 Jan 2021 00:23:55 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 20:19:52 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 21 Jan 2021 20:19:55 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 20:19:55 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 20:19:56 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 20:19:58 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Jan 2021 20:19:58 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 20:19:58 GMT
EXPOSE 9000
# Thu, 21 Jan 2021 20:19:59 GMT
CMD ["php-fpm"]
# Thu, 21 Jan 2021 23:30:32 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 21 Jan 2021 23:32:28 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.19; 	pecl install redis-5.3.2; 		docker-php-ext-enable 		apcu 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 21 Jan 2021 23:32:29 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 21 Jan 2021 23:32:29 GMT
ENV MATOMO_VERSION=4.1.1
# Thu, 21 Jan 2021 23:32:37 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Thu, 21 Jan 2021 23:32:37 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 21 Jan 2021 23:32:37 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Thu, 21 Jan 2021 23:32:37 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 23:32:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 21 Jan 2021 23:32:38 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:596ba82af5aaa3e2fd9d6f955b8b94f0744a2b60710e3c243ba3e4a467f051d1`  
		Last Modified: Fri, 15 Jan 2021 02:08:10 GMT  
		Size: 2.8 MB (2810825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af74f285bb27c6623f2b5c8c3a2e487603c7dd5c51859fd6e13859542f4310c3`  
		Last Modified: Sat, 16 Jan 2021 01:00:24 GMT  
		Size: 1.7 MB (1694838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ab8440e5667ccb2ffd4e62ed905a106742dfdd7dd3167d9d64b4bdeed8a4945`  
		Last Modified: Sat, 16 Jan 2021 01:00:20 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64889fa545ec919e6fe392c368b8cb41a10e7834c1ba4d4d96fd9ee2e3405cc1`  
		Last Modified: Sat, 16 Jan 2021 01:00:20 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1574f57dd7477afc6537729230a9c1c1b56203348d92f4f7e40962d1d7e7e639`  
		Last Modified: Sat, 16 Jan 2021 01:01:54 GMT  
		Size: 10.3 MB (10346226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9eb0b6a13f93ffbe654b6c829f9a0be28accc453e2372c2ff9035e187916e8f3`  
		Last Modified: Sat, 16 Jan 2021 01:01:50 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc6edb18b1734a7d41a9dd879437b828d368e3e993bb3ae1cd44bf6fae9541a5`  
		Last Modified: Sat, 16 Jan 2021 01:01:53 GMT  
		Size: 14.7 MB (14698701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf63a6c9649702a6b74c071ab4c39f303531a1191d47541cc9ecfd40b7f4a20`  
		Last Modified: Thu, 21 Jan 2021 20:31:29 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec352a4611cbe69170666ad226ce834e66b765ed7aa2adf9fbe410d7b76d856a`  
		Last Modified: Thu, 21 Jan 2021 20:31:31 GMT  
		Size: 17.5 KB (17537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:682a80dc7ae119bfb9d05c0722ec047600f0ea847da044afc6e5319f05363014`  
		Last Modified: Thu, 21 Jan 2021 20:31:31 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0eb49e4ed864f42380da2d2274d38869b11488efa7625e21b99f8ce50ba6b070`  
		Last Modified: Thu, 21 Jan 2021 23:33:48 GMT  
		Size: 5.5 MB (5490019 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d46130e78223646d97397156f0db68608260306e623be5433302fa3e6a150360`  
		Last Modified: Thu, 21 Jan 2021 23:33:48 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12fdcff73e10956e9b0abd07511e34c4f41e284e1b34808c384538938edb0011`  
		Last Modified: Thu, 21 Jan 2021 23:33:53 GMT  
		Size: 14.6 MB (14601345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9d48a76369cc39fe59f0d9b9d3aa57b5f295aa7a32d35c3a4a5a2681008b1ff`  
		Last Modified: Thu, 21 Jan 2021 23:33:47 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c49b21dfab76cc240a6983cac5f86673f40de19808c7a430df624ac89709b28`  
		Last Modified: Thu, 21 Jan 2021 23:33:47 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:fpm-alpine` - linux; arm variant v6

```console
$ docker pull matomo@sha256:964d23b2522cb1fc32bb44619c76589f16235189cd7d8a68b5df576d99cf62c6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.0 MB (48030556 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:254f23b368093be6f1292be67b1d044e4e7f9fdeb12e12d1ceccdf3597b9ee04`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 15 Jan 2021 01:51:19 GMT
ADD file:f2665ccfd90cf53580dc87c3e57db7c223147c686554b1d6e3fc166cce818b3e in / 
# Fri, 15 Jan 2021 01:51:20 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 22:53:55 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 22:53:58 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 22:54:00 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 22:54:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 22:54:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 22:57:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 15 Jan 2021 22:57:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 22:57:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 22:57:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 23:04:53 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 15 Jan 2021 23:04:54 GMT
ENV PHP_VERSION=7.4.14
# Fri, 15 Jan 2021 23:04:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 15 Jan 2021 23:04:57 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 15 Jan 2021 23:05:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:05:05 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:08:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:04:48 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:04:53 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:04:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:04:54 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 19:04:56 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Jan 2021 19:04:56 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 19:04:57 GMT
EXPOSE 9000
# Thu, 21 Jan 2021 19:04:58 GMT
CMD ["php-fpm"]
# Thu, 21 Jan 2021 20:31:45 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 21 Jan 2021 20:34:17 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.19; 	pecl install redis-5.3.2; 		docker-php-ext-enable 		apcu 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 21 Jan 2021 20:34:19 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 21 Jan 2021 20:34:20 GMT
ENV MATOMO_VERSION=4.1.1
# Thu, 21 Jan 2021 20:34:33 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Thu, 21 Jan 2021 20:34:36 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 21 Jan 2021 20:34:37 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Thu, 21 Jan 2021 20:34:38 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 20:34:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 21 Jan 2021 20:34:40 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b550170d5d44558603032e2371fa7a2fb3575b38b2c64ad8be4ab798bcad44d3`  
		Last Modified: Fri, 15 Jan 2021 01:52:01 GMT  
		Size: 2.6 MB (2621576 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3110258b4da6fc6756faa0ee4ede2d02a24ff821ba8f1ba72a75739fc89161fa`  
		Last Modified: Fri, 15 Jan 2021 23:27:01 GMT  
		Size: 1.7 MB (1684838 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef6d6cdd312890c0852fd22903c40d68137566e06f947a0c3461bba58aab6fb`  
		Last Modified: Fri, 15 Jan 2021 23:27:00 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61428ad89e8a3dd97317b0da99d3c4b4f36306fd1b554393af68eea521ad75c`  
		Last Modified: Fri, 15 Jan 2021 23:27:00 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:501e96d58ae0f12c5a1a41afdbb32e1483b1b2c04ca3397b061dafb8cb17cfda`  
		Last Modified: Fri, 15 Jan 2021 23:28:56 GMT  
		Size: 10.3 MB (10346238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8133164fb29d3f035534996fcd855903daae10abf48150745921a635cb886488`  
		Last Modified: Fri, 15 Jan 2021 23:28:54 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fceb2932ca7e517d29e62262eb0b808e81373d1c0783c35acbdfeb76bd494293`  
		Last Modified: Fri, 15 Jan 2021 23:28:59 GMT  
		Size: 13.7 MB (13693430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94b07309fe7a769cb2cdc0997e6877b11a6a4460a2e202a4d518f7dbd166bd8e`  
		Last Modified: Thu, 21 Jan 2021 19:11:11 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d488dce450026098bc3d57f1d17c3aaf3dd1c160c9842f7c3098d84d50eca48`  
		Last Modified: Thu, 21 Jan 2021 19:11:12 GMT  
		Size: 17.5 KB (17540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3adff18a0e168726716ffe8e95f4c281dc85983a0121c24b6c0d5058e69ba9`  
		Last Modified: Thu, 21 Jan 2021 19:11:12 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29c7638e2c9f3919d97c2f93d4c6e0bab1b119e3dca5de219ea783764f8e8764`  
		Last Modified: Thu, 21 Jan 2021 20:35:03 GMT  
		Size: 5.1 MB (5051973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4049ebd438b7666b9a40fed4f9d265b1f97838e97ba727957ce7c64fcc18b25`  
		Last Modified: Thu, 21 Jan 2021 20:35:02 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b7bfdbe65955f6c3432db326e57450a0309860cad1ccb4f3c13224b7ce070da`  
		Last Modified: Thu, 21 Jan 2021 20:35:32 GMT  
		Size: 14.6 MB (14601361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9795d79af691da135173e879d15ba3255c3ebfddd4f039c580484a4ce91a47cf`  
		Last Modified: Thu, 21 Jan 2021 20:35:01 GMT  
		Size: 307.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8eec8b2e18a813688432ae53d0264b29224077fe5c85e11f455ee8eb22037d`  
		Last Modified: Thu, 21 Jan 2021 20:35:00 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:fpm-alpine` - linux; arm variant v7

```console
$ docker pull matomo@sha256:19213de88a605d582e457b88119fc792293522581d6bbefa32afce453948ea06
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46842447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c446529fc05d3090cec8f85f1aacd9da9d82b1e9b1c664161d415d873da7b22`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 15 Jan 2021 01:58:27 GMT
ADD file:718d7c24a8d6ff0feb2843cf8c3ca4b7ef1fb523a45dea568404259a7b4e6f10 in / 
# Fri, 15 Jan 2021 01:58:29 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 23:04:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 23:04:05 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 23:04:07 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 23:04:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 23:04:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 23:08:08 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 15 Jan 2021 23:08:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:08:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:08:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 23:16:20 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 15 Jan 2021 23:16:21 GMT
ENV PHP_VERSION=7.4.14
# Fri, 15 Jan 2021 23:16:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 15 Jan 2021 23:16:23 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 15 Jan 2021 23:16:29 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:16:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:19:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:12:36 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:12:39 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:12:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:12:42 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 19:12:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Jan 2021 19:12:44 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 19:12:45 GMT
EXPOSE 9000
# Thu, 21 Jan 2021 19:12:46 GMT
CMD ["php-fpm"]
# Fri, 22 Jan 2021 00:19:40 GMT
LABEL maintainer=pierre@piwik.org
# Fri, 22 Jan 2021 00:21:59 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.19; 	pecl install redis-5.3.2; 		docker-php-ext-enable 		apcu 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Fri, 22 Jan 2021 00:22:02 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 22 Jan 2021 00:22:03 GMT
ENV MATOMO_VERSION=4.1.1
# Fri, 22 Jan 2021 00:22:21 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Fri, 22 Jan 2021 00:22:24 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Fri, 22 Jan 2021 00:22:25 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Fri, 22 Jan 2021 00:22:26 GMT
VOLUME [/var/www/html]
# Fri, 22 Jan 2021 00:22:27 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 22 Jan 2021 00:22:29 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:0f34ce5da94097b8c334f6b2065a010aced9855c3532e4462e9bd1b0a4c4b3f6`  
		Last Modified: Fri, 15 Jan 2021 01:59:13 GMT  
		Size: 2.4 MB (2422744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cecec77a7b5b50913bcb9f7bfe0c5fdcebb948b947747285290197c13902be91`  
		Last Modified: Fri, 15 Jan 2021 23:42:36 GMT  
		Size: 1.6 MB (1555130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0496082b3c55009a50b47ce80bf27dd7451aaa7e13b5b4ccbe886a780c614dd1`  
		Last Modified: Fri, 15 Jan 2021 23:42:33 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af351861d88fff830659b71d51e45b8e623d31cb86c764fab107e6c39ca5a717`  
		Last Modified: Fri, 15 Jan 2021 23:42:33 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b641e2b9da12e18bef312739ada811a79b50ce5892b425292468662ef536b8b0`  
		Last Modified: Fri, 15 Jan 2021 23:44:59 GMT  
		Size: 10.3 MB (10346235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3dc9fd32bbef60ac4128a4c440ce73f136bda82cb0e7fb09d6340e33c251770`  
		Last Modified: Fri, 15 Jan 2021 23:44:55 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80249d618c0703ada578087f1f9d0bfcb4cfcfee735c95aeed1766d38d1dd6ba`  
		Last Modified: Fri, 15 Jan 2021 23:44:59 GMT  
		Size: 12.8 MB (12818131 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb2d4866cbb138499291928931dbb6a9076b7797a4d2753c0560307460388d7`  
		Last Modified: Thu, 21 Jan 2021 19:27:34 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6e03d6251ca595a2d8b2f0c2d62078ebdf5ec94000180fca49088aa1a916ec0`  
		Last Modified: Thu, 21 Jan 2021 19:27:36 GMT  
		Size: 17.5 KB (17535 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff4a52522143794d8a541271ce7e596f51ca77582587bba2bf8539bb5271a5b`  
		Last Modified: Thu, 21 Jan 2021 19:27:36 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb90627c812f5e25ec1bbfa90d233af6034133b2dfcb5c5ffa09261ed3eb304b`  
		Last Modified: Fri, 22 Jan 2021 00:24:02 GMT  
		Size: 5.1 MB (5067718 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68a9ea6d037606455dfe4f9f9054797c5f725ab01c7f442eb229b94e4a8aa139`  
		Last Modified: Fri, 22 Jan 2021 00:24:00 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac409b9c4d9c28a3c8ef988141c2a16533ea58a2347e683594bd485c3835993`  
		Last Modified: Fri, 22 Jan 2021 00:24:07 GMT  
		Size: 14.6 MB (14601353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4178a4432e8d8276ce5d27e0e91d4dac921bc8a37960a56b1e0634f01675ed40`  
		Last Modified: Fri, 22 Jan 2021 00:24:01 GMT  
		Size: 311.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2358f1f70df50033a1d0e50b45944a7947014829b01e174dd68f0a9625a5ee8`  
		Last Modified: Fri, 22 Jan 2021 00:24:02 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull matomo@sha256:8fac0306a44d6174f3a6567c7d068f1a64f615e0782e139e3222cdeea0852351
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.3 MB (49290796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0e4afbbabe2eacefd053ff3b16beabd77c449498c87e942ed1912304e038ab3`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 15 Jan 2021 01:47:51 GMT
ADD file:95be2cec37537b3fd70aeb1d4eb3479fc4a56b00ad7180788ddd7fa772ca65e7 in / 
# Fri, 15 Jan 2021 01:47:52 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 23:04:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 23:04:24 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 23:04:28 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 23:04:32 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 23:04:35 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 23:09:58 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 15 Jan 2021 23:09:59 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:10:00 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:10:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 23:20:47 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 15 Jan 2021 23:20:49 GMT
ENV PHP_VERSION=7.4.14
# Fri, 15 Jan 2021 23:20:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 15 Jan 2021 23:20:55 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 15 Jan 2021 23:21:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:21:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:25:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:54:16 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:54:21 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:54:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:54:22 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 19:54:24 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Jan 2021 19:54:25 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 19:54:26 GMT
EXPOSE 9000
# Thu, 21 Jan 2021 19:54:27 GMT
CMD ["php-fpm"]
# Thu, 21 Jan 2021 23:41:34 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 21 Jan 2021 23:44:09 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.19; 	pecl install redis-5.3.2; 		docker-php-ext-enable 		apcu 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 21 Jan 2021 23:44:13 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 21 Jan 2021 23:44:15 GMT
ENV MATOMO_VERSION=4.1.1
# Thu, 21 Jan 2021 23:44:28 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Thu, 21 Jan 2021 23:44:31 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 21 Jan 2021 23:44:33 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Thu, 21 Jan 2021 23:44:34 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 23:44:35 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 21 Jan 2021 23:44:36 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:30d5333d20a68dd6ea3689e2c5692d7071f2d68e72c06f0b3b4c7e213df454e2`  
		Last Modified: Fri, 15 Jan 2021 01:48:29 GMT  
		Size: 2.7 MB (2710904 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b72077bc47778707d4c51904bf6932e44a09d9a5a37f1bac45ef59fe94bc54e1`  
		Last Modified: Fri, 15 Jan 2021 23:49:43 GMT  
		Size: 1.7 MB (1694577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81bfc628cf72db6285835ff062834a15ee7c9067f6b7ccb55fad0a8bb0f292be`  
		Last Modified: Fri, 15 Jan 2021 23:49:41 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5ab015e378a2ad2e4c345884006fc6b1678a0ebba44214fbc5e9dcb48ef7bb2`  
		Last Modified: Fri, 15 Jan 2021 23:49:41 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:792cc737729aa6e718b720be680dbc48c988bb8eb87d736d1fc409b737e2ffe0`  
		Last Modified: Fri, 15 Jan 2021 23:52:03 GMT  
		Size: 10.3 MB (10346269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b873d49dc5a9b2322c7457957bada740ad7aee44f3cf2d7536c0d07f891712db`  
		Last Modified: Fri, 15 Jan 2021 23:52:00 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a593da87207d671fd075a4337d248d0823427f55cbfba9e1c64a91f9282e5706`  
		Last Modified: Fri, 15 Jan 2021 23:52:03 GMT  
		Size: 14.5 MB (14490136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5847e0687002fdc5c4d260cc9c1d30146fe5139b2e4efd91078c4b4387633423`  
		Last Modified: Thu, 21 Jan 2021 20:08:57 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1d63d1a823bd3f6f80d87ad4b5bfceb4e6b50d2280f685b8596b0946f85c463`  
		Last Modified: Thu, 21 Jan 2021 20:08:58 GMT  
		Size: 17.6 KB (17552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3cdd544ac1b539bfc9d7c4c5c4cb947e6643675467f9ab7b3323b44e69dd54e`  
		Last Modified: Thu, 21 Jan 2021 20:08:56 GMT  
		Size: 8.4 KB (8448 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18cffcbb3bd51aa8a65522d5c90d882f322a04f0418df6c09e2fd7f2fa01f30d`  
		Last Modified: Thu, 21 Jan 2021 23:46:00 GMT  
		Size: 5.4 MB (5416407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fae8a91ea32c69a1bf767164784ddbc15809a42cd44f7e1e1368bd4230e3a523`  
		Last Modified: Thu, 21 Jan 2021 23:45:59 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427171fe7a0fc290d1eb9082cdc93cc4a0c3e568001119089f485ad9859f5cd0`  
		Last Modified: Thu, 21 Jan 2021 23:46:03 GMT  
		Size: 14.6 MB (14601350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3c75090fdb2852603e2df61ef72c471e479f45e54932a078525c8c8c847166b`  
		Last Modified: Thu, 21 Jan 2021 23:45:58 GMT  
		Size: 306.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0064ce4057140ed19bf2dcd48e1d4d6f33deeecdcbbd00c3705edb4032e3cf3`  
		Last Modified: Thu, 21 Jan 2021 23:45:58 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:fpm-alpine` - linux; 386

```console
$ docker pull matomo@sha256:960410e28e404b0bc1cb4a5ddfc3a57d92f5ad1d087e93b1b61fc212c20803fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50147449 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54318580446c644c464fc716b64bff8ab0216b77e85c0401fdd391cce4b9fab5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 15 Jan 2021 01:38:28 GMT
ADD file:d8723c02f1eb0efa4dadc6480a753d18d7e28d9815bff96a92ff09ff55a92b11 in / 
# Fri, 15 Jan 2021 01:38:29 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 22:42:20 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 22:42:22 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 22:42:23 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 22:42:23 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 22:42:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 22:49:42 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 15 Jan 2021 22:49:43 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 22:49:43 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 22:49:43 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 23:04:49 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 15 Jan 2021 23:04:49 GMT
ENV PHP_VERSION=7.4.14
# Fri, 15 Jan 2021 23:04:49 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 15 Jan 2021 23:04:50 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 15 Jan 2021 23:04:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:04:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:11:47 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:46:50 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:46:52 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:46:53 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:46:53 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 19:46:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Jan 2021 19:46:55 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 19:46:56 GMT
EXPOSE 9000
# Thu, 21 Jan 2021 19:46:56 GMT
CMD ["php-fpm"]
# Thu, 21 Jan 2021 21:29:58 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 21 Jan 2021 21:31:45 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.19; 	pecl install redis-5.3.2; 		docker-php-ext-enable 		apcu 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 21 Jan 2021 21:31:46 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 21 Jan 2021 21:31:46 GMT
ENV MATOMO_VERSION=4.1.1
# Thu, 21 Jan 2021 21:31:55 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Thu, 21 Jan 2021 21:31:56 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 21 Jan 2021 21:31:56 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Thu, 21 Jan 2021 21:31:56 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 21:31:57 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 21 Jan 2021 21:31:57 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:9e6a151110e36daa7a487250f98425289313f856e3a586d89d82bafc1bf322c3`  
		Last Modified: Fri, 15 Jan 2021 01:39:01 GMT  
		Size: 2.8 MB (2817152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46b194694eae0c8525a66d3c56796eb37a9e263d63f03eaecf6bc83d2ab3f7c9`  
		Last Modified: Fri, 15 Jan 2021 23:50:55 GMT  
		Size: 1.8 MB (1793505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99a9a95dec7f2cd3bcf6903d006a870fa7113f6a974d30ec6634ab82b0a0a792`  
		Last Modified: Fri, 15 Jan 2021 23:50:52 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5ad687f5cfc54121cc70af5ff69cb844177c4325a2c14efcd144cb096ecfba2`  
		Last Modified: Fri, 15 Jan 2021 23:50:54 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88e10b48d67881d4e60a8e47d6b24b5ee0eec86c60e97b307f2b8b3cd187cf29`  
		Last Modified: Fri, 15 Jan 2021 23:52:38 GMT  
		Size: 10.3 MB (10346200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54ef2b1b94c7b36b4e0ebe4e26c202cc8f2c8ebb05a20dccc525e0043ced685`  
		Last Modified: Fri, 15 Jan 2021 23:52:35 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b498664a2a3d8e77b1493ab6788504c38a11f035555733715aae3a79ae8dc6d8`  
		Last Modified: Fri, 15 Jan 2021 23:52:43 GMT  
		Size: 15.1 MB (15062200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55fa1a93ccdadbd73f469217b030bfb85a3fd375a8434b4cb846196b3cd1d28d`  
		Last Modified: Thu, 21 Jan 2021 19:58:54 GMT  
		Size: 2.3 KB (2265 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf92eae98f53a6f40b4245d24fe6c7acbdec1add0ac604feef9d207f5acca0c6`  
		Last Modified: Thu, 21 Jan 2021 19:58:54 GMT  
		Size: 17.5 KB (17525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e687d5f6f0aabedaa33d0d40eb9f42228fda786a6a1fc16b09f13137f019cb84`  
		Last Modified: Thu, 21 Jan 2021 19:58:54 GMT  
		Size: 8.4 KB (8449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e9809348c03c9657c671607f152b0ec06a4ea37eb6d675581e10dfd43769817`  
		Last Modified: Thu, 21 Jan 2021 21:33:21 GMT  
		Size: 5.5 MB (5496078 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f564979159f2ae010349b7faf9e4eab37b15a96ce2b38c31f15d675a49b7ab3`  
		Last Modified: Thu, 21 Jan 2021 21:33:19 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfbfa0b42f25a050de6f302a0f4776f11c8e898d2832293868d48d09224ce644`  
		Last Modified: Thu, 21 Jan 2021 21:33:24 GMT  
		Size: 14.6 MB (14601269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27f10180c2ccdca1172a992e8e51d25318eae07a4de301ffd3af18377466c244`  
		Last Modified: Thu, 21 Jan 2021 21:33:19 GMT  
		Size: 308.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20d008dd1b62f398019868afc9ecb61e4058c35ec7e8ad354fcf30bb92d9ba2e`  
		Last Modified: Thu, 21 Jan 2021 21:33:18 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:fpm-alpine` - linux; ppc64le

```console
$ docker pull matomo@sha256:9a8a3eaafae83e4ac8246d7dcfa4e16aa982626add0e11b403a20e311ffcc403
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.8 MB (50831710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6cb972d185358e1b1866b207b0a49a912c45ca9e930904dbb2f2e6e5960eceda`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 15 Jan 2021 02:41:43 GMT
ADD file:137e8f98476d5dceaeb2e8359f50eb818dee4c327e4492d16e87fb27d40aa891 in / 
# Fri, 15 Jan 2021 02:41:46 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 23:17:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 23:17:44 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 23:17:56 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 23:18:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 23:18:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 23:25:54 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 15 Jan 2021 23:26:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:26:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:26:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 23:39:37 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 15 Jan 2021 23:39:45 GMT
ENV PHP_VERSION=7.4.14
# Fri, 15 Jan 2021 23:39:48 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 15 Jan 2021 23:39:51 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 15 Jan 2021 23:40:02 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:40:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:44:46 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Fri, 15 Jan 2021 23:44:50 GMT
COPY multi:ebc915bbde1078ce3122b918e2e4c7726858af785343ade1a8d1a94f1052a4c7 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:45:01 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 Jan 2021 23:45:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 Jan 2021 23:45:09 GMT
WORKDIR /var/www/html
# Fri, 15 Jan 2021 23:45:16 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 15 Jan 2021 23:45:20 GMT
STOPSIGNAL SIGQUIT
# Fri, 15 Jan 2021 23:45:26 GMT
EXPOSE 9000
# Fri, 15 Jan 2021 23:45:29 GMT
CMD ["php-fpm"]
# Sat, 16 Jan 2021 01:26:42 GMT
LABEL maintainer=pierre@piwik.org
# Sat, 16 Jan 2021 01:29:01 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.19; 	pecl install redis-5.3.2; 		docker-php-ext-enable 		apcu 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Sat, 16 Jan 2021 01:29:14 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 16 Jan 2021 01:29:17 GMT
ENV MATOMO_VERSION=4.1.1
# Sat, 16 Jan 2021 01:29:36 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Sat, 16 Jan 2021 01:29:40 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Sat, 16 Jan 2021 01:29:43 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Sat, 16 Jan 2021 01:29:47 GMT
VOLUME [/var/www/html]
# Sat, 16 Jan 2021 01:29:50 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 16 Jan 2021 01:29:54 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:cb0f06c26ffdc2117b9a3467f79e69cdf8d9c677a3c0bacabc8a694a9fe303a8`  
		Last Modified: Fri, 15 Jan 2021 02:42:19 GMT  
		Size: 2.8 MB (2812389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb9a7aad5bd113c5dca33b681663b0c58f66e510017e693801a6688a9c4bab60`  
		Last Modified: Sat, 16 Jan 2021 00:14:01 GMT  
		Size: 1.7 MB (1741834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45ce1d80ff72759b98cf2f5ad1efa6dd181e5f4343bb0e25cbb4ec9d5d3847f4`  
		Last Modified: Sat, 16 Jan 2021 00:14:01 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48055526d8202af50f6248db9b3cb8938cab9cfec15a1312b4c1e3782f3307c4`  
		Last Modified: Sat, 16 Jan 2021 00:14:02 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a94ca067e23579248e149be4715ec5f2901e93a3c90da6ad15714ea10459957e`  
		Last Modified: Sat, 16 Jan 2021 00:16:47 GMT  
		Size: 10.3 MB (10346247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd8c2745c3d8eff18c4dea197abf3612dc043b641c2bc851c160d3d7c16491f6`  
		Last Modified: Sat, 16 Jan 2021 00:16:41 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786720966d074fc141c61f61755f50f52b12496acf7336780585a6dcfc5de151`  
		Last Modified: Sat, 16 Jan 2021 00:16:46 GMT  
		Size: 15.7 MB (15739967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf3deaf362ddab68947e98e70b9f7035cac2d1a4f47807174e3e34d4ed1e92b1`  
		Last Modified: Sat, 16 Jan 2021 00:16:41 GMT  
		Size: 2.3 KB (2255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae6beae6370449fadf46fcb853a7870a689ce0525957ab8a0388339927d48a2`  
		Last Modified: Sat, 16 Jan 2021 00:16:41 GMT  
		Size: 17.5 KB (17525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b93eef73081f3f01d63acca16ac3c8cef83230ac9bc203297a13a4babaa639ee`  
		Last Modified: Sat, 16 Jan 2021 00:16:41 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0cb8c291b942dc2e67bfe9545260bfd547003cecb6f59ee861ee661440ea8e8`  
		Last Modified: Sat, 16 Jan 2021 01:30:34 GMT  
		Size: 5.6 MB (5558803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5eb98a53632fe1deb02921fa2c4344cb41aa01dfbbe2f7ba54c387a3c4b4b30`  
		Last Modified: Sat, 16 Jan 2021 01:30:32 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c53602ec205091e9346f341209a413f1c44bd4f2c22af3797c414a157417789`  
		Last Modified: Sat, 16 Jan 2021 01:30:38 GMT  
		Size: 14.6 MB (14601368 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ceb5019978611c5efda9fadbed813528ab2245db89461920e69547d49eb76ed`  
		Last Modified: Sat, 16 Jan 2021 01:30:32 GMT  
		Size: 305.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1da6f61bb98d2fe35a746ee7872b67aa4b7e9e2f592fb07e6fc4a2461e821fd8`  
		Last Modified: Sat, 16 Jan 2021 01:30:32 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `matomo:fpm-alpine` - linux; s390x

```console
$ docker pull matomo@sha256:534dc92ddcc48877d67fc2dae00152baca823a49da61cc2a102a35fdf7c76757
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.5 MB (48531053 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2b3daed908f3f60b62f8db8e33b3ae997db69d7631fa0ca24e552f4262bac479`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 15 Jan 2021 01:51:34 GMT
ADD file:3ba807ca8ed73ca14224dd26a883f2399031fa32430f035cc5ae97b5e6db0ca7 in / 
# Fri, 15 Jan 2021 01:51:35 GMT
CMD ["/bin/sh"]
# Fri, 15 Jan 2021 22:57:04 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 15 Jan 2021 22:57:12 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 15 Jan 2021 22:57:13 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 15 Jan 2021 22:57:14 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 15 Jan 2021 22:57:15 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 15 Jan 2021 23:02:27 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 15 Jan 2021 23:02:27 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:02:28 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 15 Jan 2021 23:02:28 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 15 Jan 2021 23:12:03 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 15 Jan 2021 23:12:04 GMT
ENV PHP_VERSION=7.4.14
# Fri, 15 Jan 2021 23:12:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.14.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.14.tar.xz.asc
# Fri, 15 Jan 2021 23:12:05 GMT
ENV PHP_SHA256=f9f3c37969fcd9006c1dbb1dd76ab53f28c698a1646fa2dde8547c3f45e02886
# Fri, 15 Jan 2021 23:12:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 Jan 2021 23:12:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 Jan 2021 23:17:09 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 21 Jan 2021 19:55:56 GMT
COPY multi:6dfba8f7e64bd54e4d9aa0855ff6ce7a53059e0a733752b4537fd3fdfd32d837 in /usr/local/bin/ 
# Thu, 21 Jan 2021 19:55:58 GMT
RUN docker-php-ext-enable sodium
# Thu, 21 Jan 2021 19:55:59 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 21 Jan 2021 19:55:59 GMT
WORKDIR /var/www/html
# Thu, 21 Jan 2021 19:56:01 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 21 Jan 2021 19:56:02 GMT
STOPSIGNAL SIGQUIT
# Thu, 21 Jan 2021 19:56:03 GMT
EXPOSE 9000
# Thu, 21 Jan 2021 19:56:03 GMT
CMD ["php-fpm"]
# Thu, 21 Jan 2021 23:22:57 GMT
LABEL maintainer=pierre@piwik.org
# Thu, 21 Jan 2021 23:25:15 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		freetype-dev 		icu-dev 		libjpeg-turbo-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 	; 		docker-php-ext-configure gd --with-freetype --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		gd 		ldap 		mysqli 		opcache 		pdo_mysql 		zip 	; 		pecl install APCu-5.1.19; 	pecl install redis-5.3.2; 		docker-php-ext-enable 		apcu 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .matomo-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 21 Jan 2021 23:25:17 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 21 Jan 2021 23:25:18 GMT
ENV MATOMO_VERSION=4.1.1
# Thu, 21 Jan 2021 23:25:32 GMT
RUN set -ex; 	apk add --no-cache --virtual .fetch-deps 		gnupg 	; 		curl -fsSL -o matomo.tar.gz 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz"; 	curl -fsSL -o matomo.tar.gz.asc 		"https://builds.matomo.org/matomo-${MATOMO_VERSION}.tar.gz.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys 814E346FA01A20DBB04B6807B5DBD5925590A237; 	gpg --batch --verify matomo.tar.gz.asc matomo.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" matomo.tar.gz.asc; 	tar -xzf matomo.tar.gz -C /usr/src/; 	rm matomo.tar.gz; 	apk del .fetch-deps
# Thu, 21 Jan 2021 23:25:38 GMT
COPY file:5a36d7fba12e383595e7235267e54c5714dbf865acd4c4596c92ac0f17d139b3 in /usr/local/etc/php/conf.d/php-matomo.ini 
# Thu, 21 Jan 2021 23:25:38 GMT
COPY file:0fafaeb399f05cbf0a84d0276a6353eb053cd1a1537e5631be96c2a2ffa2fd31 in /entrypoint.sh 
# Thu, 21 Jan 2021 23:25:39 GMT
VOLUME [/var/www/html]
# Thu, 21 Jan 2021 23:25:39 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 21 Jan 2021 23:25:40 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3997176601fb5d5ac06922718668ede4acac00a5c0daef8a9099fd76ce93047f`  
		Last Modified: Fri, 15 Jan 2021 01:52:40 GMT  
		Size: 2.6 MB (2601720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:497e79d9095f9ba4812f1150c33ad07d399f559fea8e3c4fe8553e02f2cf8b6a`  
		Last Modified: Fri, 15 Jan 2021 23:39:10 GMT  
		Size: 1.8 MB (1756352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99527660904ffc5aed1d27bb86166f189e04b5df76d7becf74efffb1836eaf5e`  
		Last Modified: Fri, 15 Jan 2021 23:39:10 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd9b51111e1ef5a5156e505d6369bb2d4e21354a1203636fca6f26de34df9c15`  
		Last Modified: Fri, 15 Jan 2021 23:39:10 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92d269e26eca744ab118d303ed1eac4fca6b7baa5e74aea3e5f37f74dfe29114`  
		Last Modified: Fri, 15 Jan 2021 23:45:52 GMT  
		Size: 10.3 MB (10346239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d8122b6ee9e9743feec1e0415d4126b817779545ecdee127a76ad836819965`  
		Last Modified: Fri, 15 Jan 2021 23:45:49 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b24745045083bc2b62ee123b2d4a91ac9e43bf73b286436cce7be1603699771`  
		Last Modified: Fri, 15 Jan 2021 23:45:51 GMT  
		Size: 14.1 MB (14073331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4a74b4ad33c850bb801a49b3a8df1143213b4b0d2a38cc3abf75690316aecc8`  
		Last Modified: Thu, 21 Jan 2021 20:09:53 GMT  
		Size: 2.3 KB (2269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c20dcfe6a580282a8a796e47ca221251c3aa76fa4664044336a65584e6f86b44`  
		Last Modified: Thu, 21 Jan 2021 20:09:53 GMT  
		Size: 17.5 KB (17542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b01ee49cb611b3b49831bf0d7603b930ae4af07d23f472d6e1274cd50d8a998`  
		Last Modified: Thu, 21 Jan 2021 20:09:54 GMT  
		Size: 8.4 KB (8449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b34dcc8c666a0d14f61cda7cb33aedeca1daa3e4d0feed4a7929d2c8dce6b2ad`  
		Last Modified: Thu, 21 Jan 2021 23:27:26 GMT  
		Size: 5.1 MB (5120844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cff66d0b1644127af714ea320df46c55e010610d5b4aeb8290a1132133bd0bc`  
		Last Modified: Thu, 21 Jan 2021 23:27:26 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a489693adcf077695b5ade997002f87f0c3285ff13300c0e22bb82635c65ecfc`  
		Last Modified: Thu, 21 Jan 2021 23:27:28 GMT  
		Size: 14.6 MB (14601424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6019988b5cd25b85fff0920e969d95bb606b8b37f1def128f63ec91f77f6e17`  
		Last Modified: Thu, 21 Jan 2021 23:27:26 GMT  
		Size: 310.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939ea62d99e7e2bcc04637c71f2b3053360d64e58f6b1c798740c8b93b975ee2`  
		Last Modified: Thu, 21 Jan 2021 23:27:24 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
