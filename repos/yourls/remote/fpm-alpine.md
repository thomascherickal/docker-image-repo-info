## `yourls:fpm-alpine`

```console
$ docker pull yourls@sha256:52ffcd2a642af0dfe9b56e6633e0c07a37d06aa04587f4c4777da57313bf9a11
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

### `yourls:fpm-alpine` - linux; amd64

```console
$ docker pull yourls@sha256:8662aacc39211f5f6f9d872f0021be3253b2218a879b737f2101f8b577348b2b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.5 MB (32506109 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ab5bcbd9f9341a2069d44beb938680b48ebf0d48e6e90b341d128b83ce3d3ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Thu, 11 Jun 2020 19:00:53 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 11 Jun 2020 19:00:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 19:00:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 19:00:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 19:00:54 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 06 Aug 2020 19:39:08 GMT
ENV PHP_VERSION=7.4.9
# Thu, 06 Aug 2020 19:39:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.9.tar.xz.asc
# Thu, 06 Aug 2020 19:39:08 GMT
ENV PHP_SHA256=23733f4a608ad1bebdcecf0138ebc5fd57cf20d6e0915f98a9444c3f747dc57b PHP_MD5=
# Thu, 06 Aug 2020 19:39:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Aug 2020 19:39:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Sep 2020 03:00:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Sep 2020 03:00:15 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Tue, 01 Sep 2020 03:00:17 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Sep 2020 03:00:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Sep 2020 03:00:18 GMT
WORKDIR /var/www/html
# Tue, 01 Sep 2020 03:00:20 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 01 Sep 2020 03:00:20 GMT
STOPSIGNAL SIGQUIT
# Tue, 01 Sep 2020 03:00:20 GMT
EXPOSE 9000
# Tue, 01 Sep 2020 03:00:21 GMT
CMD ["php-fpm"]
# Tue, 01 Sep 2020 23:00:00 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Tue, 01 Sep 2020 23:00:01 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 01 Sep 2020 23:00:02 GMT
RUN apk add --no-cache bash
# Tue, 01 Sep 2020 23:00:02 GMT
ENV YOURLS_VERSION=1.7.9
# Tue, 01 Sep 2020 23:00:03 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Tue, 01 Sep 2020 23:00:04 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 01 Sep 2020 23:00:04 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Tue, 01 Sep 2020 23:00:04 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Tue, 01 Sep 2020 23:00:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Sep 2020 23:00:04 GMT
CMD ["php-fpm"]
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
	-	`sha256:69251dafcb2dd13dccf0e9db086733643de7d1c4b4ba6ff4cad410c432c287a0`  
		Last Modified: Fri, 07 Aug 2020 00:25:37 GMT  
		Size: 10.3 MB (10308414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f538119c59ade2b941eea78bafe33a141d25ccb409512fa15c6592836191d8`  
		Last Modified: Fri, 07 Aug 2020 00:25:33 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5653f160c702278c224f9b5b718bfc5e5c5ed351ec47b33d8a3547f422440b48`  
		Last Modified: Tue, 01 Sep 2020 07:21:47 GMT  
		Size: 14.6 MB (14634015 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4523b848ecf070d6547ce3d586b1c0a2af13fe49ab029e002fa4eccb30fa387b`  
		Last Modified: Tue, 01 Sep 2020 07:21:44 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cb652edfb2b4c1e9485450802abf5cb68d30f38642dedd157ab808855306a50`  
		Last Modified: Tue, 01 Sep 2020 07:21:45 GMT  
		Size: 17.0 KB (17020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bff8f4e6b6d5eae46e65461ba135aef568b2ecb5ef4bec1917adb937cb25d946`  
		Last Modified: Tue, 01 Sep 2020 07:21:44 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64acea76a73fd28643a47b3fb67542737772eeb3c296401aaaf691cae41826bb`  
		Last Modified: Tue, 01 Sep 2020 23:00:29 GMT  
		Size: 348.1 KB (348051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a12fcd4fe5e942907363e748a0806a7c730dd074cd70144ea9f3a5e4b94b8b9`  
		Last Modified: Tue, 01 Sep 2020 23:00:28 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3c4a66a6be18f7780ffddbec01c3a5932abda4d60c8107ec08477d2ba87608c`  
		Last Modified: Tue, 01 Sep 2020 23:00:28 GMT  
		Size: 557.5 KB (557455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ac171e064fc6410ca00932fbc92c7081166759650e39ad12da3531abe789d2f`  
		Last Modified: Tue, 01 Sep 2020 23:00:28 GMT  
		Size: 2.5 MB (2486762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6525e632674d4a738095b4dbc876fea156f93cd3f49356b65fd10a34aff1ca32`  
		Last Modified: Tue, 01 Sep 2020 23:00:28 GMT  
		Size: 1.2 KB (1183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f79872b768b7c974b93b089c29cfea85ad2dc9a963b72fe10262b64ca352e0d0`  
		Last Modified: Tue, 01 Sep 2020 23:00:28 GMT  
		Size: 1.9 KB (1856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; arm variant v6

```console
$ docker pull yourls@sha256:332c4fbc1bf1988eb51f12264556c0c069b26b738cd9abf6e91b60626168de4b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.3 MB (31258839 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1a62534f61def5b6a6e80ebea88c9944c3f5779699b8de8f7abf5f2c1e5f5c49`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Thu, 11 Jun 2020 18:20:14 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 11 Jun 2020 18:20:15 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:20:16 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:20:17 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:20:18 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 06 Aug 2020 18:33:45 GMT
ENV PHP_VERSION=7.4.9
# Thu, 06 Aug 2020 18:34:03 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.9.tar.xz.asc
# Thu, 06 Aug 2020 18:34:13 GMT
ENV PHP_SHA256=23733f4a608ad1bebdcecf0138ebc5fd57cf20d6e0915f98a9444c3f747dc57b PHP_MD5=
# Thu, 06 Aug 2020 18:34:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Aug 2020 18:35:14 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Sep 2020 00:58:56 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Sep 2020 00:59:43 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Tue, 01 Sep 2020 01:00:56 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Sep 2020 01:01:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Sep 2020 01:01:43 GMT
WORKDIR /var/www/html
# Tue, 01 Sep 2020 01:02:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 01 Sep 2020 01:03:09 GMT
STOPSIGNAL SIGQUIT
# Tue, 01 Sep 2020 01:03:25 GMT
EXPOSE 9000
# Tue, 01 Sep 2020 01:03:39 GMT
CMD ["php-fpm"]
# Tue, 01 Sep 2020 05:29:52 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Tue, 01 Sep 2020 05:30:24 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 01 Sep 2020 05:31:12 GMT
RUN apk add --no-cache bash
# Tue, 01 Sep 2020 05:31:26 GMT
ENV YOURLS_VERSION=1.7.9
# Tue, 01 Sep 2020 05:31:40 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Tue, 01 Sep 2020 05:32:24 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 01 Sep 2020 05:32:35 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Tue, 01 Sep 2020 05:32:45 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Tue, 01 Sep 2020 05:32:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Sep 2020 05:32:56 GMT
CMD ["php-fpm"]
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
	-	`sha256:3947f012a249fab434e5f236291eaa5556b1ca03a2e3f1aaa3f45c058934d6ae`  
		Last Modified: Thu, 06 Aug 2020 21:05:44 GMT  
		Size: 10.3 MB (10308439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b22adc129c11668e2a4ef1c0edf506cde63e480ef319f2b314df02458e4ba42`  
		Last Modified: Thu, 06 Aug 2020 21:05:39 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:261ab6fe9ab5c0f9f6934b2920a046c1bf73f94cf83a0a246df606c651b165f8`  
		Last Modified: Tue, 01 Sep 2020 03:30:07 GMT  
		Size: 13.7 MB (13651937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd9ca96197848298c42f177a9cdbd25b778dde3f093d427dc49958a084d82f3f`  
		Last Modified: Tue, 01 Sep 2020 03:30:01 GMT  
		Size: 2.3 KB (2275 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83638788fd3e53c309cb721752113a4344ff8eea5991b645dc78e91c72cdeead`  
		Last Modified: Tue, 01 Sep 2020 03:30:04 GMT  
		Size: 17.0 KB (16971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9698dab591c2e0999530db37bd7590c61153ab6106bd8ac3858860877512c0ea`  
		Last Modified: Tue, 01 Sep 2020 03:30:04 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b8836db78ee2f8db04ee9db936ef11100ced45a4142a63de0a94f78c11a65ac`  
		Last Modified: Tue, 01 Sep 2020 05:33:15 GMT  
		Size: 326.6 KB (326568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6ff4f4dac2a13d4cd78bb471d1b1ca4685841adec7174f7c376c7a66a6b4142`  
		Last Modified: Tue, 01 Sep 2020 05:33:11 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa4e0ae8896ef639c7e381dd0a5e005c9c9093852656c44eccc2da1d38230c70`  
		Last Modified: Tue, 01 Sep 2020 05:33:13 GMT  
		Size: 538.4 KB (538426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ce9b486571ceafe8d1e641bd87bbdbd64208517105ec649f44f021b749fe36a`  
		Last Modified: Tue, 01 Sep 2020 05:33:13 GMT  
		Size: 2.5 MB (2486821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed7dc35db46d3ccc18d4d4775a70594002806da9c36b6b38ac2f2b1a23753cd4`  
		Last Modified: Tue, 01 Sep 2020 05:33:11 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cef7bd55f7d9cb01fc50e1bcae021e0a0a3004f095dfe128169c7f5e662898f3`  
		Last Modified: Tue, 01 Sep 2020 05:33:11 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; arm variant v7

```console
$ docker pull yourls@sha256:6f0a4f74b9be8e6a3e604dafa59603342fd4e6089a9505e853394dc163582a99
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.0 MB (30011777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2caae23bc18ecbd6d5176de710a42c7082e5aff0c9a9b4e0c6e69e03bfc769`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Thu, 11 Jun 2020 18:38:52 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 11 Jun 2020 18:38:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:38:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:38:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:38:57 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 06 Aug 2020 19:37:56 GMT
ENV PHP_VERSION=7.4.9
# Thu, 06 Aug 2020 19:38:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.9.tar.xz.asc
# Thu, 06 Aug 2020 19:38:22 GMT
ENV PHP_SHA256=23733f4a608ad1bebdcecf0138ebc5fd57cf20d6e0915f98a9444c3f747dc57b PHP_MD5=
# Thu, 06 Aug 2020 19:39:13 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Aug 2020 19:39:43 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 06 Aug 2020 19:43:12 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 06 Aug 2020 19:43:45 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 06 Aug 2020 19:44:20 GMT
RUN docker-php-ext-enable sodium
# Thu, 06 Aug 2020 19:44:31 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 06 Aug 2020 19:44:40 GMT
WORKDIR /var/www/html
# Thu, 06 Aug 2020 19:45:28 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 06 Aug 2020 19:45:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 06 Aug 2020 19:45:46 GMT
EXPOSE 9000
# Thu, 06 Aug 2020 19:45:54 GMT
CMD ["php-fpm"]
# Fri, 07 Aug 2020 07:44:58 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Fri, 07 Aug 2020 07:45:00 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 07 Aug 2020 07:45:02 GMT
RUN apk add --no-cache bash
# Fri, 07 Aug 2020 07:45:03 GMT
ENV YOURLS_VERSION=1.7.9
# Fri, 07 Aug 2020 07:45:03 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Fri, 07 Aug 2020 07:45:07 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Fri, 07 Aug 2020 07:45:08 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Fri, 07 Aug 2020 07:45:09 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Fri, 07 Aug 2020 07:45:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 07 Aug 2020 07:45:10 GMT
CMD ["php-fpm"]
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
	-	`sha256:afde29a1e0f524bddb0bb015fabf0dfdd34fe072acde70082b2d2c60d5697006`  
		Last Modified: Fri, 07 Aug 2020 01:03:50 GMT  
		Size: 10.3 MB (10308438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06f189b3b15e46d1949c8f50947392618fe13290cd72fa14735eb65c8e51ce3`  
		Last Modified: Fri, 07 Aug 2020 01:03:46 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8658aa25074470fd63afb939f8bbe06ba08b3e45047357db90e73b6a26c77c26`  
		Last Modified: Fri, 07 Aug 2020 01:03:50 GMT  
		Size: 12.8 MB (12769288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:863c399f4a618587eba1756162a2b1ce6030a56336072d76fbd85fd9ea6a50ad`  
		Last Modified: Fri, 07 Aug 2020 01:03:46 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82a2d98f1383ac3b7b000f39c6f468f14bf0c2d3b629de26952b32cf6785a957`  
		Last Modified: Fri, 07 Aug 2020 01:03:47 GMT  
		Size: 17.0 KB (16956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecd9c3f0d1c9f6d651f3d3af35d708d5d58b9957cffded1211fe10455eaba6be`  
		Last Modified: Fri, 07 Aug 2020 01:03:47 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8c2644f7c2b9b510d56d9028a846b031c6fc7f0854801346503ff4fefc99fe9`  
		Last Modified: Fri, 07 Aug 2020 07:46:09 GMT  
		Size: 302.5 KB (302546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64c1d50e8cbe6cd321bf06f096f06123c3a08d704728b6eeeb8bb35a5f1b4b97`  
		Last Modified: Fri, 07 Aug 2020 07:46:05 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9de0d92f551b6d6238aa6a76aaf4ddc8860c2e2a5a8fba0f746d1b2741f4ed2c`  
		Last Modified: Fri, 07 Aug 2020 07:46:06 GMT  
		Size: 490.5 KB (490467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:798cc22e154bf146d80f58e5dbb16dfdad85477175a732f1a74d67db4343c39b`  
		Last Modified: Fri, 07 Aug 2020 07:46:07 GMT  
		Size: 2.5 MB (2486828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7517a95119a0daaea4ec0cb5ff03b9660cdf2a637e0c93f8cfa7613bed9c997f`  
		Last Modified: Fri, 07 Aug 2020 07:46:06 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06d2cc28cf2ae1a3985f7928c4f18893f600ff65df527dc2c3abff7dcd79f968`  
		Last Modified: Fri, 07 Aug 2020 07:46:06 GMT  
		Size: 1.9 KB (1860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:7fa20be714540fc14fbe415640eba6e1091892f805ca8e73a957af0961826fb8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.2 MB (32238349 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:56c90b14777e6f20e9ed43f544bbf591a7e8f29e8a594aee0e88fe5a102b60d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Thu, 11 Jun 2020 18:45:04 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 11 Jun 2020 18:45:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:45:07 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:45:07 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 06 Aug 2020 19:14:07 GMT
ENV PHP_VERSION=7.4.9
# Thu, 06 Aug 2020 19:14:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.9.tar.xz.asc
# Thu, 06 Aug 2020 19:14:18 GMT
ENV PHP_SHA256=23733f4a608ad1bebdcecf0138ebc5fd57cf20d6e0915f98a9444c3f747dc57b PHP_MD5=
# Thu, 06 Aug 2020 19:14:34 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Aug 2020 19:14:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Sep 2020 04:30:14 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Sep 2020 04:30:28 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Tue, 01 Sep 2020 04:30:51 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Sep 2020 04:30:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Sep 2020 04:31:02 GMT
WORKDIR /var/www/html
# Tue, 01 Sep 2020 04:31:25 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 01 Sep 2020 04:31:33 GMT
STOPSIGNAL SIGQUIT
# Tue, 01 Sep 2020 04:31:42 GMT
EXPOSE 9000
# Tue, 01 Sep 2020 04:31:54 GMT
CMD ["php-fpm"]
# Tue, 01 Sep 2020 19:32:15 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Tue, 01 Sep 2020 19:32:29 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 01 Sep 2020 19:32:32 GMT
RUN apk add --no-cache bash
# Tue, 01 Sep 2020 19:32:33 GMT
ENV YOURLS_VERSION=1.7.9
# Tue, 01 Sep 2020 19:32:38 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Tue, 01 Sep 2020 19:32:40 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 01 Sep 2020 19:32:43 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Tue, 01 Sep 2020 19:32:48 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Tue, 01 Sep 2020 19:32:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Sep 2020 19:32:57 GMT
CMD ["php-fpm"]
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
	-	`sha256:00cce70fc39c9a694e09e76796fff80b2c822b1a3232d2534fce657af7b2dcf9`  
		Last Modified: Thu, 06 Aug 2020 23:30:05 GMT  
		Size: 10.3 MB (10308454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e031ee12589510a53f13fbb0ce6142098568f67fdad9ad6b62681261fb6e833d`  
		Last Modified: Thu, 06 Aug 2020 23:30:00 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e595d7a2b9b239e58f1e45fd3130487c000cc2417c8b0deadfc0ac92da07c7a`  
		Last Modified: Tue, 01 Sep 2020 07:05:56 GMT  
		Size: 14.4 MB (14449459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af695fed2475f46e882e6c08d24ddd121fa4cb16e5a992cd282cb97c3201e1e4`  
		Last Modified: Tue, 01 Sep 2020 07:05:51 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a819651692773e2154c810c05326087959dd94b76e01c1d5fdd03ae7c1821e5b`  
		Last Modified: Tue, 01 Sep 2020 07:05:52 GMT  
		Size: 17.0 KB (17024 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b04103ade4399705dd562fd7d3e1fe1f79b5f5e6c9250c86c23f6fdc5b134422`  
		Last Modified: Tue, 01 Sep 2020 07:05:51 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab9b469cf4566c22cd73b2756eee52a17f8f802690479ef5640660529d9e87f8`  
		Last Modified: Tue, 01 Sep 2020 19:33:55 GMT  
		Size: 340.9 KB (340914 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee5f1172208101d7f5b80f7ca87aabe30af836c038e926a637ed508998298911`  
		Last Modified: Tue, 01 Sep 2020 19:33:52 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df26cb8df295316cb90b95c1137699b7dc112678b5b3219dee6bc21d71350af8`  
		Last Modified: Tue, 01 Sep 2020 19:33:52 GMT  
		Size: 568.6 KB (568600 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e2a070852897642c085a2d55be70207d44814ed0e50c4a0a04c162422efe11c`  
		Last Modified: Tue, 01 Sep 2020 19:33:56 GMT  
		Size: 2.5 MB (2486826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91975ecb4f3500cc041e5d8fd8e930222b0edce814a0cf5164dee07edd777cee`  
		Last Modified: Tue, 01 Sep 2020 19:33:52 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97621bbb0ab928afbe354652af173c50fe7040adc916737d4e3c2c5503e3ca8c`  
		Last Modified: Tue, 01 Sep 2020 19:33:52 GMT  
		Size: 1.9 KB (1860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; 386

```console
$ docker pull yourls@sha256:24bb0ac5d21e5a1aab5bc8f19cfc2a00af0a2920ededc167c51414c0d87b6143
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.0 MB (33038383 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8bc51323d8e8430617a3156b7cb118c1c6b86405adf6b91218e4d59d9cb8f002`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Thu, 11 Jun 2020 19:03:11 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 11 Jun 2020 19:03:12 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 19:03:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 19:03:12 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 19:03:13 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 06 Aug 2020 19:45:06 GMT
ENV PHP_VERSION=7.4.9
# Thu, 06 Aug 2020 19:45:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.9.tar.xz.asc
# Thu, 06 Aug 2020 19:45:07 GMT
ENV PHP_SHA256=23733f4a608ad1bebdcecf0138ebc5fd57cf20d6e0915f98a9444c3f747dc57b PHP_MD5=
# Thu, 06 Aug 2020 19:45:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Aug 2020 19:45:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Sep 2020 00:50:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Sep 2020 00:50:05 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Tue, 01 Sep 2020 00:50:08 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Sep 2020 00:50:08 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Sep 2020 00:50:08 GMT
WORKDIR /var/www/html
# Tue, 01 Sep 2020 00:50:09 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 01 Sep 2020 00:50:09 GMT
STOPSIGNAL SIGQUIT
# Tue, 01 Sep 2020 00:50:09 GMT
EXPOSE 9000
# Tue, 01 Sep 2020 00:50:10 GMT
CMD ["php-fpm"]
# Tue, 01 Sep 2020 16:10:49 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Tue, 01 Sep 2020 16:10:51 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 01 Sep 2020 16:10:53 GMT
RUN apk add --no-cache bash
# Tue, 01 Sep 2020 16:10:53 GMT
ENV YOURLS_VERSION=1.7.9
# Tue, 01 Sep 2020 16:10:54 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Tue, 01 Sep 2020 16:10:56 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 01 Sep 2020 16:10:57 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Tue, 01 Sep 2020 16:10:57 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Tue, 01 Sep 2020 16:10:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Sep 2020 16:10:58 GMT
CMD ["php-fpm"]
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
	-	`sha256:93972427193c396d3baef259db8a6b45f26bef74847b8162c0c11d8f874b3dee`  
		Last Modified: Fri, 07 Aug 2020 00:48:04 GMT  
		Size: 10.3 MB (10308420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2b0722c7ea9f3853989b3777f4f61dbe2f8cd31d65af8ab5ddd20bc4536570b`  
		Last Modified: Fri, 07 Aug 2020 00:48:00 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c7318ac9e797d755d5406c5192e86fa257fa89c26f64d2cda9f8fe8c28a2135`  
		Last Modified: Tue, 01 Sep 2020 05:13:05 GMT  
		Size: 15.0 MB (15022835 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5cb47370795a30e440fa52e964c5156e4699abef81b5fe075e9261ffa305ede`  
		Last Modified: Tue, 01 Sep 2020 05:12:56 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dc1f663351692499691e81781a499bc74779e3b0960e29a6f75c030a81751d0`  
		Last Modified: Tue, 01 Sep 2020 05:12:56 GMT  
		Size: 17.0 KB (16980 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ed717bf9bc4ced68d7f80aeddc8b156c7fb09f63bc59b93440ceba8ecdb2d56`  
		Last Modified: Tue, 01 Sep 2020 05:12:56 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c044d360a0a1c45f75554cecc888c75ec77f29217dec473ac61593a1873733e0`  
		Last Modified: Tue, 01 Sep 2020 16:11:38 GMT  
		Size: 356.6 KB (356553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e450f0fcd524a46cf452d01a46388cf7d49d579a60822502ae0e07ecc790dc1`  
		Last Modified: Tue, 01 Sep 2020 16:11:37 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3fd8b576092ad5a3dc3caec9bcfc33288db934fe99d371ea07e35c0f5fc934`  
		Last Modified: Tue, 01 Sep 2020 16:11:37 GMT  
		Size: 598.7 KB (598665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40a8a94ece886e24130463545d2c7f6814b949c1203246d5dbadd161a133319d`  
		Last Modified: Tue, 01 Sep 2020 16:11:38 GMT  
		Size: 2.5 MB (2486758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:895ca65288e58d9edff5abacd4d213311359bd9ebe397af0736f6c05d44a9a3c`  
		Last Modified: Tue, 01 Sep 2020 16:11:37 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bdb8621c1edff81cf7bd180fdff475b2ea723411ca5a342936deb474fe95b81`  
		Last Modified: Tue, 01 Sep 2020 16:11:37 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; ppc64le

```console
$ docker pull yourls@sha256:1717f7599e24ca33c74cf7ed4ef4555e1e957adfbff061bcb5f25596384cc5ac
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.6 MB (33641841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb1824d919208de42a5b55c8521b3c16fb93f40de1df9675de5459f4c582a490`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Thu, 11 Jun 2020 18:50:39 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 11 Jun 2020 18:50:43 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:50:48 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:50:50 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:50:52 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 06 Aug 2020 19:30:15 GMT
ENV PHP_VERSION=7.4.9
# Thu, 06 Aug 2020 19:30:19 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.9.tar.xz.asc
# Thu, 06 Aug 2020 19:30:26 GMT
ENV PHP_SHA256=23733f4a608ad1bebdcecf0138ebc5fd57cf20d6e0915f98a9444c3f747dc57b PHP_MD5=
# Thu, 06 Aug 2020 19:30:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Aug 2020 19:30:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Sep 2020 04:12:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Sep 2020 04:12:21 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Tue, 01 Sep 2020 04:12:33 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Sep 2020 04:12:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Sep 2020 04:12:38 GMT
WORKDIR /var/www/html
# Tue, 01 Sep 2020 04:12:46 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 01 Sep 2020 04:12:50 GMT
STOPSIGNAL SIGQUIT
# Tue, 01 Sep 2020 04:12:57 GMT
EXPOSE 9000
# Tue, 01 Sep 2020 04:13:05 GMT
CMD ["php-fpm"]
# Wed, 02 Sep 2020 01:58:24 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Wed, 02 Sep 2020 01:58:32 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 02 Sep 2020 01:58:42 GMT
RUN apk add --no-cache bash
# Wed, 02 Sep 2020 01:58:47 GMT
ENV YOURLS_VERSION=1.7.9
# Wed, 02 Sep 2020 01:58:53 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Wed, 02 Sep 2020 01:59:09 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 02 Sep 2020 01:59:12 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Wed, 02 Sep 2020 01:59:13 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Wed, 02 Sep 2020 01:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 02 Sep 2020 01:59:18 GMT
CMD ["php-fpm"]
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
	-	`sha256:d7c779303f6360f9d66b9912cffbfe5185d818eebb5294a339fcf3fa964ff075`  
		Last Modified: Thu, 06 Aug 2020 22:41:04 GMT  
		Size: 10.3 MB (10308451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af4a714b18c5d47131a2e50a00844f1fe1b46a94b973973423fd60c4838266c7`  
		Last Modified: Thu, 06 Aug 2020 22:40:56 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db582eb2a193dd0ebfb20c25d3fac4b9120da9519a8b1b93601220aa9da3e096`  
		Last Modified: Tue, 01 Sep 2020 07:02:57 GMT  
		Size: 15.6 MB (15621184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:390906c63aacc6f015d85d419b4fcb88fe6b56997eb21a97ba98de9c9f0ead66`  
		Last Modified: Tue, 01 Sep 2020 07:02:40 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d15f8d51f5f4c3a602e01d7eb8f9b1cd804ca59a4bcdf6bd9263b5372f10518`  
		Last Modified: Tue, 01 Sep 2020 07:02:40 GMT  
		Size: 17.0 KB (17026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f84590916dc87da7606b4fccbad2cb31913c4d9a828e9483ed98dd98fe754de`  
		Last Modified: Tue, 01 Sep 2020 07:02:40 GMT  
		Size: 8.4 KB (8441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11b500e6e7b243697163c7d6bede14983b9c1096031ca924aeccb604c21048da`  
		Last Modified: Wed, 02 Sep 2020 02:00:43 GMT  
		Size: 382.0 KB (381961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a29354b94661c378fe745e77645df19d69995134afef6f9b7a2827a5d593d96`  
		Last Modified: Wed, 02 Sep 2020 02:00:39 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b90a482bbcf03399ad3fa97552544cb61f079ef14a39030c6314c6dfe56932e6`  
		Last Modified: Wed, 02 Sep 2020 02:00:39 GMT  
		Size: 621.8 KB (621778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db70dcd408a84a2b5aa10e40c5c6ca2aa625c0c0af3209a68cb0380bb523162`  
		Last Modified: Wed, 02 Sep 2020 02:00:40 GMT  
		Size: 2.5 MB (2486818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9beba294816e2cfd9255c5f01fe0091f2ce7db17aac6bd75c52666f3bdb952`  
		Last Modified: Wed, 02 Sep 2020 02:00:39 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef95af008b827c7a307d2bb980637fe39cc4bad5eeb015724d5c605a25a7973`  
		Last Modified: Wed, 02 Sep 2020 02:00:39 GMT  
		Size: 1.9 KB (1863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm-alpine` - linux; s390x

```console
$ docker pull yourls@sha256:78bb1ca90315f501663e36a58e5b597b6c8c1b3768322a6c718facf50f2956fb
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.6 MB (31640709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61eff5030de4906a02625c76c0930dcb0ccd7d980ae5a024754b0721afd76de1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

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
# Thu, 11 Jun 2020 18:32:25 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 11 Jun 2020 18:32:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:32:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 11 Jun 2020 18:32:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 11 Jun 2020 18:32:26 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 06 Aug 2020 18:31:45 GMT
ENV PHP_VERSION=7.4.9
# Thu, 06 Aug 2020 18:31:45 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.9.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.9.tar.xz.asc
# Thu, 06 Aug 2020 18:31:46 GMT
ENV PHP_SHA256=23733f4a608ad1bebdcecf0138ebc5fd57cf20d6e0915f98a9444c3f747dc57b PHP_MD5=
# Thu, 06 Aug 2020 18:31:48 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Aug 2020 18:31:49 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Sep 2020 00:38:32 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Sep 2020 00:38:35 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Tue, 01 Sep 2020 00:38:37 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Sep 2020 00:38:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Sep 2020 00:38:38 GMT
WORKDIR /var/www/html
# Tue, 01 Sep 2020 00:38:40 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 01 Sep 2020 00:38:40 GMT
STOPSIGNAL SIGQUIT
# Tue, 01 Sep 2020 00:38:41 GMT
EXPOSE 9000
# Tue, 01 Sep 2020 00:38:41 GMT
CMD ["php-fpm"]
# Tue, 01 Sep 2020 08:11:20 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Tue, 01 Sep 2020 08:11:21 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 01 Sep 2020 08:11:22 GMT
RUN apk add --no-cache bash
# Tue, 01 Sep 2020 08:11:22 GMT
ENV YOURLS_VERSION=1.7.9
# Tue, 01 Sep 2020 08:11:23 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Tue, 01 Sep 2020 08:11:25 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 01 Sep 2020 08:11:25 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Tue, 01 Sep 2020 08:11:25 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Tue, 01 Sep 2020 08:11:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 01 Sep 2020 08:11:26 GMT
CMD ["php-fpm"]
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
	-	`sha256:7d51e4d8457567779a3fada86c3e334db1d4aefec50cf6a47f75f537dce6bdb3`  
		Last Modified: Thu, 06 Aug 2020 19:48:02 GMT  
		Size: 10.3 MB (10308439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b25125812a7321805d8d1febb01b4102c94936568f43282a4f411a4e55aa289`  
		Last Modified: Thu, 06 Aug 2020 19:47:59 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dc9e1a50f007d300e48040836bdd04dad3446946b4d523c38cc211cce31f7f8`  
		Last Modified: Tue, 01 Sep 2020 02:26:30 GMT  
		Size: 13.9 MB (13942540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a789ef6260742a18d66c66e7044a716c216e3af6c145e1afdcf113ffb54e763e`  
		Last Modified: Tue, 01 Sep 2020 02:26:27 GMT  
		Size: 2.3 KB (2278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2b764b62adf97a7535715fae171a18f233b5e5a5dd7d2e7a37aed1d13a6db5d`  
		Last Modified: Tue, 01 Sep 2020 02:26:27 GMT  
		Size: 17.0 KB (17002 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2fb055b55c651d4d1988019417d3d1d3ee6382f2b8ac2b01bd25b81ae30f677`  
		Last Modified: Tue, 01 Sep 2020 02:26:27 GMT  
		Size: 8.4 KB (8447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6e6b0008b45048b99092f5e25b1545d1ec7ea29231655f06b222ea50f162a59`  
		Last Modified: Tue, 01 Sep 2020 08:12:12 GMT  
		Size: 344.1 KB (344097 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6594300c27e4cdec0d422cec601c39b91e6d35482a8c9dcd8749ca9b8e1cd8`  
		Last Modified: Tue, 01 Sep 2020 08:12:10 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26480a647307b7405761dbb8763d75abcc8a8940f834643c0a26aba9841cafae`  
		Last Modified: Tue, 01 Sep 2020 08:12:10 GMT  
		Size: 576.8 KB (576770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:733f443eaccf1694e62477fafbb9cb3f110a93c59ce39f981269910650ede193`  
		Last Modified: Tue, 01 Sep 2020 08:12:11 GMT  
		Size: 2.5 MB (2486816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20401cdc48e800da9833cb7ab26a364efdfc4b6ef376fa0190f27b221be91868`  
		Last Modified: Tue, 01 Sep 2020 08:12:10 GMT  
		Size: 1.2 KB (1180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff512e0d9a536d2ea561928fc670cf1ea75cafb92675ca92ead5e8d1746d363b`  
		Last Modified: Tue, 01 Sep 2020 08:12:10 GMT  
		Size: 1.9 KB (1857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
