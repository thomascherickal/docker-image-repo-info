## `yourls:1-fpm-alpine`

```console
$ docker pull yourls@sha256:0ddca7af0702bc5721b509a1f1a9c6d4e2bee571b89ccf2fd704664fa3e9a20b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `yourls:1-fpm-alpine` - linux; amd64

```console
$ docker pull yourls@sha256:2ab8aa24049bf4e120ebd8b3e9e23ef7ccdafb489848f1e4e9f8174cac406d0a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.0 MB (34045359 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7440a2bd6693cffa42698220328aeb4f16c09a88d374ddb6db6bf4048c671f81`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:19:34 GMT
ADD file:0c4555f363c2672e350001f1293e689875a3760afe7b3f9146886afe67121cba in / 
# Mon, 23 Mar 2020 21:19:34 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 01:18:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 01:18:34 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 01:18:35 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 01:18:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 01:18:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 01:27:38 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 01:27:38 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 01:27:38 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 17 Apr 2020 11:58:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 17 Apr 2020 14:53:29 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 17 Apr 2020 22:44:55 GMT
ENV PHP_VERSION=7.2.30
# Fri, 17 Apr 2020 22:44:55 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.30.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.30.tar.xz.asc/from/this/mirror
# Fri, 17 Apr 2020 22:44:55 GMT
ENV PHP_SHA256=aa93df27b58a45d6c9800ac813245dfdca03490a918ebe515b3a70189b1bf8c3 PHP_MD5=
# Fri, 17 Apr 2020 22:44:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 17 Apr 2020 22:45:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 17 Apr 2020 22:53:43 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 17 Apr 2020 22:53:44 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 17 Apr 2020 22:53:46 GMT
RUN docker-php-ext-enable sodium
# Fri, 17 Apr 2020 22:53:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 17 Apr 2020 22:53:47 GMT
WORKDIR /var/www/html
# Fri, 17 Apr 2020 22:53:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 17 Apr 2020 22:53:48 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Apr 2020 22:53:49 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 22:53:49 GMT
CMD ["php-fpm"]
# Sat, 18 Apr 2020 00:15:29 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Sat, 18 Apr 2020 00:15:30 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 18 Apr 2020 00:15:31 GMT
RUN apk add --no-cache bash
# Sat, 18 Apr 2020 00:15:31 GMT
ENV YOURLS_VERSION=1.7.6
# Sat, 18 Apr 2020 00:15:32 GMT
ENV YOURLS_SHA256=f3623af6e4cabee61a39d3deca3c941717c5e0a60bc288b6f3a668f87a20ae2e
# Sat, 18 Apr 2020 00:15:33 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 18 Apr 2020 00:15:33 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Sat, 18 Apr 2020 00:15:33 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Sat, 18 Apr 2020 00:15:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Apr 2020 00:15:34 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:aad63a9339440e7c3e1fff2b988991b9bfb81280042fa7f39a5e327023056819`  
		Last Modified: Mon, 23 Mar 2020 21:19:53 GMT  
		Size: 2.8 MB (2803255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b61c449d5d9102f11bc559aba323f82389b7be6118dea453e8273a7f8cc971ea`  
		Last Modified: Tue, 24 Mar 2020 02:42:25 GMT  
		Size: 1.4 MB (1354647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3fde16e1397a31e46a1030c8f769012ebe10f171fc564c77a692053c845975ff`  
		Last Modified: Tue, 24 Mar 2020 02:42:24 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1096698ab2a54e6370c1f2b9c6bb71ae2bb54e306f246aa436b77e1351ff1cf`  
		Last Modified: Tue, 24 Mar 2020 02:42:25 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:381ffbcaa997dce4a769b396ef067b6fb9098fe996ba2b75dd2df523a168b12d`  
		Last Modified: Fri, 17 Apr 2020 23:37:33 GMT  
		Size: 12.3 MB (12303502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35416e20ade5da4488f598d9086a2ae353311a6a740dd34cc92e08ddbbc7d34e`  
		Last Modified: Fri, 17 Apr 2020 23:37:30 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67a50055a278a41d646aa0c6415341617cf28e175513cc7408ca0dce77642f77`  
		Last Modified: Fri, 17 Apr 2020 23:37:35 GMT  
		Size: 14.2 MB (14203884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d26e40cd0d5c86ec5b2af2f894127c2fad724bc01c9fa5451fe446461cf205b8`  
		Last Modified: Fri, 17 Apr 2020 23:37:30 GMT  
		Size: 2.2 KB (2217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60830a6244eeec28bf5d2d621652aa2796bdf9a2db64d7d581429eafcf12d9c1`  
		Last Modified: Fri, 17 Apr 2020 23:37:30 GMT  
		Size: 17.1 KB (17063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6347356cdc3c118b5f0d00e36e9679b4a2a8355b87cb1542bb243b285e6b71e9`  
		Last Modified: Fri, 17 Apr 2020 23:37:30 GMT  
		Size: 7.8 KB (7782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44d07d86feec1d4ba2beb08fd7e700c3aa27ee163418ef112b8618046eb3e6c2`  
		Last Modified: Sat, 18 Apr 2020 00:16:09 GMT  
		Size: 304.9 KB (304920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5650de30e713e12023f1806a4030303c463fdae8e5d8a30447287fc052989b2a`  
		Last Modified: Sat, 18 Apr 2020 00:16:08 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960afcd3d04826204f9ed03bc7aa4c8f44369c6c95b9f798f07214092fbf065d`  
		Last Modified: Sat, 18 Apr 2020 00:16:08 GMT  
		Size: 557.5 KB (557530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cacd5a7ba8ac9dd1f3ff6e181edefc228a210299d8dc62a0c9c729ac843a9b37`  
		Last Modified: Sat, 18 Apr 2020 00:16:10 GMT  
		Size: 2.5 MB (2485253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31b0536d468d1e8af4ba655a61a21b96324123dd25310e8604cff8c9668384e5`  
		Last Modified: Sat, 18 Apr 2020 00:16:08 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21d19a7cc3864983f1d79fac0f6188a608521d1cb055ad6471f843b878b89dda`  
		Last Modified: Sat, 18 Apr 2020 00:16:08 GMT  
		Size: 1.9 KB (1853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; arm variant v6

```console
$ docker pull yourls@sha256:aeb8680615feea64cbe7658f105cac9b5013a8801154857c2eed23956436f62a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.8 MB (32783699 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d1abd9bf50d3d85915798b6b02dcc126f02e90c756a84b2c3f74942f9b645d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:49:26 GMT
ADD file:e2fdfc637b534345942caf4097883508a5ed23be97d85ccc3357b8277aaa5430 in / 
# Mon, 23 Mar 2020 21:49:27 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 02:16:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 02:16:45 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 02:16:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 02:16:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 02:16:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 02:21:00 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 02:21:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 02:21:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 17 Apr 2020 07:54:46 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 17 Apr 2020 08:45:48 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 17 Apr 2020 21:39:53 GMT
ENV PHP_VERSION=7.2.30
# Fri, 17 Apr 2020 21:39:54 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.30.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.30.tar.xz.asc/from/this/mirror
# Fri, 17 Apr 2020 21:39:56 GMT
ENV PHP_SHA256=aa93df27b58a45d6c9800ac813245dfdca03490a918ebe515b3a70189b1bf8c3 PHP_MD5=
# Fri, 17 Apr 2020 21:40:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 17 Apr 2020 21:40:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 17 Apr 2020 21:44:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 17 Apr 2020 21:44:08 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 17 Apr 2020 21:44:11 GMT
RUN docker-php-ext-enable sodium
# Fri, 17 Apr 2020 21:44:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 17 Apr 2020 21:44:13 GMT
WORKDIR /var/www/html
# Fri, 17 Apr 2020 21:44:15 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 17 Apr 2020 21:44:15 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Apr 2020 21:44:16 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 21:44:17 GMT
CMD ["php-fpm"]
# Fri, 17 Apr 2020 22:27:34 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Fri, 17 Apr 2020 22:27:36 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 17 Apr 2020 22:27:40 GMT
RUN apk add --no-cache bash
# Fri, 17 Apr 2020 22:27:44 GMT
ENV YOURLS_VERSION=1.7.6
# Fri, 17 Apr 2020 22:27:45 GMT
ENV YOURLS_SHA256=f3623af6e4cabee61a39d3deca3c941717c5e0a60bc288b6f3a668f87a20ae2e
# Fri, 17 Apr 2020 22:27:48 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 17 Apr 2020 22:27:49 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Fri, 17 Apr 2020 22:27:49 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Fri, 17 Apr 2020 22:27:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 22:27:51 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:0776aeec3430c5a5ba3f43937f0ee6a7770a1fe81a318c9d94cc76512e5375e9`  
		Last Modified: Mon, 23 Mar 2020 21:49:50 GMT  
		Size: 2.6 MB (2618579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6ea08e138832a1357c5a2058da55929de016d0715372ec90df8716d8f08e8aa`  
		Last Modified: Tue, 24 Mar 2020 02:56:26 GMT  
		Size: 1.3 MB (1321096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6155177d2f4f58391e952733581935ca259371ca891a8e72311ff15a4b0caaf9`  
		Last Modified: Tue, 24 Mar 2020 02:56:26 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64588fb2e6842997faa53e9e5d4ec63be60ac226be4ae2eb5a97bff62263b14e`  
		Last Modified: Tue, 24 Mar 2020 02:56:25 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37e414c58bff3684b8c89036efb73336da9e05cc3f53772bf3416a7ef3fb23b6`  
		Last Modified: Fri, 17 Apr 2020 22:03:59 GMT  
		Size: 12.3 MB (12303520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b9dd510a8dc858342d5c8176cb3adb993e3052e219430cebe186f8d1150f939`  
		Last Modified: Fri, 17 Apr 2020 22:03:56 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2605f09420dd244d9398dd9b770030e58ff4a931b0ae60d5e63b1581272b6b24`  
		Last Modified: Fri, 17 Apr 2020 22:04:00 GMT  
		Size: 13.2 MB (13198959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f70d77537aa3057cf8d53e40efbf675118fd721f8b987c8fc8fe2a32090246a`  
		Last Modified: Fri, 17 Apr 2020 22:03:55 GMT  
		Size: 2.2 KB (2212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc1a6c803a7695267073d3a31457af9ae44bfa985d809e2cddff4e71e2b15890`  
		Last Modified: Fri, 17 Apr 2020 22:03:55 GMT  
		Size: 17.1 KB (17060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c79dbbe48ca0139867c4266067e988529bf3b5e1ff537f526f979ce20203e11`  
		Last Modified: Fri, 17 Apr 2020 22:03:55 GMT  
		Size: 7.8 KB (7783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a8e1299c0a34ad699fccbca5c99fc1bbce806cc7e59777aa8196adb6c99934`  
		Last Modified: Fri, 17 Apr 2020 22:28:07 GMT  
		Size: 287.0 KB (286967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36c270a94e1caf7ad52b3a730ba5d3b3170e2ddbd193eda6199a49915bbab70`  
		Last Modified: Fri, 17 Apr 2020 22:28:05 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab846defa5971f6e2fcd1b34b906e9ee41bdba3aa6592243282308527625338`  
		Last Modified: Fri, 17 Apr 2020 22:28:05 GMT  
		Size: 536.9 KB (536852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc5ce67f18a06513a742343e7bcf1ca3d32f140edf5e90ee5ba84624b598833`  
		Last Modified: Fri, 17 Apr 2020 22:28:05 GMT  
		Size: 2.5 MB (2485286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2e6cb931d4af5f8b80f330456bcfd1afcd94003b2606560fccfd8426aa5b591`  
		Last Modified: Fri, 17 Apr 2020 22:28:05 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b927255c032a2ff039e44efedf03c83698b6f1f45103360b7a6cf1cc76e635cb`  
		Last Modified: Fri, 17 Apr 2020 22:28:05 GMT  
		Size: 1.9 KB (1856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; arm variant v7

```console
$ docker pull yourls@sha256:ab52d4877004a4d2c975c64c36da5178f8f793077c94974b4044815f6ab1f547
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.6 MB (31562442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ddae34f3fe816cc5f31b86a8a1e30af0b697efb76c63e45db3192e89665657f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:57:55 GMT
ADD file:3bde6b6fd06efbf24e66446c6d32f72294fc749ae9ee6191776242e92b2f8ab4 in / 
# Mon, 23 Mar 2020 21:57:56 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 01:36:34 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 01:36:37 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 01:36:39 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 01:36:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 01:36:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 01:39:39 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 01:39:40 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 01:39:41 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 17 Apr 2020 12:34:31 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 17 Apr 2020 14:17:48 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 17 Apr 2020 22:18:33 GMT
ENV PHP_VERSION=7.2.30
# Fri, 17 Apr 2020 22:18:33 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.30.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.30.tar.xz.asc/from/this/mirror
# Fri, 17 Apr 2020 22:18:34 GMT
ENV PHP_SHA256=aa93df27b58a45d6c9800ac813245dfdca03490a918ebe515b3a70189b1bf8c3 PHP_MD5=
# Fri, 17 Apr 2020 22:18:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 17 Apr 2020 22:18:38 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 17 Apr 2020 22:21:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 17 Apr 2020 22:21:35 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 17 Apr 2020 22:21:39 GMT
RUN docker-php-ext-enable sodium
# Fri, 17 Apr 2020 22:21:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 17 Apr 2020 22:21:41 GMT
WORKDIR /var/www/html
# Fri, 17 Apr 2020 22:21:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 17 Apr 2020 22:21:44 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Apr 2020 22:21:45 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 22:21:45 GMT
CMD ["php-fpm"]
# Fri, 17 Apr 2020 23:11:07 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Fri, 17 Apr 2020 23:11:09 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 17 Apr 2020 23:11:11 GMT
RUN apk add --no-cache bash
# Fri, 17 Apr 2020 23:11:12 GMT
ENV YOURLS_VERSION=1.7.6
# Fri, 17 Apr 2020 23:11:13 GMT
ENV YOURLS_SHA256=f3623af6e4cabee61a39d3deca3c941717c5e0a60bc288b6f3a668f87a20ae2e
# Fri, 17 Apr 2020 23:11:16 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 17 Apr 2020 23:11:17 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Fri, 17 Apr 2020 23:11:17 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Fri, 17 Apr 2020 23:11:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 23:11:18 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d9bf605ce3d4449f4b90035c3e21d691806324781d43a5287b1da25a01779d6b`  
		Last Modified: Mon, 23 Mar 2020 21:58:16 GMT  
		Size: 2.4 MB (2420493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:221e0c8c991c3fdd8db1ec76c1a911aa0f946325ec2cf15d22a25693accc6edc`  
		Last Modified: Tue, 24 Mar 2020 02:07:16 GMT  
		Size: 1.2 MB (1227325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:edeaee6722c9e078934e8f34fe0dc55d3f3c28d742e92ce6b3e86775beaeeb44`  
		Last Modified: Tue, 24 Mar 2020 02:07:16 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84528978bcc1c0fe1d795bbe412f0a4123fa9119c11c98cd9b1ab8c5db8203f0`  
		Last Modified: Tue, 24 Mar 2020 02:07:16 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4524898b92378a80e481eb72f428b3c9fe12998f0392d12ea5ea5e118e53742d`  
		Last Modified: Fri, 17 Apr 2020 22:40:20 GMT  
		Size: 12.3 MB (12303524 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03a38a26c37f048b744095e590ba29b4d28700ff016398720fbec8283a31940e`  
		Last Modified: Fri, 17 Apr 2020 22:40:17 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de78c068028e3a7dda0ffc957ebbd27a41da957d55aa84bf591f4a31bae1fb63`  
		Last Modified: Fri, 17 Apr 2020 22:40:20 GMT  
		Size: 12.3 MB (12338593 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18711556a480f5bbf7a69345d44dbeaae89e2b88e80f5fb2f76cebb1751dce6b`  
		Last Modified: Fri, 17 Apr 2020 22:40:17 GMT  
		Size: 2.2 KB (2216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d78fb234dc7760e0cde5a8278545f4d5e6add1cff5c2317935a30204b358569d`  
		Last Modified: Fri, 17 Apr 2020 22:40:17 GMT  
		Size: 17.0 KB (17041 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:96c7394db64f45dd98ec31d7e3aa1d7019a5fbcf7f88daf4a155354cd3b65dea`  
		Last Modified: Fri, 17 Apr 2020 22:40:17 GMT  
		Size: 7.8 KB (7783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8485176941f7ddc05a5bd5f702df125fdd7ce873a7673f69b74c3789b48e3ad5`  
		Last Modified: Fri, 17 Apr 2020 23:12:03 GMT  
		Size: 265.7 KB (265660 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2323c19f6e9ef8c030a09c976d8bf7b811e65de7271479958f72779eba230eb4`  
		Last Modified: Fri, 17 Apr 2020 23:12:02 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6689f6369ec7c9c2915228bae7eecddd5100f3d2b6f43bb45489e5c861f1050e`  
		Last Modified: Fri, 17 Apr 2020 23:12:02 GMT  
		Size: 489.1 KB (489134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:585a4cf980b96c0c3d7a8006865cc05d1811a76f1c880ced31b2e85c3cad5c20`  
		Last Modified: Fri, 17 Apr 2020 23:12:03 GMT  
		Size: 2.5 MB (2485284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccbcd9be6bc785316cdc0d63fabeac63cd7c427ec86d9a68bfdc8944d171c08d`  
		Last Modified: Fri, 17 Apr 2020 23:12:02 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aaf4e2203dd5cb16f102395156f67bffaefb0578ad09da43d577404ea49ab515`  
		Last Modified: Fri, 17 Apr 2020 23:12:02 GMT  
		Size: 1.9 KB (1856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:7c8e4e83db13e7d304d13184c150c6499e3d206582178d2207239e50fd061a2c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33714923 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b30be97927728b268148aa901e77e07110d84d863082503428d26e32513d5002`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:39:52 GMT
ADD file:746a5c3838a898d6acf7877552ff13d1ab40d0036ace7a662e7c747018315ddb in / 
# Mon, 23 Mar 2020 21:39:53 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:27:16 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 00:27:19 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 00:27:21 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 00:27:22 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 00:27:23 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 00:31:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 00:31:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 00:31:23 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 17 Apr 2020 13:23:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 17 Apr 2020 15:16:32 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 17 Apr 2020 22:20:14 GMT
ENV PHP_VERSION=7.2.30
# Fri, 17 Apr 2020 22:20:15 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.30.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.30.tar.xz.asc/from/this/mirror
# Fri, 17 Apr 2020 22:20:16 GMT
ENV PHP_SHA256=aa93df27b58a45d6c9800ac813245dfdca03490a918ebe515b3a70189b1bf8c3 PHP_MD5=
# Fri, 17 Apr 2020 22:20:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 17 Apr 2020 22:20:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 17 Apr 2020 22:23:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 17 Apr 2020 22:23:36 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 17 Apr 2020 22:23:39 GMT
RUN docker-php-ext-enable sodium
# Fri, 17 Apr 2020 22:23:40 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 17 Apr 2020 22:23:41 GMT
WORKDIR /var/www/html
# Fri, 17 Apr 2020 22:23:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 17 Apr 2020 22:23:44 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Apr 2020 22:23:44 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 22:23:45 GMT
CMD ["php-fpm"]
# Fri, 17 Apr 2020 23:46:42 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Fri, 17 Apr 2020 23:46:44 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 17 Apr 2020 23:46:46 GMT
RUN apk add --no-cache bash
# Fri, 17 Apr 2020 23:46:47 GMT
ENV YOURLS_VERSION=1.7.6
# Fri, 17 Apr 2020 23:46:47 GMT
ENV YOURLS_SHA256=f3623af6e4cabee61a39d3deca3c941717c5e0a60bc288b6f3a668f87a20ae2e
# Fri, 17 Apr 2020 23:46:50 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 17 Apr 2020 23:46:51 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Fri, 17 Apr 2020 23:46:51 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Fri, 17 Apr 2020 23:46:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 17 Apr 2020 23:46:52 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:8a0637ca1ac98db4cf29f7632449c92801adc80cf0da2cd9c9e39882ce466561`  
		Last Modified: Mon, 23 Mar 2020 21:40:19 GMT  
		Size: 2.7 MB (2723139 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee501176ea6c9d16dc12649d7c62f4b6466cc96eaf80bfcea3aa261a052ec099`  
		Last Modified: Tue, 24 Mar 2020 01:03:05 GMT  
		Size: 1.4 MB (1359430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e876007701d95df62eb874f76916e4d139709812e5e0be471c4107729808d6af`  
		Last Modified: Tue, 24 Mar 2020 01:03:04 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ed02bd016dcfb57e62d938f46a81237af426353ef7df647b64c3b3a93276a7`  
		Last Modified: Tue, 24 Mar 2020 01:03:04 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6227779d538deb8b4879794748886d746a383835324877c5608185aeffa55b3`  
		Last Modified: Fri, 17 Apr 2020 22:42:44 GMT  
		Size: 12.3 MB (12303519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:411bad23e4ee46a6d73f5ed55607034d395ea297470c8c71652820a8831e470b`  
		Last Modified: Fri, 17 Apr 2020 22:42:41 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b797ab4775160a0bf13c44dbdc767dd221f800972ecf07539e6ce12be7099c1e`  
		Last Modified: Fri, 17 Apr 2020 22:42:46 GMT  
		Size: 13.9 MB (13942906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a46bf61aac1c4c6821a81f32d2c6464b8a11db9058b3d2a3bf7dcac7036396b3`  
		Last Modified: Fri, 17 Apr 2020 22:42:41 GMT  
		Size: 2.2 KB (2217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8dd32c14c22b35a15ccb6afbcffa41f37765b0079718181269c31825a1d18d55`  
		Last Modified: Fri, 17 Apr 2020 22:42:41 GMT  
		Size: 17.0 KB (17049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4ad9def6411e6368a3f434dab43c56e3a8261ef1603e85caf4aa2c805473ed0`  
		Last Modified: Fri, 17 Apr 2020 22:42:41 GMT  
		Size: 7.8 KB (7782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67b096ee589658307a5728ad64331bcc92ddee2aee44875b126385c6c8e6646e`  
		Last Modified: Fri, 17 Apr 2020 23:47:36 GMT  
		Size: 299.3 KB (299279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510a40b7af1aab9a202bdfea10d7b256a914a37f25caba09463c0c75e9f2dbc9`  
		Last Modified: Fri, 17 Apr 2020 23:47:34 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31187590f2a49cffd432cf2333295ea48a0a148e3bbfe97a1e3b0caf97e3d7f6`  
		Last Modified: Fri, 17 Apr 2020 23:47:35 GMT  
		Size: 568.9 KB (568940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2fb12ed1f77374d67c5fa5a67a7c95b3c82b3b123f0253c9f78e07fdc4fae9dd`  
		Last Modified: Fri, 17 Apr 2020 23:47:35 GMT  
		Size: 2.5 MB (2485278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24a93ba069085af0d5b126ed100f69caa1f00a3d3fce95369fececd0c8a64474`  
		Last Modified: Fri, 17 Apr 2020 23:47:34 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bffb25c0a8f1425040624ac600773dbed32a272d9fadbc13245c6b1408f77a01`  
		Last Modified: Fri, 17 Apr 2020 23:47:34 GMT  
		Size: 1.9 KB (1854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; 386

```console
$ docker pull yourls@sha256:51d522f2d960e6d0b6512d0b9d703b90293148cf3f032e4416fd855646cb8f2d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.6 MB (34598250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:709e8cad34e93094540bf4c44a59b12327acb0697d1676315944e94ba94140dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:38:28 GMT
ADD file:99c8234abafd4fa915c0b826eb0e3be0e6aaa7c1e33cb1214ef71a99e9c02e06 in / 
# Mon, 23 Mar 2020 21:38:28 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 02:43:33 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 02:43:35 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 02:43:36 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 02:43:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 02:43:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 02:51:22 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 02:51:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 02:51:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 17 Apr 2020 08:09:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 17 Apr 2020 11:06:15 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Fri, 17 Apr 2020 22:52:15 GMT
ENV PHP_VERSION=7.2.30
# Fri, 17 Apr 2020 22:52:15 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.30.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.30.tar.xz.asc/from/this/mirror
# Fri, 17 Apr 2020 22:52:16 GMT
ENV PHP_SHA256=aa93df27b58a45d6c9800ac813245dfdca03490a918ebe515b3a70189b1bf8c3 PHP_MD5=
# Fri, 17 Apr 2020 22:52:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 17 Apr 2020 22:52:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 17 Apr 2020 23:02:05 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 17 Apr 2020 23:02:06 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 17 Apr 2020 23:02:07 GMT
RUN docker-php-ext-enable sodium
# Fri, 17 Apr 2020 23:02:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 17 Apr 2020 23:02:08 GMT
WORKDIR /var/www/html
# Fri, 17 Apr 2020 23:02:08 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 17 Apr 2020 23:02:09 GMT
STOPSIGNAL SIGQUIT
# Fri, 17 Apr 2020 23:02:09 GMT
EXPOSE 9000
# Fri, 17 Apr 2020 23:02:09 GMT
CMD ["php-fpm"]
# Sat, 18 Apr 2020 00:20:57 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Sat, 18 Apr 2020 00:20:58 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 18 Apr 2020 00:20:59 GMT
RUN apk add --no-cache bash
# Sat, 18 Apr 2020 00:20:59 GMT
ENV YOURLS_VERSION=1.7.6
# Sat, 18 Apr 2020 00:20:59 GMT
ENV YOURLS_SHA256=f3623af6e4cabee61a39d3deca3c941717c5e0a60bc288b6f3a668f87a20ae2e
# Sat, 18 Apr 2020 00:21:01 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 18 Apr 2020 00:21:01 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Sat, 18 Apr 2020 00:21:01 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Sat, 18 Apr 2020 00:21:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Apr 2020 00:21:02 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:43f6a4398e1c9e860dfb5c93d7049ab9eedf814513bd6d07e06077c560303c7a`  
		Last Modified: Mon, 23 Mar 2020 21:38:48 GMT  
		Size: 2.8 MB (2806122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8addccc9b68d6aad59a5f93e0ca1813c5d09a0c7943108d860d8c29f6bebdb5`  
		Last Modified: Tue, 24 Mar 2020 04:03:48 GMT  
		Size: 1.5 MB (1452601 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb273244de1495dfb0044080245a9fa0c6f3d8a2ab5f30610237d9a76e66cd4`  
		Last Modified: Tue, 24 Mar 2020 04:03:47 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13d6dffa3f09145ac45428f87b062a4603137dadcaa84454812f81f70b71ea07`  
		Last Modified: Tue, 24 Mar 2020 04:03:47 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c71e2eb4a502fdfe6c9bfd65a07af16accf0593dffa36d07641ebfc60310b310`  
		Last Modified: Fri, 17 Apr 2020 23:43:35 GMT  
		Size: 12.3 MB (12303511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31fcd54055c4bbf82fd4905b0675577012ce1cf8c5cab58e9e23476af16ad392`  
		Last Modified: Fri, 17 Apr 2020 23:43:32 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab378631934cb59a7960dc4375d9749fe1cb6f36b20ce59ead1a7b75b368bf03`  
		Last Modified: Fri, 17 Apr 2020 23:43:37 GMT  
		Size: 14.6 MB (14603469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce76a0f96cb509833ebf57287098355ba4de374f1183d22ced60ff85ac4014d7`  
		Last Modified: Fri, 17 Apr 2020 23:43:33 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e801211afb77035b16b4c2836a9f4cb74733c057086f9ae6112867830f2bf847`  
		Last Modified: Fri, 17 Apr 2020 23:43:33 GMT  
		Size: 17.1 KB (17058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:601685bccc0113b2940935b98fca6dd29d398bd2cb885b9b1512a40655b1663a`  
		Last Modified: Fri, 17 Apr 2020 23:43:33 GMT  
		Size: 7.8 KB (7784 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9babd9568600c3252cfbbbc0e46d970baa16d06d88824d53a30ae84d8c04412c`  
		Last Modified: Sat, 18 Apr 2020 00:21:42 GMT  
		Size: 316.2 KB (316235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc68cf793df57eb7b41dc8d37fd9a9e766f8a95151011b4fee8e9aed452c0b5`  
		Last Modified: Sat, 18 Apr 2020 00:21:41 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60dfe5b4a4985e7f6f85418ccc1d326e1852809ecad01e80a2f8fdcc5f160e30`  
		Last Modified: Sat, 18 Apr 2020 00:21:41 GMT  
		Size: 598.7 KB (598686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6757aa9b9a1a5ae84a2a072e9e79de559023b80b81651cb9dcdd48152f31ae42`  
		Last Modified: Sat, 18 Apr 2020 00:21:42 GMT  
		Size: 2.5 MB (2485254 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:009c1c13e9b2f60c8d4cc6bd2833e692b305421f0c276ff313c27d6983fb0e65`  
		Last Modified: Sat, 18 Apr 2020 00:21:41 GMT  
		Size: 1.2 KB (1179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac0edb84a4e8a34073ac345ec7d3cb8ce48b3ff62b31107d1d2f238554e39edc`  
		Last Modified: Sat, 18 Apr 2020 00:21:41 GMT  
		Size: 1.9 KB (1854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; ppc64le

```console
$ docker pull yourls@sha256:039e4bf1917e214b4dc11819604ad311c3337b628161fba32e8597570c39187c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35188877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:902a025a3da9849dfbc09e18c15e82b6752efeb2b342cc9304c82fa8909cd617`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Mon, 23 Mar 2020 21:21:29 GMT
ADD file:4b35131542b9682214e1c2c72fe3cea215a10e2f775e87befecd80fe2228d5a0 in / 
# Mon, 23 Mar 2020 21:21:32 GMT
CMD ["/bin/sh"]
# Tue, 24 Mar 2020 00:27:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 24 Mar 2020 00:27:27 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 24 Mar 2020 00:27:38 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 24 Mar 2020 00:27:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 24 Mar 2020 00:27:49 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 24 Mar 2020 00:32:28 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Tue, 24 Mar 2020 00:32:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 24 Mar 2020 00:32:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 17 Apr 2020 16:39:44 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 17 Apr 2020 19:37:27 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 B1B44D8F021E4E2D6021E995DC9FF8D3EE5AF27F
# Sat, 18 Apr 2020 05:34:00 GMT
ENV PHP_VERSION=7.2.30
# Sat, 18 Apr 2020 05:34:03 GMT
ENV PHP_URL=https://www.php.net/get/php-7.2.30.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.2.30.tar.xz.asc/from/this/mirror
# Sat, 18 Apr 2020 05:34:05 GMT
ENV PHP_SHA256=aa93df27b58a45d6c9800ac813245dfdca03490a918ebe515b3a70189b1bf8c3 PHP_MD5=
# Sat, 18 Apr 2020 05:34:17 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Sat, 18 Apr 2020 05:34:19 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Sat, 18 Apr 2020 05:38:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Sat, 18 Apr 2020 05:38:39 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Sat, 18 Apr 2020 05:38:44 GMT
RUN docker-php-ext-enable sodium
# Sat, 18 Apr 2020 05:38:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Sat, 18 Apr 2020 05:38:49 GMT
WORKDIR /var/www/html
# Sat, 18 Apr 2020 05:38:55 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Sat, 18 Apr 2020 05:38:56 GMT
STOPSIGNAL SIGQUIT
# Sat, 18 Apr 2020 05:38:59 GMT
EXPOSE 9000
# Sat, 18 Apr 2020 05:39:01 GMT
CMD ["php-fpm"]
# Sat, 18 Apr 2020 06:29:33 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Sat, 18 Apr 2020 06:29:40 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Sat, 18 Apr 2020 06:29:51 GMT
RUN apk add --no-cache bash
# Sat, 18 Apr 2020 06:29:54 GMT
ENV YOURLS_VERSION=1.7.6
# Sat, 18 Apr 2020 06:29:58 GMT
ENV YOURLS_SHA256=f3623af6e4cabee61a39d3deca3c941717c5e0a60bc288b6f3a668f87a20ae2e
# Sat, 18 Apr 2020 06:30:06 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Sat, 18 Apr 2020 06:30:08 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Sat, 18 Apr 2020 06:30:09 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Sat, 18 Apr 2020 06:30:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 18 Apr 2020 06:30:18 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:bc1c99f4ba60de0d3ca52dc6855483e24c91884e33df71f502bbff6eb909d9b9`  
		Last Modified: Mon, 23 Mar 2020 21:22:12 GMT  
		Size: 2.8 MB (2820052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681c4a6dbdeb5b4877c85db3edbb08e40a877342795a3e7ba7f543a65586c417`  
		Last Modified: Tue, 24 Mar 2020 01:16:24 GMT  
		Size: 1.4 MB (1397873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e23455f025d83291061d4165e722b934e986f58c2b3d71b62a0918166d19db`  
		Last Modified: Tue, 24 Mar 2020 01:16:23 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74c3447d90e80a01a72c494bf3563b1379704fcf4fb8b5b207596bbeeac49fc3`  
		Last Modified: Tue, 24 Mar 2020 01:16:22 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20f32e490d405a9b863a631c6d10acfdf032c1c16ba92f19b77e8b5516494b28`  
		Last Modified: Sat, 18 Apr 2020 06:07:05 GMT  
		Size: 12.3 MB (12303537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa0f715c1f048f550acb9fef596c6227f0cbb9e53e6d38d98379d56883939e8c`  
		Last Modified: Sat, 18 Apr 2020 06:07:01 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c319e6d48c9343fe02826543eb0a73b087facb0b04e8d977752e5f4c39b1bbb`  
		Last Modified: Sat, 18 Apr 2020 06:07:04 GMT  
		Size: 15.2 MB (15191149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0692e48ec3d881345197c95a71ed8848572393ffbf2efd372b3f92c2ec4b2b9c`  
		Last Modified: Sat, 18 Apr 2020 06:07:00 GMT  
		Size: 2.2 KB (2217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a988b4f0c85a91dd6c2ec2fd4e4dd31619a19decb77b1b999da9f1e0f61c4bdd`  
		Last Modified: Sat, 18 Apr 2020 06:07:00 GMT  
		Size: 17.1 KB (17055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0359bc2a9f9b9f712471f2523eecd6987699a2689819f4e410c5fff5b349b8d2`  
		Last Modified: Sat, 18 Apr 2020 06:07:01 GMT  
		Size: 7.8 KB (7782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1d9cc307d0fbaee05005ca68361a6feee37bebf3a8e112ebd36627aebcf8502`  
		Last Modified: Sat, 18 Apr 2020 06:32:10 GMT  
		Size: 336.3 KB (336297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:735ca689924959f9267ed963afc0efc5f98cee3b50a31251e6d876704bd4f781`  
		Last Modified: Sat, 18 Apr 2020 06:32:07 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e36910037ce7ea90f93ef27a0bf26569dd688d8668a9904e96febf888f35d240`  
		Last Modified: Sat, 18 Apr 2020 06:32:07 GMT  
		Size: 622.2 KB (622241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44a9019a50559efdc77ed39dc29b9844f867f9f5bdf68f2ac10be2a2f0746209`  
		Last Modified: Sat, 18 Apr 2020 06:32:07 GMT  
		Size: 2.5 MB (2485286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ddada402c653535c680c63d50a4d3d0d5360aade81cd9f091db7a991d8d818d`  
		Last Modified: Sat, 18 Apr 2020 06:32:06 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e9f8be77c8e0de6aa353b0f7dceed7047e360eae1138d437481ae55e1350fdf`  
		Last Modified: Sat, 18 Apr 2020 06:32:07 GMT  
		Size: 1.9 KB (1857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
