## `joomla:php7.4-fpm-alpine`

```console
$ docker pull joomla@sha256:0e98c994221d6a8afbe3265e1fbb4654393ce0f02e4c02825c90f6a72b22dfe3
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

### `joomla:php7.4-fpm-alpine` - linux; amd64

```console
$ docker pull joomla@sha256:f94628f06f7f134a477748fc7fa3431f6c1f6ffb6ca2b4cec2f5e93c360600f3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.5 MB (45504792 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b960a1ec4e760c1e7c890e013be9465ab8f6ee5080966320f00294494ed49002`
-	Entrypoint: `["\/entrypoint.sh"]`
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
# Fri, 15 May 2020 01:35:56 GMT
ENV PHP_VERSION=7.4.6
# Fri, 15 May 2020 01:35:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.6.tar.xz.asc
# Fri, 15 May 2020 01:35:57 GMT
ENV PHP_SHA256=d740322f84f63019622b9f369d64ea5ab676547d2bdcf12be77a5a4cffd06832 PHP_MD5=
# Fri, 15 May 2020 01:36:00 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 May 2020 01:36:00 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 01:44:57 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 01:44:58 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 15 May 2020 01:45:00 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 01:45:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 01:45:00 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 01:45:01 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 15 May 2020 01:45:01 GMT
STOPSIGNAL SIGQUIT
# Fri, 15 May 2020 01:45:02 GMT
EXPOSE 9000
# Fri, 15 May 2020 01:45:02 GMT
CMD ["php-fpm"]
# Fri, 15 May 2020 15:55:27 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Fri, 15 May 2020 15:55:27 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 15 May 2020 15:55:28 GMT
RUN apk add --no-cache 	bash
# Fri, 15 May 2020 15:56:54 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Fri, 15 May 2020 15:56:55 GMT
VOLUME [/var/www/html]
# Fri, 15 May 2020 15:56:55 GMT
ENV JOOMLA_VERSION=3.9.18
# Fri, 15 May 2020 15:56:55 GMT
ENV JOOMLA_SHA512=1bf4590a761cc24f59fc0d5b07ffbb8f9e50073b3536edc261b8785ff168aca2066d133a81c4ac33bcfe7b843559320ef4d1f97c5eb16096ca4b550a18b7f44d
# Fri, 15 May 2020 15:57:00 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 15 May 2020 15:57:00 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Fri, 15 May 2020 15:57:01 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 15 May 2020 15:57:01 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 May 2020 15:57:01 GMT
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
	-	`sha256:30c8e28ed739837b28c0efb4f9502fce5796dc54780d4dc3b2a1fbf6bfc6971c`  
		Last Modified: Fri, 15 May 2020 06:19:22 GMT  
		Size: 10.3 MB (10303922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74857c12e32695fd9e9e0da2f677169b5bd8e701e27a13118a6ac52412921313`  
		Last Modified: Fri, 15 May 2020 06:19:20 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec3e05bb2638ed5b6b4c4255c30a0ee2c3e21a7690a579ab276bfa55a941c5ca`  
		Last Modified: Fri, 15 May 2020 06:19:23 GMT  
		Size: 14.2 MB (14210570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2595c48bd4da7ac1a4e6b0beeb97054e1726e15f84da8e6d4e59e967af6de801`  
		Last Modified: Fri, 15 May 2020 06:19:20 GMT  
		Size: 2.2 KB (2216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61816dddc67c0a71bdc3defe2029967f2f0a78972bf397f7f9b67e6bb446c8a`  
		Last Modified: Fri, 15 May 2020 06:19:20 GMT  
		Size: 17.1 KB (17101 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:804bb92077e51e107186dc31274ac43bbbb4254fc467e2fd5db94f574ff33e18`  
		Last Modified: Fri, 15 May 2020 06:19:20 GMT  
		Size: 8.4 KB (8444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d11d5530d223c64ac34ac4ac7bccbf89497ff998e2e14689a319ad5ec008b11`  
		Last Modified: Fri, 15 May 2020 15:59:56 GMT  
		Size: 557.6 KB (557575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:128561bd47013fac37a9be74ed173a9f813b53493e6ebabb001785ccc817e1c1`  
		Last Modified: Fri, 15 May 2020 15:59:57 GMT  
		Size: 6.6 MB (6579105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38a7c67c8f6b80bc2e6c196ba4ccab31d1be2516c50019207e18b404b9948e25`  
		Last Modified: Fri, 15 May 2020 16:00:05 GMT  
		Size: 9.7 MB (9653511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4d7c11e44f6a553ea5197872fde4737bbec3fa45f079c205ee0a742faf5540b`  
		Last Modified: Fri, 15 May 2020 15:59:56 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eff007dcab516d2e0dfddc21448df9c09d0fd53f85f57c5bfab333c7d2987497`  
		Last Modified: Fri, 15 May 2020 15:59:56 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4-fpm-alpine` - linux; arm variant v6

```console
$ docker pull joomla@sha256:6c2c75a9d00b82a0c5141867243e3a10c2ac8410255031ba9eb48a461b500f58
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43874694 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b80c8f670f13c27b1998175c3ec8d5d36b220c1da31624617faf893e4b88b0fa`
-	Entrypoint: `["\/entrypoint.sh"]`
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
# Thu, 14 May 2020 20:05:06 GMT
ENV PHP_VERSION=7.4.6
# Thu, 14 May 2020 20:05:09 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.6.tar.xz.asc
# Thu, 14 May 2020 20:05:11 GMT
ENV PHP_SHA256=d740322f84f63019622b9f369d64ea5ab676547d2bdcf12be77a5a4cffd06832 PHP_MD5=
# Thu, 14 May 2020 20:05:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 14 May 2020 20:05:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 May 2020 20:10:18 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 14 May 2020 20:10:20 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 14 May 2020 20:10:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 May 2020 20:10:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 May 2020 20:10:27 GMT
WORKDIR /var/www/html
# Thu, 14 May 2020 20:10:32 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 14 May 2020 20:10:34 GMT
STOPSIGNAL SIGQUIT
# Thu, 14 May 2020 20:10:35 GMT
EXPOSE 9000
# Thu, 14 May 2020 20:10:37 GMT
CMD ["php-fpm"]
# Thu, 14 May 2020 22:34:29 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Thu, 14 May 2020 22:34:31 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 14 May 2020 22:34:37 GMT
RUN apk add --no-cache 	bash
# Thu, 14 May 2020 22:37:45 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 14 May 2020 22:37:46 GMT
VOLUME [/var/www/html]
# Thu, 14 May 2020 22:37:48 GMT
ENV JOOMLA_VERSION=3.9.18
# Thu, 14 May 2020 22:37:49 GMT
ENV JOOMLA_SHA512=1bf4590a761cc24f59fc0d5b07ffbb8f9e50073b3536edc261b8785ff168aca2066d133a81c4ac33bcfe7b843559320ef4d1f97c5eb16096ca4b550a18b7f44d
# Thu, 14 May 2020 22:38:00 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Thu, 14 May 2020 22:38:05 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Thu, 14 May 2020 22:38:06 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Thu, 14 May 2020 22:38:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 14 May 2020 22:38:07 GMT
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
	-	`sha256:232f384bfce8e2f9683c212ce30ba799449b43e9c18073b39f6cc8123a730e2f`  
		Last Modified: Thu, 14 May 2020 21:18:25 GMT  
		Size: 10.3 MB (10303942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b872556acd3b5bc4f9b5d872b2d04ddc331b6bd1bd7ee73564302ebe8d7e66e`  
		Last Modified: Thu, 14 May 2020 21:18:22 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7c7723a0f63f2f93f4b7d9bc5aeea46ee09a7458dd7b3bc82aaa758fddf870`  
		Last Modified: Thu, 14 May 2020 21:18:27 GMT  
		Size: 13.2 MB (13238288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:509b89d228873df176587c26f53e8eec942c0ba89eef97d6a6509ae518681717`  
		Last Modified: Thu, 14 May 2020 21:18:22 GMT  
		Size: 2.2 KB (2214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a67d283a16825836e642fe832411bb26997b35d80eb1e574f39678a3a561d75`  
		Last Modified: Thu, 14 May 2020 21:18:22 GMT  
		Size: 17.1 KB (17084 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0292c329c7e8eb846bfb8f456c508ce7e69bf2846720fc2e34decf8d5c3b769d`  
		Last Modified: Thu, 14 May 2020 21:18:23 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffb869b6b20c7c81bbd7d69d9ace631a5027a5e9e91023fb2138a58702bab432`  
		Last Modified: Thu, 14 May 2020 22:39:08 GMT  
		Size: 536.9 KB (536884 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0982ea42683480b2e4ea55162c37f5894bdf1b23b113821cf55e022dd86d9ab0`  
		Last Modified: Thu, 14 May 2020 22:39:10 GMT  
		Size: 6.2 MB (6169331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f78bd0a48234617a1016b2a119eb5ffba9d188fdbd35e0dd4101b4de9e2414de`  
		Last Modified: Thu, 14 May 2020 22:39:12 GMT  
		Size: 9.7 MB (9653459 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf0ad97756c33bdc9f0cf2569ca4651738ea999ea4232798fbe68c4548601561`  
		Last Modified: Thu, 14 May 2020 22:39:08 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a02d01580abeeb973b5bce7080ed18a5dbb8c8d2b3b64314dff92cc158a1418`  
		Last Modified: Thu, 14 May 2020 22:39:08 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4-fpm-alpine` - linux; arm variant v7

```console
$ docker pull joomla@sha256:6e69131139b138c78838015ecbf40934605ac4a242413dff5682076ff1064adc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **42.5 MB (42457620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1e152579ca1d39754150387e853c7ccbc79b7df16784b5c1987adcb542aabb58`
-	Entrypoint: `["\/entrypoint.sh"]`
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
# Thu, 14 May 2020 22:28:56 GMT
ENV PHP_VERSION=7.4.6
# Thu, 14 May 2020 22:28:57 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.6.tar.xz.asc
# Thu, 14 May 2020 22:28:58 GMT
ENV PHP_SHA256=d740322f84f63019622b9f369d64ea5ab676547d2bdcf12be77a5a4cffd06832 PHP_MD5=
# Thu, 14 May 2020 22:29:03 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 14 May 2020 22:29:04 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 May 2020 22:31:41 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 14 May 2020 22:31:44 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 14 May 2020 22:31:48 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 May 2020 22:31:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 May 2020 22:31:49 GMT
WORKDIR /var/www/html
# Thu, 14 May 2020 22:31:51 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 14 May 2020 22:31:52 GMT
STOPSIGNAL SIGQUIT
# Thu, 14 May 2020 22:31:53 GMT
EXPOSE 9000
# Thu, 14 May 2020 22:31:53 GMT
CMD ["php-fpm"]
# Fri, 15 May 2020 07:14:41 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Fri, 15 May 2020 07:14:42 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 15 May 2020 07:14:45 GMT
RUN apk add --no-cache 	bash
# Fri, 15 May 2020 07:17:08 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Fri, 15 May 2020 07:17:09 GMT
VOLUME [/var/www/html]
# Fri, 15 May 2020 07:17:10 GMT
ENV JOOMLA_VERSION=3.9.18
# Fri, 15 May 2020 07:17:11 GMT
ENV JOOMLA_SHA512=1bf4590a761cc24f59fc0d5b07ffbb8f9e50073b3536edc261b8785ff168aca2066d133a81c4ac33bcfe7b843559320ef4d1f97c5eb16096ca4b550a18b7f44d
# Fri, 15 May 2020 07:17:25 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 15 May 2020 07:17:28 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Fri, 15 May 2020 07:17:30 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 15 May 2020 07:17:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 May 2020 07:17:31 GMT
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
	-	`sha256:dbd57012e64e15a4094767425b079ed5de19afffc5c1f22ec385b87b4e746322`  
		Last Modified: Fri, 15 May 2020 00:41:18 GMT  
		Size: 10.3 MB (10303934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b9e1673ae83216863693126764ea238af4c557e7b66253f0da80f84fbe7b701`  
		Last Modified: Fri, 15 May 2020 00:41:15 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f10d9722b2008341ad39711fc7a6a8805116ad549290f100f803bfd885701de`  
		Last Modified: Fri, 15 May 2020 00:41:19 GMT  
		Size: 12.4 MB (12383989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb0c0245788fba8ea55ec0fc3542d31de91dd6e90aee33a1c6f4857cbd088f1`  
		Last Modified: Fri, 15 May 2020 00:41:15 GMT  
		Size: 2.2 KB (2213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3adf473d167247a3ffb866b02b0c0afa2360f07afc942bd72f6fb775de8f46e7`  
		Last Modified: Fri, 15 May 2020 00:41:15 GMT  
		Size: 17.1 KB (17074 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905c77c51fa1147a5ee48c0ceb19d65890d242c36367baab3b10985b17b5c109`  
		Last Modified: Fri, 15 May 2020 00:41:15 GMT  
		Size: 8.4 KB (8439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3730f106629871b44b481fd5bc8e83d6448d3b147f5b0616cbefc7784a77408`  
		Last Modified: Fri, 15 May 2020 07:21:27 GMT  
		Size: 489.2 KB (489199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:622b31d20aca59bcfafaab9249f9f069fef28c11867c00382625e6c6a21361d8`  
		Last Modified: Fri, 15 May 2020 07:21:29 GMT  
		Size: 5.9 MB (5945542 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f539c658882deaaf75c236c96f4edf1866bc54eaced9f064e5483b8f155f967`  
		Last Modified: Fri, 15 May 2020 07:21:33 GMT  
		Size: 9.7 MB (9653462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b47a4da89226b60f86fe55a4ae1217c0c72a53fdf195b344e4b07a7861c208f4`  
		Last Modified: Fri, 15 May 2020 07:21:26 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50797349df52d223b3693e37fb61860598389ed76d39b0df5579d0b5716da612`  
		Last Modified: Fri, 15 May 2020 07:21:27 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull joomla@sha256:1d6ec6011ed785230ad70663c539544cbbd0a53768cb30b6a623ab90ad4bb900
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.2 MB (45200238 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8fac730b68d8a7023e499802b58ee9e5365c039758d9d75dd4e6b5e4e7d8fa02`
-	Entrypoint: `["\/entrypoint.sh"]`
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
# Fri, 15 May 2020 00:03:15 GMT
ENV PHP_VERSION=7.4.6
# Fri, 15 May 2020 00:03:15 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.6.tar.xz.asc
# Fri, 15 May 2020 00:03:16 GMT
ENV PHP_SHA256=d740322f84f63019622b9f369d64ea5ab676547d2bdcf12be77a5a4cffd06832 PHP_MD5=
# Fri, 15 May 2020 00:03:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 May 2020 00:03:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 00:07:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 00:07:03 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 15 May 2020 00:07:06 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 00:07:07 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 00:07:08 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 00:07:10 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 15 May 2020 00:07:11 GMT
STOPSIGNAL SIGQUIT
# Fri, 15 May 2020 00:07:11 GMT
EXPOSE 9000
# Fri, 15 May 2020 00:07:12 GMT
CMD ["php-fpm"]
# Fri, 15 May 2020 17:26:13 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Fri, 15 May 2020 17:26:14 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 15 May 2020 17:26:18 GMT
RUN apk add --no-cache 	bash
# Fri, 15 May 2020 17:28:49 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Fri, 15 May 2020 17:28:50 GMT
VOLUME [/var/www/html]
# Fri, 15 May 2020 17:28:51 GMT
ENV JOOMLA_VERSION=3.9.18
# Fri, 15 May 2020 17:28:52 GMT
ENV JOOMLA_SHA512=1bf4590a761cc24f59fc0d5b07ffbb8f9e50073b3536edc261b8785ff168aca2066d133a81c4ac33bcfe7b843559320ef4d1f97c5eb16096ca4b550a18b7f44d
# Fri, 15 May 2020 17:29:02 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 15 May 2020 17:29:04 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Fri, 15 May 2020 17:29:05 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 15 May 2020 17:29:06 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 May 2020 17:29:06 GMT
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
	-	`sha256:23c367f3733bd91296d39b3bbfc83ee5332b7a4844ed08beb4f888a6d3624d44`  
		Last Modified: Fri, 15 May 2020 02:26:37 GMT  
		Size: 10.3 MB (10303940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d668978336e77957180c4918597383b7e59a8afef4269972386fbfc74c13de2`  
		Last Modified: Fri, 15 May 2020 02:26:34 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110de7167eb33a901b39c5cda56f4698c3d06b5aeb987bb57f40e9aa7bb266b`  
		Last Modified: Fri, 15 May 2020 02:26:40 GMT  
		Size: 14.0 MB (14023846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94cb3c3c01ff20f321ca42ff45fa2f2d1bf4a870d3d33e3290a82c1873330f55`  
		Last Modified: Fri, 15 May 2020 02:26:34 GMT  
		Size: 2.2 KB (2211 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ebe61c13d98ebe202ebd0531dfd570db5f0c1e53806e7845a92ab4d4ebaecd6`  
		Last Modified: Fri, 15 May 2020 02:26:34 GMT  
		Size: 17.1 KB (17095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dcd52d6a20868785cc183711337abb03887c4e63c9bf07f95d6ed9248e5dcc1`  
		Last Modified: Fri, 15 May 2020 02:26:33 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d3443d2e4745dc0d0c5a0dd37bb1c3351cb83a07d63af0203727e996836ab1e`  
		Last Modified: Fri, 15 May 2020 17:33:00 GMT  
		Size: 569.0 KB (568999 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7887254cdfdcdc6daeba89d16f550b6127832d273616fb1169196090d4ef7747`  
		Last Modified: Fri, 15 May 2020 17:33:01 GMT  
		Size: 6.5 MB (6534286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c31d939a461e44c1157a730ff3e8f4204c918adc44d437dcc72aee8afad2c1b4`  
		Last Modified: Fri, 15 May 2020 17:33:03 GMT  
		Size: 9.7 MB (9653468 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69fae45c5341b6eacebbb69c9959c3fece0a8e795e88f8dec3b7d233f9ec4e0c`  
		Last Modified: Fri, 15 May 2020 17:33:00 GMT  
		Size: 1.2 KB (1173 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:244983b3091b6a9e089a74bfdb899405a5c7e570fbcce7d7015017e1ca76ac5c`  
		Last Modified: Fri, 15 May 2020 17:33:00 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4-fpm-alpine` - linux; 386

```console
$ docker pull joomla@sha256:a3b418125fb2f31c8e5e562d2070fd28c616e2f9b1831276bad6816e76c944f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.2 MB (46166092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a5df8c660032c8335e46fc8294f1f394a7cb694ee1646b67e0d5cdcad1c574e3`
-	Entrypoint: `["\/entrypoint.sh"]`
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
# Fri, 15 May 2020 02:02:38 GMT
ENV PHP_VERSION=7.4.6
# Fri, 15 May 2020 02:02:38 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.6.tar.xz.asc
# Fri, 15 May 2020 02:02:38 GMT
ENV PHP_SHA256=d740322f84f63019622b9f369d64ea5ab676547d2bdcf12be77a5a4cffd06832 PHP_MD5=
# Fri, 15 May 2020 02:02:40 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 15 May 2020 02:02:41 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Fri, 15 May 2020 02:12:11 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Fri, 15 May 2020 02:12:12 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Fri, 15 May 2020 02:12:13 GMT
RUN docker-php-ext-enable sodium
# Fri, 15 May 2020 02:12:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Fri, 15 May 2020 02:12:13 GMT
WORKDIR /var/www/html
# Fri, 15 May 2020 02:12:14 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Fri, 15 May 2020 02:12:14 GMT
STOPSIGNAL SIGQUIT
# Fri, 15 May 2020 02:12:14 GMT
EXPOSE 9000
# Fri, 15 May 2020 02:12:15 GMT
CMD ["php-fpm"]
# Fri, 15 May 2020 15:25:37 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Fri, 15 May 2020 15:25:38 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 15 May 2020 15:25:39 GMT
RUN apk add --no-cache 	bash
# Fri, 15 May 2020 15:27:10 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Fri, 15 May 2020 15:27:10 GMT
VOLUME [/var/www/html]
# Fri, 15 May 2020 15:27:11 GMT
ENV JOOMLA_VERSION=3.9.18
# Fri, 15 May 2020 15:27:11 GMT
ENV JOOMLA_SHA512=1bf4590a761cc24f59fc0d5b07ffbb8f9e50073b3536edc261b8785ff168aca2066d133a81c4ac33bcfe7b843559320ef4d1f97c5eb16096ca4b550a18b7f44d
# Fri, 15 May 2020 15:27:17 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 15 May 2020 15:27:17 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Fri, 15 May 2020 15:27:17 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 15 May 2020 15:27:18 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 May 2020 15:27:18 GMT
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
	-	`sha256:5119117f959a143a1ecc22ea788ee8ffa3f0393655f6677691e4a1854544a923`  
		Last Modified: Fri, 15 May 2020 06:55:30 GMT  
		Size: 10.3 MB (10303940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a54fd0ef1525868874f1e523f97944844c066d7e7e1f91631e13d7070a50227c`  
		Last Modified: Fri, 15 May 2020 06:55:27 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead567aa5b609fd7609ebe758dbae3dee371f3fd8cda345ac57dca2fb678f0f4`  
		Last Modified: Fri, 15 May 2020 06:55:33 GMT  
		Size: 14.6 MB (14619324 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e70f6c76ee2f99776ea98369fc85bd0e499650e4764a6c81c29f38015c6370`  
		Last Modified: Fri, 15 May 2020 06:55:28 GMT  
		Size: 2.2 KB (2215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cc4e9f607eeced852faebbfafd1b6af0796b77b02514e09fd80f3e1ef08752d`  
		Last Modified: Fri, 15 May 2020 06:55:27 GMT  
		Size: 17.1 KB (17100 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:899fd16af8eb0d93ecf5076951d362cf2664c8e1e9da1ac2fab92b12bac97f91`  
		Last Modified: Fri, 15 May 2020 06:55:28 GMT  
		Size: 8.4 KB (8446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ec3bd37b5567dbfb0fb37720598d2cfbcae27b6b620d0c8d7984b17419c9e9`  
		Last Modified: Fri, 15 May 2020 15:30:34 GMT  
		Size: 598.7 KB (598738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b51b13fbbca0a14aa81156116e5708757f7a964896de227feb000d421d1ccca`  
		Last Modified: Fri, 15 May 2020 15:30:36 GMT  
		Size: 6.7 MB (6697577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c03d4f801e2f153fe9da741e4a0e75900ffbf6f1590b2def7e19ffc9d1385cc7`  
		Last Modified: Fri, 15 May 2020 15:30:40 GMT  
		Size: 9.7 MB (9653498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0579eea1ad4f467a30b53a5e1adabb6c0c2ad6b408ec56b35e278c075f3c582e`  
		Last Modified: Fri, 15 May 2020 15:30:33 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d7f70559071b8d8459fc8325d7754ea691797e31b0163b254cf7d9063d103ad`  
		Last Modified: Fri, 15 May 2020 15:30:33 GMT  
		Size: 614.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4-fpm-alpine` - linux; ppc64le

```console
$ docker pull joomla@sha256:9e40279a162cacb0302fd016c496aedcc2b4595ead9d13344b638717333c72a2
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.8 MB (46822202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e6cc5954215fd9975657cc4de5163fb55b0dbe2bd52e0477fb350ccc51835cd`
-	Entrypoint: `["\/entrypoint.sh"]`
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
# Thu, 07 May 2020 03:07:31 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Thu, 07 May 2020 03:07:36 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Thu, 07 May 2020 03:07:46 GMT
RUN apk add --no-cache 	bash
# Thu, 07 May 2020 03:09:48 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Thu, 07 May 2020 03:09:51 GMT
VOLUME [/var/www/html]
# Mon, 11 May 2020 15:32:07 GMT
ENV JOOMLA_VERSION=3.9.18
# Mon, 11 May 2020 15:32:11 GMT
ENV JOOMLA_SHA512=1bf4590a761cc24f59fc0d5b07ffbb8f9e50073b3536edc261b8785ff168aca2066d133a81c4ac33bcfe7b843559320ef4d1f97c5eb16096ca4b550a18b7f44d
# Mon, 11 May 2020 15:32:45 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Mon, 11 May 2020 15:32:50 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Mon, 11 May 2020 15:32:51 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Mon, 11 May 2020 15:32:53 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 May 2020 15:32:55 GMT
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
	-	`sha256:8ab8c2621128ff2f012b60b7ecd793e1db71922e11733b10d3c2d4410609ae14`  
		Last Modified: Thu, 07 May 2020 03:16:41 GMT  
		Size: 622.3 KB (622282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40f0816929bfa3471c4da4c173f71e2fc9db38294fb7e981579507eee715113a`  
		Last Modified: Thu, 07 May 2020 03:16:42 GMT  
		Size: 6.8 MB (6833599 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8bc23d70a3d07fd1eb45df164209c7955d2c49ac798b0a2b95f67a9c285241b`  
		Last Modified: Mon, 11 May 2020 15:40:50 GMT  
		Size: 9.7 MB (9653469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:709bd16c28d7b6fb342bdcae61c54971130d12d7ba487a1d0816edb44c72f7b3`  
		Last Modified: Mon, 11 May 2020 15:40:35 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1f512e89fa9099e93d3c67645262631fbc6bdbed8a93da9b375927e031bba7c`  
		Last Modified: Mon, 11 May 2020 15:40:35 GMT  
		Size: 616.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `joomla:php7.4-fpm-alpine` - linux; s390x

```console
$ docker pull joomla@sha256:7e7484fbc7bcb60787a4ddbe985cafa9b0f270eecff622b2dee56c9bf0555dcc
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.6 MB (44643598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6a51a94bcc8fa74dfb32bba70d478936bfcea8d71a677202f538b2adad4df2c6`
-	Entrypoint: `["\/entrypoint.sh"]`
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
# Thu, 14 May 2020 21:15:21 GMT
ENV PHP_VERSION=7.4.6
# Thu, 14 May 2020 21:15:22 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.4.6.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.4.6.tar.xz.asc
# Thu, 14 May 2020 21:15:22 GMT
ENV PHP_SHA256=d740322f84f63019622b9f369d64ea5ab676547d2bdcf12be77a5a4cffd06832 PHP_MD5=
# Thu, 14 May 2020 21:15:25 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 14 May 2020 21:15:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 14 May 2020 21:17:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 14 May 2020 21:17:46 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 14 May 2020 21:17:47 GMT
RUN docker-php-ext-enable sodium
# Thu, 14 May 2020 21:17:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 14 May 2020 21:17:47 GMT
WORKDIR /var/www/html
# Thu, 14 May 2020 21:17:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 14 May 2020 21:17:48 GMT
STOPSIGNAL SIGQUIT
# Thu, 14 May 2020 21:17:49 GMT
EXPOSE 9000
# Thu, 14 May 2020 21:17:49 GMT
CMD ["php-fpm"]
# Fri, 15 May 2020 02:01:23 GMT
LABEL maintainer=Michael Babker <michael.babker@joomla.org> (@mbabker)
# Fri, 15 May 2020 02:01:24 GMT
ENV JOOMLA_INSTALLATION_DISABLE_LOCALHOST_CHECK=1
# Fri, 15 May 2020 02:01:25 GMT
RUN apk add --no-cache 	bash
# Fri, 15 May 2020 02:02:55 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		autoconf 		bzip2-dev 		libjpeg-turbo-dev 		libmemcached-dev 		libpng-dev 		libzip-dev 		openldap-dev 		pcre-dev 		postgresql-dev 	; 		docker-php-ext-configure gd --with-jpeg; 	docker-php-ext-configure ldap; 	docker-php-ext-install -j "$(nproc)" 		bz2 		gd 		ldap 		mysqli 		pdo_mysql 		pdo_pgsql 		pgsql 		zip 	; 		pecl install APCu-5.1.18; 	pecl install memcached-3.1.5; 	pecl install redis-4.3.0; 		docker-php-ext-enable 		apcu 		memcached 		redis 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 		| tr ',' '\n' 		| sort -u 		| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 		)"; 	apk add --virtual .joomla-phpext-rundeps $runDeps; 	apk del .build-deps
# Fri, 15 May 2020 02:02:55 GMT
VOLUME [/var/www/html]
# Fri, 15 May 2020 02:02:55 GMT
ENV JOOMLA_VERSION=3.9.18
# Fri, 15 May 2020 02:02:56 GMT
ENV JOOMLA_SHA512=1bf4590a761cc24f59fc0d5b07ffbb8f9e50073b3536edc261b8785ff168aca2066d133a81c4ac33bcfe7b843559320ef4d1f97c5eb16096ca4b550a18b7f44d
# Fri, 15 May 2020 02:03:01 GMT
RUN set -ex; 	curl -o joomla.tar.bz2 -SL https://github.com/joomla/joomla-cms/releases/download/${JOOMLA_VERSION}/Joomla_${JOOMLA_VERSION}-Stable-Full_Package.tar.bz2; 	echo "$JOOMLA_SHA512 *joomla.tar.bz2" | sha512sum -c -; 	mkdir /usr/src/joomla; 	tar -xf joomla.tar.bz2 -C /usr/src/joomla; 	rm joomla.tar.bz2; 	chown -R www-data:www-data /usr/src/joomla
# Fri, 15 May 2020 02:03:02 GMT
COPY file:fcc18c5b9c2d514cfb965bab84e10b4f924a39a5f202055df75d7990da099d8f in /entrypoint.sh 
# Fri, 15 May 2020 02:03:03 GMT
COPY file:5a85d779aaae74cfa3ab6228df0f24236d4d5ad9097e2a1b277e3daea0d6d3dc in /makedb.php 
# Fri, 15 May 2020 02:03:03 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 15 May 2020 02:03:03 GMT
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
	-	`sha256:e562c7a857c24c8a93256cafb59305bccef794c4af2f790df79e6f9d7c22b74f`  
		Last Modified: Thu, 14 May 2020 22:54:11 GMT  
		Size: 10.3 MB (10303951 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acc443d8c2085e8afd6b3191a0f0fa24cffdf0ca1404458fb321b3c50f2520cc`  
		Last Modified: Thu, 14 May 2020 22:54:08 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76721dfa500dd3d50d3e8fe2006931fee1da416f3b201e13c4d2c980c91d1c63`  
		Last Modified: Thu, 14 May 2020 22:54:11 GMT  
		Size: 13.5 MB (13518303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4ed7355bcdf22629a9b6c96ae6778de789c7e72258eaa6b156c54eef4ff3c`  
		Last Modified: Thu, 14 May 2020 22:54:14 GMT  
		Size: 2.2 KB (2219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01e186f43957fefe833cb1934c5c045c773f616b4e522e6ef37a275740e50ebd`  
		Last Modified: Thu, 14 May 2020 22:54:14 GMT  
		Size: 17.1 KB (17082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a841536686c347798f039ffecfe5a13bdf240f5910d5a1745ea9062bc2996344`  
		Last Modified: Thu, 14 May 2020 22:54:14 GMT  
		Size: 8.4 KB (8445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a18fc371b9fcead90a12ad87886b4ccb5df6e2ece6927dbbdb415c1f847f0416`  
		Last Modified: Fri, 15 May 2020 02:06:33 GMT  
		Size: 576.8 KB (576761 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:609a90d30e06758baeb2d926a82ce96113a2153ec3608051247a454f85351815`  
		Last Modified: Fri, 15 May 2020 02:06:39 GMT  
		Size: 6.6 MB (6579607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f4738eb47139e3b6b7be1be1d0f38fe0be92775b0f698c1ae89e280b3f147f5`  
		Last Modified: Fri, 15 May 2020 02:06:35 GMT  
		Size: 9.7 MB (9653467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e9f719bacae2b8fe3894dc1e0d300f8056e1b9e436595341c67a32dcc1a8db9`  
		Last Modified: Fri, 15 May 2020 02:06:38 GMT  
		Size: 1.2 KB (1172 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ac6f16129941a7947986f5ae1fe27745cb6b103ae4f210fafa4c19e94904f8`  
		Last Modified: Fri, 15 May 2020 02:06:38 GMT  
		Size: 615.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
