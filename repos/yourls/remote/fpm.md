## `yourls:fpm`

```console
$ docker pull yourls@sha256:14172d7ba4300851dbc61b9ac99f26cf982fee4db332915a419d932fc0eed03d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `yourls:fpm` - linux; amd64

```console
$ docker pull yourls@sha256:88247f46354b377dd0db80467a61d1ce319471013f5c956b5ed4c9607a23e413
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.8 MB (165797902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57ed56fc10bc7248ea9521d7adc942edfdc0db2e415c67ec8b8ce3af61741788`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 09 Feb 2023 03:20:20 GMT
ADD file:3ea7c69e4bfac2ebb6f86baaedab31827c86a594dba8080a49928e211ad3c7a0 in / 
# Thu, 09 Feb 2023 03:20:20 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 07:35:42 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 07:35:42 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 07:36:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 07:36:01 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 07:36:02 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 07:36:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 07:36:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 07:36:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 08:03:16 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 14 Feb 2023 21:10:06 GMT
ENV PHP_VERSION=8.1.16
# Tue, 14 Feb 2023 21:10:06 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Thu, 16 Feb 2023 00:47:06 GMT
ENV PHP_SHA256=d61f13d96a58b93c39672b58f25e1ee4ce88500f4acb1430cb01a514875c1258
# Thu, 16 Feb 2023 00:47:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Feb 2023 00:47:20 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Feb 2023 00:56:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Feb 2023 00:56:49 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 16 Feb 2023 00:56:50 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Feb 2023 00:56:50 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Feb 2023 00:56:50 GMT
WORKDIR /var/www/html
# Thu, 16 Feb 2023 00:56:50 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 16 Feb 2023 00:56:51 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Feb 2023 00:56:51 GMT
EXPOSE 9000
# Thu, 16 Feb 2023 00:56:51 GMT
CMD ["php-fpm"]
# Thu, 16 Feb 2023 03:20:24 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 16 Feb 2023 03:20:24 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 16 Feb 2023 03:20:24 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 16 Feb 2023 03:20:24 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 16 Feb 2023 03:20:24 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 16 Feb 2023 03:20:24 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 16 Feb 2023 03:20:24 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 16 Feb 2023 03:20:24 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Thu, 16 Feb 2023 03:21:03 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 16 Feb 2023 03:21:04 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 16 Feb 2023 03:21:04 GMT
ARG YOURLS_VERSION=1.9.1
# Thu, 16 Feb 2023 03:21:04 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 16 Feb 2023 03:21:04 GMT
LABEL org.opencontainers.image.version=1.9.1
# Thu, 16 Feb 2023 03:21:04 GMT
ENV YOURLS_VERSION=1.9.1
# Thu, 16 Feb 2023 03:21:04 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 16 Feb 2023 03:21:06 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 16 Feb 2023 03:21:06 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 16 Feb 2023 03:21:07 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 16 Feb 2023 03:21:07 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Feb 2023 03:21:07 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:bb263680fed18eecdc67f885094df6f589bafc19004839d7fdf141df236a61aa`  
		Last Modified: Thu, 09 Feb 2023 03:25:13 GMT  
		Size: 31.4 MB (31411810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0825793cba86d855da45c20858c3c3bd7121ac697fb1741bc38a779e261ab82e`  
		Last Modified: Thu, 09 Feb 2023 08:57:35 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de3c011d207b2fa9b335817876040ab36845c702e712599e055c5613c0e23154`  
		Last Modified: Thu, 09 Feb 2023 08:57:49 GMT  
		Size: 91.6 MB (91636221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e3c5bd9650e8a316cedc37895a14fb3c7555d183f74eabe3888ff504558f8c5`  
		Last Modified: Thu, 09 Feb 2023 08:57:35 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef09b4a598662f2c2fec41c7cb5ea17adf8d3277938c961b601001234a0f2194`  
		Last Modified: Thu, 16 Feb 2023 01:40:54 GMT  
		Size: 12.1 MB (12079268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39f8d9841f7805bb7a758412963c279212e26bec852abd33bb4862e44365f873`  
		Last Modified: Thu, 16 Feb 2023 01:40:53 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31c247a24222ca3ae6330b1460a1994dfce51532a0fbfd52e63c88c66118232b`  
		Last Modified: Thu, 16 Feb 2023 01:41:41 GMT  
		Size: 26.2 MB (26235370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0853d8028071fd6b1b43544e7fc2d56b250315be5aba41bde7291a2863ddc85f`  
		Last Modified: Thu, 16 Feb 2023 01:41:37 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05616b37f67cfbd971f6f46a8b51a3a4520277bc6832ba0aa1125a01d089e15e`  
		Last Modified: Thu, 16 Feb 2023 01:41:37 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:023b847a8b91f17bd0e8028a14eff661d87f3abefffcf8afa0bf12e7cd3c9b37`  
		Last Modified: Thu, 16 Feb 2023 01:41:37 GMT  
		Size: 8.8 KB (8849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94abff182c646ff878ec3b7c8c2892cb8ab6975da30341f46eb5f3cb67f42df4`  
		Last Modified: Thu, 16 Feb 2023 03:22:57 GMT  
		Size: 515.2 KB (515230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe5d89690dbb1ef0042a89a70eff8d7dbc8425ba0865a15f6f26960459284e2a`  
		Last Modified: Thu, 16 Feb 2023 03:22:56 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e958ccef087f5c3b43300cacd4f153210dfc600ea9390f97f5ffc1331d359995`  
		Last Modified: Thu, 16 Feb 2023 03:22:57 GMT  
		Size: 3.9 MB (3903531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a6227218e6faaafc56866483d3b9114456451b2e1a5ae6f524a0dd90a1f39c06`  
		Last Modified: Thu, 16 Feb 2023 03:22:56 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:076a80d9f2ba866fbea193b578371425fedb3fef09eeda29d992725708ec15e8`  
		Last Modified: Thu, 16 Feb 2023 03:22:56 GMT  
		Size: 1.6 KB (1559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; arm variant v5

```console
$ docker pull yourls@sha256:f614527bc1abb9d2c5adb2e23eac769f721db311b797bf29952ff0eb5d4010b7
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.6 MB (143572319 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edd5e8099479f396e9be562042992e099aebdb6010c32a7d73ced5e76e00deac`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 01 Mar 2023 01:48:54 GMT
ADD file:b4fb1081f6eb8a0560d56d5781bbcedaac1453615d56e0943245dca784785ea2 in / 
# Wed, 01 Mar 2023 01:48:54 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 07:25:30 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 01 Mar 2023 07:25:30 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 01 Mar 2023 07:25:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 07:25:51 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Mar 2023 07:25:51 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Mar 2023 07:25:51 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 07:25:51 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 07:25:51 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Mar 2023 07:38:07 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 01 Mar 2023 07:38:07 GMT
ENV PHP_VERSION=8.1.16
# Wed, 01 Mar 2023 07:38:07 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Wed, 01 Mar 2023 07:38:07 GMT
ENV PHP_SHA256=d61f13d96a58b93c39672b58f25e1ee4ce88500f4acb1430cb01a514875c1258
# Wed, 01 Mar 2023 07:38:22 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 01 Mar 2023 07:38:22 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Mar 2023 07:46:26 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Mar 2023 07:46:27 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 01 Mar 2023 07:46:27 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Mar 2023 07:46:27 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Mar 2023 07:46:27 GMT
WORKDIR /var/www/html
# Wed, 01 Mar 2023 07:46:28 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 01 Mar 2023 07:46:28 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Mar 2023 07:46:28 GMT
EXPOSE 9000
# Wed, 01 Mar 2023 07:46:28 GMT
CMD ["php-fpm"]
# Wed, 01 Mar 2023 14:14:44 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 01 Mar 2023 14:14:44 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 01 Mar 2023 14:14:44 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 01 Mar 2023 14:14:44 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 01 Mar 2023 14:14:44 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 01 Mar 2023 14:14:45 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 01 Mar 2023 14:14:45 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 01 Mar 2023 14:14:45 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 01 Mar 2023 14:15:00 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 01 Mar 2023 14:15:01 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 01 Mar 2023 14:15:01 GMT
ARG YOURLS_VERSION=1.9.1
# Wed, 01 Mar 2023 14:15:01 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Wed, 01 Mar 2023 14:15:01 GMT
LABEL org.opencontainers.image.version=1.9.1
# Wed, 01 Mar 2023 14:15:01 GMT
ENV YOURLS_VERSION=1.9.1
# Wed, 01 Mar 2023 14:15:01 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Wed, 01 Mar 2023 14:15:03 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 01 Mar 2023 14:15:03 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 01 Mar 2023 14:15:03 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 01 Mar 2023 14:15:03 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 14:15:04 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3c3af56dbec5913ef8aec0f1ca7112eb5914b4ad346ccd48f836dd7ec0621ba5`  
		Last Modified: Wed, 01 Mar 2023 01:52:57 GMT  
		Size: 28.9 MB (28915776 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1044c4575d4778015b215cd7a0b8db635e1f2e17e4ba34b5f9080212fac9134`  
		Last Modified: Wed, 01 Mar 2023 08:04:31 GMT  
		Size: 229.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06bd7621ae8bab5f68149ef7bcec1c34c0efda6f0fb358786d675a2ac37bd916`  
		Last Modified: Wed, 01 Mar 2023 08:04:44 GMT  
		Size: 73.7 MB (73685661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9538a1bda8fb2c8a8a1108568a117227fe284f6d24dd97a49deced6de3997b6a`  
		Last Modified: Wed, 01 Mar 2023 08:04:31 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19942f97dea89e8100a3d00639eb18cba6344386bf1ed39d167f3554fa2d21e0`  
		Last Modified: Wed, 01 Mar 2023 08:07:22 GMT  
		Size: 12.1 MB (12077618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de91e32bc892a4c7987da8c22abea80a286987d79c206bb9cb76240d77078dd9`  
		Last Modified: Wed, 01 Mar 2023 08:07:21 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c176f89950b4b70e2175332c9d19c71399141457d0fdb0c0c99c8dd3bc1d8542`  
		Last Modified: Wed, 01 Mar 2023 08:08:19 GMT  
		Size: 24.8 MB (24822504 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f0ee5b5b99f2d2d67c4f1ee72b29da20dd4ea511a993c01b271195c1c312c8`  
		Last Modified: Wed, 01 Mar 2023 08:08:14 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:708ef8236f73ac83227cad825642ce723940ea756994094a9eb6e418c12d6986`  
		Last Modified: Wed, 01 Mar 2023 08:08:14 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:533ca3e0015bab87b7aadfa741f90f7c3d12bd551bb90794eaf367e1132b25dd`  
		Last Modified: Wed, 01 Mar 2023 08:08:14 GMT  
		Size: 8.8 KB (8850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d18ba090ed5971f39041719e97354089567dbb46c0e38b2f66c390e3f7e59c0e`  
		Last Modified: Wed, 01 Mar 2023 14:16:16 GMT  
		Size: 150.8 KB (150763 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2ed395156d130302d0c1800079cb028e00677c5f2df8093520082e09c74c37`  
		Last Modified: Wed, 01 Mar 2023 14:16:16 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3e433e6a81562a6a6fc9cde1f1a1e79f9d6d0924a1e06ac1528fb0f6ce307530`  
		Last Modified: Wed, 01 Mar 2023 14:16:17 GMT  
		Size: 3.9 MB (3903531 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3268d95c84addc00ed955d1a72537abf068f0d7d3f036030c677e9e802d81b45`  
		Last Modified: Wed, 01 Mar 2023 14:16:16 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e81b8520cfc5a701336b9c1b5cf4ce4c22f3c74f79570495ab91670dcc66da`  
		Last Modified: Wed, 01 Mar 2023 14:16:16 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; arm variant v7

```console
$ docker pull yourls@sha256:6567114eb6a5dc73518484037acc881d54f4b90f3dba7791c7d6a44b931966e2
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.0 MB (136017877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad34ba90a6e94c15b1df316468b7331f20383c339afbd142ac0e92307d7b551c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 09 Feb 2023 06:12:09 GMT
ADD file:5f1a343224e8486690bd90dd1e50c8d84b3d770c51bb6829544e5cf650c0419c in / 
# Thu, 09 Feb 2023 06:12:10 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 08:47:38 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 08:47:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 08:47:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 08:47:58 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 08:47:58 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 08:47:58 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 08:47:58 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 08:47:58 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 09:15:34 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 14 Feb 2023 23:43:54 GMT
ENV PHP_VERSION=8.1.16
# Tue, 14 Feb 2023 23:43:54 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Thu, 16 Feb 2023 00:36:17 GMT
ENV PHP_SHA256=d61f13d96a58b93c39672b58f25e1ee4ce88500f4acb1430cb01a514875c1258
# Thu, 16 Feb 2023 00:36:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Feb 2023 00:36:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Feb 2023 00:44:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Feb 2023 00:44:15 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 16 Feb 2023 00:44:15 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Feb 2023 00:44:15 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Feb 2023 00:44:16 GMT
WORKDIR /var/www/html
# Thu, 16 Feb 2023 00:44:16 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 16 Feb 2023 00:44:16 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Feb 2023 00:44:16 GMT
EXPOSE 9000
# Thu, 16 Feb 2023 00:44:16 GMT
CMD ["php-fpm"]
# Thu, 16 Feb 2023 03:03:56 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 16 Feb 2023 03:03:56 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 16 Feb 2023 03:03:56 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 16 Feb 2023 03:03:56 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 16 Feb 2023 03:03:56 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 16 Feb 2023 03:03:57 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 16 Feb 2023 03:03:57 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 16 Feb 2023 03:03:57 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Thu, 16 Feb 2023 03:04:16 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 16 Feb 2023 03:04:16 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 16 Feb 2023 03:04:16 GMT
ARG YOURLS_VERSION=1.9.1
# Thu, 16 Feb 2023 03:04:17 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 16 Feb 2023 03:04:17 GMT
LABEL org.opencontainers.image.version=1.9.1
# Thu, 16 Feb 2023 03:04:17 GMT
ENV YOURLS_VERSION=1.9.1
# Thu, 16 Feb 2023 03:04:17 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 16 Feb 2023 03:04:19 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 16 Feb 2023 03:04:19 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 16 Feb 2023 03:04:19 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 16 Feb 2023 03:04:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Feb 2023 03:04:19 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:e7318f6106ad75d7d482ae9dddf4d927b0872ef3ddb6e1330aa691fc8d17279e`  
		Last Modified: Thu, 09 Feb 2023 06:19:19 GMT  
		Size: 26.6 MB (26577666 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a62799bf19ad9233ac3078e8cc582836e83b92de17042cedcf5dc1da7a98f23a`  
		Last Modified: Thu, 09 Feb 2023 10:17:28 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51d6564f926ab623011cf9b95ae4137b43cb32a02e52377138cd1ec6e9683597`  
		Last Modified: Thu, 09 Feb 2023 10:17:42 GMT  
		Size: 69.3 MB (69321683 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8102ba0459df46db99ce3cd44312aa557923b4610cc04cddec86c41075105d69`  
		Last Modified: Thu, 09 Feb 2023 10:17:28 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:685eb6f2df20fdfb4a597821b9c215d68e08611f2d699f7bfcf8c7c54aaefb31`  
		Last Modified: Thu, 16 Feb 2023 01:42:43 GMT  
		Size: 12.1 MB (12077618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac4fb3a46cf828ff25fbcb75bc0a50eb34ca956f49f1a95c6ec64349f0582f87`  
		Last Modified: Thu, 16 Feb 2023 01:42:42 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b87569b006757abf168016272a17b254906c58c897d447f167b60923d32bae9d`  
		Last Modified: Thu, 16 Feb 2023 01:43:44 GMT  
		Size: 24.0 MB (23982547 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f4bbbd7afa5b90227f6f11aacae122a6eaca485fea87a6216e5ccbbe0cbde43`  
		Last Modified: Thu, 16 Feb 2023 01:43:40 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6921d87be84beac301369790a48a6cf7879d90d7fc05039acd5d92e6345d945f`  
		Last Modified: Thu, 16 Feb 2023 01:43:40 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1544bf4b1b5231b8b8a417ba1d562cf9ccfd197dbb9ef769c2ae391b026a0bfd`  
		Last Modified: Thu, 16 Feb 2023 01:43:40 GMT  
		Size: 8.9 KB (8851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65d39a6a5a409f7c3c9b4728837eaa0cea4ce5b50b186dd0a0eda8c1049bf07a`  
		Last Modified: Thu, 16 Feb 2023 03:06:21 GMT  
		Size: 138.4 KB (138396 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce4c6209ae29e52847d3fc8523641280c947b5ea7485174d5361a3514b13f642`  
		Last Modified: Thu, 16 Feb 2023 03:06:21 GMT  
		Size: 331.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5ddae158aa5767cd9f56273fc417f4185e30d43dd3c41c635891a559e19936b`  
		Last Modified: Thu, 16 Feb 2023 03:06:22 GMT  
		Size: 3.9 MB (3903533 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1e98e01222a907d7e5fb7b024bb7e6a72df5ffc1975316e3aeedc7c8be4b4c8`  
		Last Modified: Thu, 16 Feb 2023 03:06:21 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4cf53dc79ca32b25d29dab55c81cde55ac9cadabcaf1eedb1dbcfc312d6d5a58`  
		Last Modified: Thu, 16 Feb 2023 03:06:21 GMT  
		Size: 1.6 KB (1556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:490b7e583e11248abdb1d6e4953964906d17fa13921ca91d5ba846b834c88ae1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.1 MB (160057760 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e267adcc9aa89e1ff77694d571077b64e215f89539b12035e6a16d76b8bbb5a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 09 Feb 2023 03:58:40 GMT
ADD file:3276ac85bb957360f20720da5b37498a6b5f91a017046049f8d2fd791f728a9a in / 
# Thu, 09 Feb 2023 03:58:40 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 05:27:10 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 05:27:10 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 05:27:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 05:27:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 05:27:26 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 05:27:26 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 05:27:26 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 05:27:26 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 05:52:24 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 14 Feb 2023 21:34:24 GMT
ENV PHP_VERSION=8.1.16
# Tue, 14 Feb 2023 21:34:24 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Thu, 16 Feb 2023 01:01:36 GMT
ENV PHP_SHA256=d61f13d96a58b93c39672b58f25e1ee4ce88500f4acb1430cb01a514875c1258
# Thu, 16 Feb 2023 01:01:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Feb 2023 01:01:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Feb 2023 01:10:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Feb 2023 01:10:38 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 16 Feb 2023 01:10:38 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Feb 2023 01:10:38 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Feb 2023 01:10:38 GMT
WORKDIR /var/www/html
# Thu, 16 Feb 2023 01:10:39 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 16 Feb 2023 01:10:39 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Feb 2023 01:10:39 GMT
EXPOSE 9000
# Thu, 16 Feb 2023 01:10:39 GMT
CMD ["php-fpm"]
# Thu, 16 Feb 2023 03:22:39 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 16 Feb 2023 03:22:39 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 16 Feb 2023 03:22:40 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 16 Feb 2023 03:22:40 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 16 Feb 2023 03:22:40 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 16 Feb 2023 03:22:40 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 16 Feb 2023 03:22:40 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 16 Feb 2023 03:22:40 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Thu, 16 Feb 2023 03:23:34 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 16 Feb 2023 03:23:34 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 16 Feb 2023 03:23:34 GMT
ARG YOURLS_VERSION=1.9.1
# Thu, 16 Feb 2023 03:23:35 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 16 Feb 2023 03:23:35 GMT
LABEL org.opencontainers.image.version=1.9.1
# Thu, 16 Feb 2023 03:23:35 GMT
ENV YOURLS_VERSION=1.9.1
# Thu, 16 Feb 2023 03:23:35 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 16 Feb 2023 03:23:36 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 16 Feb 2023 03:23:37 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 16 Feb 2023 03:23:37 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 16 Feb 2023 03:23:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Feb 2023 03:23:37 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:5731adb3a4abcefe78d75783ea6e5ee87c4604d0c6a4f8c00b50085e162a7f5d`  
		Last Modified: Thu, 09 Feb 2023 04:02:34 GMT  
		Size: 30.1 MB (30062509 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2bbb2734b4952adc9c052061ffab6144238949bcbf2bf5234b71bba52f01e330`  
		Last Modified: Thu, 09 Feb 2023 06:37:24 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea02c4abdd5e6e36a734a5f78a3688e52b8c01015ef8a12ea244607e82fcba02`  
		Last Modified: Thu, 09 Feb 2023 06:37:35 GMT  
		Size: 86.9 MB (86928495 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:155431a8265f1bc742a122e275f209cbf6bdd3d1cdfcd423ca23920f97e07692`  
		Last Modified: Thu, 09 Feb 2023 06:37:24 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c3211b85d1eedffe612d89b4b1922bce3ac5724142035ff167762f574ebbcf`  
		Last Modified: Thu, 16 Feb 2023 01:53:49 GMT  
		Size: 12.1 MB (12078511 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd240d6540bcdc808638d0beb4674735d27f1ada4dc9295b1bd4bdf72c69b5bb`  
		Last Modified: Thu, 16 Feb 2023 01:53:48 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2ccbe397fb6534990e4d81a503fd143bcdd4cb222dfa2acc32cee2ed0a76a57`  
		Last Modified: Thu, 16 Feb 2023 01:54:34 GMT  
		Size: 26.3 MB (26274958 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bae852e9a8ad32830879ffc8c7ead53c4ad8e2cef94fe6acda0ef0ee6463294`  
		Last Modified: Thu, 16 Feb 2023 01:54:31 GMT  
		Size: 2.5 KB (2456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aab281cce6ddc260a63da90ac0849ec8e558cf37511ae481e66f47a152b05cc`  
		Last Modified: Thu, 16 Feb 2023 01:54:31 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7be936c674b6d100696f2086a3874c124ad95572c9dfeefe5348a1cc5c9fe87c`  
		Last Modified: Thu, 16 Feb 2023 01:54:31 GMT  
		Size: 8.8 KB (8847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99acd5f0689ef1138937218d93e415bd4a55566da3ab78c74e72972bc6f0043`  
		Last Modified: Thu, 16 Feb 2023 03:25:58 GMT  
		Size: 793.3 KB (793287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805ec2ab9a01e39619d96a475fc9a1df9477bfc2d5a720027dd667db0c1ab99a`  
		Last Modified: Thu, 16 Feb 2023 03:25:58 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0393640194d372db18656a3857ff84c79fba6f0cdd4ebf41b7a38ea6e7e2c6e4`  
		Last Modified: Thu, 16 Feb 2023 03:25:59 GMT  
		Size: 3.9 MB (3903534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0527418d2b561bf229450c06df91928eb4a5b7ccf022fbb4e5dbeeebe1fa5463`  
		Last Modified: Thu, 16 Feb 2023 03:25:58 GMT  
		Size: 2.1 KB (2051 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ce39b43044d1145ac6bcf9a1f7c3dee2fe57bfdd5cdf7af015628445baf8d7f`  
		Last Modified: Thu, 16 Feb 2023 03:25:58 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; 386

```console
$ docker pull yourls@sha256:d1cebb3e41f7b4790d55fa6e02d070aadfe2f6b3cd80dbefc1f8b4ceb447dbe2
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.7 MB (167685766 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe51965f4ba013b4bd4db608ba08df64d2e5b5808919a8156dfaf7ff13ac57fd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 09 Feb 2023 05:12:53 GMT
ADD file:7740abd3129d33122ce51153c0b6c3323b9cbe9ea0e81672e16b2d7b210d24e3 in / 
# Thu, 09 Feb 2023 05:12:53 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 06:35:08 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 06:35:09 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 06:35:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 06:35:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 06:35:31 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 06:35:31 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 06:35:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 06:35:33 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 07:02:09 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 14 Feb 2023 21:29:16 GMT
ENV PHP_VERSION=8.1.16
# Tue, 14 Feb 2023 21:29:16 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Thu, 16 Feb 2023 00:43:48 GMT
ENV PHP_SHA256=d61f13d96a58b93c39672b58f25e1ee4ce88500f4acb1430cb01a514875c1258
# Thu, 16 Feb 2023 00:44:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Feb 2023 00:44:02 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Feb 2023 00:52:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Feb 2023 00:52:56 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 16 Feb 2023 00:52:56 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Feb 2023 00:52:57 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Feb 2023 00:52:58 GMT
WORKDIR /var/www/html
# Thu, 16 Feb 2023 00:52:59 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 16 Feb 2023 00:53:00 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Feb 2023 00:53:01 GMT
EXPOSE 9000
# Thu, 16 Feb 2023 00:53:02 GMT
CMD ["php-fpm"]
# Thu, 16 Feb 2023 03:55:19 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 16 Feb 2023 03:55:20 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 16 Feb 2023 03:55:21 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 16 Feb 2023 03:55:22 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 16 Feb 2023 03:55:23 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 16 Feb 2023 03:55:24 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 16 Feb 2023 03:55:25 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 16 Feb 2023 03:55:26 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Thu, 16 Feb 2023 03:56:02 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 16 Feb 2023 03:56:03 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 16 Feb 2023 03:56:04 GMT
ARG YOURLS_VERSION=1.9.1
# Thu, 16 Feb 2023 03:56:05 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 16 Feb 2023 03:56:06 GMT
LABEL org.opencontainers.image.version=1.9.1
# Thu, 16 Feb 2023 03:56:07 GMT
ENV YOURLS_VERSION=1.9.1
# Thu, 16 Feb 2023 03:56:08 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 16 Feb 2023 03:56:11 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 16 Feb 2023 03:56:12 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 16 Feb 2023 03:56:13 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 16 Feb 2023 03:56:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Feb 2023 03:56:14 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:20744f4988404b1dee2cd438157b288d16a89da472583c0f04332ed389b258f8`  
		Last Modified: Thu, 09 Feb 2023 05:18:42 GMT  
		Size: 32.4 MB (32396875 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7d813867a2f676dc535176f61e52aa3a440060fe71341c0ecca003ff22f1e52`  
		Last Modified: Thu, 09 Feb 2023 07:58:29 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15d0c09cb272ba4eef1c58df4e5b9432ea523cfe1a0ccd5b746fcbb378affe7e`  
		Last Modified: Thu, 09 Feb 2023 07:58:41 GMT  
		Size: 92.5 MB (92510382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3105d7eab02cfecefb73c028462dbe22304a988e6668a5d2cb50dd6cb7309bc`  
		Last Modified: Thu, 09 Feb 2023 07:58:28 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a22509f0014a2a232ed034dd1ac90501a6fe61ae11fc4d1a0947bdd99edc579`  
		Last Modified: Thu, 16 Feb 2023 01:40:10 GMT  
		Size: 11.9 MB (11862661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cda9d7005c6df670c843531450a1dae0f7387c5848e3f8bb0f8f2a5f51577f9`  
		Last Modified: Thu, 16 Feb 2023 01:40:08 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f831e7211d27915d99d976d5217b3ff51e967cd941776c1a2d4861f8d0f6440`  
		Last Modified: Thu, 16 Feb 2023 01:41:06 GMT  
		Size: 26.5 MB (26501068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:353ff5635a1e1c5fb33d53c42f03cbbac6a7629a74adeeb856f720e198112d09`  
		Last Modified: Thu, 16 Feb 2023 01:41:02 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72be56d113d2467470e461117a29ad7c6c3afb9c265e78b7aa14ec318e7d90c4`  
		Last Modified: Thu, 16 Feb 2023 01:41:02 GMT  
		Size: 245.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f37421675fb5841691ed4faccc2d7717d174d2f4429c22ab4c75b0a87a956429`  
		Last Modified: Thu, 16 Feb 2023 01:41:02 GMT  
		Size: 8.9 KB (8852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0e587e05b88ec29cb11563c14d51070ec3abba6bd5ab4f57cae5623d69be923`  
		Last Modified: Thu, 16 Feb 2023 03:58:41 GMT  
		Size: 494.9 KB (494920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c2aca455b44e62d88d676609a5b75f1bf698376e16b810424b6d04fa2da0942`  
		Last Modified: Thu, 16 Feb 2023 03:58:41 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:600037e0792625260500440829ba1c587643ad9d8f0b9fc1102aeb0e307346cf`  
		Last Modified: Thu, 16 Feb 2023 03:58:42 GMT  
		Size: 3.9 MB (3903427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:17719b3826811c0c8242a092170ecc2d773db46853bb190a115de93319773345`  
		Last Modified: Thu, 16 Feb 2023 03:58:41 GMT  
		Size: 2.1 KB (2054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56ee7d56b7028c886e188ba984aa98cd93a9b5ed5cd1ef037ee7cdc165503088`  
		Last Modified: Thu, 16 Feb 2023 03:58:41 GMT  
		Size: 1.6 KB (1557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; mips64le

```console
$ docker pull yourls@sha256:9208c81e5be5297f338f5662eade74c7f7b826d92789e199802d57cde10fb1a6
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.6 MB (142616999 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95a3d6f492f0ee4a46ca915331af9ca74b576909857b5d2ba409056f6bdebeb0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 09 Feb 2023 02:45:21 GMT
ADD file:68e11645a37c49c8f8f9d79ba579d0d192aaab78bb28059f07d69d56aa5ace71 in / 
# Thu, 09 Feb 2023 02:45:25 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 16:47:25 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 16:47:27 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 16:48:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 16:49:00 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 16:49:06 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 16:49:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 16:49:12 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 16:49:15 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 17:48:01 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 14 Feb 2023 23:23:39 GMT
ENV PHP_VERSION=8.1.16
# Tue, 14 Feb 2023 23:23:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Thu, 16 Feb 2023 03:30:45 GMT
ENV PHP_SHA256=d61f13d96a58b93c39672b58f25e1ee4ce88500f4acb1430cb01a514875c1258
# Thu, 16 Feb 2023 03:31:39 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Feb 2023 03:31:42 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Feb 2023 04:13:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Feb 2023 04:13:14 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 16 Feb 2023 04:13:19 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Feb 2023 04:13:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Feb 2023 04:13:26 GMT
WORKDIR /var/www/html
# Thu, 16 Feb 2023 04:13:33 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 16 Feb 2023 04:13:36 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Feb 2023 04:13:40 GMT
EXPOSE 9000
# Thu, 16 Feb 2023 04:13:43 GMT
CMD ["php-fpm"]
# Thu, 16 Feb 2023 08:55:52 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 16 Feb 2023 08:55:55 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 16 Feb 2023 08:55:58 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 16 Feb 2023 08:56:02 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 16 Feb 2023 08:56:05 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 16 Feb 2023 08:56:08 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 16 Feb 2023 08:56:11 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 16 Feb 2023 08:56:15 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Thu, 16 Feb 2023 08:57:18 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 16 Feb 2023 08:57:24 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 16 Feb 2023 08:57:27 GMT
ARG YOURLS_VERSION=1.9.1
# Thu, 16 Feb 2023 08:57:31 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 16 Feb 2023 08:57:34 GMT
LABEL org.opencontainers.image.version=1.9.1
# Thu, 16 Feb 2023 08:57:37 GMT
ENV YOURLS_VERSION=1.9.1
# Thu, 16 Feb 2023 08:57:41 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 16 Feb 2023 08:57:49 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 16 Feb 2023 08:57:52 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 16 Feb 2023 08:57:55 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 16 Feb 2023 08:57:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Feb 2023 08:58:02 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:1b5516936229d6629ab88588210eb90edc2613c94e5952fd1caf9200284f298a`  
		Last Modified: Thu, 09 Feb 2023 02:53:48 GMT  
		Size: 29.6 MB (29634449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cadf458950d68867a313d27047074490e6171bb745a965ecd2270a62a6934fe`  
		Last Modified: Thu, 09 Feb 2023 19:40:43 GMT  
		Size: 225.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b02e1e2a67f8dc04dd6155300edf3d8403e5bfd3243879a434ac158b8245e25d`  
		Last Modified: Thu, 09 Feb 2023 19:41:36 GMT  
		Size: 71.8 MB (71814207 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4fdb53a8ae5f57cf6956c9c7d61c643b363e8bf124074dc3f947417f88179a5`  
		Last Modified: Thu, 09 Feb 2023 19:40:43 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e01e5e18577d97bdaf082d47694a7089e0844bf732d4473591835c93d22db888`  
		Last Modified: Thu, 16 Feb 2023 04:28:27 GMT  
		Size: 11.9 MB (11861712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bada67665a44d7811a11eb76a02a07c73b8ae353afd4b6e77971ba44a33879`  
		Last Modified: Thu, 16 Feb 2023 04:28:24 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9598957b6882419e92441ac13109e14ee8455da585b9cc138a50d3ed68f213e4`  
		Last Modified: Thu, 16 Feb 2023 04:29:49 GMT  
		Size: 25.2 MB (25237790 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85310ed5b764f00b283254eaafc3d0d1f57fbc7d2ad67c68da18a543dbe486e1`  
		Last Modified: Thu, 16 Feb 2023 04:29:32 GMT  
		Size: 2.5 KB (2457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06e7ca74310198fd45ce37ae386192d8c70a625728f733125ad40a35840f4c49`  
		Last Modified: Thu, 16 Feb 2023 04:29:32 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbdd75004d35f74bf7526e061a2be4539053d8fc674877e39af1fd0c578dab6d`  
		Last Modified: Thu, 16 Feb 2023 04:29:32 GMT  
		Size: 8.9 KB (8854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28c8fcfcca0503a2d5f85188557ce7b02fbf6d8016c26371e34d122164a06dc5`  
		Last Modified: Thu, 16 Feb 2023 08:59:00 GMT  
		Size: 149.0 KB (148970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdc1e171ab2fd1b022dc3ea901104f65c95df8946f64e1e7e930a1763a0b9abc`  
		Last Modified: Thu, 16 Feb 2023 08:59:00 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbccc3854465f5b6716b2061d901751aaac7afc0667e9a1b0f10ebf947c75c02`  
		Last Modified: Thu, 16 Feb 2023 08:59:03 GMT  
		Size: 3.9 MB (3903427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83058df67250b0504959251584a8ad3bcdb7050fca5a7ef1401aa1ad54c49bc9`  
		Last Modified: Thu, 16 Feb 2023 08:59:00 GMT  
		Size: 2.1 KB (2055 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33183f9c824fd79da955551b9b3fc6762171734431524308661fd1f1dce373c0`  
		Last Modified: Thu, 16 Feb 2023 08:59:00 GMT  
		Size: 1.6 KB (1559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; ppc64le

```console
$ docker pull yourls@sha256:1a3a6340ab7a4361e58d79b6f197c910ea676a245d3cda81031d70416bd62877
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **165.4 MB (165368178 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a4764dce82d29ac39cb65ad9df7cc43a251ed6b81a696683f418289f8cb35f5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 09 Feb 2023 06:21:49 GMT
ADD file:b09577b8131a90731fdfb00b824a97dc65ccb51d484cb9004382035d64a5741c in / 
# Thu, 09 Feb 2023 06:21:52 GMT
CMD ["bash"]
# Thu, 09 Feb 2023 10:19:40 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 09 Feb 2023 10:19:41 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 09 Feb 2023 10:20:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 09 Feb 2023 10:20:30 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Thu, 09 Feb 2023 10:20:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Thu, 09 Feb 2023 10:20:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 10:20:33 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Thu, 09 Feb 2023 10:20:34 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Thu, 09 Feb 2023 10:39:35 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Tue, 14 Feb 2023 21:04:25 GMT
ENV PHP_VERSION=8.1.16
# Tue, 14 Feb 2023 21:04:26 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Thu, 16 Feb 2023 00:44:53 GMT
ENV PHP_SHA256=d61f13d96a58b93c39672b58f25e1ee4ce88500f4acb1430cb01a514875c1258
# Thu, 16 Feb 2023 00:45:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 16 Feb 2023 00:45:25 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 16 Feb 2023 00:58:37 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Thu, 16 Feb 2023 00:58:39 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Thu, 16 Feb 2023 00:58:41 GMT
RUN docker-php-ext-enable sodium
# Thu, 16 Feb 2023 00:58:41 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 16 Feb 2023 00:58:42 GMT
WORKDIR /var/www/html
# Thu, 16 Feb 2023 00:58:43 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Thu, 16 Feb 2023 00:58:44 GMT
STOPSIGNAL SIGQUIT
# Thu, 16 Feb 2023 00:58:45 GMT
EXPOSE 9000
# Thu, 16 Feb 2023 00:58:45 GMT
CMD ["php-fpm"]
# Thu, 16 Feb 2023 04:55:57 GMT
LABEL org.opencontainers.image.title=YOURLS
# Thu, 16 Feb 2023 04:55:58 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Thu, 16 Feb 2023 04:55:59 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Thu, 16 Feb 2023 04:56:00 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Thu, 16 Feb 2023 04:56:01 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Thu, 16 Feb 2023 04:56:03 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Thu, 16 Feb 2023 04:56:05 GMT
LABEL org.opencontainers.image.licenses=MIT
# Thu, 16 Feb 2023 04:56:06 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Thu, 16 Feb 2023 04:56:46 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Thu, 16 Feb 2023 04:56:48 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Thu, 16 Feb 2023 04:56:49 GMT
ARG YOURLS_VERSION=1.9.1
# Thu, 16 Feb 2023 04:56:49 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 16 Feb 2023 04:56:50 GMT
LABEL org.opencontainers.image.version=1.9.1
# Thu, 16 Feb 2023 04:56:50 GMT
ENV YOURLS_VERSION=1.9.1
# Thu, 16 Feb 2023 04:56:52 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Thu, 16 Feb 2023 04:56:55 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Thu, 16 Feb 2023 04:56:56 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Thu, 16 Feb 2023 04:56:56 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Thu, 16 Feb 2023 04:56:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 16 Feb 2023 04:56:57 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:4ea90e1a094ae86c7950bbec99e7a79b08fae641ad5f3bc3af9081c925894c41`  
		Last Modified: Thu, 09 Feb 2023 06:28:27 GMT  
		Size: 35.3 MB (35289252 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43232fc55c8ccbdec23837fdbabf8a55f62e81b11637630eb5c442a99b423f4c`  
		Last Modified: Thu, 09 Feb 2023 11:19:20 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:878184cd9e854f6d9186e01d93ec972e9536692520fdcf2fcaf34c63b608a9a3`  
		Last Modified: Thu, 09 Feb 2023 11:19:44 GMT  
		Size: 86.6 MB (86632950 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:939821d7ebd845237190718862054b702fa19155bf8e8a7adb0a6f6e0f5f2b05`  
		Last Modified: Thu, 09 Feb 2023 11:19:20 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd107bdedaf4d535fcec86f38df1dc4cfc0f58af61323a1dcfc036a7225c3cd`  
		Last Modified: Thu, 16 Feb 2023 01:42:15 GMT  
		Size: 12.1 MB (12079285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbcaf5e74ec9eae98358be49336c5e3b43fe5f15a475a8801d619c9a29b917b4`  
		Last Modified: Thu, 16 Feb 2023 01:42:13 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d19f80e6e0abd103c1b5dca0b8b1b639a41eacefe07ada31f2716c856594779e`  
		Last Modified: Thu, 16 Feb 2023 01:43:23 GMT  
		Size: 27.3 MB (27262844 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e018313af9f8088f6d7325fff7a583a51e2bfa5b0a0679bfea3c86419f1e8eed`  
		Last Modified: Thu, 16 Feb 2023 01:43:16 GMT  
		Size: 2.5 KB (2455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45152e15495bdf8a29ed5e1a7ae2e105153f67e61650b0852e6dcfe2ada0a820`  
		Last Modified: Thu, 16 Feb 2023 01:43:16 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d18d4d3314290d6f92d4cc010db155a68697bd87a5b63ec4f42136c3b4a16e9`  
		Last Modified: Thu, 16 Feb 2023 01:43:16 GMT  
		Size: 8.9 KB (8852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:274795f059713f8564a2a566c3a6f68c89e6f8e80280977d53a6f616ff32ed24`  
		Last Modified: Thu, 16 Feb 2023 04:59:37 GMT  
		Size: 183.8 KB (183828 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa96d14ffe2dce7c2e9ff737e01e0946e39b92f91eca44cf2bdee219c95f6b6d`  
		Last Modified: Thu, 16 Feb 2023 04:59:37 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32a7a865594fb1e7db249bcabe1ed8c332dee6424b97e34f801c44f1472a13ba`  
		Last Modified: Thu, 16 Feb 2023 04:59:38 GMT  
		Size: 3.9 MB (3903534 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0548c4e7b92b7aecacdd2ffe0b3910b73a121880f14e46c0bceffe4725b0530`  
		Last Modified: Thu, 16 Feb 2023 04:59:37 GMT  
		Size: 2.1 KB (2052 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eac304542b40ec593d637d1d6b79bbc9cbe0606f7369e82aa527e7e19d61121`  
		Last Modified: Thu, 16 Feb 2023 04:59:37 GMT  
		Size: 1.6 KB (1559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; s390x

```console
$ docker pull yourls@sha256:00d8bd7cca62f51dbb9e45bf29900318f65c51e3375d9f9e485cbafc47f55ff4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.7 MB (142722535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2b5a7df451abe1e10e16a6ae48d9978155b0e2b044c74d0b9c17cb24dd382b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 01 Mar 2023 02:50:30 GMT
ADD file:01aa3de7444f0716938e0d85522be065193be4ffb6788b3190a0f4fefdbb8d65 in / 
# Wed, 01 Mar 2023 02:50:31 GMT
CMD ["bash"]
# Wed, 01 Mar 2023 04:42:17 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 01 Mar 2023 04:42:17 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 01 Mar 2023 04:42:32 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 01 Mar 2023 04:42:36 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 01 Mar 2023 04:42:36 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 01 Mar 2023 04:42:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 04:42:37 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 01 Mar 2023 04:42:37 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Wed, 01 Mar 2023 04:52:53 GMT
ENV GPG_KEYS=528995BFEDFBA7191D46839EF9BA0ADA31CBD89E 39B641343D8C104B2B146DC3F9C39DC0B9698544 F1F692238FBC1666E5A5CCD4199F9DFEF6FFBAFD
# Wed, 01 Mar 2023 04:52:53 GMT
ENV PHP_VERSION=8.1.16
# Wed, 01 Mar 2023 04:52:53 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.1.16.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.1.16.tar.xz.asc
# Wed, 01 Mar 2023 04:52:53 GMT
ENV PHP_SHA256=d61f13d96a58b93c39672b58f25e1ee4ce88500f4acb1430cb01a514875c1258
# Wed, 01 Mar 2023 04:53:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Wed, 01 Mar 2023 04:53:01 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Wed, 01 Mar 2023 04:59:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Wed, 01 Mar 2023 04:59:48 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Wed, 01 Mar 2023 04:59:48 GMT
RUN docker-php-ext-enable sodium
# Wed, 01 Mar 2023 04:59:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Wed, 01 Mar 2023 04:59:49 GMT
WORKDIR /var/www/html
# Wed, 01 Mar 2023 04:59:49 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Wed, 01 Mar 2023 04:59:49 GMT
STOPSIGNAL SIGQUIT
# Wed, 01 Mar 2023 04:59:50 GMT
EXPOSE 9000
# Wed, 01 Mar 2023 04:59:50 GMT
CMD ["php-fpm"]
# Wed, 01 Mar 2023 15:09:18 GMT
LABEL org.opencontainers.image.title=YOURLS
# Wed, 01 Mar 2023 15:09:19 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Wed, 01 Mar 2023 15:09:19 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Wed, 01 Mar 2023 15:09:20 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Wed, 01 Mar 2023 15:09:20 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Wed, 01 Mar 2023 15:09:21 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Wed, 01 Mar 2023 15:09:21 GMT
LABEL org.opencontainers.image.licenses=MIT
# Wed, 01 Mar 2023 15:09:22 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Wed, 01 Mar 2023 15:09:41 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Wed, 01 Mar 2023 15:09:41 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Wed, 01 Mar 2023 15:09:41 GMT
ARG YOURLS_VERSION=1.9.1
# Wed, 01 Mar 2023 15:09:41 GMT
ARG YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Wed, 01 Mar 2023 15:09:41 GMT
LABEL org.opencontainers.image.version=1.9.1
# Wed, 01 Mar 2023 15:09:42 GMT
ENV YOURLS_VERSION=1.9.1
# Wed, 01 Mar 2023 15:09:42 GMT
ENV YOURLS_SHA256=0bf53290e8f86ea2e0121aac70f7c64d70d3dfb54823acb9dcc343dd7c5f455a
# Wed, 01 Mar 2023 15:09:44 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Wed, 01 Mar 2023 15:09:44 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Wed, 01 Mar 2023 15:09:44 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Wed, 01 Mar 2023 15:09:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 01 Mar 2023 15:09:44 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:7b8d78f42e32e7fa234bcf890ae6603acab2881bca68a9d8c429981c7f42b1d6`  
		Last Modified: Wed, 01 Mar 2023 02:54:48 GMT  
		Size: 29.6 MB (29646854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1a3153b8d8ab0a55b01c916b5704c35a9a92f4d5c00160bbd0f311c27819b90`  
		Last Modified: Wed, 01 Mar 2023 05:17:21 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:260f172314829288dab841521073cdf8c8817323bb202d12a8646d66cfd533fa`  
		Last Modified: Wed, 01 Mar 2023 05:17:31 GMT  
		Size: 71.6 MB (71628866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:059a6285c36a8aa48b77664be1ef8ec729d5fe9ab616e1cb55378e771e051a23`  
		Last Modified: Wed, 01 Mar 2023 05:17:21 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8995962a0f97692915ee20450493a8924b44c8c3fae449d706105f75fe002513`  
		Last Modified: Wed, 01 Mar 2023 05:19:42 GMT  
		Size: 12.1 MB (12078026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a73ac4b9544b3c112d1048ff16cc90da049131f032346ee92094c13841dcaf3`  
		Last Modified: Wed, 01 Mar 2023 05:19:41 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:743fd2f9cc4dd59dfcc8fed4768eebd76b1ed78bd8e56ef57f0272171463bf87`  
		Last Modified: Wed, 01 Mar 2023 05:20:19 GMT  
		Size: 25.3 MB (25290569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f179c0c1410b0cf967bdbd4859784869d20218e512039fb25e8b3e0379975288`  
		Last Modified: Wed, 01 Mar 2023 05:20:15 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ae1de8943cd3f88523f9cc421953039f3c90299fa8d84ac8a58ca3f6266f374`  
		Last Modified: Wed, 01 Mar 2023 05:20:15 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a12250735a7cb35ecbd7a24fac208c11964c92632460774bbbf233416ba07462`  
		Last Modified: Wed, 01 Mar 2023 05:20:15 GMT  
		Size: 8.8 KB (8847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67ad555902e0c4d4cdf5ff34ae6b1acf73afef59c557ae2eddb2144dee307477`  
		Last Modified: Wed, 01 Mar 2023 15:10:50 GMT  
		Size: 158.2 KB (158225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e77ddbcafbafb9cbd43f2eb494854c6475125cb567d6a0153477a8441981c611`  
		Last Modified: Wed, 01 Mar 2023 15:10:50 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3522f35ea19aa4e03720b930a476b62f189ca3bf3002cd62fb8a808d74b44c9`  
		Last Modified: Wed, 01 Mar 2023 15:10:50 GMT  
		Size: 3.9 MB (3903530 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:116093440867ff3e4a546f748a2f48411a3e4fe5e79aa59929b396d0138a9de8`  
		Last Modified: Wed, 01 Mar 2023 15:10:50 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65c299eef44aa6a7e3107ea9c3b2fcb9d18f8542b66b591fe52add3988f25b1b`  
		Last Modified: Wed, 01 Mar 2023 15:10:50 GMT  
		Size: 1.6 KB (1552 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
