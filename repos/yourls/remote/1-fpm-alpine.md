## `yourls:1-fpm-alpine`

```console
$ docker pull yourls@sha256:fca69c889257fedd4c0ca5bfb792888ecb9d2f93b1733e4e3831ef0414fbe4ed
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

### `yourls:1-fpm-alpine` - linux; amd64

```console
$ docker pull yourls@sha256:7c90dd1884989a78e08ee3c12929e28e68e40921ca7f42edee828c157ee722ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32073915 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18d03bd4ac124a881fd86ae4e4a0a28175a9f3b33733b9c9839bf34ba51cfa74`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:03 GMT
ADD file:b91adb67b670d3a6ff9463e48b7def903ed516be66fc4282d22c53e41512be49 in / 
# Fri, 24 Apr 2020 01:05:03 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 17:35:49 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 24 Apr 2020 17:35:50 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 24 Apr 2020 17:35:51 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 24 Apr 2020 17:35:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 24 Apr 2020 17:35:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 24 Apr 2020 17:41:08 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 24 Apr 2020 17:41:08 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 17:41:08 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 17:41:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Apr 2020 17:41:09 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 24 Apr 2020 17:41:09 GMT
ENV PHP_VERSION=7.4.5
# Wed, 06 May 2020 21:47:12 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.5.tar.xz.asc
# Wed, 06 May 2020 21:47:12 GMT
ENV PHP_SHA256=d059fd7f55bdc4d2eada15a00a2976697010d3631ef6f83149cc5289e1f23c2c PHP_MD5=
# Wed, 06 May 2020 21:47:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 06 May 2020 21:47:15 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 06 May 2020 21:55:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 06 May 2020 21:55:02 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Wed, 06 May 2020 21:55:03 GMT
RUN docker-php-ext-enable sodium
# Wed, 06 May 2020 21:55:03 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 06 May 2020 21:55:03 GMT
WORKDIR /var/www/html
# Wed, 06 May 2020 21:55:04 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 06 May 2020 21:55:04 GMT
STOPSIGNAL SIGQUIT
# Wed, 06 May 2020 21:55:05 GMT
EXPOSE 9000
# Wed, 06 May 2020 21:55:05 GMT
CMD ["php-fpm"]
# Thu, 07 May 2020 04:22:59 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 07 May 2020 04:23:01 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 07 May 2020 04:23:03 GMT
RUN apk add --no-cache bash
# Thu, 07 May 2020 04:23:03 GMT
ENV YOURLS_VERSION=1.7.9
# Thu, 07 May 2020 04:23:04 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Thu, 07 May 2020 04:23:05 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 07 May 2020 04:23:06 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Thu, 07 May 2020 04:23:06 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 07 May 2020 04:23:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 May 2020 04:23:06 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:cbdbe7a5bc2a134ca8ec91be58565ec07d037386d1f1d8385412d224deafca08`  
		Last Modified: Thu, 23 Apr 2020 14:07:19 GMT  
		Size: 2.8 MB (2813316 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bc86e4cff5f320d778d7412cab415d31e8e986659b5e453545b0a7afe86d472`  
		Last Modified: Fri, 24 Apr 2020 19:16:17 GMT  
		Size: 1.4 MB (1355296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be142bd33f5003d85a3e056208af127ac6c5f627f263469134baafdd011ad59`  
		Last Modified: Fri, 24 Apr 2020 19:16:16 GMT  
		Size: 1.2 KB (1232 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8132c9e52be363f64724649f370635dd54cac7b8696c6365dd2011290afbc7c0`  
		Last Modified: Fri, 24 Apr 2020 19:16:16 GMT  
		Size: 221.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9467fff4c3068c9f9af51bc4aa9274eb3218f837a9cfe85b964ad8b183140e32`  
		Last Modified: Thu, 07 May 2020 02:27:09 GMT  
		Size: 10.3 MB (10290376 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee9ddeb5909ea2e72947667948a1756a382e59c0c3fc9bf64272c9da3cfc5c45`  
		Last Modified: Thu, 07 May 2020 02:27:08 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2667b8d524974614a1a2c51c2036639857401ea193ef4aa3e485f2f8f5843bae`  
		Last Modified: Thu, 07 May 2020 02:27:11 GMT  
		Size: 14.2 MB (14189414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56da801a07b57e39fc20126cace9149c31273de66e8c31b0711e959f81168be`  
		Last Modified: Thu, 07 May 2020 02:27:08 GMT  
		Size: 2.2 KB (2217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ada6e169bdb446e459de6f1c47b23499ea02ea058e4b193c34a94edf4967b0b`  
		Last Modified: Thu, 07 May 2020 02:27:07 GMT  
		Size: 17.1 KB (17107 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756aad2aea0a80949e1c88f4974132a68fa8a3d218674ad5c2e7467e2240d10a`  
		Last Modified: Thu, 07 May 2020 02:27:07 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0147cb696b8ce633de61b595ed041d32b7e02b4ca020ab13a053f840e52c13`  
		Last Modified: Thu, 07 May 2020 04:23:39 GMT  
		Size: 348.1 KB (348100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9e940b59b7f987a3dd9e990ab28fcb5cd3ef9689963f32d3f5a3c7b74ff7255`  
		Last Modified: Thu, 07 May 2020 04:23:37 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f6ba708a336c48b29c96a1ff027afa3cd3776d6095c69c94749dad64d0b704c`  
		Last Modified: Thu, 07 May 2020 04:23:38 GMT  
		Size: 557.6 KB (557574 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:100b8cfa9da52d20480debac0317f3bc363be1c746cbc6aec6ae2235e550f4ea`  
		Last Modified: Thu, 07 May 2020 04:23:38 GMT  
		Size: 2.5 MB (2486756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a966c448f675c88f6d109265673ba06bea64f085ba8900f488f75fda8ee82e9`  
		Last Modified: Thu, 07 May 2020 04:23:38 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd47cb7b045f658d5518cce0959e48c23738d3d7714a98c22ae7ad6df4044443`  
		Last Modified: Thu, 07 May 2020 04:23:37 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; arm variant v6

```console
$ docker pull yourls@sha256:cc49b6b84668498748348d7ef2a5a84722fe9bae5c48564d5d273cb8a249d5c7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.8 MB (30833279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d16087edf1068f8a6a72d9db2054441c3ac4ff9bc06cf1529ffe53815df3289c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:24 GMT
ADD file:cc0770cddff6b50d5e31f39886420eb8a0b4af55664d6f7599207c9aeaf6a501 in / 
# Thu, 23 Apr 2020 15:51:25 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 22:40:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 23 Apr 2020 22:40:31 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 23 Apr 2020 22:40:34 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 23 Apr 2020 22:40:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 22:40:37 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 22:44:52 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 23 Apr 2020 22:44:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 22:44:54 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 22:44:55 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 22:44:56 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Apr 2020 22:44:56 GMT
ENV PHP_VERSION=7.4.5
# Wed, 06 May 2020 21:53:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.5.tar.xz.asc
# Wed, 06 May 2020 21:53:48 GMT
ENV PHP_SHA256=d059fd7f55bdc4d2eada15a00a2976697010d3631ef6f83149cc5289e1f23c2c PHP_MD5=
# Wed, 06 May 2020 21:53:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 06 May 2020 21:53:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 06 May 2020 21:57:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 06 May 2020 21:57:44 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Wed, 06 May 2020 21:57:53 GMT
RUN docker-php-ext-enable sodium
# Wed, 06 May 2020 21:57:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 06 May 2020 21:58:01 GMT
WORKDIR /var/www/html
# Wed, 06 May 2020 21:58:05 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 06 May 2020 21:58:06 GMT
STOPSIGNAL SIGQUIT
# Wed, 06 May 2020 21:58:07 GMT
EXPOSE 9000
# Wed, 06 May 2020 21:58:07 GMT
CMD ["php-fpm"]
# Thu, 07 May 2020 00:28:25 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 07 May 2020 00:28:26 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 07 May 2020 00:28:29 GMT
RUN apk add --no-cache bash
# Thu, 07 May 2020 00:28:29 GMT
ENV YOURLS_VERSION=1.7.9
# Thu, 07 May 2020 00:28:30 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Thu, 07 May 2020 00:28:33 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 07 May 2020 00:28:34 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Thu, 07 May 2020 00:28:35 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 07 May 2020 00:28:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 May 2020 00:28:36 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b9e3228833e92f0688e0f87234e75965e62e47cfbb9ca8cc5fa19c2e7cd13f80`  
		Last Modified: Thu, 23 Apr 2020 15:52:05 GMT  
		Size: 2.6 MB (2619936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e4a0b35ae612f97f86d2cb9a5c35d9974c53c9693ed9c503293a2ed4d1f5eb`  
		Last Modified: Thu, 23 Apr 2020 23:53:32 GMT  
		Size: 1.3 MB (1321299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:744673dda954515280697917b25c13df9ff57231c28643848fc80b349d6b246b`  
		Last Modified: Thu, 23 Apr 2020 23:53:31 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6829673d00afbe39285f6e4d9977770c99d7bf841436086efa137773c99fd188`  
		Last Modified: Thu, 23 Apr 2020 23:53:31 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d633e7dbb2e24ee5e0103e7957d30a1f498b7d297e7c050d6eb1dcf34c2159eb`  
		Last Modified: Wed, 06 May 2020 23:06:51 GMT  
		Size: 10.3 MB (10290398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2cdbbf67c433fa39c3b6ca958a7643207e98fc3ab71c0d17d5c6126318bd3b4`  
		Last Modified: Wed, 06 May 2020 23:06:49 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fccd5a9be4326c709b72820ae25b4ec7541bc258585a9524c7785904995f8f41`  
		Last Modified: Wed, 06 May 2020 23:06:54 GMT  
		Size: 13.2 MB (13218115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:001c46f4cc0e6fc460a107ba7b695521a589b09b484a9cce716894c49e96e89b`  
		Last Modified: Wed, 06 May 2020 23:06:49 GMT  
		Size: 2.2 KB (2219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:681a1e8fae8446ebb8b7d875183264264bc8f5b805b24842ae9a0a4e4e031d10`  
		Last Modified: Wed, 06 May 2020 23:06:49 GMT  
		Size: 17.1 KB (17092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbb16ed95f2527fd256504d376dac4429930d2af50f78e415ac6d9b56fc95e1e`  
		Last Modified: Wed, 06 May 2020 23:06:49 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7aa64a98d2f8a639f332389cc6e81ff7f4591e5a042733f2c1ada0f4321dd569`  
		Last Modified: Thu, 07 May 2020 00:28:53 GMT  
		Size: 326.7 KB (326677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f45c393920c59ac03e7c151e24d60146706b4cb40b582a7fc148e13e7ef26b4e`  
		Last Modified: Thu, 07 May 2020 00:28:52 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4b5e86782af72b086d7d50d867c9efc2f0d077b305f46985d7d03c55f0428d8`  
		Last Modified: Thu, 07 May 2020 00:28:52 GMT  
		Size: 536.9 KB (536889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcae962844dd2f1ba462a0e947be3d7e4f1bdc86a0272f748a2ba76e6d30e5f4`  
		Last Modified: Thu, 07 May 2020 00:28:52 GMT  
		Size: 2.5 MB (2486816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577bb5478b1b70c520b02abb60b9d6810239f966c0ebf5c054adeec1f505cd79`  
		Last Modified: Thu, 07 May 2020 00:28:52 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d326b69f0666707fedd040a0d606ad4a0d48080ff57647d063012d3968b78a27`  
		Last Modified: Thu, 07 May 2020 00:28:51 GMT  
		Size: 1.9 KB (1860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; arm variant v7

```console
$ docker pull yourls@sha256:2e4d5b0bad3bf05734916aa50ec1c759b383ad08dd7de5114f3de9cd39ea0158
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.6 MB (29617244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3351b05c7cb0e1a452892287bcdd665e39523dcd2bd08d0d7ede85c91825a4c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Apr 2020 22:04:19 GMT
ADD file:33578d3cacfab86c195d99396dd012ec511796a1d2d8d6f0a02b8a055673c294 in / 
# Thu, 23 Apr 2020 22:04:22 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 09:12:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 24 Apr 2020 09:12:32 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 24 Apr 2020 09:12:34 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 24 Apr 2020 09:12:35 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 24 Apr 2020 09:12:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 24 Apr 2020 09:15:20 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 24 Apr 2020 09:15:21 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 09:15:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 09:15:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Apr 2020 09:15:23 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 24 Apr 2020 09:15:23 GMT
ENV PHP_VERSION=7.4.5
# Wed, 06 May 2020 22:19:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.5.tar.xz.asc
# Wed, 06 May 2020 22:19:07 GMT
ENV PHP_SHA256=d059fd7f55bdc4d2eada15a00a2976697010d3631ef6f83149cc5289e1f23c2c PHP_MD5=
# Wed, 06 May 2020 22:19:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 06 May 2020 22:19:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 06 May 2020 22:22:28 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 06 May 2020 22:22:30 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Wed, 06 May 2020 22:22:33 GMT
RUN docker-php-ext-enable sodium
# Wed, 06 May 2020 22:22:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 06 May 2020 22:22:35 GMT
WORKDIR /var/www/html
# Wed, 06 May 2020 22:22:37 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 06 May 2020 22:22:38 GMT
STOPSIGNAL SIGQUIT
# Wed, 06 May 2020 22:22:39 GMT
EXPOSE 9000
# Wed, 06 May 2020 22:22:40 GMT
CMD ["php-fpm"]
# Thu, 07 May 2020 04:05:57 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 07 May 2020 04:06:00 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 07 May 2020 04:06:02 GMT
RUN apk add --no-cache bash
# Thu, 07 May 2020 04:06:04 GMT
ENV YOURLS_VERSION=1.7.9
# Thu, 07 May 2020 04:06:04 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Thu, 07 May 2020 04:06:08 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 07 May 2020 04:06:09 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Thu, 07 May 2020 04:06:09 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 07 May 2020 04:06:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 May 2020 04:06:11 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3cfb62949d9d8613854db4d5fe502a9219c2b55a153043500078a64e880ae234`  
		Last Modified: Thu, 23 Apr 2020 22:05:12 GMT  
		Size: 2.4 MB (2422063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39281f57fe7d3f99c4fe23af0e5eb45caa0646180d5ff71304d26ff35a0b9856`  
		Last Modified: Fri, 24 Apr 2020 11:16:34 GMT  
		Size: 1.2 MB (1227897 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8df36ec4ede8343ef6e75d1f33f8dbbe0ccdfa6522152dda7801db48b8a06b85`  
		Last Modified: Fri, 24 Apr 2020 11:16:33 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2e16ed34ef7f3b453ef768e1198de2318c7d1cdd60f43223f1c53df2e82119e`  
		Last Modified: Fri, 24 Apr 2020 11:16:33 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c87109265e035b6386876832025dc78ed209196557e248043020bcdf4cb7725`  
		Last Modified: Thu, 07 May 2020 00:30:47 GMT  
		Size: 10.3 MB (10290405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1374a3e0f04a48634adf3411d8e5c8b6eaf45093fcbdee1b67b03928e557d2d`  
		Last Modified: Thu, 07 May 2020 00:30:40 GMT  
		Size: 498.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab1ec5b5cea0f9c133f27590747d61058a23b262570f47e4e8f81593ed72d39a`  
		Last Modified: Thu, 07 May 2020 00:30:47 GMT  
		Size: 12.4 MB (12365008 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd1b02cbdf1c02db1df55435e8c24e111128c498b3e8e72a5d86fb49a39caf5`  
		Last Modified: Thu, 07 May 2020 00:30:40 GMT  
		Size: 2.2 KB (2217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccc7b0148d6f35df83321d5ed9bbafe91bf890f75cdede191f1a3305bbabd460`  
		Last Modified: Thu, 07 May 2020 00:30:40 GMT  
		Size: 17.1 KB (17076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49e5dc7111790dc58ea3743e4c872e25ea37150e72c255165ea9958d1a59ef01`  
		Last Modified: Thu, 07 May 2020 00:30:40 GMT  
		Size: 8.4 KB (8442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94e7c64e96e703d3270fb461370508e341c34ed52e2ef5957c73e362870dd552`  
		Last Modified: Thu, 07 May 2020 04:06:58 GMT  
		Size: 302.7 KB (302738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:607afbdbf090b0789fe5aa87905a2dc78114311a18b040a8b25a2e020e65a9fc`  
		Last Modified: Thu, 07 May 2020 04:06:57 GMT  
		Size: 324.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91406b1f400b372f2d54bb0f0e24604faafc056749f01efd32687c21420008ac`  
		Last Modified: Thu, 07 May 2020 04:06:56 GMT  
		Size: 489.2 KB (489189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09be42028a0810b3b04484a20b045c55be1fddbe078608100996def46d57cc06`  
		Last Modified: Thu, 07 May 2020 04:06:57 GMT  
		Size: 2.5 MB (2486816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0fec7c12f5d982943a8aad77cbda1a3e813a8efb1c0c6106488c9f813f270c4`  
		Last Modified: Thu, 07 May 2020 04:06:57 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bdc507860becb1ef6e5ee279bdf73446ad8b147fba746f9ddbbffe15a4c24e2`  
		Last Modified: Thu, 07 May 2020 04:06:56 GMT  
		Size: 1.9 KB (1860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:5a73a827b7fe24e451d9398c60f7594d1f8ae013e960d0703ddee8fc390cf3e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31795557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df802d45fb280666ae9e549789ded89bb46e1c1ef840f3eb0cd6cd850388bcec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:18 GMT
ADD file:85ae77bc1e43353ff14e6fe1658be1ed4ecbf4330212ac3d7ab7462add32dd39 in / 
# Fri, 24 Apr 2020 00:14:21 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 12:51:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 24 Apr 2020 12:51:32 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 24 Apr 2020 12:51:35 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 24 Apr 2020 12:51:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 24 Apr 2020 12:51:38 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 24 Apr 2020 12:55:36 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 24 Apr 2020 12:55:37 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 12:55:39 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 12:55:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Apr 2020 12:55:41 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 24 Apr 2020 12:55:43 GMT
ENV PHP_VERSION=7.4.5
# Wed, 06 May 2020 22:01:28 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.5.tar.xz.asc
# Wed, 06 May 2020 22:01:28 GMT
ENV PHP_SHA256=d059fd7f55bdc4d2eada15a00a2976697010d3631ef6f83149cc5289e1f23c2c PHP_MD5=
# Wed, 06 May 2020 22:01:33 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 06 May 2020 22:01:34 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 06 May 2020 22:05:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 06 May 2020 22:05:21 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Wed, 06 May 2020 22:05:24 GMT
RUN docker-php-ext-enable sodium
# Wed, 06 May 2020 22:05:25 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 06 May 2020 22:05:26 GMT
WORKDIR /var/www/html
# Wed, 06 May 2020 22:05:28 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 06 May 2020 22:05:28 GMT
STOPSIGNAL SIGQUIT
# Wed, 06 May 2020 22:05:29 GMT
EXPOSE 9000
# Wed, 06 May 2020 22:05:31 GMT
CMD ["php-fpm"]
# Thu, 07 May 2020 03:24:09 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 07 May 2020 03:24:11 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 07 May 2020 03:24:14 GMT
RUN apk add --no-cache bash
# Thu, 07 May 2020 03:24:15 GMT
ENV YOURLS_VERSION=1.7.9
# Thu, 07 May 2020 03:24:16 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Thu, 07 May 2020 03:24:19 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 07 May 2020 03:24:20 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Thu, 07 May 2020 03:24:21 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 07 May 2020 03:24:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 May 2020 03:24:25 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:29e5d40040c18c692ed73df24511071725b74956ca1a61fe6056a651d86a13bd`  
		Last Modified: Fri, 24 Apr 2020 00:15:41 GMT  
		Size: 2.7 MB (2724424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f8614da4aa8d46e10af7f7788136931561b8f1d1efe1a78311b26f5cf57506f`  
		Last Modified: Fri, 24 Apr 2020 14:02:47 GMT  
		Size: 1.4 MB (1359714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ececdba1264fbd4760d671f21f71713e4038fc665ad77ae891d54cc1d8db0cc3`  
		Last Modified: Fri, 24 Apr 2020 14:02:46 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eab4eb699b8d1e5be3d1e82202067c943b8869558f71be0d2557563912b0f942`  
		Last Modified: Fri, 24 Apr 2020 14:02:47 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28613a2dfdaaf8030e7d55d7e1d619fbbc7d3c88b1d484dd1da916d7ddb0fd31`  
		Last Modified: Thu, 07 May 2020 00:24:13 GMT  
		Size: 10.3 MB (10290395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1f125f384cef77fc4a225ec84d3a73ac45f47ba62c615d58063e15a3c4f82c3`  
		Last Modified: Thu, 07 May 2020 00:24:11 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ca36b76af7c72301a47c9e7b255c17f1e80a9e42e976447316915c8824f64dc`  
		Last Modified: Thu, 07 May 2020 00:24:14 GMT  
		Size: 14.0 MB (13991089 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:297cb3dc5909929558b9d2e887862137b0e776fc0a2f19b0d98c3d3f863f3be6`  
		Last Modified: Thu, 07 May 2020 00:24:10 GMT  
		Size: 2.2 KB (2217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5afcb3ee02e9e8f8bd94acb2d204bb15af9a46af972b69a210d8c4f8beee7de7`  
		Last Modified: Thu, 07 May 2020 00:24:11 GMT  
		Size: 17.1 KB (17096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bca2c9abf750153a8901dc9bbbda0ca71dd1287439f1a2e185508822d8d63e17`  
		Last Modified: Thu, 07 May 2020 00:24:10 GMT  
		Size: 8.4 KB (8443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26434b17017cf728f00c37694364d8e62e84ea676223aa8a396647e45dce286a`  
		Last Modified: Thu, 07 May 2020 03:25:11 GMT  
		Size: 341.0 KB (340960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82640af21988c857002149bb5dc1fe27fa9a0ca7a30318bff8ca79865d55a21f`  
		Last Modified: Thu, 07 May 2020 03:25:09 GMT  
		Size: 325.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b425ac13d94dceafe52ac694c9b090dbfdd6247b0ce6385ee0e279cd9a15c2b`  
		Last Modified: Thu, 07 May 2020 03:25:09 GMT  
		Size: 569.0 KB (568999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7384bad66072dcff31c4efcc5a156e39f62080840a31ec9ed8137330c4b3c290`  
		Last Modified: Thu, 07 May 2020 03:25:10 GMT  
		Size: 2.5 MB (2486824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:173b2b40822651bd98c4aedd3858651c9bc944ef819b5373790fd59d28ff90c9`  
		Last Modified: Thu, 07 May 2020 03:25:09 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7d4323fc2fc99af71b74b74b412c5a9aaa86efc7dab8f342b9f13752583d3ee`  
		Last Modified: Thu, 07 May 2020 03:25:09 GMT  
		Size: 1.9 KB (1861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; 386

```console
$ docker pull yourls@sha256:858b3675bfd678163e31cc300b0be998544f764d16f6900989d57d22d5cb8373
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.6 MB (32626816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:245367aa58de4510e525e6803c5a7f2d82b62eaf6ff0aac7d2beb32c462390f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:04 GMT
ADD file:63bd8a316cba8c404cc2e32a5120406c24aee8db3224c469a6077b941d900863 in / 
# Thu, 23 Apr 2020 21:16:04 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 06:05:44 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 24 Apr 2020 06:05:46 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 24 Apr 2020 06:05:47 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 24 Apr 2020 06:05:47 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 24 Apr 2020 06:05:48 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 24 Apr 2020 06:11:34 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 24 Apr 2020 06:11:35 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 06:11:35 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 06:11:35 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Apr 2020 06:11:35 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 24 Apr 2020 06:11:35 GMT
ENV PHP_VERSION=7.4.5
# Wed, 06 May 2020 22:22:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.5.tar.xz.asc
# Wed, 06 May 2020 22:22:25 GMT
ENV PHP_SHA256=d059fd7f55bdc4d2eada15a00a2976697010d3631ef6f83149cc5289e1f23c2c PHP_MD5=
# Wed, 06 May 2020 22:22:28 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 06 May 2020 22:22:28 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 06 May 2020 22:32:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 06 May 2020 22:32:08 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Wed, 06 May 2020 22:32:09 GMT
RUN docker-php-ext-enable sodium
# Wed, 06 May 2020 22:32:09 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 06 May 2020 22:32:10 GMT
WORKDIR /var/www/html
# Wed, 06 May 2020 22:32:10 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 06 May 2020 22:32:11 GMT
STOPSIGNAL SIGQUIT
# Wed, 06 May 2020 22:32:11 GMT
EXPOSE 9000
# Wed, 06 May 2020 22:32:11 GMT
CMD ["php-fpm"]
# Thu, 07 May 2020 05:29:23 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 07 May 2020 05:29:23 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 07 May 2020 05:29:25 GMT
RUN apk add --no-cache bash
# Thu, 07 May 2020 05:29:25 GMT
ENV YOURLS_VERSION=1.7.9
# Thu, 07 May 2020 05:29:25 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Thu, 07 May 2020 05:29:27 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 07 May 2020 05:29:27 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Thu, 07 May 2020 05:29:27 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 07 May 2020 05:29:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 May 2020 05:29:28 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:2826c1e79865da7e0da0a993a2a38db61c3911e05b5df617439a86d4deac90fb`  
		Last Modified: Thu, 23 Apr 2020 21:16:32 GMT  
		Size: 2.8 MB (2808418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:990138137e85533c48403b0cd1aee9ac6c5f3fc3be67a74a44a22f1a30e39af6`  
		Last Modified: Fri, 24 Apr 2020 07:59:39 GMT  
		Size: 1.5 MB (1453100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d973cd3524efeb6727b2144c33f96c71896f4ee22b1a55cc0c5aa5756f9b758`  
		Last Modified: Fri, 24 Apr 2020 07:59:37 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f386ab173ce6081c15380f99f906f8ea531e5748425804a21ebb0b5c433e6782`  
		Last Modified: Fri, 24 Apr 2020 07:59:38 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c75d1ba3f1786b1cb10f05c660d98da3d9aea858073a6eacba203d07571b51ec`  
		Last Modified: Thu, 07 May 2020 03:04:45 GMT  
		Size: 10.3 MB (10290393 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982a4f02de2ed6a91f6a172841e750168f104afc2f7f0b9e2993c7a4cb529201`  
		Last Modified: Thu, 07 May 2020 03:04:42 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75ea0a816a2f0877e4e8beb560f2222100d50f438d9789ccd6e0cd5a42c6999f`  
		Last Modified: Thu, 07 May 2020 03:04:48 GMT  
		Size: 14.6 MB (14599571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57b7137caa893703c7f307c2d0adda2d35a1ece228b0cf87ec491e9995cb093`  
		Last Modified: Thu, 07 May 2020 03:04:43 GMT  
		Size: 2.2 KB (2218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f34e1766cca5c5bf49713f116377075618ab21f69f8ac80a796df959163a0df0`  
		Last Modified: Thu, 07 May 2020 03:04:42 GMT  
		Size: 17.1 KB (17108 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee203a7d5bfd77cdad8c0ba109d858cd7c918f535940d035c3d9576fabe5cc37`  
		Last Modified: Thu, 07 May 2020 03:04:42 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60f87d035c0edb6cbf27733baf76505503087a660c6f06ae2ae64fa47f3d2a3f`  
		Last Modified: Thu, 07 May 2020 05:29:59 GMT  
		Size: 356.8 KB (356760 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77b0e643f802cd367d18bf14a14ca730b1abd2670ff85e439a9f62d544e355c`  
		Last Modified: Thu, 07 May 2020 05:29:58 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:281b5b9af806a7ec0f12f5430b7bdf7a375c454de4e07cba7e9f480bde186b04`  
		Last Modified: Thu, 07 May 2020 05:29:58 GMT  
		Size: 598.7 KB (598729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368de5da3c0850dd399fff257a6dad24a91baf68df325d7f848d6080a33467b8`  
		Last Modified: Thu, 07 May 2020 05:29:58 GMT  
		Size: 2.5 MB (2486756 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c791856421c58a0938c10f54d3c5245c4d0121e4ab31699795c961888238c851`  
		Last Modified: Thu, 07 May 2020 05:29:58 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:523b02585cf448776ca6fc7ec4209a81ecd6a26d4282e854c4362c24e8d31e01`  
		Last Modified: Thu, 07 May 2020 05:29:58 GMT  
		Size: 1.9 KB (1859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; ppc64le

```console
$ docker pull yourls@sha256:d4a23764948b7e6a53a36c9ea23ed980f28690e967bcab5ffe9ab16ba8bdb12c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.2 MB (33205557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3632440a4019cbe72c905ae842fe61943b7383ff5e44c9f7a06ea15c526a0431`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Apr 2020 20:39:04 GMT
ADD file:1aaebe252dfb1885e066fcbc84aaa915bae149c3608f19600855ad1d4f7450c1 in / 
# Thu, 23 Apr 2020 20:39:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Apr 2020 07:11:31 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Fri, 24 Apr 2020 07:11:47 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Fri, 24 Apr 2020 07:12:07 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Fri, 24 Apr 2020 07:12:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Fri, 24 Apr 2020 07:12:28 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Fri, 24 Apr 2020 07:18:49 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Fri, 24 Apr 2020 07:18:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 07:18:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Fri, 24 Apr 2020 07:18:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Fri, 24 Apr 2020 07:19:03 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Fri, 24 Apr 2020 07:19:06 GMT
ENV PHP_VERSION=7.4.5
# Wed, 06 May 2020 21:45:11 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.5.tar.xz.asc
# Wed, 06 May 2020 21:45:19 GMT
ENV PHP_SHA256=d059fd7f55bdc4d2eada15a00a2976697010d3631ef6f83149cc5289e1f23c2c PHP_MD5=
# Wed, 06 May 2020 21:45:49 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 06 May 2020 21:45:50 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 06 May 2020 21:49:37 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 06 May 2020 21:49:39 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Wed, 06 May 2020 21:49:43 GMT
RUN docker-php-ext-enable sodium
# Wed, 06 May 2020 21:49:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 06 May 2020 21:49:50 GMT
WORKDIR /var/www/html
# Wed, 06 May 2020 21:50:02 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 06 May 2020 21:50:06 GMT
STOPSIGNAL SIGQUIT
# Wed, 06 May 2020 21:50:09 GMT
EXPOSE 9000
# Wed, 06 May 2020 21:50:11 GMT
CMD ["php-fpm"]
# Thu, 07 May 2020 05:11:48 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 07 May 2020 05:11:53 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 07 May 2020 05:11:58 GMT
RUN apk add --no-cache bash
# Thu, 07 May 2020 05:12:00 GMT
ENV YOURLS_VERSION=1.7.9
# Thu, 07 May 2020 05:12:03 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Thu, 07 May 2020 05:12:08 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 07 May 2020 05:12:12 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Thu, 07 May 2020 05:12:13 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 07 May 2020 05:12:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 May 2020 05:12:16 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:9a8fdc5b698322331ee7eba7dd6f66f3a4e956554db22dd1e834d519415b4f8e`  
		Last Modified: Thu, 23 Apr 2020 20:41:33 GMT  
		Size: 2.8 MB (2821843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d52f33021895c8254527a626bd23b02f5ffb7cf7d498663099bfb52bc36cb4f`  
		Last Modified: Fri, 24 Apr 2020 08:53:41 GMT  
		Size: 1.4 MB (1398496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca0df5facaec815af37eabcf3f16b8d84fbf49322219c06e6d19e7067b54f86`  
		Last Modified: Fri, 24 Apr 2020 08:53:38 GMT  
		Size: 1.3 KB (1266 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5eafa9bf45f1a09b417cf061af38e982c6a4e2c77a1f1f3c59b8587f215c9208`  
		Last Modified: Fri, 24 Apr 2020 08:53:37 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd6f9fc5f5dd5a6a01d122eceb81e154d6b504a4824dfd1cf3d30bb7a9e9e97c`  
		Last Modified: Thu, 07 May 2020 01:07:44 GMT  
		Size: 10.3 MB (10290417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29a43bd66c21c56dbd152e7576bd7d3267023382761fcd2f22d9c040fb4a968d`  
		Last Modified: Thu, 07 May 2020 01:07:39 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7efdee5bd1f78cf0c558b086caea4e00215615bd684bc2cc5a37edcf881f2e21`  
		Last Modified: Thu, 07 May 2020 01:07:47 GMT  
		Size: 15.2 MB (15170513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:825f3b822c1c1afaa23874e2526891cef8118b2595814954a67087320cebce2b`  
		Last Modified: Thu, 07 May 2020 01:07:39 GMT  
		Size: 2.2 KB (2220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa15e99095f038dfdf4add1f9bd7321440da65e191755920838b890383ee5a3e`  
		Last Modified: Thu, 07 May 2020 01:07:40 GMT  
		Size: 17.1 KB (17095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34aa754600f43b8d422d8942d68b3012a94dc7b1641add826c12f369a56a5bb1`  
		Last Modified: Thu, 07 May 2020 01:07:39 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff85c62557f4b78ee229f604d3f63072385d15b205710b7eaaa1870414e0d2e5`  
		Last Modified: Thu, 07 May 2020 05:13:36 GMT  
		Size: 382.0 KB (382032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee2c7685bd6b9c398780deb22d0fa22ca1eacc092a25f9095b460359643101d`  
		Last Modified: Thu, 07 May 2020 05:13:35 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c86e6a9e3444e00698f58c0ec502050a1f2e9b05d78304b439158c4831a0330`  
		Last Modified: Thu, 07 May 2020 05:13:34 GMT  
		Size: 622.3 KB (622277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02dd8c4d8df15a5a7f977c4ddff3a38ee24c2a45e79bb70e197fbc31d7772b59`  
		Last Modified: Thu, 07 May 2020 05:13:35 GMT  
		Size: 2.5 MB (2486814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b10a0c2566583792e2c71379ae4b69932045e4243abfcceb4038302bdd9e3ae3`  
		Last Modified: Thu, 07 May 2020 05:13:33 GMT  
		Size: 1.2 KB (1185 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b30be6ed4f954204067529bc38809c222af7522b63891777e4af7aef674006c`  
		Last Modified: Thu, 07 May 2020 05:13:34 GMT  
		Size: 1.9 KB (1858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; s390x

```console
$ docker pull yourls@sha256:1a005f5fb7a4c9a5f11052baea9927ffb2ebdb82e837d9d417863ea2439541ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.2 MB (31208769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:17a7f524d1b2b2c9bd13712ef8df2180c56064af48490f59d0d85e61a8e94243`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Apr 2020 17:50:57 GMT
ADD file:a59a30c2fd43c9f3b820751a6f5a54688c14440a1ddace1ab255475f46e6ba2d in / 
# Thu, 23 Apr 2020 17:50:58 GMT
CMD ["/bin/sh"]
# Thu, 23 Apr 2020 23:04:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Thu, 23 Apr 2020 23:04:49 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Thu, 23 Apr 2020 23:04:50 GMT
RUN set -eux; 	addgroup -g 82 -S www-data; 	adduser -u 82 -D -S -G www-data www-data
# Thu, 23 Apr 2020 23:04:50 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 23 Apr 2020 23:04:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 23 Apr 2020 23:07:22 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Thu, 23 Apr 2020 23:07:22 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 23:07:22 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 23 Apr 2020 23:07:22 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 23 Apr 2020 23:07:23 GMT
ENV GPG_KEYS=42670A7FE4D0441C8E4632349E4FDC074A4EF02D 5A52880781F755608BF815FC910DEB46F53EA312
# Thu, 23 Apr 2020 23:07:23 GMT
ENV PHP_VERSION=7.4.5
# Wed, 06 May 2020 22:46:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.5.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.5.tar.xz.asc
# Wed, 06 May 2020 22:46:28 GMT
ENV PHP_SHA256=d059fd7f55bdc4d2eada15a00a2976697010d3631ef6f83149cc5289e1f23c2c PHP_MD5=
# Wed, 06 May 2020 22:46:31 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Wed, 06 May 2020 22:46:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 06 May 2020 22:49:59 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Wed, 06 May 2020 22:50:03 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Wed, 06 May 2020 22:50:04 GMT
RUN docker-php-ext-enable sodium
# Wed, 06 May 2020 22:50:04 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 06 May 2020 22:50:05 GMT
WORKDIR /var/www/html
# Wed, 06 May 2020 22:50:06 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 06 May 2020 22:50:07 GMT
STOPSIGNAL SIGQUIT
# Wed, 06 May 2020 22:50:07 GMT
EXPOSE 9000
# Wed, 06 May 2020 22:50:08 GMT
CMD ["php-fpm"]
# Thu, 07 May 2020 03:02:56 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" opcache pdo_mysql mysqli
# Thu, 07 May 2020 03:02:57 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=60';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 07 May 2020 03:02:59 GMT
RUN apk add --no-cache bash
# Thu, 07 May 2020 03:03:00 GMT
ENV YOURLS_VERSION=1.7.9
# Thu, 07 May 2020 03:03:00 GMT
ENV YOURLS_SHA256=0d9106b2936289d2fe5d4d6c017a77f96c79f4b2cacf1b59a0837d0032ca96d7
# Thu, 07 May 2020 03:03:02 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 07 May 2020 03:03:03 GMT
COPY file:faa5e93643253a8f7b19a0098e9286cc1914eaa7154c418de43e161d69f2f157 in /usr/local/bin/ 
# Thu, 07 May 2020 03:03:03 GMT
COPY file:3694b933d9d31fc65ed3f78f65289b778a21bf67c518d2cb89c6294ef1d41b60 in /usr/src/yourls/user/ 
# Thu, 07 May 2020 03:03:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 May 2020 03:03:04 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:7184c046fdf17da4c16ca482e5ede36e1f2d41ac8cea9c036e488fd149d6e8e7`  
		Last Modified: Thu, 23 Apr 2020 17:51:38 GMT  
		Size: 2.6 MB (2582859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce9311aad926b3cb7924b7f1bbfda3972f2b64dca32e8decf8257ba49353a285`  
		Last Modified: Thu, 23 Apr 2020 23:53:51 GMT  
		Size: 1.4 MB (1397092 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c77861eec55084cb75eb6742ba23b02781c9311acbf6d27f56e08d1323565fe2`  
		Last Modified: Thu, 23 Apr 2020 23:53:50 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:628ed6ecb36cf955a18714674b47d5822ae7eb0372cd31f3c2edd4a3c38fce32`  
		Last Modified: Thu, 23 Apr 2020 23:53:48 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3faf160454dce513a4c972dc1de2a373c12995ca162c532472188c86a9f6325a`  
		Last Modified: Thu, 07 May 2020 01:05:15 GMT  
		Size: 10.3 MB (10290401 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31542bbaeb5bd84d148ffeef31f0cc90cd2a729b1122c4cf1153fb906489c2bc`  
		Last Modified: Thu, 07 May 2020 01:05:13 GMT  
		Size: 496.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acf00e4685edc224333a9710859ff1bbb95f8af4b61593e16ec6a30c68dfac46`  
		Last Modified: Thu, 07 May 2020 01:05:16 GMT  
		Size: 13.5 MB (13497485 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eeee72401783f87715e0ff2de9cb4b457236897b908214dfdde2ffb4e36a84aa`  
		Last Modified: Thu, 07 May 2020 01:05:18 GMT  
		Size: 2.2 KB (2214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19e3a8e8bfb8e8edaa4800154318ea949f9352f5a43cad3cb62cc32d8b612f2a`  
		Last Modified: Thu, 07 May 2020 01:05:12 GMT  
		Size: 17.1 KB (17084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f13624d23a13e3f9ebe75c072c8aa0409862c5b9f213ad6f14034393883db54d`  
		Last Modified: Thu, 07 May 2020 01:05:13 GMT  
		Size: 8.4 KB (8439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dbff9ef236219f54e24681350c76d0008480092e9842c1653e0aa545f26cb65`  
		Last Modified: Thu, 07 May 2020 03:05:11 GMT  
		Size: 344.2 KB (344223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b10379f9dae858774405ddae226f3bf4b1e7db3c587f5c383c10226ac968efa`  
		Last Modified: Thu, 07 May 2020 03:05:09 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b449a3f5a47cf96ad840b75ab12a6866f1b58702b1a0428ff1664f0e257d571b`  
		Last Modified: Thu, 07 May 2020 03:05:10 GMT  
		Size: 576.8 KB (576754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e270c8235e409b0026237fddc922032310803dd069e709f7ef5ff2facb51fd0`  
		Last Modified: Thu, 07 May 2020 03:05:10 GMT  
		Size: 2.5 MB (2486824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f9ffb3b3c7f3a0787cfe931f9a147262d964b6acd9fa901ae1dc9214a963e8c`  
		Last Modified: Thu, 07 May 2020 03:05:15 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:efb457fc0aabcb0e2e3abaceb2c8d574c5d8d27fed174cc89ecc224badc05e8e`  
		Last Modified: Thu, 07 May 2020 03:05:15 GMT  
		Size: 1.9 KB (1860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
