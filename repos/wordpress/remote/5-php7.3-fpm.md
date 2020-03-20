## `wordpress:5-php7.3-fpm`

```console
$ docker pull wordpress@sha256:ed32584bae652a3fddfb2552c61e0686a83dc87f3b5fd197f7049de60bb37358
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `wordpress:5-php7.3-fpm` - linux; amd64

```console
$ docker pull wordpress@sha256:22a3b60132ec74ede2938869bf6ffc734ebcaaf6b285128c4a550d79eea29b33
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **183.6 MB (183553113 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:510d2bbf250407a015de3bfe09854a662530b499e31aae42bfb3aad32783fe5c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:39 GMT
ADD file:e5a364615e0f6961626089c7d658adbf8c8d95b3ae95a390a8bb33875317d434 in / 
# Wed, 26 Feb 2020 00:37:39 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:59:19 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Feb 2020 11:59:19 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Feb 2020 11:59:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 11:59:41 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Feb 2020 11:59:42 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Feb 2020 12:12:09 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 26 Feb 2020 12:12:09 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 12:12:09 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 12:12:09 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Wed, 26 Feb 2020 12:40:32 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 19 Mar 2020 23:35:22 GMT
ENV PHP_VERSION=7.3.16
# Thu, 19 Mar 2020 23:35:22 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.16.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.16.tar.xz.asc/from/this/mirror
# Thu, 19 Mar 2020 23:35:23 GMT
ENV PHP_SHA256=91aaee3dbdc71b69b4f3292f9d99211172a2fa926c3f3bbdb0e85dab03dd2bcb PHP_MD5=
# Thu, 19 Mar 2020 23:35:31 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Mar 2020 23:35:31 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Mar 2020 23:43:14 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 19 Mar 2020 23:43:14 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 19 Mar 2020 23:43:15 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Mar 2020 23:43:16 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 19 Mar 2020 23:43:16 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Mar 2020 23:43:16 GMT
WORKDIR /var/www/html
# Thu, 19 Mar 2020 23:43:17 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 19 Mar 2020 23:43:17 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Mar 2020 23:43:17 GMT
EXPOSE 9000
# Thu, 19 Mar 2020 23:43:18 GMT
CMD ["php-fpm"]
# Fri, 20 Mar 2020 05:47:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 05:48:42 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 05:48:42 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 20 Mar 2020 05:48:43 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 20 Mar 2020 05:48:43 GMT
VOLUME [/var/www/html]
# Fri, 20 Mar 2020 05:48:44 GMT
ENV WORDPRESS_VERSION=5.3.2
# Fri, 20 Mar 2020 05:48:44 GMT
ENV WORDPRESS_SHA1=fded476f112dbab14e3b5acddd2bcfa550e7b01b
# Fri, 20 Mar 2020 05:48:49 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 20 Mar 2020 05:48:49 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 20 Mar 2020 05:48:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 05:48:49 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:68ced04f60ab5c7a5f1d0b0b4e7572c5a4c8cce44866513d30d9df1a15277d6b`  
		Last Modified: Wed, 26 Feb 2020 00:44:23 GMT  
		Size: 27.1 MB (27091819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d2a5d8fa5852468a297ff0881d1804da6f72f49f9307031dfeff2602022170d`  
		Last Modified: Wed, 26 Feb 2020 14:14:05 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d59ec4ae241b4fb63be2a1f6852dad2846c086b03d4335ed97e812f74698b84`  
		Last Modified: Wed, 26 Feb 2020 14:14:21 GMT  
		Size: 76.7 MB (76651455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42331ef4d446806549ef08fef2deaf4f9297cb292ffab7e2c127f5f73a98bce`  
		Last Modified: Wed, 26 Feb 2020 14:14:04 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a413239948bb54da3ebd71b9155bd38014cfac4b50fc5b51fc15a8628b121759`  
		Last Modified: Fri, 20 Mar 2020 03:19:08 GMT  
		Size: 12.4 MB (12435874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e862908399b7cde5c4f53fa65f9f369f448011b903cd05c856d29847ffa104c`  
		Last Modified: Fri, 20 Mar 2020 03:19:04 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b149e595ce9bc0e0bdbb30f5eb8d97ea4bcfd1fbe1ae48487ffb81ee269b636`  
		Last Modified: Fri, 20 Mar 2020 03:19:12 GMT  
		Size: 28.8 MB (28785627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92fa4dca6f089be02c8064c9eedfb131a50369d9c34dcb82b1a142c442bfb4b9`  
		Last Modified: Fri, 20 Mar 2020 03:19:03 GMT  
		Size: 2.2 KB (2217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:075eb11836cc31caa3adbf5d96a3279fe5762ff8605b665dbc9c953031d340f8`  
		Last Modified: Fri, 20 Mar 2020 03:19:03 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8851c85bc26363917fb770dc0f750844264acc1ee4478641cfaf8267c77c6d0b`  
		Last Modified: Fri, 20 Mar 2020 03:19:03 GMT  
		Size: 209.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c67ad9c8a9df2ea38929d9dfde8ccbc798b637c544db33a3879575ea93928f28`  
		Last Modified: Fri, 20 Mar 2020 03:19:03 GMT  
		Size: 8.4 KB (8414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:972e0b6a2621f6ade94a7e06b47fa8b884858296e92d2e3a62a4b76090d736a7`  
		Last Modified: Fri, 20 Mar 2020 06:01:38 GMT  
		Size: 16.8 MB (16847021 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc2348171db9abe51fd39ed61fbed097165cd27b8e80bb4138ea849a548c2430`  
		Last Modified: Fri, 20 Mar 2020 06:01:36 GMT  
		Size: 9.5 MB (9496799 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b85d90c1c46f8e0352538704fce00de4b2b69b0e046101c8a75b6d8c638b2e4`  
		Last Modified: Fri, 20 Mar 2020 06:01:33 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffdc55b56e5a2a9983463502ad4f0d0008a13c4d1e7ea26262631b310563ceee`  
		Last Modified: Fri, 20 Mar 2020 06:01:33 GMT  
		Size: 390.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0da71207fdaadd2ce7561f81ea523cfb4a65b17494a19009ac7e42b4ced32aee`  
		Last Modified: Fri, 20 Mar 2020 06:01:37 GMT  
		Size: 12.2 MB (12227880 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cde1e16c675b08a5838918e07b3704e221f3e5da7117a669bef2e9c2dcc3c3ac`  
		Last Modified: Fri, 20 Mar 2020 06:01:33 GMT  
		Size: 3.9 KB (3890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.3-fpm` - linux; arm variant v5

```console
$ docker pull wordpress@sha256:ada4dcb2eb677199fb4f0fc1983d6048615e57ba7843924bec0d88bfe002e8aa
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.4 MB (160406889 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65488f3e6fa91edada0cf8e48ba943910b46c25a7c6aaa5aba522bbb48289bcc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 26 Feb 2020 00:47:49 GMT
ADD file:745d3236976c8213b805ca6d14f150561816cd2eeec5aa7e1aaea44d9d5675e9 in / 
# Wed, 26 Feb 2020 00:47:53 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:32:47 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Feb 2020 04:32:48 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Feb 2020 04:33:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:33:40 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Feb 2020 04:33:43 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Feb 2020 04:42:36 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 26 Feb 2020 04:42:36 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 04:42:37 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 04:42:37 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Wed, 26 Feb 2020 05:00:09 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 19 Mar 2020 22:25:21 GMT
ENV PHP_VERSION=7.3.16
# Thu, 19 Mar 2020 22:25:22 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.16.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.16.tar.xz.asc/from/this/mirror
# Thu, 19 Mar 2020 22:25:23 GMT
ENV PHP_SHA256=91aaee3dbdc71b69b4f3292f9d99211172a2fa926c3f3bbdb0e85dab03dd2bcb PHP_MD5=
# Thu, 19 Mar 2020 22:25:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Mar 2020 22:25:48 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Mar 2020 22:30:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 19 Mar 2020 22:30:10 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 19 Mar 2020 22:30:17 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Mar 2020 22:30:21 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 19 Mar 2020 22:30:23 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Mar 2020 22:30:25 GMT
WORKDIR /var/www/html
# Thu, 19 Mar 2020 22:30:30 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 19 Mar 2020 22:30:31 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Mar 2020 22:30:33 GMT
EXPOSE 9000
# Thu, 19 Mar 2020 22:30:35 GMT
CMD ["php-fpm"]
# Fri, 20 Mar 2020 03:09:52 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 03:13:28 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 03:13:32 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 20 Mar 2020 03:13:34 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 20 Mar 2020 03:13:35 GMT
VOLUME [/var/www/html]
# Fri, 20 Mar 2020 03:13:36 GMT
ENV WORDPRESS_VERSION=5.3.2
# Fri, 20 Mar 2020 03:13:37 GMT
ENV WORDPRESS_SHA1=fded476f112dbab14e3b5acddd2bcfa550e7b01b
# Fri, 20 Mar 2020 03:13:44 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 20 Mar 2020 03:13:46 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 20 Mar 2020 03:13:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 03:13:49 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:d9f9009f908455fa93c5b3e0d3230df44ea75299b2de375ab35b74193f679076`  
		Last Modified: Wed, 26 Feb 2020 00:59:18 GMT  
		Size: 24.8 MB (24830277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d924f652197b083a9a110930b7548ba9fe1fcc87e963cd10516dd54b172a9804`  
		Last Modified: Wed, 26 Feb 2020 06:04:05 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd86ee1863629868607b0a8c088897c302f5f1e23d0bd51a610f0d5aae26bdcf`  
		Last Modified: Wed, 26 Feb 2020 06:04:26 GMT  
		Size: 58.8 MB (58799831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e751ab6d9f11edd9376e6fa63465ad0c6a006fc52c130bdf4f5b8ff05ffe936`  
		Last Modified: Wed, 26 Feb 2020 06:04:04 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12a42bc2829bd41d348063711616a3097903a7a931d7f59aed12ed1c00d17abe`  
		Last Modified: Thu, 19 Mar 2020 23:42:43 GMT  
		Size: 12.4 MB (12434126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c6413571a6296e61013c663d89d8dc6591f021544c8fd51c1e80f16ed7ef076`  
		Last Modified: Thu, 19 Mar 2020 23:42:42 GMT  
		Size: 494.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ee8032b65708fad99bb5d8d59b92e9e3ee82f0b20b107a3640766842774f26f`  
		Last Modified: Thu, 19 Mar 2020 23:42:49 GMT  
		Size: 27.3 MB (27336355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9c68521003ac4d9395287572cd99cee6d7f40f4caba1ed058f40fb2bf1300e`  
		Last Modified: Thu, 19 Mar 2020 23:42:40 GMT  
		Size: 2.2 KB (2221 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1186dd27d4806ea18f29990caa86ff1c609f16a45afde43eaf93663a57208b`  
		Last Modified: Thu, 19 Mar 2020 23:42:40 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:177c32d2f0e346d6d6a0bd2934c24f3055044a76a386cf7c4c6ae5e42798a1b6`  
		Last Modified: Thu, 19 Mar 2020 23:42:40 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e507b32db93cb536ccb86067e8f69de8cb3483401c0f502b5ede432da09eed6`  
		Last Modified: Thu, 19 Mar 2020 23:42:40 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab9cda760cfeffd076f6dd3422934091b79895aeed6ae3be65ff4706bd949a9`  
		Last Modified: Fri, 20 Mar 2020 03:24:48 GMT  
		Size: 16.4 MB (16402673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f1f8d9ffd006ab8d8527f9812d73c8707e55d4e2f08f8eb8fa83c6d6187586`  
		Last Modified: Fri, 20 Mar 2020 03:24:42 GMT  
		Size: 8.4 MB (8359028 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:829df024ab2d737fe84ba6cb42c481439755a365954b02202ad002517ba60980`  
		Last Modified: Fri, 20 Mar 2020 03:24:39 GMT  
		Size: 333.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0f3d7275f2596f1d4ef9e82f062963ee88f817f26c4c2e92939e5a607ffa145`  
		Last Modified: Fri, 20 Mar 2020 03:24:39 GMT  
		Size: 399.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbbd17b58e23f2035f4b6233651bba8c9b7b72067338fb2eb66d1bc43a648bd1`  
		Last Modified: Fri, 20 Mar 2020 03:24:44 GMT  
		Size: 12.2 MB (12227882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d090a188c120f9128fb4c186b4e960a6cdbac7f73b9b340177f7966576881ba9`  
		Last Modified: Fri, 20 Mar 2020 03:24:39 GMT  
		Size: 3.9 KB (3896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.3-fpm` - linux; arm variant v7

```console
$ docker pull wordpress@sha256:3d37caa4529a9be7000b1debe0805a582eb6c4f8280921b2d87d9bf6166825f4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **156.7 MB (156695204 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d46fd49da2450d5f351d5e190eeaf68278f806991c515144c20f66addab6107d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 26 Feb 2020 00:52:11 GMT
ADD file:2488038744e2e15217e67dd7f4bec5dcc7e9abe8a1010fe720a5ba7cbe7ab0eb in / 
# Wed, 26 Feb 2020 00:52:13 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 14:27:11 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Feb 2020 14:27:11 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Feb 2020 14:27:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 14:27:57 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Feb 2020 14:28:00 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Feb 2020 14:36:00 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 26 Feb 2020 14:36:01 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 14:36:01 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 14:36:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Wed, 26 Feb 2020 14:52:03 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 19 Mar 2020 22:43:11 GMT
ENV PHP_VERSION=7.3.16
# Thu, 19 Mar 2020 22:43:12 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.16.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.16.tar.xz.asc/from/this/mirror
# Thu, 19 Mar 2020 22:43:13 GMT
ENV PHP_SHA256=91aaee3dbdc71b69b4f3292f9d99211172a2fa926c3f3bbdb0e85dab03dd2bcb PHP_MD5=
# Thu, 19 Mar 2020 22:43:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Mar 2020 22:43:33 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Mar 2020 22:47:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 19 Mar 2020 22:47:53 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 19 Mar 2020 22:47:55 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Mar 2020 22:47:58 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 19 Mar 2020 22:48:00 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Mar 2020 22:48:02 GMT
WORKDIR /var/www/html
# Thu, 19 Mar 2020 22:48:06 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 19 Mar 2020 22:48:06 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Mar 2020 22:48:07 GMT
EXPOSE 9000
# Thu, 19 Mar 2020 22:48:08 GMT
CMD ["php-fpm"]
# Fri, 20 Mar 2020 05:49:33 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 05:52:26 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 05:52:29 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 20 Mar 2020 05:52:31 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 20 Mar 2020 05:52:31 GMT
VOLUME [/var/www/html]
# Fri, 20 Mar 2020 05:52:32 GMT
ENV WORDPRESS_VERSION=5.3.2
# Fri, 20 Mar 2020 05:52:32 GMT
ENV WORDPRESS_SHA1=fded476f112dbab14e3b5acddd2bcfa550e7b01b
# Fri, 20 Mar 2020 05:52:38 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 20 Mar 2020 05:52:39 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 20 Mar 2020 05:52:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 05:52:40 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:fff3167bf8c79dc08baf67eb607823aadcbee2033f9620cc502e2c49423f605b`  
		Last Modified: Wed, 26 Feb 2020 01:07:32 GMT  
		Size: 22.7 MB (22699783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1cd5cd61b6f8de3cb9b8eaf9920ee92db196f4c73365a731f08c51fdec97be4`  
		Last Modified: Wed, 26 Feb 2020 15:55:26 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:45b7e5098979c0c6921b0ba0a8f1e1625ffe7a6f8b565feae67a7a293e74e9db`  
		Last Modified: Wed, 26 Feb 2020 15:55:46 GMT  
		Size: 59.5 MB (59501205 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd2e6e500bc14a91c0e209ad61d4cab4947d2f99c2be6908475b8c3d61189f25`  
		Last Modified: Wed, 26 Feb 2020 15:55:26 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8181450ae65b331a7bf3a8b00909f2fa83aa767dc4a55e33074ff9a60838d2`  
		Last Modified: Fri, 20 Mar 2020 00:41:06 GMT  
		Size: 12.4 MB (12434059 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295c874a0d0b661b81d0751c6caadc19c4425ec41a590fef031eba0e2a3fa12d`  
		Last Modified: Fri, 20 Mar 2020 00:41:04 GMT  
		Size: 495.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae7f6e27a0fd1b1bc4cf882f897642ceda22a75f82a4a44b3a045e6592b44eb3`  
		Last Modified: Fri, 20 Mar 2020 00:41:10 GMT  
		Size: 26.4 MB (26350398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbeab313fadaa0dc0283e249f1e39a58c5687e8617e1b97fa85e3d681e9441d1`  
		Last Modified: Fri, 20 Mar 2020 00:41:02 GMT  
		Size: 2.2 KB (2223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:987aa7c36b69324528bcf3c5339d15def053dcd733fd4ab75b7894ab00be537f`  
		Last Modified: Fri, 20 Mar 2020 00:41:02 GMT  
		Size: 249.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd2c8a8285147cffa0e7c50f48ca673614f1b7fe6431105474640757d78b0bdc`  
		Last Modified: Fri, 20 Mar 2020 00:41:02 GMT  
		Size: 211.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:971a0e22cd44af165241b9674ca9443b2f91f65a4cbca18a14cde0b8e26e2e3e`  
		Last Modified: Fri, 20 Mar 2020 00:41:02 GMT  
		Size: 8.4 KB (8418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805614002566aac18a015ab1a41f2d6be35eb6a086b7377f8c02348cfada9e1e`  
		Last Modified: Fri, 20 Mar 2020 06:12:07 GMT  
		Size: 16.0 MB (15954467 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ead602cea99dfdba6c39e27676a2c9ec88051d6a80adc065f9fa9300ea42275f`  
		Last Modified: Fri, 20 Mar 2020 06:12:03 GMT  
		Size: 7.5 MB (7510696 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01a90f73313dc559d572e0bd7253317940758c47486989c051a3efa6ee52b0e4`  
		Last Modified: Fri, 20 Mar 2020 06:11:59 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b71f31a43339332147fb9baeb344b7e348e64da5617e8a87f436e70e32b345a`  
		Last Modified: Fri, 20 Mar 2020 06:11:59 GMT  
		Size: 398.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8628e25a6dd9dc8e16771372d30cb5393958a881bc943c80b7abc3dba1e6d3d2`  
		Last Modified: Fri, 20 Mar 2020 06:12:05 GMT  
		Size: 12.2 MB (12227882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b3ba0f303a12bfd9bdd02e5ca9b7e5d7537cf9c45c07b0d987dbf58cac91f34`  
		Last Modified: Fri, 20 Mar 2020 06:12:00 GMT  
		Size: 3.9 KB (3893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.3-fpm` - linux; arm64 variant v8

```console
$ docker pull wordpress@sha256:c2d1a94fb67560ae601ce0e3c4e0e814119a191481ec7ab523d56bf699a6e7f9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **174.0 MB (174014010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44465237ba5ce949a3e06ac8485b6ad35f2295be51507b5b45b940eec9d4d8a5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:51 GMT
ADD file:a93818b0ffcb2823807811dffd78092a3e3f4981aabf48c3cb75f2fa319ac055 in / 
# Wed, 26 Feb 2020 00:46:55 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 11:55:28 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Feb 2020 11:55:29 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Feb 2020 11:56:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 11:56:05 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Feb 2020 11:56:07 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Feb 2020 12:04:52 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 26 Feb 2020 12:04:53 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 12:04:53 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 12:04:54 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Wed, 26 Feb 2020 12:21:52 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 19 Mar 2020 22:51:54 GMT
ENV PHP_VERSION=7.3.16
# Thu, 19 Mar 2020 22:51:55 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.16.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.16.tar.xz.asc/from/this/mirror
# Thu, 19 Mar 2020 22:51:56 GMT
ENV PHP_SHA256=91aaee3dbdc71b69b4f3292f9d99211172a2fa926c3f3bbdb0e85dab03dd2bcb PHP_MD5=
# Thu, 19 Mar 2020 22:52:12 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Mar 2020 22:52:13 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Mar 2020 22:57:05 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 19 Mar 2020 22:57:07 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 19 Mar 2020 22:57:10 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Mar 2020 22:57:13 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 19 Mar 2020 22:57:13 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Mar 2020 22:57:14 GMT
WORKDIR /var/www/html
# Thu, 19 Mar 2020 22:57:17 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 19 Mar 2020 22:57:18 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Mar 2020 22:57:19 GMT
EXPOSE 9000
# Thu, 19 Mar 2020 22:57:20 GMT
CMD ["php-fpm"]
# Fri, 20 Mar 2020 05:29:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 05:32:27 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 05:32:30 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 20 Mar 2020 05:32:31 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 20 Mar 2020 05:32:32 GMT
VOLUME [/var/www/html]
# Fri, 20 Mar 2020 05:32:33 GMT
ENV WORDPRESS_VERSION=5.3.2
# Fri, 20 Mar 2020 05:32:33 GMT
ENV WORDPRESS_SHA1=fded476f112dbab14e3b5acddd2bcfa550e7b01b
# Fri, 20 Mar 2020 05:32:38 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 20 Mar 2020 05:32:39 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 20 Mar 2020 05:32:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 05:32:40 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f338bc35613f66cfaad272234de7b77a91d6c5422855bf6239f2b0ff9d73f0a4`  
		Last Modified: Wed, 26 Feb 2020 00:56:15 GMT  
		Size: 25.9 MB (25851563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abe4ded10aa84b08ce645b2a064c692746e119bd7bdbeb50d004635ceec99237`  
		Last Modified: Wed, 26 Feb 2020 13:27:03 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90a0cd710bad4e7ac9d5be343f0970fef306eeb91d1a80f7ad1849724764c4bc`  
		Last Modified: Wed, 26 Feb 2020 13:27:20 GMT  
		Size: 70.3 MB (70334994 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4988beed3268a0092cad73bf3915a3dd39e2d730a4d549bb9c333b6bcc9cba6`  
		Last Modified: Wed, 26 Feb 2020 13:27:02 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24d0dadddb46676dc2285c3a7c649629b7df3f00b175e89848f46911192a4814`  
		Last Modified: Fri, 20 Mar 2020 00:53:29 GMT  
		Size: 12.4 MB (12434809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c72ebd7d85dac84b415f665a69be849faf71b1bf98013290e53ae4865d09da9`  
		Last Modified: Fri, 20 Mar 2020 00:53:27 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a791e10c299c4e354141bd316b7ce6b3b9199dc7c5b5a02cf501acecaa09fbc`  
		Last Modified: Fri, 20 Mar 2020 00:53:30 GMT  
		Size: 28.5 MB (28458262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c60b7d867cbebc16f8478b23f29e1fc64dff2cabc1b7353797a4563dac216d`  
		Last Modified: Fri, 20 Mar 2020 00:53:21 GMT  
		Size: 2.2 KB (2224 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4b7dda2eafc70fc4810d1254b58cde419676fd14890bb95ab0600667a360144`  
		Last Modified: Fri, 20 Mar 2020 00:53:21 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbc4b64f0977db50a346034b6d0bf5bb787cb7410c77a4f14762bc164096bc2d`  
		Last Modified: Fri, 20 Mar 2020 00:53:22 GMT  
		Size: 214.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4bd82d0223a84f5974f840b9db5dcdd91ce222387a1dfdda64d62a8cfeecebe`  
		Last Modified: Fri, 20 Mar 2020 00:53:21 GMT  
		Size: 8.4 KB (8417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a937ca223b12bd578d25171185fa079478215f8d89073a813220238d49ae9c5`  
		Last Modified: Fri, 20 Mar 2020 05:53:30 GMT  
		Size: 16.8 MB (16778068 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bb5cb00661f2ebdd2a9b408b5849a6960fdb132154d6d2ea5825a34bffe6f1f`  
		Last Modified: Fri, 20 Mar 2020 05:53:26 GMT  
		Size: 7.9 MB (7911727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00b8febe129b6d20933f1ef890c962f962b49ae15c667fb75de5929815f72fc2`  
		Last Modified: Fri, 20 Mar 2020 05:53:23 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bd4bc0fd7ccbf54b47f7ff3450ea9535e9302449f07e71f95e8d1e91a84e96e`  
		Last Modified: Fri, 20 Mar 2020 05:53:23 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:267bd1ab2a3db48e8beb05426593be1ccd9f40f7cd61f971f33173cc651a0076`  
		Last Modified: Fri, 20 Mar 2020 05:53:28 GMT  
		Size: 12.2 MB (12227877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ffd5ab9b6e4344c2ce7819e62cfe3d530570ba7bc767b67010ddd53a2e8efda6`  
		Last Modified: Fri, 20 Mar 2020 05:53:23 GMT  
		Size: 3.9 KB (3894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.3-fpm` - linux; 386

```console
$ docker pull wordpress@sha256:8e2a80c166bbfcdf42bde4e46a366b4d9375e5dfe7e329a224ae59a10da1e568
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.9 MB (188920151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38920c20b8d8230077a0de619d62dadd372067c4110f208d3dee523419a05142`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 26 Feb 2020 00:32:17 GMT
ADD file:08977fa54555a1ed2ae44a3aec04df157092a6c1c1b70ce0407cc2dc2f8bcd76 in / 
# Wed, 26 Feb 2020 00:32:17 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 17:09:58 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Feb 2020 17:09:59 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Feb 2020 17:10:23 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 17:10:24 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Feb 2020 17:10:25 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Feb 2020 17:22:01 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 26 Feb 2020 17:22:02 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 17:22:02 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 17:22:02 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Wed, 26 Feb 2020 17:47:51 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 19 Mar 2020 23:42:42 GMT
ENV PHP_VERSION=7.3.16
# Thu, 19 Mar 2020 23:42:42 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.16.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.16.tar.xz.asc/from/this/mirror
# Thu, 19 Mar 2020 23:42:42 GMT
ENV PHP_SHA256=91aaee3dbdc71b69b4f3292f9d99211172a2fa926c3f3bbdb0e85dab03dd2bcb PHP_MD5=
# Thu, 19 Mar 2020 23:42:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Mar 2020 23:42:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Mar 2020 23:51:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 19 Mar 2020 23:51:54 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 19 Mar 2020 23:51:55 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Mar 2020 23:51:56 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 19 Mar 2020 23:51:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Mar 2020 23:51:56 GMT
WORKDIR /var/www/html
# Thu, 19 Mar 2020 23:51:57 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 19 Mar 2020 23:51:57 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Mar 2020 23:51:58 GMT
EXPOSE 9000
# Thu, 19 Mar 2020 23:51:58 GMT
CMD ["php-fpm"]
# Fri, 20 Mar 2020 05:58:00 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 05:59:52 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 05:59:53 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 20 Mar 2020 05:59:53 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 20 Mar 2020 05:59:54 GMT
VOLUME [/var/www/html]
# Fri, 20 Mar 2020 05:59:54 GMT
ENV WORDPRESS_VERSION=5.3.2
# Fri, 20 Mar 2020 05:59:54 GMT
ENV WORDPRESS_SHA1=fded476f112dbab14e3b5acddd2bcfa550e7b01b
# Fri, 20 Mar 2020 06:00:07 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 20 Mar 2020 06:00:08 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 20 Mar 2020 06:00:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 06:00:08 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:1de10f1ae2a5bfd5f34f19421ebd282580e443321e4947cdf5f943875782b018`  
		Last Modified: Wed, 26 Feb 2020 00:38:34 GMT  
		Size: 27.7 MB (27747667 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b63da883d1acf485a7b1cc92daec610b51a3619bad1c74646d2349d702e66678`  
		Last Modified: Wed, 26 Feb 2020 19:26:48 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6194ab862f4a0b8d6069fe53227b0a99ede3c9572bdd3a7a53f1c345933b00e`  
		Last Modified: Wed, 26 Feb 2020 19:27:12 GMT  
		Size: 81.2 MB (81198469 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a3174e482c145c56e48af068bfededb0f4176a4d233274aba6343c48fb2a056`  
		Last Modified: Wed, 26 Feb 2020 19:26:48 GMT  
		Size: 222.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:997f07203c21343523f595aa176671b1ac97e5fba21b72e33a143621092b1e5c`  
		Last Modified: Fri, 20 Mar 2020 03:39:28 GMT  
		Size: 12.4 MB (12435190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e30e577c2f628346978878733189ffd52b5075e4efbf0d59d2ebe52b58160f`  
		Last Modified: Fri, 20 Mar 2020 03:39:21 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0676d72c54b8fa45cff2bc811b0e40793af51179a297b23fbd969fe03f5718b3`  
		Last Modified: Fri, 20 Mar 2020 03:39:29 GMT  
		Size: 29.4 MB (29355668 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4efe655f684bfda45ce1b1e25fb0ccc643e53303fa4061d39cafdac8e1107fb`  
		Last Modified: Fri, 20 Mar 2020 03:39:20 GMT  
		Size: 2.2 KB (2222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82c3b73a62e6cacf97b9c5bbe278453283156f40b599e79b10697ae287be6ed7`  
		Last Modified: Fri, 20 Mar 2020 03:39:20 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ea95acceaaf630be591878dedbb2cbbfd20f3677c334e87b463378059f3a357`  
		Last Modified: Fri, 20 Mar 2020 03:39:20 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b099014466c34177b87fec8e2c51cb347afa02dfc065d72b78a243f719f880cd`  
		Last Modified: Fri, 20 Mar 2020 03:39:20 GMT  
		Size: 8.4 KB (8415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f939db2594fbc01107bad1eec781c61c025674c984808c166b91903fcd3162d`  
		Last Modified: Fri, 20 Mar 2020 06:13:19 GMT  
		Size: 17.2 MB (17162842 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f33fe7459567c46c0d82be45e1ddd5357a210177729d7efa0d249778cf58290f`  
		Last Modified: Fri, 20 Mar 2020 06:13:15 GMT  
		Size: 8.8 MB (8775794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2757fdeb62c52df35015d891b4ac561adce887376030a358c8bbe8cc3bb8bc2c`  
		Last Modified: Fri, 20 Mar 2020 06:13:11 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:15ec0f34f4c87567bbeb177794444e4a23a439475463e66d942a2d2bb0f02400`  
		Last Modified: Fri, 20 Mar 2020 06:13:11 GMT  
		Size: 392.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1baf7364ca76c9218c763653485e5d245a057d9e11add432d26e00a0e6e616f2`  
		Last Modified: Fri, 20 Mar 2020 06:13:18 GMT  
		Size: 12.2 MB (12227874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d14ce2bf5534613d573c0ebff15b170dc39846a8365f34a6bcbae711be1388f3`  
		Last Modified: Fri, 20 Mar 2020 06:13:11 GMT  
		Size: 3.9 KB (3888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `wordpress:5-php7.3-fpm` - linux; ppc64le

```console
$ docker pull wordpress@sha256:99d8ac8b977c26dfefab5e89805a95b35af9bbb40bff4b659ffd07e005993e9a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.9 MB (194938217 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:19446a2507e0fbe3cbe9cde32f14bf68a3b43d5e0d5a8418c0cf833f8dbe5239`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Wed, 26 Feb 2020 01:31:23 GMT
ADD file:430f1f769b86c60db1b8d2f96ed26c24837b3ff5730264be42a9c0cd8e43df7f in / 
# Wed, 26 Feb 2020 01:31:29 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 13:39:22 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Wed, 26 Feb 2020 13:39:24 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Wed, 26 Feb 2020 13:40:56 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 13:41:04 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Wed, 26 Feb 2020 13:41:09 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 777 /var/www/html
# Wed, 26 Feb 2020 13:53:31 GMT
ENV PHP_EXTRA_CONFIGURE_ARGS=--enable-fpm --with-fpm-user=www-data --with-fpm-group=www-data --disable-cgi
# Wed, 26 Feb 2020 13:53:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 13:53:37 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Wed, 26 Feb 2020 13:53:39 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -Wl,--hash-style=both -pie
# Wed, 26 Feb 2020 14:18:56 GMT
ENV GPG_KEYS=CBAF69F173A0FEA4B537F470D66C9593118BCCB6 F38252826ACD957EF380D39F2F7956BC5DA04B5D
# Thu, 19 Mar 2020 23:04:11 GMT
ENV PHP_VERSION=7.3.16
# Thu, 19 Mar 2020 23:04:13 GMT
ENV PHP_URL=https://www.php.net/get/php-7.3.16.tar.xz/from/this/mirror PHP_ASC_URL=https://www.php.net/get/php-7.3.16.tar.xz.asc/from/this/mirror
# Thu, 19 Mar 2020 23:04:18 GMT
ENV PHP_SHA256=91aaee3dbdc71b69b4f3292f9d99211172a2fa926c3f3bbdb0e85dab03dd2bcb PHP_MD5=
# Thu, 19 Mar 2020 23:05:27 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 	if [ -n "$PHP_MD5" ]; then 		echo "$PHP_MD5 *php.tar.xz" | md5sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Thu, 19 Mar 2020 23:05:30 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Thu, 19 Mar 2020 23:09:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libedit-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 		${PHP_EXTRA_BUILD_DEPS:-} 	; 	rm -rf /var/lib/apt/lists/*; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-libedit 		--with-openssl 		--with-zlib 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				${PHP_EXTRA_CONFIGURE_ARGS:-} 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find /usr/local/bin /usr/local/sbin -type f -executable -exec strip --strip-all '{}' + || true; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 	php --version
# Thu, 19 Mar 2020 23:09:54 GMT
COPY multi:5581a34bba21fbf2472e857e8cdc8db6d57694020e568954d2fd5901ee074da0 in /usr/local/bin/ 
# Thu, 19 Mar 2020 23:10:02 GMT
RUN docker-php-ext-enable sodium
# Thu, 19 Mar 2020 23:10:14 GMT
RUN { echo '#!/bin/sh'; echo 'exec pkg-config "$@" freetype2'; } > /usr/local/bin/freetype-config && chmod +x /usr/local/bin/freetype-config
# Thu, 19 Mar 2020 23:10:18 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Thu, 19 Mar 2020 23:10:21 GMT
WORKDIR /var/www/html
# Thu, 19 Mar 2020 23:10:27 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; if we send this to /proc/self/fd/1, it never appears'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf
# Thu, 19 Mar 2020 23:10:30 GMT
STOPSIGNAL SIGQUIT
# Thu, 19 Mar 2020 23:10:34 GMT
EXPOSE 9000
# Thu, 19 Mar 2020 23:10:38 GMT
CMD ["php-fpm"]
# Fri, 20 Mar 2020 08:11:51 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ghostscript 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 08:18:55 GMT
RUN set -ex; 		savedAptMark="$(apt-mark showmanual)"; 		apt-get update; 	apt-get install -y --no-install-recommends 		libfreetype6-dev 		libjpeg-dev 		libmagickwand-dev 		libpng-dev 		libzip-dev 	; 		docker-php-ext-configure gd --with-freetype-dir=/usr --with-jpeg-dir=/usr --with-png-dir=/usr; 	docker-php-ext-install -j "$(nproc)" 		bcmath 		exif 		gd 		mysqli 		opcache 		zip 	; 	pecl install imagick-3.4.4; 	docker-php-ext-enable imagick; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark; 	ldd "$(php -r 'echo ini_get("extension_dir");')"/*.so 		| awk '/=>/ { print $3 }' 		| sort -u 		| xargs -r dpkg-query -S 		| cut -d: -f1 		| sort -u 		| xargs -rt apt-mark manual; 		apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*
# Fri, 20 Mar 2020 08:19:05 GMT
RUN { 		echo 'opcache.memory_consumption=128'; 		echo 'opcache.interned_strings_buffer=8'; 		echo 'opcache.max_accelerated_files=4000'; 		echo 'opcache.revalidate_freq=2'; 		echo 'opcache.fast_shutdown=1'; 	} > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Fri, 20 Mar 2020 08:19:13 GMT
RUN { 		echo 'error_reporting = E_ERROR | E_WARNING | E_PARSE | E_CORE_ERROR | E_CORE_WARNING | E_COMPILE_ERROR | E_COMPILE_WARNING | E_RECOVERABLE_ERROR'; 		echo 'display_errors = Off'; 		echo 'display_startup_errors = Off'; 		echo 'log_errors = On'; 		echo 'error_log = /dev/stderr'; 		echo 'log_errors_max_len = 1024'; 		echo 'ignore_repeated_errors = On'; 		echo 'ignore_repeated_source = Off'; 		echo 'html_errors = Off'; 	} > /usr/local/etc/php/conf.d/error-logging.ini
# Fri, 20 Mar 2020 08:19:15 GMT
VOLUME [/var/www/html]
# Fri, 20 Mar 2020 08:19:17 GMT
ENV WORDPRESS_VERSION=5.3.2
# Fri, 20 Mar 2020 08:19:20 GMT
ENV WORDPRESS_SHA1=fded476f112dbab14e3b5acddd2bcfa550e7b01b
# Fri, 20 Mar 2020 08:19:29 GMT
RUN set -ex; 	curl -o wordpress.tar.gz -fSL "https://wordpress.org/wordpress-${WORDPRESS_VERSION}.tar.gz"; 	echo "$WORDPRESS_SHA1 *wordpress.tar.gz" | sha1sum -c -; 	tar -xzf wordpress.tar.gz -C /usr/src/; 	rm wordpress.tar.gz; 	chown -R www-data:www-data /usr/src/wordpress
# Fri, 20 Mar 2020 08:19:32 GMT
COPY file:d93be233af180b81b8838a1d00e9f930eb82172c751ffaafb4732db4a09a7534 in /usr/local/bin/ 
# Fri, 20 Mar 2020 08:19:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 08:19:39 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:975241fcd2057cc8f4cb8f066d68ed18877152b88da11e682911ccc3bc3da7c4`  
		Last Modified: Wed, 26 Feb 2020 01:52:57 GMT  
		Size: 30.5 MB (30518427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c57d9b8bc2eac5c6f4f9993a4c4b7bd08403a98d069eb7b3678d6fe8396f488`  
		Last Modified: Wed, 26 Feb 2020 15:58:45 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:420ef5ae09970b307979254c32570cf02e8b0979b1bc6df0941e38eb670262a5`  
		Last Modified: Wed, 26 Feb 2020 15:59:12 GMT  
		Size: 82.3 MB (82259740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72af4000b0056d6328c78e7b5aa5de14c173ffd361612045bc4e3013bcb0fa8f`  
		Last Modified: Wed, 26 Feb 2020 15:58:44 GMT  
		Size: 268.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ddd3141df10db924405e9d2f7e56fabefd316644b69af434c5f6955372e4814`  
		Last Modified: Fri, 20 Mar 2020 02:17:58 GMT  
		Size: 12.4 MB (12435608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7d9e55bfcd36a88ccdc072ec48e51c6ee6c7846533015d601e4aaca454b5ea8`  
		Last Modified: Fri, 20 Mar 2020 02:17:57 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c54e48666f3ec1bc016ea5e4da358b03cdb4852467a0d7a045016670b45d8ac7`  
		Last Modified: Fri, 20 Mar 2020 02:17:59 GMT  
		Size: 30.5 MB (30488215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cbbf9285872d61031e434e42e149a9078c8943deed3248a653841eca450938d`  
		Last Modified: Fri, 20 Mar 2020 02:17:52 GMT  
		Size: 2.2 KB (2220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2436ed76e2e54e5e5fea3148361860a523dfd7210a0c8903c0faacf579b4d357`  
		Last Modified: Fri, 20 Mar 2020 02:17:51 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1cb4175bc25f50f3144a2deb98c9ab96bdfe470103555c0e12e37ecbf90bddc8`  
		Last Modified: Fri, 20 Mar 2020 02:17:53 GMT  
		Size: 213.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1fc4db835413a64550fe62846d3d02c5bfe898f3876f57529b6fa0911892600b`  
		Last Modified: Fri, 20 Mar 2020 02:17:52 GMT  
		Size: 8.4 KB (8417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0362833b11416a3d86b85f5f148d98f4569ae345f2b6bb553e277f7bad240b8e`  
		Last Modified: Fri, 20 Mar 2020 09:05:14 GMT  
		Size: 17.6 MB (17627968 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c728be9efc162cde5693a0c33e4457a9cc307cd27529becf2c815574037e0f61`  
		Last Modified: Fri, 20 Mar 2020 09:05:08 GMT  
		Size: 9.4 MB (9363671 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5d832317ea6604305b32e874d4f7ad19a4ecc2f3cddc64b4e1e843710bc4dae`  
		Last Modified: Fri, 20 Mar 2020 09:05:05 GMT  
		Size: 332.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab137aa196d1589dd414d3f5bef72836fc69a7562d33b45c7dde7fa6873227f2`  
		Last Modified: Fri, 20 Mar 2020 09:05:05 GMT  
		Size: 394.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:752d92a9a659751dd799c6df24a270ba410785c5b2bda4afec15e9329baf59aa`  
		Last Modified: Fri, 20 Mar 2020 09:05:09 GMT  
		Size: 12.2 MB (12227877 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4018446aeccc46de9ebc38efbbd6b65f81685b760161b8dd3c4b1b81c6f3accf`  
		Last Modified: Fri, 20 Mar 2020 09:05:06 GMT  
		Size: 3.9 KB (3896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
