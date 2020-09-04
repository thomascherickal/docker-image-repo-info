## `postfixadmin:3-fpm-alpine`

```console
$ docker pull postfixadmin@sha256:8c8ae5308311e4d3d3a19ff3858f52ce4207a8d83046306e7798d95d8d7cc3f0
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

### `postfixadmin:3-fpm-alpine` - linux; amd64

```console
$ docker pull postfixadmin@sha256:61585d25790523eb2fb803c704cb420d6be19ee2655d784691b97938dcd2e6af
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.2 MB (36249925 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:62ada2679a22d016dd0ea087bee455bfc0e30d79397c181713e1df1002eca1ac`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
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
# Thu, 11 Jun 2020 20:58:14 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 03 Sep 2020 21:56:01 GMT
ENV PHP_VERSION=7.3.22
# Thu, 03 Sep 2020 21:56:01 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.22.tar.xz.asc
# Thu, 03 Sep 2020 21:56:01 GMT
ENV PHP_SHA256=0e66606d3bdab5c2ae3f778136bfe8788e574913a3d8138695e54d98562f1fb5 PHP_MD5=
# Thu, 03 Sep 2020 21:56:05 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 21:56:06 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 22:05:20 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 22:05:21 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 03 Sep 2020 22:05:22 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 22:05:22 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 22:05:22 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 22:05:23 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 03 Sep 2020 22:05:23 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Sep 2020 22:05:24 GMT
EXPOSE 9000
# Thu, 03 Sep 2020 22:05:24 GMT
CMD ["php-fpm"]
# Fri, 04 Sep 2020 00:57:14 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 04 Sep 2020 00:57:15 GMT
RUN apk add --no-cache 		bash
# Fri, 04 Sep 2020 00:57:44 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		sqlite-dev 		postgresql-dev 	; 	docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 04 Sep 2020 00:57:45 GMT
ARG POSTFIXADMIN_VERSION=3.2.4
# Fri, 04 Sep 2020 00:57:45 GMT
ARG POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Fri, 04 Sep 2020 00:57:45 GMT
ENV POSTFIXADMIN_VERSION=3.2.4
# Fri, 04 Sep 2020 00:57:45 GMT
ENV POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Fri, 04 Sep 2020 00:57:47 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 04 Sep 2020 00:57:47 GMT
COPY file:c6e11ee7dda40f44aa31f3bcb74669e99572ad86040276440b444d5699d333f5 in /usr/local/bin/ 
# Fri, 04 Sep 2020 00:57:48 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 04 Sep 2020 00:57:48 GMT
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
	-	`sha256:b6a939932fea284e2f3b3c6d41f2e75bad4b767530e97d62fb56028963eb9a74`  
		Last Modified: Thu, 03 Sep 2020 22:54:34 GMT  
		Size: 12.2 MB (12153539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6a332cd2d1b0248b9c3a09108ea598b74648e962d1a38828dbe1ae9dcb7ec84`  
		Last Modified: Thu, 03 Sep 2020 22:54:31 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8e3086a0f5acbd955298c0bf743532d9ca56347d5312c8f110e40bf980723d5`  
		Last Modified: Thu, 03 Sep 2020 22:54:36 GMT  
		Size: 14.9 MB (14860057 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1738fa2518d6bba0db824bb4ef995bb0eb630d928513e47207459b2d6eb0ae62`  
		Last Modified: Thu, 03 Sep 2020 22:54:31 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7099ad02f2acd772ea2fd93f5ab7334147a379e9fa9fca83d77aeb7ec3d5bd18`  
		Last Modified: Thu, 03 Sep 2020 22:54:32 GMT  
		Size: 16.8 KB (16791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2eb1c332f90407ddce6f5aea47429e6eb8d3d07fde4e8c508d325233f10299e`  
		Last Modified: Thu, 03 Sep 2020 22:54:31 GMT  
		Size: 8.4 KB (8413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea126504778b63fb22f9e81d1d572068ea35ac0271959a3269188cd068c85531`  
		Last Modified: Fri, 04 Sep 2020 00:58:29 GMT  
		Size: 557.2 KB (557228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ab8669a71d67e7f659187d39d58e27717aabfed139f626fe1251b43643599c0`  
		Last Modified: Fri, 04 Sep 2020 00:58:30 GMT  
		Size: 3.2 MB (3175295 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1d1aa9992bb01d97ca33e56012fab6bb445b8df795253d0bda788e9607ea494`  
		Last Modified: Fri, 04 Sep 2020 00:58:30 GMT  
		Size: 1.3 MB (1334689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d3c9f582fb9cb8605328e213ba19fdad921de3a20701b5a3effe7cca82c30db`  
		Last Modified: Fri, 04 Sep 2020 00:58:30 GMT  
		Size: 1.3 KB (1330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; arm variant v6

```console
$ docker pull postfixadmin@sha256:ee170b42b5257050c2a100550a915f7bf3dde0d11047234cfb96a0590db83489
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.7 MB (34657829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42d2843394ba97c6f4e0c1b8d7d8bc3c3b05a82a329b9a2e1bab98ec165f6e5a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
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
# Thu, 11 Jun 2020 18:49:43 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 03 Sep 2020 20:09:23 GMT
ENV PHP_VERSION=7.3.22
# Thu, 03 Sep 2020 20:09:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.22.tar.xz.asc
# Thu, 03 Sep 2020 20:09:42 GMT
ENV PHP_SHA256=0e66606d3bdab5c2ae3f778136bfe8788e574913a3d8138695e54d98562f1fb5 PHP_MD5=
# Thu, 03 Sep 2020 20:10:27 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 20:10:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 20:15:29 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 20:16:06 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 03 Sep 2020 20:16:57 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 20:17:12 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 20:17:24 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 20:18:04 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 03 Sep 2020 20:18:14 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Sep 2020 20:18:27 GMT
EXPOSE 9000
# Thu, 03 Sep 2020 20:18:44 GMT
CMD ["php-fpm"]
# Thu, 03 Sep 2020 22:45:23 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 03 Sep 2020 22:46:12 GMT
RUN apk add --no-cache 		bash
# Thu, 03 Sep 2020 22:47:59 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		sqlite-dev 		postgresql-dev 	; 	docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 03 Sep 2020 22:48:08 GMT
ARG POSTFIXADMIN_VERSION=3.2.4
# Thu, 03 Sep 2020 22:48:20 GMT
ARG POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Thu, 03 Sep 2020 22:48:35 GMT
ENV POSTFIXADMIN_VERSION=3.2.4
# Thu, 03 Sep 2020 22:48:49 GMT
ENV POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Thu, 03 Sep 2020 22:49:36 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 03 Sep 2020 22:49:48 GMT
COPY file:c6e11ee7dda40f44aa31f3bcb74669e99572ad86040276440b444d5699d333f5 in /usr/local/bin/ 
# Thu, 03 Sep 2020 22:49:59 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 03 Sep 2020 22:50:07 GMT
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
	-	`sha256:0c22881d81be30bd8f637b0f9f336248d62f0acc50f8cb9d99a26f6a8591a7c8`  
		Last Modified: Thu, 03 Sep 2020 21:01:16 GMT  
		Size: 12.2 MB (12153568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba1e7eb25be5f00a1ccd567a083f72cf4f19c75c787fe9da6df270ad0363ed3`  
		Last Modified: Thu, 03 Sep 2020 21:01:11 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b1662d3428cf823e4acb9f9ad4022c7e8ebcdeb95510ecc07cb1fcb535fe83ea`  
		Last Modified: Thu, 03 Sep 2020 21:01:16 GMT  
		Size: 13.8 MB (13808567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77250da35e2253901207545cdc6b323c3e34b95b7ae4f2d16340987422cae3c`  
		Last Modified: Thu, 03 Sep 2020 21:01:12 GMT  
		Size: 2.3 KB (2273 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c999239009879dd9ef7f1c2fc7f84ceeb390ec480b81facd5ebd93d8efe00bd1`  
		Last Modified: Thu, 03 Sep 2020 21:01:11 GMT  
		Size: 16.8 KB (16789 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21aa2cb659e611a03615e2fc4c858e742dde55f4fe018228fd50a62d527f6e95`  
		Last Modified: Thu, 03 Sep 2020 21:01:11 GMT  
		Size: 8.4 KB (8416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:368ab2574e758e052d9add0225359550fa99dfbaa3f91a8bfe718a2b45d1da07`  
		Last Modified: Thu, 03 Sep 2020 22:50:33 GMT  
		Size: 538.2 KB (538214 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f6e0429dca64077c32992d56c8dd01955f36aff7d082cc494db8648783a25c7`  
		Last Modified: Thu, 03 Sep 2020 22:50:34 GMT  
		Size: 2.9 MB (2878352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05b67bfe4df657900013cb4568c8f3acbbfcf60e542e3e40bc7d46d56115a46a`  
		Last Modified: Thu, 03 Sep 2020 22:50:34 GMT  
		Size: 1.3 MB (1334731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff9d9a24be071ac177931a4047b74de610e7bd9c383beff0b69813c6f90abf41`  
		Last Modified: Thu, 03 Sep 2020 22:50:33 GMT  
		Size: 1.3 KB (1331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; arm variant v7

```console
$ docker pull postfixadmin@sha256:25ea1bcde663ad446a50545506e6f04afcaa30e56ac344e0796f9b41bfd4a963
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.5 MB (33461271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cebe17eab63f994ae1061ce83e02c8d88f79eedbb7a30b0720efc91f17174321`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
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
# Thu, 11 Jun 2020 19:38:55 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 06 Aug 2020 21:37:04 GMT
ENV PHP_VERSION=7.3.21
# Thu, 06 Aug 2020 21:37:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.21.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.21.tar.xz.asc
# Thu, 06 Aug 2020 21:37:52 GMT
ENV PHP_SHA256=4c8b065746ef776d84b7ae47908c21a79e3d4704b86b60d816716b8697c58ce9 PHP_MD5=
# Thu, 06 Aug 2020 21:39:38 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 06 Aug 2020 21:40:03 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 01 Sep 2020 09:39:07 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 01 Sep 2020 09:39:10 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Tue, 01 Sep 2020 09:39:12 GMT
RUN docker-php-ext-enable sodium
# Tue, 01 Sep 2020 09:39:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 01 Sep 2020 09:39:14 GMT
WORKDIR /var/www/html
# Tue, 01 Sep 2020 09:39:18 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Tue, 01 Sep 2020 09:39:18 GMT
STOPSIGNAL SIGQUIT
# Tue, 01 Sep 2020 09:39:19 GMT
EXPOSE 9000
# Tue, 01 Sep 2020 09:39:20 GMT
CMD ["php-fpm"]
# Wed, 02 Sep 2020 03:37:48 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Wed, 02 Sep 2020 03:38:12 GMT
RUN apk add --no-cache 		bash
# Wed, 02 Sep 2020 03:39:17 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		sqlite-dev 		postgresql-dev 	; 	docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Wed, 02 Sep 2020 03:39:22 GMT
ARG POSTFIXADMIN_VERSION=3.2.4
# Wed, 02 Sep 2020 03:39:27 GMT
ARG POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Wed, 02 Sep 2020 03:39:32 GMT
ENV POSTFIXADMIN_VERSION=3.2.4
# Wed, 02 Sep 2020 03:39:36 GMT
ENV POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Wed, 02 Sep 2020 03:39:53 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Wed, 02 Sep 2020 03:40:03 GMT
COPY file:c6e11ee7dda40f44aa31f3bcb74669e99572ad86040276440b444d5699d333f5 in /usr/local/bin/ 
# Wed, 02 Sep 2020 03:40:10 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Wed, 02 Sep 2020 03:40:16 GMT
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
	-	`sha256:cfb8a476e521ba10c675a48b30d17fd946fa1270bd5039e2c831a821dcf60a90`  
		Last Modified: Fri, 07 Aug 2020 01:10:29 GMT  
		Size: 12.1 MB (12142655 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56deaf475c2d470bfcd9f2799fde7de42c33b46f5d430cf0c673f5fd495107e2`  
		Last Modified: Fri, 07 Aug 2020 01:10:24 GMT  
		Size: 503.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3750083e44002f63a3d52d81e649f2258c9aed0dc969320d3ad8f1626a940084`  
		Last Modified: Tue, 01 Sep 2020 10:47:42 GMT  
		Size: 12.9 MB (12921926 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95c1122c86cf8b5f270603b2484faaf3bacb445d8d5e954863f105a830d3e156`  
		Last Modified: Tue, 01 Sep 2020 10:47:37 GMT  
		Size: 2.3 KB (2272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbe9174554722deab7ae7b1478c10709a1e0200abbebb38a5d9580271ac182f2`  
		Last Modified: Tue, 01 Sep 2020 10:47:38 GMT  
		Size: 16.8 KB (16773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af1cf873ec51cf5593d71906407d3ed6fbe34f0a7e9b5ba51da520a059270c8`  
		Last Modified: Tue, 01 Sep 2020 10:47:37 GMT  
		Size: 8.4 KB (8411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a5b3fdadb8b277526583bc0021945658ef0970d7b67492ba549ba58f849c616`  
		Last Modified: Wed, 02 Sep 2020 03:41:10 GMT  
		Size: 490.2 KB (490213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c70f1e5f403b153426c20378ae18b939e9746665c02daed2c2103c6911c4a7`  
		Last Modified: Wed, 02 Sep 2020 03:41:10 GMT  
		Size: 2.9 MB (2919790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a60403fc5578f2f7c3563b8b87c076dfcd8fdb12d80fed2cf710159e30e573bd`  
		Last Modified: Wed, 02 Sep 2020 03:41:10 GMT  
		Size: 1.3 MB (1334732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0b36263acaaaf8d6035e7d6aeef14c3e441baa6287d56bb175d471d5d7eb46d`  
		Last Modified: Wed, 02 Sep 2020 03:41:10 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull postfixadmin@sha256:a85889f73946b4ef5494d2cecd1a1a21085e2a002560e68d0c6b96710a818e97
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.9 MB (35912382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f49f7ba8bd4de61c9e75c90395df74ff4e4f5f7b37a57b5daf54fc310bb9fe42`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
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
# Thu, 11 Jun 2020 19:52:41 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 03 Sep 2020 21:17:26 GMT
ENV PHP_VERSION=7.3.22
# Thu, 03 Sep 2020 21:17:27 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.22.tar.xz.asc
# Thu, 03 Sep 2020 21:17:36 GMT
ENV PHP_SHA256=0e66606d3bdab5c2ae3f778136bfe8788e574913a3d8138695e54d98562f1fb5 PHP_MD5=
# Thu, 03 Sep 2020 21:18:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 21:18:23 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 21:21:36 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 21:21:53 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 03 Sep 2020 21:22:18 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 21:22:20 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 21:22:25 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 21:22:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 03 Sep 2020 21:22:49 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Sep 2020 21:22:55 GMT
EXPOSE 9000
# Thu, 03 Sep 2020 21:23:00 GMT
CMD ["php-fpm"]
# Fri, 04 Sep 2020 02:48:23 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 04 Sep 2020 02:48:25 GMT
RUN apk add --no-cache 		bash
# Fri, 04 Sep 2020 02:49:19 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		sqlite-dev 		postgresql-dev 	; 	docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 04 Sep 2020 02:49:20 GMT
ARG POSTFIXADMIN_VERSION=3.2.4
# Fri, 04 Sep 2020 02:49:21 GMT
ARG POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Fri, 04 Sep 2020 02:49:21 GMT
ENV POSTFIXADMIN_VERSION=3.2.4
# Fri, 04 Sep 2020 02:49:22 GMT
ENV POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Fri, 04 Sep 2020 02:49:25 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 04 Sep 2020 02:49:26 GMT
COPY file:c6e11ee7dda40f44aa31f3bcb74669e99572ad86040276440b444d5699d333f5 in /usr/local/bin/ 
# Fri, 04 Sep 2020 02:49:27 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 04 Sep 2020 02:49:28 GMT
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
	-	`sha256:8b4576cfe44ea3ec520b8405e3e0ad653fedff3809924060f37d0e9dccc3283d`  
		Last Modified: Thu, 03 Sep 2020 21:53:31 GMT  
		Size: 12.2 MB (12153577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07667047409d32f3e79ef0030ac4bbaf0e36ff9300a212f9960ae8bf588761f9`  
		Last Modified: Thu, 03 Sep 2020 21:53:27 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63c775eb5f280deed89c6afadf56a682c262abec02bd59cd779352d447938b9b`  
		Last Modified: Thu, 03 Sep 2020 21:53:29 GMT  
		Size: 14.6 MB (14600482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c187145b36f5d73b5115246305233efb3fc0b04561b04cb9afdbdb5376e4c55d`  
		Last Modified: Thu, 03 Sep 2020 21:53:27 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61f7c250ada3b6d24acf9d0f4c68d56f35fb12bcdaad516927521313e5f3aaa3`  
		Last Modified: Thu, 03 Sep 2020 21:53:28 GMT  
		Size: 16.8 KB (16801 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f71ee337983119d9ddac11ed0883afddc881e4f3c51b91419e637a029acf522`  
		Last Modified: Thu, 03 Sep 2020 21:53:28 GMT  
		Size: 8.4 KB (8416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:237eed64e65e820f8550fc0aaa7a58269694b19904da45dccd39156baf4c4b29`  
		Last Modified: Fri, 04 Sep 2020 02:50:31 GMT  
		Size: 568.4 KB (568388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a5fe7e08ae6aca37fa2f2fbb7af5991f72e3369cabdb26e15ea925b56af932`  
		Last Modified: Fri, 04 Sep 2020 02:50:31 GMT  
		Size: 3.2 MB (3173422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db6f1dc33af9ed5e6b6fec0f62195d769cf02d5485943fdd58510b3cd07739a`  
		Last Modified: Fri, 04 Sep 2020 02:50:31 GMT  
		Size: 1.3 MB (1334714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb83d12f61ed967a88f9c14e6968d307e055ef67e1d1c7645606079396adc438`  
		Last Modified: Fri, 04 Sep 2020 02:50:31 GMT  
		Size: 1.3 KB (1327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; 386

```console
$ docker pull postfixadmin@sha256:60886ab8f1677079b1279c261ebb9bd70dda74a63e9aad401881091bb73a1e51
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.8 MB (36823903 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fbb486ef48491ad7fb4ca11caf2161308167397923fe8f018395ff0dc057af06`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
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
# Thu, 11 Jun 2020 21:10:10 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 03 Sep 2020 22:42:31 GMT
ENV PHP_VERSION=7.3.22
# Thu, 03 Sep 2020 22:42:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.22.tar.xz.asc
# Thu, 03 Sep 2020 22:42:32 GMT
ENV PHP_SHA256=0e66606d3bdab5c2ae3f778136bfe8788e574913a3d8138695e54d98562f1fb5 PHP_MD5=
# Thu, 03 Sep 2020 22:42:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 22:42:36 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 22:49:35 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 22:49:35 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 03 Sep 2020 22:49:37 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 22:49:37 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 22:49:37 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 22:49:38 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 03 Sep 2020 22:49:38 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Sep 2020 22:49:38 GMT
EXPOSE 9000
# Thu, 03 Sep 2020 22:49:39 GMT
CMD ["php-fpm"]
# Fri, 04 Sep 2020 01:36:55 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 04 Sep 2020 01:36:56 GMT
RUN apk add --no-cache 		bash
# Fri, 04 Sep 2020 01:37:31 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		sqlite-dev 		postgresql-dev 	; 	docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 04 Sep 2020 01:37:32 GMT
ARG POSTFIXADMIN_VERSION=3.2.4
# Fri, 04 Sep 2020 01:37:32 GMT
ARG POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Fri, 04 Sep 2020 01:37:32 GMT
ENV POSTFIXADMIN_VERSION=3.2.4
# Fri, 04 Sep 2020 01:37:32 GMT
ENV POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Fri, 04 Sep 2020 01:37:34 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 04 Sep 2020 01:37:34 GMT
COPY file:c6e11ee7dda40f44aa31f3bcb74669e99572ad86040276440b444d5699d333f5 in /usr/local/bin/ 
# Fri, 04 Sep 2020 01:37:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 04 Sep 2020 01:37:34 GMT
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
	-	`sha256:1a54af47a399a680f8e8e7e1ebbe06c8799b832e032845b157f5e76396be8bc6`  
		Last Modified: Thu, 03 Sep 2020 23:26:19 GMT  
		Size: 12.2 MB (12153552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4686f5b512f801e9e7b5360357547551bb13ae39362d622c1f414106a812167d`  
		Last Modified: Thu, 03 Sep 2020 23:26:16 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc4dffbdd31d72fc018d916c9dd69fc28df906ebd46f3a1f20f94b69a1d58bab`  
		Last Modified: Thu, 03 Sep 2020 23:26:22 GMT  
		Size: 15.2 MB (15217858 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8729bda5ba512dff79c2c9456f1346e2057f0eb4b8c1847a33679889557de164`  
		Last Modified: Thu, 03 Sep 2020 23:26:16 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6c265de0f15ca66715cf3aff554902fb80eb7ab8f2c6329de6f92a16522a0df`  
		Last Modified: Thu, 03 Sep 2020 23:26:16 GMT  
		Size: 16.8 KB (16798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:139c440a934a35b37d8e2ffa8355995da406ff58b71b8c8c98845c99f93e0c73`  
		Last Modified: Thu, 03 Sep 2020 23:26:16 GMT  
		Size: 8.4 KB (8410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176ef8dd0617a02ac520eec31130f1235e2c8ab6809ac62f0234e294fa5b8ff4`  
		Last Modified: Fri, 04 Sep 2020 01:38:14 GMT  
		Size: 598.5 KB (598487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:064093ed3cb963c7c69bba59b6b58fb40bb01412948bbfde9a738f6e1c09400b`  
		Last Modified: Fri, 04 Sep 2020 01:38:15 GMT  
		Size: 3.3 MB (3256426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6cd7a28ef19fc810ccc2054006eab2f7d394922ec0b6ae4a6415e67a78d022`  
		Last Modified: Fri, 04 Sep 2020 01:38:15 GMT  
		Size: 1.3 MB (1334687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9edf0dab718d1717215debd1ab91b1cae4f7fb4741308895cbafb0ca1b088d45`  
		Last Modified: Fri, 04 Sep 2020 01:38:15 GMT  
		Size: 1.3 KB (1328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; ppc64le

```console
$ docker pull postfixadmin@sha256:184a5427969c507e6684763c30e8dbe36380c9823376b41bfead4c59be037fed
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.4 MB (37376156 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e254b57d24b9bebdafffc8cd77fa7337a061ef8709a51663757879d3ab8f5a77`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
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
# Thu, 11 Jun 2020 20:12:17 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 03 Sep 2020 21:33:41 GMT
ENV PHP_VERSION=7.3.22
# Thu, 03 Sep 2020 21:33:47 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.22.tar.xz.asc
# Thu, 03 Sep 2020 21:33:54 GMT
ENV PHP_SHA256=0e66606d3bdab5c2ae3f778136bfe8788e574913a3d8138695e54d98562f1fb5 PHP_MD5=
# Thu, 03 Sep 2020 21:34:23 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 21:34:27 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 21:39:00 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 21:39:06 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 03 Sep 2020 21:39:21 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 21:39:29 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 21:39:36 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 21:39:59 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 03 Sep 2020 21:40:06 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Sep 2020 21:40:15 GMT
EXPOSE 9000
# Thu, 03 Sep 2020 21:40:24 GMT
CMD ["php-fpm"]
# Fri, 04 Sep 2020 04:17:05 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Fri, 04 Sep 2020 04:17:14 GMT
RUN apk add --no-cache 		bash
# Fri, 04 Sep 2020 04:18:09 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		sqlite-dev 		postgresql-dev 	; 	docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Fri, 04 Sep 2020 04:18:13 GMT
ARG POSTFIXADMIN_VERSION=3.2.4
# Fri, 04 Sep 2020 04:18:17 GMT
ARG POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Fri, 04 Sep 2020 04:18:19 GMT
ENV POSTFIXADMIN_VERSION=3.2.4
# Fri, 04 Sep 2020 04:18:22 GMT
ENV POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Fri, 04 Sep 2020 04:18:32 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Fri, 04 Sep 2020 04:18:33 GMT
COPY file:c6e11ee7dda40f44aa31f3bcb74669e99572ad86040276440b444d5699d333f5 in /usr/local/bin/ 
# Fri, 04 Sep 2020 04:18:35 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Fri, 04 Sep 2020 04:18:38 GMT
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
	-	`sha256:2acb24c98381c83d0499031de0bc6e7b5b47b6a600b46c32289b715f1f7c5b53`  
		Last Modified: Thu, 03 Sep 2020 22:27:57 GMT  
		Size: 12.2 MB (12153579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35fde3c33f6bd77f724338ef4d66b71f8b745a910f2efebd618ca05d62106eda`  
		Last Modified: Thu, 03 Sep 2020 22:27:50 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7c76db27b1cb0c84fbe2eac417ddfd508971dd6f0a5faa7fbf810d9772f8b18`  
		Last Modified: Thu, 03 Sep 2020 22:27:57 GMT  
		Size: 15.9 MB (15874513 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae1dae76d67a997b671e7d382e9637ff1a472c2b5bd60a251ddc841f971a1c5a`  
		Last Modified: Thu, 03 Sep 2020 22:27:50 GMT  
		Size: 2.3 KB (2270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d38a0f8fdec56edf0708873e5dcafb2d429b4855d6358b4d13abfe66d3e95b4`  
		Last Modified: Thu, 03 Sep 2020 22:27:50 GMT  
		Size: 16.8 KB (16799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24fdeaa8eaac8caaa8d97ee9f5fdcc2dd410e41280258590df3f92f0c7df36f5`  
		Last Modified: Thu, 03 Sep 2020 22:27:50 GMT  
		Size: 8.4 KB (8412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bc6587ca0b12822c0dd58b7c8a37b87822eed1f9d3c5d2b4c1272b8184d9a9c`  
		Last Modified: Fri, 04 Sep 2020 04:20:01 GMT  
		Size: 621.7 KB (621677 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56a3451d5dd89c4ccc3e431422264b8af4eaaf5dbbe18f425a5b9a34d4a39319`  
		Last Modified: Fri, 04 Sep 2020 04:20:02 GMT  
		Size: 3.2 MB (3172297 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c72fd15814babf739ba4451b55429e88b4506c3d8e7a054a7fc0cf927da276a3`  
		Last Modified: Fri, 04 Sep 2020 04:20:03 GMT  
		Size: 1.3 MB (1334740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d47695c2d635341dd46f6920e23c7cee1f2a170f2f3dfb7efa9a7973f92c3d`  
		Last Modified: Fri, 04 Sep 2020 04:20:00 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `postfixadmin:3-fpm-alpine` - linux; s390x

```console
$ docker pull postfixadmin@sha256:38822a595a6730b8561883b4a389156d7462fd7e46c08f118cb9111c93286d0e
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.2 MB (35198116 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7830d4e2d294a7bd1baeac03eaa5882ab67e888b4a21e1f871f647d70d6f1354`
-	Entrypoint: `["\/usr\/local\/bin\/docker-entrypoint.sh"]`
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
# Thu, 11 Jun 2020 19:07:14 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 03 Sep 2020 19:50:40 GMT
ENV PHP_VERSION=7.3.22
# Thu, 03 Sep 2020 19:50:40 GMT
ENV PHP_URL=https://www.php.net/distributions/php-7.3.22.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-7.3.22.tar.xz.asc
# Thu, 03 Sep 2020 19:50:41 GMT
ENV PHP_SHA256=0e66606d3bdab5c2ae3f778136bfe8788e574913a3d8138695e54d98562f1fb5 PHP_MD5=
# Thu, 03 Sep 2020 19:50:46 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Thu, 03 Sep 2020 19:50:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Sep 2020 19:54:19 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libedit-dev 		libsodium-dev 		libxml2-dev 		openssl-dev 		sqlite-dev 	; 		export CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -perm +0111 -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Sep 2020 19:54:22 GMT
COPY multi:bd67471e0c4047be362a8a0e199558e6245207a6f70b72fdfe55aa2d2cae15e6 in /usr/local/bin/ 
# Thu, 03 Sep 2020 19:54:24 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Sep 2020 19:54:24 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Sep 2020 19:54:25 GMT
WORKDIR /var/www/html
# Thu, 03 Sep 2020 19:54:26 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 03 Sep 2020 19:54:27 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Sep 2020 19:54:27 GMT
EXPOSE 9000
# Thu, 03 Sep 2020 19:54:28 GMT
CMD ["php-fpm"]
# Thu, 03 Sep 2020 22:08:05 GMT
LABEL maintainer=David Goodwin <david@codepoets.co.uk> (@DavidGoodwin)
# Thu, 03 Sep 2020 22:08:05 GMT
RUN apk add --no-cache 		bash
# Thu, 03 Sep 2020 22:08:26 GMT
RUN set -ex; 		apk add --no-cache --virtual .build-deps 		sqlite-dev 		postgresql-dev 	; 	docker-php-ext-install -j "$(nproc)" 		mysqli 		pdo_mysql 		pdo_pgsql 		pdo_sqlite 		pgsql 	; 	runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local/lib/php/extensions 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --virtual .postfixadmin-phpexts-rundeps $runDeps; 	apk del .build-deps
# Thu, 03 Sep 2020 22:08:26 GMT
ARG POSTFIXADMIN_VERSION=3.2.4
# Thu, 03 Sep 2020 22:08:27 GMT
ARG POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Thu, 03 Sep 2020 22:08:27 GMT
ENV POSTFIXADMIN_VERSION=3.2.4
# Thu, 03 Sep 2020 22:08:27 GMT
ENV POSTFIXADMIN_SHA512=2bd7ae05addbaf3c6c7eebea16ec1e21b2c67c8e6161446ed82a9553c26c04e19c1ec9ce248a9b9df504df56d309590259e6f04907b04b593548028b40e40d47
# Thu, 03 Sep 2020 22:08:28 GMT
RUN set -eu; 	curl -fsSL -o postfixadmin.tar.gz "https://github.com/postfixadmin/postfixadmin/archive/postfixadmin-${POSTFIXADMIN_VERSION}.tar.gz"; 	echo "$POSTFIXADMIN_SHA512 *postfixadmin.tar.gz" | sha512sum -c -; 	mkdir /usr/src/postfixadmin; 	tar -xf postfixadmin.tar.gz -C /usr/src/postfixadmin --strip-components=1; 	rm postfixadmin.tar.gz; 	mkdir -p /usr/src/postfixadmin/templates_c; 	chown -R www-data:www-data /usr/src/postfixadmin
# Thu, 03 Sep 2020 22:08:29 GMT
COPY file:c6e11ee7dda40f44aa31f3bcb74669e99572ad86040276440b444d5699d333f5 in /usr/local/bin/ 
# Thu, 03 Sep 2020 22:08:29 GMT
ENTRYPOINT ["/usr/local/bin/docker-entrypoint.sh"]
# Thu, 03 Sep 2020 22:08:29 GMT
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
	-	`sha256:0d8dfa06481be2036a91c2c52a85e332aef966b0c3171dd47bdfa4511a06bb25`  
		Last Modified: Thu, 03 Sep 2020 20:19:30 GMT  
		Size: 12.2 MB (12153571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fe846965d9a8c6ce582f1edded356b011f28c80aa4e6f440be57cf14d19f06d`  
		Last Modified: Thu, 03 Sep 2020 20:19:28 GMT  
		Size: 497.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1041419e18496c551a124baf156c1cf1a3c341dd2511cc556807d6f996c97dd2`  
		Last Modified: Thu, 03 Sep 2020 20:19:30 GMT  
		Size: 14.2 MB (14178993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c300997115a4110e44afd79edadba995222d9daee37a5010977667396061cc53`  
		Last Modified: Thu, 03 Sep 2020 20:19:28 GMT  
		Size: 2.3 KB (2274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b84aa9614c96876ef70e566f82d9ab2d1b88b6c48ce8d08fed87e9bc10cc7d1`  
		Last Modified: Thu, 03 Sep 2020 20:19:28 GMT  
		Size: 16.8 KB (16795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4c72b9c1e81052b135aa6d9a7a3f69b4da440a83d13ce52fada71311271f15d`  
		Last Modified: Thu, 03 Sep 2020 20:19:28 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee612ae59d55af3b2241be82d629a99b19ea1d95d32ca69cad434a5985c5b939`  
		Last Modified: Thu, 03 Sep 2020 22:09:10 GMT  
		Size: 576.6 KB (576583 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91f9869df9f3b78a8051e678fedc5919353d6b1a2e741c811d3179739fef57a7`  
		Last Modified: Thu, 03 Sep 2020 22:09:10 GMT  
		Size: 3.0 MB (2974483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ef65ee6d7527e74c35341c13e79b46990ae23f2ffc80fa48a5cedef1b4b18fb`  
		Last Modified: Thu, 03 Sep 2020 22:09:10 GMT  
		Size: 1.3 MB (1334721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15481bcbc4f440254ac928001022faad5798e42c6d8e327056fd543f9d446283`  
		Last Modified: Thu, 03 Sep 2020 22:09:10 GMT  
		Size: 1.3 KB (1325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
