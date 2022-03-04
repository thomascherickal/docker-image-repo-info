## `yourls:1-fpm-alpine`

```console
$ docker pull yourls@sha256:8a2e7d84ee36619126feed25f4ad70cf49866a4fb2371dc6b8e0af05b93efbb9
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
$ docker pull yourls@sha256:577904a6a1cb1f99736635bf7d79a43e639596427a65971856daf1e66ba2b5bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.0 MB (31950537 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:28032bed508f4b5f800342eaabb2f6ef70aa9f5a5cceeadcbb4fb2b191c3fadf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 07:06:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 07:06:03 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 07:06:04 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 07:06:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 07:06:05 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 07:06:05 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 07:06:06 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 07:06:06 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 07:50:54 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 18 Feb 2022 22:07:31 GMT
ENV PHP_VERSION=8.0.16
# Fri, 18 Feb 2022 22:07:31 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.16.tar.xz.asc
# Fri, 18 Feb 2022 22:07:31 GMT
ENV PHP_SHA256=f27a2f25259e8c51e42dfd74e24a546ee521438ad7d9f6c6e794aa91f38bab0a
# Fri, 18 Feb 2022 22:08:47 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 18 Feb 2022 22:08:47 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Mar 2022 09:34:45 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Mar 2022 09:34:45 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 03 Mar 2022 09:34:47 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Mar 2022 09:34:47 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Mar 2022 09:34:47 GMT
WORKDIR /var/www/html
# Thu, 03 Mar 2022 09:34:47 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 03 Mar 2022 09:34:47 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Mar 2022 09:34:48 GMT
EXPOSE 9000
# Thu, 03 Mar 2022 09:34:48 GMT
CMD ["php-fpm"]
# Thu, 03 Mar 2022 18:27:49 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 03 Mar 2022 18:27:49 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 03 Mar 2022 18:27:49 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 03 Mar 2022 18:27:49 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 03 Mar 2022 18:27:49 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 03 Mar 2022 18:27:49 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 03 Mar 2022 18:27:49 GMT
LABEL org.opencontainers.image.version=1.8.2
# Thu, 03 Mar 2022 18:28:49 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 03 Mar 2022 18:28:50 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 03 Mar 2022 18:28:51 GMT
RUN apk add --no-cache bash
# Thu, 03 Mar 2022 18:28:52 GMT
RUN set -eux;     version="1.8.2";     sha256="6d818622e3ba1d5785c2dbcc088be6890f5675fd4f24a2e3111eda4523bbd7ae";     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${version}.tar.gz";     echo "$sha256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${version}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 03 Mar 2022 18:28:52 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 03 Mar 2022 18:28:53 GMT
COPY file:6b25ad92f8d7ceda57a7891b5b9f6f74a178e41b54c0d1e9644ce8ca0debdaab in /usr/local/bin/ 
# Thu, 03 Mar 2022 18:28:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 18:28:53 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c7da25b2876b1c935b05d7e6efa3e8cd559d031cf30b246d7659ed438726acd`  
		Last Modified: Tue, 30 Nov 2021 09:03:50 GMT  
		Size: 1.7 MB (1709704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bc599114627e3bd98e0204b93b161e03065bf9a228bb02ae202469655f12b8d`  
		Last Modified: Tue, 30 Nov 2021 09:03:48 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927a0b37a45a98d7d74a6d7d1567230eca834fb89417274557de7986d1f39401`  
		Last Modified: Tue, 30 Nov 2021 09:03:48 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4980da2f4b2ff4ec9ffdfef85e5ce26f3cffabb61b890f15c5c553948bad2c65`  
		Last Modified: Fri, 18 Feb 2022 23:05:29 GMT  
		Size: 10.9 MB (10883961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d8d633f95152424fcb2f23e5cdc379d0004082718ff2d06c40155289765bcb4`  
		Last Modified: Fri, 18 Feb 2022 23:05:28 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0344fa6721078ddab6eb4f2fbd93479490352a2b9e223c36864cb64088b1817`  
		Last Modified: Thu, 03 Mar 2022 12:01:42 GMT  
		Size: 12.8 MB (12777629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e4ffc5b87420f262cf2f07402a5ef4ef8b29e01a6cde3669fd087c26e7798f6`  
		Last Modified: Thu, 03 Mar 2022 12:01:40 GMT  
		Size: 2.3 KB (2299 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d97c5b84334e1da8b5a61285710b86aeb55373e6a3baf01163a73063c306eb2c`  
		Last Modified: Thu, 03 Mar 2022 12:01:40 GMT  
		Size: 18.3 KB (18263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a4a896551df891808a1830beb963cceabeabbb8f39363e6f18eb0ad69b50c60`  
		Last Modified: Thu, 03 Mar 2022 12:01:40 GMT  
		Size: 8.6 KB (8567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1b869d84317977441a817c7f89f448d9bd7cd390f574141e5e34bdc69db52d`  
		Last Modified: Thu, 03 Mar 2022 18:30:13 GMT  
		Size: 684.5 KB (684466 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cb77add3f26fea2c9c37f2b9df2b6f45891beee92ba1bde30e1362375aa546c`  
		Last Modified: Thu, 03 Mar 2022 18:30:10 GMT  
		Size: 323.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee90e22476183139fa0f9fd191ef1406fd48504e2948390f715d5249e25bd204`  
		Last Modified: Thu, 03 Mar 2022 18:30:10 GMT  
		Size: 466.8 KB (466783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdc9745caf8c1b955f4e8b80553920453824b6ada6b3aeff6a41ba42c8595ddd`  
		Last Modified: Thu, 03 Mar 2022 18:30:11 GMT  
		Size: 2.6 MB (2574522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d123c7db5667466e717937fe4ebe99b35db667602daab9317ae74880db06423`  
		Last Modified: Thu, 03 Mar 2022 18:30:10 GMT  
		Size: 2.0 KB (2042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bd279d7e566bf6fd37a615aa3d04f20d4d9e6639ed15045aced4404dd93a4a1`  
		Last Modified: Thu, 03 Mar 2022 18:30:10 GMT  
		Size: 1.5 KB (1540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; arm variant v6

```console
$ docker pull yourls@sha256:23d4147f5d487c792c91e39b9c55324896ab0a4f03d182aa176b3ea649f4f322
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.1 MB (30082345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c36792fd54dece96dc8fe7ae05bf933667baf8168bde80e9eaeb1d4520eab528`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 03:20:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 03:20:06 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 03:20:07 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 03:20:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 03:20:10 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 03:20:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 03:20:11 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 03:20:11 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 03:40:16 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 18 Feb 2022 20:12:32 GMT
ENV PHP_VERSION=8.0.16
# Fri, 18 Feb 2022 20:12:33 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.16.tar.xz.asc
# Fri, 18 Feb 2022 20:12:33 GMT
ENV PHP_SHA256=f27a2f25259e8c51e42dfd74e24a546ee521438ad7d9f6c6e794aa91f38bab0a
# Fri, 18 Feb 2022 20:12:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 18 Feb 2022 20:12:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 02 Mar 2022 19:34:04 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 02 Mar 2022 19:34:05 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Wed, 02 Mar 2022 19:34:07 GMT
RUN docker-php-ext-enable sodium
# Wed, 02 Mar 2022 19:34:08 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 02 Mar 2022 19:34:08 GMT
WORKDIR /var/www/html
# Wed, 02 Mar 2022 19:34:10 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 02 Mar 2022 19:34:10 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Mar 2022 19:34:11 GMT
EXPOSE 9000
# Wed, 02 Mar 2022 19:34:11 GMT
CMD ["php-fpm"]
# Thu, 03 Mar 2022 00:14:16 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 03 Mar 2022 00:14:16 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 03 Mar 2022 00:14:16 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 03 Mar 2022 00:14:17 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 03 Mar 2022 00:14:17 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 03 Mar 2022 00:14:17 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 03 Mar 2022 00:14:18 GMT
LABEL org.opencontainers.image.version=1.8.2
# Thu, 03 Mar 2022 00:15:30 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 03 Mar 2022 00:15:31 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 03 Mar 2022 00:15:34 GMT
RUN apk add --no-cache bash
# Thu, 03 Mar 2022 00:15:37 GMT
RUN set -eux;     version="1.8.2";     sha256="6d818622e3ba1d5785c2dbcc088be6890f5675fd4f24a2e3111eda4523bbd7ae";     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${version}.tar.gz";     echo "$sha256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${version}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 03 Mar 2022 00:15:37 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 03 Mar 2022 00:15:38 GMT
COPY file:6b25ad92f8d7ceda57a7891b5b9f6f74a178e41b54c0d1e9644ce8ca0debdaab in /usr/local/bin/ 
# Thu, 03 Mar 2022 00:15:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 00:15:39 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289be6d758ff0faa38d64732e5736031f2250cbf78d1ca4b32abba4accd6a3fa`  
		Last Modified: Tue, 30 Nov 2021 04:29:36 GMT  
		Size: 1.7 MB (1698826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0b442a0f679dba79aa838c408cf49916ca26d27e1252e26f3904d7c5b83d6c`  
		Last Modified: Tue, 30 Nov 2021 04:29:33 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fef02b1cade59fbcc24c0ee972dd15d8caa89dda554cdb8aa742de1c6f3d5b7c`  
		Last Modified: Tue, 30 Nov 2021 04:29:33 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4abcccb86faff724c50ffc5ac62773a72be1c07cdc43ddcfcff1172313fcc2a5`  
		Last Modified: Fri, 18 Feb 2022 20:47:14 GMT  
		Size: 10.9 MB (10883952 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd66e05dd6d0fb5691229193b2debcdb8cc41f39adb7c248e9df6b85a78b173f`  
		Last Modified: Fri, 18 Feb 2022 20:47:11 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55f7ad05a39ef09ba9ad135a9f5b0828330803a32ab3d8cfbef6e45bb0af4f49`  
		Last Modified: Wed, 02 Mar 2022 20:58:00 GMT  
		Size: 11.5 MB (11468421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20042c30630573e848e7806243e0eef3a5685f62b929c6e4536c8aca4364e237`  
		Last Modified: Wed, 02 Mar 2022 20:57:51 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2d3b74d3f3b09fcf77792c7ecff5d17c256e0d47e768f04a423304573baca83`  
		Last Modified: Wed, 02 Mar 2022 20:57:51 GMT  
		Size: 18.3 KB (18259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8cfcff16623a5f341ece6b87226209c7db0ba32ecfa74e45786e33ca933927`  
		Last Modified: Wed, 02 Mar 2022 20:57:51 GMT  
		Size: 8.6 KB (8570 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53439965bd88b12b93c412d7e3167122eeb52931aea50162298ff529a00135b`  
		Last Modified: Thu, 03 Mar 2022 00:16:12 GMT  
		Size: 335.2 KB (335189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d127f69b3c8be107aa5a232bf67fe61c4e8001ca29a9e20cd8d77a72617a199`  
		Last Modified: Thu, 03 Mar 2022 00:16:10 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bb481261090d1ee5e550b4d096af2a5bbf86d699237dd48ff12cce239c22cec`  
		Last Modified: Thu, 03 Mar 2022 00:16:13 GMT  
		Size: 454.9 KB (454938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220740024431df8e7375e96fe1d99cb90545845bfcbf988287aee7a8ddd6a894`  
		Last Modified: Thu, 03 Mar 2022 00:16:12 GMT  
		Size: 2.6 MB (2574518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d135b02fbb9fc36bd1eada69c866f9ecd2aba6b17eff0e65ff1c28bffa3225ff`  
		Last Modified: Thu, 03 Mar 2022 00:16:10 GMT  
		Size: 2.0 KB (2045 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1962227307f711f9f195ec324634e689e7910860590cd3476049cb3d215c1c`  
		Last Modified: Thu, 03 Mar 2022 00:16:14 GMT  
		Size: 1.5 KB (1546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; arm variant v7

```console
$ docker pull yourls@sha256:c035afffd8826e5437f3712736825cc840f09208cd8db55bc762acc480730959
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **29.0 MB (28965341 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d34d82f6159e761a518064d1ebc44ba7f549093cbd55d4fc0b3d5de82f8446b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 05:27:13 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 05:27:16 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 05:27:18 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 05:27:18 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 05:27:20 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 05:27:20 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 05:27:21 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 05:27:21 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 05:48:42 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 18 Feb 2022 21:45:55 GMT
ENV PHP_VERSION=8.0.16
# Fri, 18 Feb 2022 21:45:56 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.16.tar.xz.asc
# Fri, 18 Feb 2022 21:45:56 GMT
ENV PHP_SHA256=f27a2f25259e8c51e42dfd74e24a546ee521438ad7d9f6c6e794aa91f38bab0a
# Fri, 18 Feb 2022 21:46:20 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 18 Feb 2022 21:46:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 03 Mar 2022 13:32:42 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 03 Mar 2022 13:32:43 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Thu, 03 Mar 2022 13:32:46 GMT
RUN docker-php-ext-enable sodium
# Thu, 03 Mar 2022 13:32:46 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 03 Mar 2022 13:32:46 GMT
WORKDIR /var/www/html
# Thu, 03 Mar 2022 13:32:48 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 03 Mar 2022 13:32:48 GMT
STOPSIGNAL SIGQUIT
# Thu, 03 Mar 2022 13:32:49 GMT
EXPOSE 9000
# Thu, 03 Mar 2022 13:32:49 GMT
CMD ["php-fpm"]
# Thu, 03 Mar 2022 23:03:17 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 03 Mar 2022 23:03:17 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 03 Mar 2022 23:03:18 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 03 Mar 2022 23:03:18 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 03 Mar 2022 23:03:19 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 03 Mar 2022 23:03:19 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 03 Mar 2022 23:03:20 GMT
LABEL org.opencontainers.image.version=1.8.2
# Thu, 03 Mar 2022 23:04:31 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 03 Mar 2022 23:04:33 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 03 Mar 2022 23:04:35 GMT
RUN apk add --no-cache bash
# Thu, 03 Mar 2022 23:04:39 GMT
RUN set -eux;     version="1.8.2";     sha256="6d818622e3ba1d5785c2dbcc088be6890f5675fd4f24a2e3111eda4523bbd7ae";     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${version}.tar.gz";     echo "$sha256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${version}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 03 Mar 2022 23:04:39 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 03 Mar 2022 23:04:40 GMT
COPY file:6b25ad92f8d7ceda57a7891b5b9f6f74a178e41b54c0d1e9644ce8ca0debdaab in /usr/local/bin/ 
# Thu, 03 Mar 2022 23:04:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 23:04:40 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:484fe107211badcebee7c4211e5ed91c7e5212cdd6d7edbb292a63ec60572bdd`  
		Last Modified: Tue, 30 Nov 2021 06:57:00 GMT  
		Size: 1.6 MB (1568802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93353d0a7113f37ba224b9ee296684e49f27c1c9440d3a3c5d310749213da97f`  
		Last Modified: Tue, 30 Nov 2021 06:56:59 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137db50a58959a68358c190d2a143088b82ab25d97cb889876fbc0728e446058`  
		Last Modified: Tue, 30 Nov 2021 06:57:00 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f85306bf3400a541262c2d867e8e2046a1539c9c71564acf85bc520d80c8999f`  
		Last Modified: Fri, 18 Feb 2022 22:45:29 GMT  
		Size: 10.9 MB (10883954 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0074d2d46affda7a8fd787c3cdac23d90ccaa67e6314a239bf7f98bfed5cb30`  
		Last Modified: Fri, 18 Feb 2022 22:45:27 GMT  
		Size: 500.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85dd41ab76ed544d2d328e4101cc30fc745bb9acbb14623570a05ae83117539a`  
		Last Modified: Thu, 03 Mar 2022 16:23:49 GMT  
		Size: 10.7 MB (10747158 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61a804a54942235b8ba370429b47d0329d13384c58a8339d6d901691019d2e05`  
		Last Modified: Thu, 03 Mar 2022 16:23:42 GMT  
		Size: 2.3 KB (2302 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bbe6e11505dbfdaa9770725e1bdc618134a2c94a794615c534d25bee68d4a6c`  
		Last Modified: Thu, 03 Mar 2022 16:23:42 GMT  
		Size: 18.3 KB (18256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c368901f69b334740b7056ace22e08b28a705341d442da0592ed97ad6920998d`  
		Last Modified: Thu, 03 Mar 2022 16:23:42 GMT  
		Size: 8.6 KB (8566 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf63a3eee6142bc40e1a41ff5760fc4b4c5a1f94a1983c95378e21b9f350e4d3`  
		Last Modified: Thu, 03 Mar 2022 23:07:07 GMT  
		Size: 305.7 KB (305667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01912e0e4ee19fccf6c5cffd2a7892ab85e55b13bb6708c263bfd697c32fe641`  
		Last Modified: Thu, 03 Mar 2022 23:07:05 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:357bdf3a2ea6285b36d0a1e0eee29451954efb816d6f1a742e23ef749de599c0`  
		Last Modified: Thu, 03 Mar 2022 23:07:05 GMT  
		Size: 415.4 KB (415405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2121646e71800af6dc968b1e5eba9a3185b0867bb784cc19dc6f692aaacbad`  
		Last Modified: Thu, 03 Mar 2022 23:07:07 GMT  
		Size: 2.6 MB (2574521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f20277abef89fafa51a19559c61f01287e3ddd7fea4896efbbc2284bcc770e`  
		Last Modified: Thu, 03 Mar 2022 23:07:05 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02e91610535bb7a61094e0bb21a2e4236a6b30d44eaccbcefd0714ea3f435d30`  
		Last Modified: Thu, 03 Mar 2022 23:07:05 GMT  
		Size: 1.5 KB (1544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:c73b15450d828735a0fd1b94913a9a719fa750d6be3e4dc62caa81693e4d13d0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.9 MB (30884945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db7d11b4a7419ac603eae96c46d8b086ba49bb2d846510db1c5940c51cd3193d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 02:50:45 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 02:50:47 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 02:50:48 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 02:50:49 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 02:50:50 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 02:50:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 02:50:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 02:50:53 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 03:15:23 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 18 Feb 2022 21:08:35 GMT
ENV PHP_VERSION=8.0.16
# Fri, 18 Feb 2022 21:08:36 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.16.tar.xz.asc
# Fri, 18 Feb 2022 21:08:37 GMT
ENV PHP_SHA256=f27a2f25259e8c51e42dfd74e24a546ee521438ad7d9f6c6e794aa91f38bab0a
# Fri, 18 Feb 2022 21:09:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 18 Feb 2022 21:09:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 02 Mar 2022 21:42:39 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 02 Mar 2022 21:42:41 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Wed, 02 Mar 2022 21:42:42 GMT
RUN docker-php-ext-enable sodium
# Wed, 02 Mar 2022 21:42:43 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 02 Mar 2022 21:42:44 GMT
WORKDIR /var/www/html
# Wed, 02 Mar 2022 21:42:45 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 02 Mar 2022 21:42:46 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Mar 2022 21:42:47 GMT
EXPOSE 9000
# Wed, 02 Mar 2022 21:42:48 GMT
CMD ["php-fpm"]
# Thu, 03 Mar 2022 05:22:08 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 03 Mar 2022 05:22:09 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 03 Mar 2022 05:22:10 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 03 Mar 2022 05:22:11 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 03 Mar 2022 05:22:12 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 03 Mar 2022 05:22:13 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 03 Mar 2022 05:22:14 GMT
LABEL org.opencontainers.image.version=1.8.2
# Thu, 03 Mar 2022 05:22:45 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 03 Mar 2022 05:22:46 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 03 Mar 2022 05:22:47 GMT
RUN apk add --no-cache bash
# Thu, 03 Mar 2022 05:22:49 GMT
RUN set -eux;     version="1.8.2";     sha256="6d818622e3ba1d5785c2dbcc088be6890f5675fd4f24a2e3111eda4523bbd7ae";     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${version}.tar.gz";     echo "$sha256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${version}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 03 Mar 2022 05:22:51 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 03 Mar 2022 05:22:52 GMT
COPY file:6b25ad92f8d7ceda57a7891b5b9f6f74a178e41b54c0d1e9644ce8ca0debdaab in /usr/local/bin/ 
# Thu, 03 Mar 2022 05:22:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 05:22:53 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd720d9f53003155e4cfe3f1974fc0e4d74a622ea8c61cfccb00ee8b842c09b6`  
		Last Modified: Tue, 30 Nov 2021 03:59:34 GMT  
		Size: 1.7 MB (1708308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680efee530f3c970c3140b358d3dc583ded463f9adbadb737ca64c765cf997ee`  
		Last Modified: Tue, 30 Nov 2021 03:59:33 GMT  
		Size: 1.2 KB (1234 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:643d01251bc949843dbd734a37e7cf28a01af4ea11443738b8b92d17e1e438de`  
		Last Modified: Tue, 30 Nov 2021 03:59:33 GMT  
		Size: 220.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1941af95e4f73bf43d47d287faeacca7a11f1ba18c8d6e81215ce3e81bf9801`  
		Last Modified: Fri, 18 Feb 2022 21:45:04 GMT  
		Size: 10.9 MB (10883763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8368295ed28c76f738f8c6945bc1599fa4c58ef9ebb0f5d3784cec7eaf07a0f0`  
		Last Modified: Fri, 18 Feb 2022 21:45:03 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac60e1a140a45d3c7482e44827d6b2be6b6a5ca9c95412358e3f2d0b57fedb67`  
		Last Modified: Wed, 02 Mar 2022 23:23:58 GMT  
		Size: 12.1 MB (12146169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53224a4648dcde85ff26e1f07b17dc27db4085c512351654c32d7a999b168a37`  
		Last Modified: Wed, 02 Mar 2022 23:23:56 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94aa00dbc780ce031d1a891ed25ff207f7edbcfe60fc8d1981ac49b226264f0e`  
		Last Modified: Wed, 02 Mar 2022 23:23:56 GMT  
		Size: 18.2 KB (18171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68625e639f458fc2cf41b3a80d054120a8e119d1d13773ee79b6cd1dbdd629c1`  
		Last Modified: Wed, 02 Mar 2022 23:23:56 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:943542235a771121149bab1b183ce9ec9513d1bd1c2312f87d924aa455041219`  
		Last Modified: Thu, 03 Mar 2022 05:24:43 GMT  
		Size: 346.9 KB (346941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7c5a9e46b065811b2db169b549e69c63b3a2a8177f960ddf982b37ed43a387a`  
		Last Modified: Thu, 03 Mar 2022 05:24:40 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aecc9cb2cee4117d347ed7bfca885a6b54b898557dce8446c6fb56cb5c9c024`  
		Last Modified: Thu, 03 Mar 2022 05:24:40 GMT  
		Size: 473.9 KB (473856 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d87d3986f07775790daf57dd1b4edc2a38d9ea83327a614d304d6c5e601e3af0`  
		Last Modified: Thu, 03 Mar 2022 05:24:40 GMT  
		Size: 2.6 MB (2575554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc9e9ba350e7f3a06c49e1f2974a5a67cd35ec9093e3834a838b05b62a5cdcc5`  
		Last Modified: Thu, 03 Mar 2022 05:24:40 GMT  
		Size: 2.0 KB (2047 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09c505adc5487fd4497fc6946342400418a7d0ebfea58561c4aa6767d7640657`  
		Last Modified: Thu, 03 Mar 2022 05:24:40 GMT  
		Size: 1.5 KB (1546 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; 386

```console
$ docker pull yourls@sha256:347e174fe261777bc1849a9754dca06dbdc55db151f7a22314d36f53e95df1f1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.3 MB (32321477 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3926aac09a3554478c18c2362f4aa92f1f20635b548b8fa757c59698c7f2df51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 05:59:02 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 05:59:06 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 05:59:07 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 05:59:08 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 05:59:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 05:59:10 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 05:59:10 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 05:59:10 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 06:44:18 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 18 Feb 2022 22:45:46 GMT
ENV PHP_VERSION=8.0.16
# Fri, 18 Feb 2022 22:45:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.16.tar.xz.asc
# Fri, 18 Feb 2022 22:45:46 GMT
ENV PHP_SHA256=f27a2f25259e8c51e42dfd74e24a546ee521438ad7d9f6c6e794aa91f38bab0a
# Fri, 18 Feb 2022 22:46:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 18 Feb 2022 22:46:58 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 02 Mar 2022 21:49:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 02 Mar 2022 21:49:34 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Wed, 02 Mar 2022 21:49:35 GMT
RUN docker-php-ext-enable sodium
# Wed, 02 Mar 2022 21:49:35 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 02 Mar 2022 21:49:35 GMT
WORKDIR /var/www/html
# Wed, 02 Mar 2022 21:49:36 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 02 Mar 2022 21:49:36 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Mar 2022 21:49:36 GMT
EXPOSE 9000
# Wed, 02 Mar 2022 21:49:36 GMT
CMD ["php-fpm"]
# Thu, 03 Mar 2022 08:37:06 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 03 Mar 2022 08:37:07 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 03 Mar 2022 08:37:07 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 03 Mar 2022 08:37:07 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 03 Mar 2022 08:37:07 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 03 Mar 2022 08:37:07 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 03 Mar 2022 08:37:08 GMT
LABEL org.opencontainers.image.version=1.8.2
# Thu, 03 Mar 2022 08:38:59 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 03 Mar 2022 08:38:59 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 03 Mar 2022 08:39:01 GMT
RUN apk add --no-cache bash
# Thu, 03 Mar 2022 08:39:03 GMT
RUN set -eux;     version="1.8.2";     sha256="6d818622e3ba1d5785c2dbcc088be6890f5675fd4f24a2e3111eda4523bbd7ae";     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${version}.tar.gz";     echo "$sha256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${version}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 03 Mar 2022 08:39:03 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 03 Mar 2022 08:39:04 GMT
COPY file:6b25ad92f8d7ceda57a7891b5b9f6f74a178e41b54c0d1e9644ce8ca0debdaab in /usr/local/bin/ 
# Thu, 03 Mar 2022 08:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 08:39:04 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14d6acd3b6e4278a7b3ef37d3525813808468237f086215b68594b244dbd1fba`  
		Last Modified: Tue, 30 Nov 2021 08:26:15 GMT  
		Size: 1.8 MB (1810453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc53af545b93519336bed63b8765255ac8280e27c8e3a17c336f92526b3f290`  
		Last Modified: Tue, 30 Nov 2021 08:26:14 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:07d406b6d62c3d67bec5f638d47d2b1b49c0ee41d80a791a1b90eaec776cf4fd`  
		Last Modified: Tue, 30 Nov 2021 08:26:13 GMT  
		Size: 267.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d05bde05ccf6474c639de373fcbb2d6cedc4098e1cd6e5a941c25e6125a82ff`  
		Last Modified: Fri, 18 Feb 2022 23:42:16 GMT  
		Size: 10.9 MB (10883956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c842b8d3c141c3cd755b4f8e01d23163154cd2de25e948f279cb5236834c66d0`  
		Last Modified: Fri, 18 Feb 2022 23:42:15 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55eacf560c6ead4a8ca49a9100cf029770f51a81191e2f4ac95913cd2c80e4cc`  
		Last Modified: Thu, 03 Mar 2022 00:36:52 GMT  
		Size: 13.0 MB (13024880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5676a0030aa46b962e99016b5f718bc486c1393541d88c869ba832978012d11`  
		Last Modified: Thu, 03 Mar 2022 00:36:49 GMT  
		Size: 2.3 KB (2305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec32ab3016916a528e66366acd415e67ee7fe8d8af5938bcd2f2d87022b79132`  
		Last Modified: Thu, 03 Mar 2022 00:36:49 GMT  
		Size: 18.3 KB (18253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5fe973d10aaa42bc1a7196c9265c0acad65bb3b27c9444228c61d91ebb3067e`  
		Last Modified: Thu, 03 Mar 2022 00:36:49 GMT  
		Size: 8.6 KB (8568 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0970e1664c631d4528c9700889797ab21d247c8dfc9b3628d5ea42641aea2d`  
		Last Modified: Thu, 03 Mar 2022 08:41:02 GMT  
		Size: 662.1 KB (662099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a021fe4efaf8dd4b12110e1aa2cb6a95fa364100abfc4a78f132198da95bb72`  
		Last Modified: Thu, 03 Mar 2022 08:40:59 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7895262befc22775b24f1fff3158d28ba8445dcfb8f93a9c1dbdfede7a7a018d`  
		Last Modified: Thu, 03 Mar 2022 08:40:59 GMT  
		Size: 503.4 KB (503387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9827f5516c82d8a111536c04d71b3d3221b40ca0e444cd889d6ebb84aa85628c`  
		Last Modified: Thu, 03 Mar 2022 08:41:00 GMT  
		Size: 2.6 MB (2574519 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b52ce47c515c1e6a9417a35e36f3944ecc1e7e348104fdc94fc719b3c0101f45`  
		Last Modified: Thu, 03 Mar 2022 08:40:59 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e09a92b58883ae90716ce233ed39d180c0ad04c192ca56f1ab5895ccb3bc61a0`  
		Last Modified: Thu, 03 Mar 2022 08:40:59 GMT  
		Size: 1.5 KB (1545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; ppc64le

```console
$ docker pull yourls@sha256:d0758e8de4626c2c03d47731b0b1f8f56eae8d89827487bf98e0117f237e8eeb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **32.1 MB (32101576 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1aa2751b1fbdc89f808f03ad64d062fdeb332939703c59c0313c995c20038d17`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 06:02:56 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 06:03:14 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 06:03:32 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 06:03:37 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 06:03:54 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 06:03:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 06:03:57 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 06:04:00 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 06:28:05 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 18 Feb 2022 21:42:56 GMT
ENV PHP_VERSION=8.0.16
# Fri, 18 Feb 2022 21:43:04 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.16.tar.xz.asc
# Fri, 18 Feb 2022 21:43:08 GMT
ENV PHP_SHA256=f27a2f25259e8c51e42dfd74e24a546ee521438ad7d9f6c6e794aa91f38bab0a
# Fri, 18 Feb 2022 21:44:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 18 Feb 2022 21:44:18 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 02 Mar 2022 22:37:01 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 02 Mar 2022 22:37:05 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Wed, 02 Mar 2022 22:37:16 GMT
RUN docker-php-ext-enable sodium
# Wed, 02 Mar 2022 22:37:21 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 02 Mar 2022 22:37:32 GMT
WORKDIR /var/www/html
# Wed, 02 Mar 2022 22:37:44 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 02 Mar 2022 22:37:51 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Mar 2022 22:37:58 GMT
EXPOSE 9000
# Wed, 02 Mar 2022 22:38:02 GMT
CMD ["php-fpm"]
# Thu, 03 Mar 2022 16:24:11 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 03 Mar 2022 16:24:14 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 03 Mar 2022 16:24:16 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 03 Mar 2022 16:24:19 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 03 Mar 2022 16:24:21 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 03 Mar 2022 16:24:25 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 03 Mar 2022 16:24:27 GMT
LABEL org.opencontainers.image.version=1.8.2
# Thu, 03 Mar 2022 16:25:34 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 03 Mar 2022 16:25:41 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 03 Mar 2022 16:25:47 GMT
RUN apk add --no-cache bash
# Thu, 03 Mar 2022 16:25:54 GMT
RUN set -eux;     version="1.8.2";     sha256="6d818622e3ba1d5785c2dbcc088be6890f5675fd4f24a2e3111eda4523bbd7ae";     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${version}.tar.gz";     echo "$sha256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${version}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 03 Mar 2022 16:25:56 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 03 Mar 2022 16:25:59 GMT
COPY file:6b25ad92f8d7ceda57a7891b5b9f6f74a178e41b54c0d1e9644ce8ca0debdaab in /usr/local/bin/ 
# Thu, 03 Mar 2022 16:26:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 16:26:02 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:603762061fb50079a4b6eb13347fd9a84cc1456d628cf781c89924a54bc419c1`  
		Last Modified: Tue, 30 Nov 2021 07:26:39 GMT  
		Size: 1.8 MB (1756276 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:645c08440cfaddc2735de2e28697acff0bc71db4cc7242494a44f92c94134e32`  
		Last Modified: Tue, 30 Nov 2021 07:26:39 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5de97a9a329d566f48c2edce253e4ccda6f021041e92326728b7499d13c823b`  
		Last Modified: Tue, 30 Nov 2021 07:26:39 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7084d629526211191f64af7f7ab019667d864049a786526c9bc40b36b960c7b`  
		Last Modified: Fri, 18 Feb 2022 22:34:26 GMT  
		Size: 10.9 MB (10883957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20e14491623599fe328d9e7a88461d7364be950384eaba733fe8264eb4fe057`  
		Last Modified: Fri, 18 Feb 2022 22:34:24 GMT  
		Size: 501.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f2229e2c67eb0c4a6feaa3348b3a767b2e2077387e5c3f991f99946cafcc783`  
		Last Modified: Thu, 03 Mar 2022 02:22:37 GMT  
		Size: 13.1 MB (13111774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df17ed1d435b3718c6e4a61b49a0aa9b491dcf68860dd36150ceb31abd649477`  
		Last Modified: Thu, 03 Mar 2022 02:22:34 GMT  
		Size: 2.3 KB (2304 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a627f90f6ba3ee8dfe0d45ddfec27dbb1b247bf753a7727ad15b6a87b0ee55e0`  
		Last Modified: Thu, 03 Mar 2022 02:22:34 GMT  
		Size: 18.2 KB (18247 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82aad80aa5c9a78040dcf21503d6fea93e79a7687ea357ea45318efdf79afa11`  
		Last Modified: Thu, 03 Mar 2022 02:22:34 GMT  
		Size: 8.6 KB (8572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7b4c21199f5154f285528c8eb37832ab8b1cc9a5a61367d0712a035c7806aae`  
		Last Modified: Thu, 03 Mar 2022 16:28:24 GMT  
		Size: 396.7 KB (396727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9ec26d00581d836aeeb6f377c6b5cc5a76b0ab85b58c5a1824ccd984204a3d7`  
		Last Modified: Thu, 03 Mar 2022 16:28:20 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515cc62c5141f047390b5a39101add344baa8416e76d9f4f4c73099c51633087`  
		Last Modified: Thu, 03 Mar 2022 16:28:21 GMT  
		Size: 528.5 KB (528460 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ed80a779799948676e647db608b258b1b4f48a3d786fa33dc1b2227883d8f86`  
		Last Modified: Thu, 03 Mar 2022 16:28:21 GMT  
		Size: 2.6 MB (2574523 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a63d62dd9a1dfd1b3acaebf1de10d494b8156b86e4c4f4c84baefb3e3cde0087`  
		Last Modified: Thu, 03 Mar 2022 16:28:20 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3a8df2e8d1661791c389421b96e11355579d04c2f45a960c48b41b4e9956f25`  
		Last Modified: Thu, 03 Mar 2022 16:28:20 GMT  
		Size: 1.5 KB (1549 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:1-fpm-alpine` - linux; s390x

```console
$ docker pull yourls@sha256:e080b10f405e2b34d36b4e7464e8d9b194cfad2530afb6f8df8ff2fd33509616
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.5 MB (30472059 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e9e048166618e58d8f6581f1396456de75261295d46e804891916c94e4c4c6d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:50:00 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev dpkg 		file 		g++ 		gcc 		libc-dev 		make 		pkgconf 		re2c
# Tue, 30 Nov 2021 04:50:01 GMT
RUN apk add --no-cache 		ca-certificates 		curl 		tar 		xz 		openssl
# Tue, 30 Nov 2021 04:50:02 GMT
RUN set -eux; 	adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 04:50:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 30 Nov 2021 04:50:03 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Tue, 30 Nov 2021 04:50:03 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 04:50:03 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 30 Nov 2021 04:50:03 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 30 Nov 2021 05:03:16 GMT
ENV GPG_KEYS=1729F83938DA44E27BA0F4D3DBDB397470D12172 BFDDD28642824F8118EF77909B67A5C12229118F
# Fri, 18 Feb 2022 20:45:30 GMT
ENV PHP_VERSION=8.0.16
# Fri, 18 Feb 2022 20:45:30 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.0.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.0.16.tar.xz.asc
# Fri, 18 Feb 2022 20:45:30 GMT
ENV PHP_SHA256=f27a2f25259e8c51e42dfd74e24a546ee521438ad7d9f6c6e794aa91f38bab0a
# Fri, 18 Feb 2022 20:46:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apk del --no-network .fetch-deps
# Fri, 18 Feb 2022 20:46:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 02 Mar 2022 20:37:33 GMT
RUN set -eux; 	apk add --no-cache --virtual .build-deps 		$PHPIZE_DEPS 		argon2-dev 		coreutils 		curl-dev 		libsodium-dev 		libxml2-dev 		linux-headers 		oniguruma-dev 		openssl-dev 		readline-dev 		sqlite-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-musl' && echo '--without-pcre-jit') 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-cache $runDeps; 		apk del --no-network .build-deps; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 02 Mar 2022 20:37:33 GMT
COPY multi:7d7d4b016ee2e2e18720a1a58004eb4d59de798c619f217398cc1066a656bfd0 in /usr/local/bin/ 
# Wed, 02 Mar 2022 20:37:34 GMT
RUN docker-php-ext-enable sodium
# Wed, 02 Mar 2022 20:37:34 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 02 Mar 2022 20:37:34 GMT
WORKDIR /var/www/html
# Wed, 02 Mar 2022 20:37:35 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Wed, 02 Mar 2022 20:37:35 GMT
STOPSIGNAL SIGQUIT
# Wed, 02 Mar 2022 20:37:35 GMT
EXPOSE 9000
# Wed, 02 Mar 2022 20:37:35 GMT
CMD ["php-fpm"]
# Thu, 03 Mar 2022 00:05:33 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 03 Mar 2022 00:05:34 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 03 Mar 2022 00:05:34 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 03 Mar 2022 00:05:34 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 03 Mar 2022 00:05:34 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 03 Mar 2022 00:05:34 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 03 Mar 2022 00:05:34 GMT
LABEL org.opencontainers.image.version=1.8.2
# Thu, 03 Mar 2022 00:05:56 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 03 Mar 2022 00:05:57 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 03 Mar 2022 00:05:58 GMT
RUN apk add --no-cache bash
# Thu, 03 Mar 2022 00:05:59 GMT
RUN set -eux;     version="1.8.2";     sha256="6d818622e3ba1d5785c2dbcc088be6890f5675fd4f24a2e3111eda4523bbd7ae";     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${version}.tar.gz";     echo "$sha256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${version}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 03 Mar 2022 00:05:59 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 03 Mar 2022 00:06:00 GMT
COPY file:6b25ad92f8d7ceda57a7891b5b9f6f74a178e41b54c0d1e9644ce8ca0debdaab in /usr/local/bin/ 
# Thu, 03 Mar 2022 00:06:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 03 Mar 2022 00:06:00 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:079fbafa3afc04920b17b503e5d173a44e68fa743eddc7a0eca5e81c7572b8a2`  
		Last Modified: Tue, 30 Nov 2021 08:33:50 GMT  
		Size: 1.8 MB (1771410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00ea1ee8ecbda317521ca15da3d8e45a369d74d9b70a0070ebd705cb9aaf88a2`  
		Last Modified: Tue, 30 Nov 2021 08:33:49 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abad577e66a4ab93646ed4a4aefb0579d577932add0d28121e5aece37cfc08dd`  
		Last Modified: Tue, 30 Nov 2021 08:33:49 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d3fce4a4f237b5c73fb33428eac72a71d234d7be2d93203a050474ff140fa39`  
		Last Modified: Fri, 18 Feb 2022 21:17:52 GMT  
		Size: 10.9 MB (10883973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:596272ae80cea3c9fef6ddbb14d319673fbd75199b5c661f208a59815d28f395`  
		Last Modified: Fri, 18 Feb 2022 21:17:51 GMT  
		Size: 499.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17dec9010ffbd43619e399522b5b1e74b435a85fde95d3dc574d6cf870a6f714`  
		Last Modified: Wed, 02 Mar 2022 22:01:37 GMT  
		Size: 11.8 MB (11765430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d171e16a8d454757eca06a60fb6d0eef9be52884980e1a8784c1499e29547d3`  
		Last Modified: Wed, 02 Mar 2022 22:01:36 GMT  
		Size: 2.3 KB (2303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45cae7ca4603cb1d0a1bea6e7f79a10d12725fe14c7047682e6b22e3ee0eebe3`  
		Last Modified: Wed, 02 Mar 2022 22:01:36 GMT  
		Size: 18.3 KB (18277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c33c27e69f369f6ba9576fae749e9d9965a6e3920f4320f8d16ce2a1838d8f6`  
		Last Modified: Wed, 02 Mar 2022 22:01:36 GMT  
		Size: 8.6 KB (8571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de6761a0530f0f8c37568f5c11512d3bd0f42ca54dc9e33f9dd4c25303b14940`  
		Last Modified: Thu, 03 Mar 2022 00:07:16 GMT  
		Size: 352.4 KB (352407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dab83d61d3f63349aea302682c83452e24c2c997aece6030675c685d8337cb62`  
		Last Modified: Thu, 03 Mar 2022 00:07:15 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58d2dc9ff3e43767bf91cdd0ca5f85ab8f7e4603dabe3ccb08445d7f0ed715e`  
		Last Modified: Thu, 03 Mar 2022 00:07:15 GMT  
		Size: 483.3 KB (483283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa7bf9d5a624a51a9ecd7246b02a9b97f9ee9862cee4263f5bb49985af89a02a`  
		Last Modified: Thu, 03 Mar 2022 00:07:15 GMT  
		Size: 2.6 MB (2574520 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208bb297fc842244f84f6e04e6fa20134c72fdccb28db4e96f9bf5dedabc4791`  
		Last Modified: Thu, 03 Mar 2022 00:07:15 GMT  
		Size: 2.0 KB (2043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7ee3fce46916bc7e91b3a8bbab709458a50fa72e994a58740b9eebbf61cc1e`  
		Last Modified: Thu, 03 Mar 2022 00:07:15 GMT  
		Size: 1.5 KB (1544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
