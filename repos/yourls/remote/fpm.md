## `yourls:fpm`

```console
$ docker pull yourls@sha256:67688f66ff19e05edcc3d2b084dbd675387eebd916f68b679a7d1c97b74c34ee
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
$ docker pull yourls@sha256:0060cbac831372efbbe05fdc2a258ceff72ed1b71f67ec68ebcfec1a9f4862ab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.5 MB (166478757 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76e9e0ea75470350efbb4ac5c36825755352ae5381815de8205dd22641391d8d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Mar 2023 01:30:27 GMT
ADD file:60911afdacfdc216e44115addb5f3cc07f4166e8a4adf7be94a58aacc327ad63 in / 
# Thu, 23 Mar 2023 01:30:27 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 09:31:02 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Mar 2023 09:31:03 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Mar 2023 09:31:19 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 09:31:19 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 27 Mar 2023 22:33:07 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Mon, 27 Mar 2023 22:33:07 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:33:07 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:33:08 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 27 Mar 2023 22:33:08 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 27 Mar 2023 22:33:08 GMT
ENV PHP_VERSION=8.2.4
# Mon, 27 Mar 2023 22:33:08 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Mon, 27 Mar 2023 22:33:08 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Mon, 27 Mar 2023 22:33:21 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 27 Mar 2023 22:33:21 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:43:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 27 Mar 2023 22:43:00 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:43:01 GMT
RUN docker-php-ext-enable sodium
# Mon, 27 Mar 2023 22:43:01 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 27 Mar 2023 22:43:01 GMT
WORKDIR /var/www/html
# Mon, 27 Mar 2023 22:43:01 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 27 Mar 2023 22:43:01 GMT
STOPSIGNAL SIGQUIT
# Mon, 27 Mar 2023 22:43:01 GMT
EXPOSE 9000
# Mon, 27 Mar 2023 22:43:02 GMT
CMD ["php-fpm"]
# Tue, 28 Mar 2023 03:47:36 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 28 Mar 2023 03:47:36 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 28 Mar 2023 03:47:36 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 28 Mar 2023 03:47:36 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 28 Mar 2023 03:47:36 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 28 Mar 2023 03:47:36 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 28 Mar 2023 03:47:37 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 28 Mar 2023 03:47:37 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 28 Mar 2023 03:48:13 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 28 Mar 2023 03:48:14 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Mar 2023 03:48:14 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 03:48:14 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 03:48:14 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 28 Mar 2023 03:48:14 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 03:48:14 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 03:48:16 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 28 Mar 2023 03:48:16 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 28 Mar 2023 03:48:16 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 28 Mar 2023 03:48:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 03:48:16 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:f1f26f5702560b7e591bef5c4d840f76a232bf13fd5aefc4e22077a1ae4440c7`  
		Last Modified: Thu, 23 Mar 2023 01:34:23 GMT  
		Size: 31.4 MB (31411405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee0a4e40ccac1c58f6ca3cf6c0cbb0a5897abd33dee49b641509d5627df02b46`  
		Last Modified: Thu, 23 Mar 2023 10:51:34 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ca9fb408faadb7bf25d58bd66104b2e93e7ba37e961bb24b245abcc09230187`  
		Last Modified: Thu, 23 Mar 2023 10:51:46 GMT  
		Size: 91.6 MB (91636283 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:25862b797d8786d6655c181772787e4fa6c932aafd6853e429409590e9f6d99b`  
		Last Modified: Tue, 28 Mar 2023 00:51:20 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86f390fbd202858b1054f09273a7332a540a1ef21a500358d9b38f3b66218500`  
		Last Modified: Tue, 28 Mar 2023 00:51:19 GMT  
		Size: 12.3 MB (12310616 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fb9a2031944f290343556fde7618b9a79e9f61afebbd8bb53ebf958809a91c3`  
		Last Modified: Tue, 28 Mar 2023 00:51:18 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66bc885eb4ddc750968950108b7d584210dbd6a93d89717a4d2c9c229ce5f725`  
		Last Modified: Tue, 28 Mar 2023 00:52:27 GMT  
		Size: 26.5 MB (26515409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78544e5e6b9b4c99849cdf6b7dbef4d5bb415e9b871537d5aaf4e5f4da60ab9e`  
		Last Modified: Tue, 28 Mar 2023 00:52:23 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:559844b552f43487910986e99395732bde44f5b97cf6c56a8e0ee4a2ca94bff1`  
		Last Modified: Tue, 28 Mar 2023 00:52:23 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b445f87985194018bb6acb185b0bb6caeb6ebcf1b1efaadbe265bbb72843bea2`  
		Last Modified: Tue, 28 Mar 2023 00:52:23 GMT  
		Size: 9.2 KB (9182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23237633ebda9ec89cc94e1fe7b4a4c896533128084092a9bac130216fa973d0`  
		Last Modified: Tue, 28 Mar 2023 03:50:00 GMT  
		Size: 514.8 KB (514809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:697bb99f72a9f3a4cf08fec99e32c8081ce6ffe441f719c54b96c1b83de06be0`  
		Last Modified: Tue, 28 Mar 2023 03:50:00 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c3af225fdeefc4faf318c6c271b0cac7d74dbadc9b2f64cbbe2db4c3185b28`  
		Last Modified: Tue, 28 Mar 2023 03:50:01 GMT  
		Size: 4.1 MB (4073446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5131aa04fd830a86d49999835efe600c4c1726e7d163378f9b3a51cedf2b3dfb`  
		Last Modified: Tue, 28 Mar 2023 03:50:00 GMT  
		Size: 2.0 KB (2046 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf96800d035968c6fb1dc9ceb3c05e854873d552a2cc93e281cebc9ec6f539f0`  
		Last Modified: Tue, 28 Mar 2023 03:50:00 GMT  
		Size: 1.6 KB (1551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; arm variant v5

```console
$ docker pull yourls@sha256:cb648055e23772dcdf418e842eeaf64776472090981417e5d0cdc9d30f846807
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.3 MB (144264207 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fd9411d62d65494f2681da63724b2e199277a62f48c0fcef7d17ccaf5c355e46`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Mar 2023 00:48:44 GMT
ADD file:7595c7bfa6b3741f57a3ec7790e3108bb526244e52bb4a54548b8b5541e66616 in / 
# Thu, 23 Mar 2023 00:48:44 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 04:35:50 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Mar 2023 04:35:50 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Mar 2023 04:36:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 04:36:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 27 Mar 2023 23:22:52 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Mon, 27 Mar 2023 23:22:52 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 23:22:52 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 23:22:52 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 27 Mar 2023 23:22:52 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 27 Mar 2023 23:22:52 GMT
ENV PHP_VERSION=8.2.4
# Mon, 27 Mar 2023 23:22:52 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Mon, 27 Mar 2023 23:22:53 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Mon, 27 Mar 2023 23:23:07 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 27 Mar 2023 23:23:07 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 27 Mar 2023 23:35:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 27 Mar 2023 23:35:44 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 27 Mar 2023 23:35:44 GMT
RUN docker-php-ext-enable sodium
# Mon, 27 Mar 2023 23:35:44 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 27 Mar 2023 23:35:44 GMT
WORKDIR /var/www/html
# Mon, 27 Mar 2023 23:35:45 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 27 Mar 2023 23:35:45 GMT
STOPSIGNAL SIGQUIT
# Mon, 27 Mar 2023 23:35:45 GMT
EXPOSE 9000
# Mon, 27 Mar 2023 23:35:45 GMT
CMD ["php-fpm"]
# Tue, 28 Mar 2023 04:58:58 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 28 Mar 2023 04:58:58 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 28 Mar 2023 04:58:58 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 28 Mar 2023 04:58:59 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 28 Mar 2023 04:58:59 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 28 Mar 2023 04:58:59 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 28 Mar 2023 04:58:59 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 28 Mar 2023 04:58:59 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 28 Mar 2023 04:59:14 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 28 Mar 2023 04:59:15 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Mar 2023 04:59:15 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 04:59:15 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 04:59:15 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 28 Mar 2023 04:59:15 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 04:59:15 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 04:59:17 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 28 Mar 2023 04:59:17 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 28 Mar 2023 04:59:17 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 28 Mar 2023 04:59:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 04:59:17 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:b83d345710cdef1626d1940689dd3160e5ce3e4f63b3154cf612c52b704baa66`  
		Last Modified: Thu, 23 Mar 2023 02:22:00 GMT  
		Size: 28.9 MB (28915852 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca57ccfd8856601954ebd3b2457e5a69c056c4d963ce14194b256a62835cf4bc`  
		Last Modified: Sat, 25 Mar 2023 06:03:15 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74e7e09b6251efeda02d5db993f49bbfce41c1b302cbdb1fc9f848c28bae71fd`  
		Last Modified: Sat, 25 Mar 2023 06:03:28 GMT  
		Size: 73.7 MB (73685421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176c9afae73d55e29361805c127030059fd775592fb965c61b2fc4d4cb902cdb`  
		Last Modified: Tue, 28 Mar 2023 03:49:17 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:315c0ac59d7ffed72cfbea3d789d31ba87cdc46e5b801ff5552247270cca60ea`  
		Last Modified: Tue, 28 Mar 2023 03:49:16 GMT  
		Size: 12.3 MB (12308971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4381c8c043fab8bc3bbbaaaca8847f70c3769821afd6b60537d9af3778d31827`  
		Last Modified: Tue, 28 Mar 2023 03:49:15 GMT  
		Size: 490.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30c02bcffac2ed8ed30bec34a0b4c0144f92d5e61c0a85d0a2a50bbee264dd13`  
		Last Modified: Tue, 28 Mar 2023 03:50:27 GMT  
		Size: 25.1 MB (25109095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af60a310a8d802dbb73a5253938c6d42a8ecd8af99985bfa9435a99234d01316`  
		Last Modified: Tue, 28 Mar 2023 03:50:23 GMT  
		Size: 2.5 KB (2453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f501574f973b9f25403f7c361f6b5ddc87ea5b990a7f74a4036c6046d146330d`  
		Last Modified: Tue, 28 Mar 2023 03:50:22 GMT  
		Size: 248.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8f1391422639a3c19df80ee3ccb84242c52df69ff1a517f6ae8f9c31f542c72`  
		Last Modified: Tue, 28 Mar 2023 03:50:22 GMT  
		Size: 9.2 KB (9186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ebae8a5ae10a229fe0b8afdf1bcd78a8a323b375512f9aca06fd1c2397d939`  
		Last Modified: Sat, 08 Apr 2023 00:07:36 GMT  
		Size: 154.6 KB (154617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f06467cec81e8b5dfa0d20af2465de629f4d2fbbe16ec82a4a9a641f523609`  
		Last Modified: Sat, 08 Apr 2023 00:07:35 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:041d7dd7270764241f9cc30651bc6a09d821f69758d3cd077efa4ed79ec35fef`  
		Last Modified: Sat, 08 Apr 2023 00:07:36 GMT  
		Size: 4.1 MB (4073445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38546fb11b48976e9cd378125bb9926df5680cf63ce044bc60e3b7b65157d9fc`  
		Last Modified: Sat, 08 Apr 2023 00:07:35 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7c40f7a797d5caf1aab5f28cee135062d782c3316ffbc2201ceb3cd5b9cbabd`  
		Last Modified: Sat, 08 Apr 2023 00:07:36 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; arm variant v7

```console
$ docker pull yourls@sha256:704e677e1982c32db13987f9c443e7d010e33e5c408acf03efd304d8fd264b47
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **136.7 MB (136679303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8b940ad98b6d9c2c4e4faacb16c271016a0938b221722957f3f6f928e024691b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Mar 2023 01:16:59 GMT
ADD file:1c83b99ee21091150a1c9ee8ef7c40bec3d6cb0d64b8bc0ef40fb97e6233aa5b in / 
# Thu, 23 Mar 2023 01:17:00 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 09:52:05 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Mar 2023 09:52:05 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Mar 2023 09:52:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 09:52:25 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Tue, 28 Mar 2023 00:07:45 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Tue, 28 Mar 2023 00:07:45 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Mar 2023 00:07:45 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Tue, 28 Mar 2023 00:07:45 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Tue, 28 Mar 2023 00:07:46 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Tue, 28 Mar 2023 00:07:46 GMT
ENV PHP_VERSION=8.2.4
# Tue, 28 Mar 2023 00:07:46 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Tue, 28 Mar 2023 00:07:46 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Tue, 28 Mar 2023 00:07:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Tue, 28 Mar 2023 00:07:59 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Tue, 28 Mar 2023 00:14:55 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Tue, 28 Mar 2023 00:14:55 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Tue, 28 Mar 2023 00:14:56 GMT
RUN docker-php-ext-enable sodium
# Tue, 28 Mar 2023 00:14:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Tue, 28 Mar 2023 00:14:56 GMT
WORKDIR /var/www/html
# Tue, 28 Mar 2023 00:14:56 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Tue, 28 Mar 2023 00:14:56 GMT
STOPSIGNAL SIGQUIT
# Tue, 28 Mar 2023 00:14:56 GMT
EXPOSE 9000
# Tue, 28 Mar 2023 00:14:57 GMT
CMD ["php-fpm"]
# Tue, 28 Mar 2023 05:04:51 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 28 Mar 2023 05:04:51 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 28 Mar 2023 05:04:51 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 28 Mar 2023 05:04:51 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 28 Mar 2023 05:04:51 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 28 Mar 2023 05:04:51 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 28 Mar 2023 05:04:51 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 28 Mar 2023 05:04:51 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 28 Mar 2023 05:05:07 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 28 Mar 2023 05:05:07 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Mar 2023 05:05:07 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 05:05:07 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 05:05:07 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 28 Mar 2023 05:05:07 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 05:05:07 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 05:05:09 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 28 Mar 2023 05:05:09 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 28 Mar 2023 05:05:10 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 28 Mar 2023 05:05:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 05:05:10 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:2bc24e24d213c286ca4011c8b5cb7a3cf2a51f3bbedee8eeced46382bb5507bc`  
		Last Modified: Thu, 23 Mar 2023 01:33:18 GMT  
		Size: 26.6 MB (26577330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5859d7bd0331fdd3db36460ff2a1ddaaccba37d32aa3dbefd1438b3d6c296aaa`  
		Last Modified: Thu, 23 Mar 2023 10:50:12 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84701bd5e662e452c2d0a2061b7bdb9e457f6d7b3906d4f95854508811c6f3e2`  
		Last Modified: Thu, 23 Mar 2023 10:50:22 GMT  
		Size: 69.3 MB (69321562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:add98d09a42374aa2e4a2f400273f88190fd5958104efb5b76eba81b992842e6`  
		Last Modified: Tue, 28 Mar 2023 03:35:34 GMT  
		Size: 271.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68662a8bd520d45584950526b793c4118aacd39fdad75ef597aa9b8e15ee9331`  
		Last Modified: Tue, 28 Mar 2023 03:35:34 GMT  
		Size: 12.3 MB (12308956 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d4b05bfee28b5877a9dd1ced644a9585bf8aeef41d645847e4f3a8e5159a93`  
		Last Modified: Tue, 28 Mar 2023 03:35:32 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce26f29476cd4f7f7a5125dfcee1ff5452bea05c27a7f6139177ba3735d92107`  
		Last Modified: Tue, 28 Mar 2023 03:36:45 GMT  
		Size: 24.2 MB (24239408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0130463a7bef76b312b7439b29b2bceab04d5d0ed711e243277e12aae593eb9`  
		Last Modified: Tue, 28 Mar 2023 03:36:41 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e1f65a84022eb7ee60e5ffff8b8c5cf26f8003f23c9bf67d597948035d595bf`  
		Last Modified: Tue, 28 Mar 2023 03:36:41 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a2f5306d44c0f855c8dd640029e3fe238117c6cf12772d5a5b18fc0f02a9a2c`  
		Last Modified: Tue, 28 Mar 2023 03:36:41 GMT  
		Size: 9.2 KB (9184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7773fb5d3e4a87c3b9cbe1b080462285a4e05b583e626c8864b01799f1784442`  
		Last Modified: Sat, 01 Apr 2023 00:37:49 GMT  
		Size: 141.8 KB (141810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd3ab793e16a70cda2173e3ce775dd39e33f64466fc8699adca9ac0f934453c8`  
		Last Modified: Sat, 01 Apr 2023 00:37:49 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e5555ebbd4d5ecfe56b979e479669fcb38a620efc20570b7719bda4ebedaea52`  
		Last Modified: Sat, 01 Apr 2023 00:37:50 GMT  
		Size: 4.1 MB (4073438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47c569adbf697371de74ec9d9429246d58185438da9aa6ed9b9755075e05ccce`  
		Last Modified: Sat, 01 Apr 2023 00:37:49 GMT  
		Size: 2.0 KB (2049 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cff3ffae960c94cdec9a821e508125f46a9b8d1bce65c5b88288abe4d4096e5`  
		Last Modified: Sat, 01 Apr 2023 00:37:49 GMT  
		Size: 1.6 KB (1555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; arm64 variant v8

```console
$ docker pull yourls@sha256:e7486051a27864150f0a04b5e908a9c5c89f0d248046a895f249e44694126723
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **160.8 MB (160766679 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e280445349a075e6278dbcfd2d257b96147d947b6129d22a240c37cd447af900`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Mar 2023 00:45:10 GMT
ADD file:83beb883b699cd442f1dbd4baf29c23f4cd15f7a5f9f120979df16a77455c69f in / 
# Thu, 23 Mar 2023 00:45:10 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 12:12:22 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Mar 2023 12:12:22 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Mar 2023 12:12:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 12:12:39 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 27 Mar 2023 22:59:42 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Mon, 27 Mar 2023 22:59:42 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:59:42 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:59:42 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 27 Mar 2023 22:59:42 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 27 Mar 2023 22:59:42 GMT
ENV PHP_VERSION=8.2.4
# Mon, 27 Mar 2023 22:59:42 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Mon, 27 Mar 2023 22:59:42 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Mon, 27 Mar 2023 22:59:54 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 27 Mar 2023 22:59:54 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 27 Mar 2023 23:09:48 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 27 Mar 2023 23:09:49 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 27 Mar 2023 23:09:49 GMT
RUN docker-php-ext-enable sodium
# Mon, 27 Mar 2023 23:09:49 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 27 Mar 2023 23:09:49 GMT
WORKDIR /var/www/html
# Mon, 27 Mar 2023 23:09:50 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 27 Mar 2023 23:09:50 GMT
STOPSIGNAL SIGQUIT
# Mon, 27 Mar 2023 23:09:50 GMT
EXPOSE 9000
# Mon, 27 Mar 2023 23:09:50 GMT
CMD ["php-fpm"]
# Tue, 28 Mar 2023 03:33:36 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 28 Mar 2023 03:33:36 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 28 Mar 2023 03:33:37 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 28 Mar 2023 03:33:37 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 28 Mar 2023 03:33:37 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 28 Mar 2023 03:33:37 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 28 Mar 2023 03:33:37 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 28 Mar 2023 03:33:37 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 28 Mar 2023 03:34:29 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 28 Mar 2023 03:34:29 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Mar 2023 03:34:29 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 03:34:29 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 03:34:29 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 28 Mar 2023 03:34:29 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 03:34:29 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 03:34:31 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 28 Mar 2023 03:34:31 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 28 Mar 2023 03:34:31 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 28 Mar 2023 03:34:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 03:34:32 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:fcdb9667c46b09d1c1d058681ea4a1db41e66bbc1a71d873a0c9da4f7a92947d`  
		Last Modified: Thu, 23 Mar 2023 00:48:09 GMT  
		Size: 30.1 MB (30062700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65bdd3f1135f89f0c6a453b25e0224ee49243ee4c2af5759ee6b592bbf84a11e`  
		Last Modified: Thu, 23 Mar 2023 13:20:28 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:183fcacf85bd0d1bea414ac64e3d6ac2272a67e46b1b296d847900d3126a39fc`  
		Last Modified: Thu, 23 Mar 2023 13:20:37 GMT  
		Size: 86.9 MB (86928489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c19018479f3e7280fbf09f9a84003c15a8cdd69eab5d36617ed4ab96196eef`  
		Last Modified: Tue, 28 Mar 2023 01:08:44 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d54264a59c274ce185d1e0a6d46ba55e33168d0097dbd17e15e5cc4c5daca0`  
		Last Modified: Tue, 28 Mar 2023 01:08:43 GMT  
		Size: 12.3 MB (12309890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:200b051effc2b01b1ad3f1ada90ffd6c033d1ca1aa99d007520fbdb7c70d8d62`  
		Last Modified: Tue, 28 Mar 2023 01:08:42 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a871dc9669ff20da6048118a77091b67ab9c9db2591692df02a7d9404cd08a2`  
		Last Modified: Tue, 28 Mar 2023 01:09:51 GMT  
		Size: 26.6 MB (26576518 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c946881523deb6990eb366dcc647073cc883855f350a42e6314f013c028fa01`  
		Last Modified: Tue, 28 Mar 2023 01:09:48 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4648a1a7de334db6ee0eee83bc2908d7b5a700fd87158fc7ceb0d90c922491e9`  
		Last Modified: Tue, 28 Mar 2023 01:09:48 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:779b2283bd5a5a62f3d74d15892c4cad9818f5ceed7bf28440621ecb38283c24`  
		Last Modified: Tue, 28 Mar 2023 01:09:48 GMT  
		Size: 9.2 KB (9183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d3ce3413915943fc456c51547793deb5550788f910cfa6bac137dec6dc22cf9`  
		Last Modified: Tue, 28 Mar 2023 03:36:32 GMT  
		Size: 798.9 KB (798851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2139aa26e30694dda756d51adeb04e1c48e8380202c68cbbedbeb684013f8a37`  
		Last Modified: Tue, 28 Mar 2023 03:36:32 GMT  
		Size: 327.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43001f9b39d792fc3d5971106ec115f3687faac79dd95ed09ea00380710c7d06`  
		Last Modified: Tue, 28 Mar 2023 03:36:33 GMT  
		Size: 4.1 MB (4073437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74ec7f600e3748c69039d964273720acdff2d4d7a5b957c846c74ff8990e977f`  
		Last Modified: Tue, 28 Mar 2023 03:36:32 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d00bd046822e9aeceb1ef857b081dc7ba3d63f638ac8b6f1277abb9a54fb6cfd`  
		Last Modified: Tue, 28 Mar 2023 03:36:32 GMT  
		Size: 1.6 KB (1550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; 386

```console
$ docker pull yourls@sha256:8e987f988aff41bbeeb2b03e032d0026ef66ab60d0bfccf31c94848038661957
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **169.0 MB (169019315 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:517af96765e70ec6854652c644e593f430a9887e55d3a999ef5457f3c4da7988`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Mar 2023 00:39:18 GMT
ADD file:315d843eefd4a8bb2345366dcd6bab00a06fca4a7970e220ae8946123d07d7ed in / 
# Thu, 23 Mar 2023 00:39:19 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 08:48:38 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Mar 2023 08:48:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Mar 2023 08:49:01 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 08:49:02 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 27 Mar 2023 22:40:24 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Mon, 27 Mar 2023 22:40:24 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:40:25 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:40:25 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 27 Mar 2023 22:40:25 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 27 Mar 2023 22:40:25 GMT
ENV PHP_VERSION=8.2.4
# Mon, 27 Mar 2023 22:40:25 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Mon, 27 Mar 2023 22:40:25 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Mon, 27 Mar 2023 22:40:40 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 27 Mar 2023 22:40:40 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:55:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 27 Mar 2023 22:55:51 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:55:52 GMT
RUN docker-php-ext-enable sodium
# Mon, 27 Mar 2023 22:55:52 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 27 Mar 2023 22:55:52 GMT
WORKDIR /var/www/html
# Mon, 27 Mar 2023 22:55:52 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 27 Mar 2023 22:55:52 GMT
STOPSIGNAL SIGQUIT
# Mon, 27 Mar 2023 22:55:53 GMT
EXPOSE 9000
# Mon, 27 Mar 2023 22:55:53 GMT
CMD ["php-fpm"]
# Tue, 28 Mar 2023 05:30:38 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 28 Mar 2023 05:30:38 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 28 Mar 2023 05:30:38 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 28 Mar 2023 05:30:38 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 28 Mar 2023 05:30:38 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 28 Mar 2023 05:30:38 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 28 Mar 2023 05:30:38 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 28 Mar 2023 05:30:38 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 28 Mar 2023 05:31:18 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 28 Mar 2023 05:31:18 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Mar 2023 05:31:18 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 05:31:18 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 05:31:18 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 28 Mar 2023 05:31:18 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 05:31:19 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 05:31:20 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 28 Mar 2023 05:31:21 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 28 Mar 2023 05:31:21 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 28 Mar 2023 05:31:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 05:31:21 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:3e638a975ea99fe8646002726dcb1ccdccc49ad33967b30337b9b2413e0619b5`  
		Last Modified: Thu, 23 Mar 2023 00:43:09 GMT  
		Size: 32.4 MB (32396277 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06aa6a41a038993b857528270326d42c797e0a981b2766ad831ae3df77110f1b`  
		Last Modified: Thu, 23 Mar 2023 10:50:14 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2e6018ce44943ea0d18b41430c9f4e71fbdf0256d6d048e01fc4b488e3dcb3c`  
		Last Modified: Thu, 23 Mar 2023 10:50:33 GMT  
		Size: 92.7 MB (92720414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9b403e42a4f652ad3a0d3a5a14c26ec7754b08b9a682399215f0820684474b9`  
		Last Modified: Tue, 28 Mar 2023 02:25:08 GMT  
		Size: 269.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d57f51ed70df2f908adcaad214c01245ff0423393e0a5409cea8262f864881b0`  
		Last Modified: Tue, 28 Mar 2023 02:25:08 GMT  
		Size: 12.3 MB (12309793 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4f337bbdde92226ba1ff572aa5539f6aefa55001309d194a935df0f0450eea4`  
		Last Modified: Tue, 28 Mar 2023 02:25:06 GMT  
		Size: 489.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bfe16813c2cf6b02e7729b6f80f5c4c320e56b9e989c747f56f673273b1d5c75`  
		Last Modified: Tue, 28 Mar 2023 02:26:23 GMT  
		Size: 27.0 MB (27007724 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7703d11c3b4bf3c725066ab62c4b647b057f65f2b0aad84f51d5e5c5c098d139`  
		Last Modified: Tue, 28 Mar 2023 02:26:18 GMT  
		Size: 2.4 KB (2449 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80e2c9aa80f1c37cfbe17abfc394ace81a56b4a90d132634fa4a9030ab78604f`  
		Last Modified: Tue, 28 Mar 2023 02:26:18 GMT  
		Size: 244.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55233040ddcace4b4d3003913f5651254d81d8c3405d8fbbd98c9c704fe6fb51`  
		Last Modified: Tue, 28 Mar 2023 02:26:18 GMT  
		Size: 9.2 KB (9179 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fee5a638f5d49f07ada03fb16743e38d48b3fccfceb77156b73c8252bfbc8eb5`  
		Last Modified: Tue, 28 Mar 2023 05:33:01 GMT  
		Size: 494.9 KB (494883 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fcc04959cb5a13561f951711c2fb4204a38471c4fc020e0277c2276d6b8d5e3a`  
		Last Modified: Tue, 28 Mar 2023 05:33:00 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e3d4db95026ae980e277f251de44a37346f12d2d7af8fb200d73925472122f0`  
		Last Modified: Tue, 28 Mar 2023 05:33:02 GMT  
		Size: 4.1 MB (4073442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61aa367e7e3e0db9b949fdecf7a15b9e34f4e805821281cc380f096ed542662b`  
		Last Modified: Tue, 28 Mar 2023 05:33:00 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c6c5eba629fd5fac631a6277affa4e53107af1a8152acf502bb43f6aa55dec5`  
		Last Modified: Tue, 28 Mar 2023 05:33:00 GMT  
		Size: 1.6 KB (1550 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; mips64le

```console
$ docker pull yourls@sha256:93240f51ab6b74485771c6ba0f54f75067ad726528129f33bac6e7f6c24a01a4
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.3 MB (143287451 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fb7e33ed732b56d4ce7d00cdc21f9182e8f20dab2cfe3a5af12433d53c1bdfe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Mar 2023 05:17:57 GMT
ADD file:fd3a8eec4ae8f6058f522536ca9af1b391f3032504c085d8ddb6f4878ca478d5 in / 
# Thu, 23 Mar 2023 05:18:02 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 20:46:36 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Mar 2023 20:46:38 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Mar 2023 20:48:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 20:48:16 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 27 Mar 2023 22:09:30 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Mon, 27 Mar 2023 22:09:33 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:09:36 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:09:40 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 27 Mar 2023 22:09:43 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 27 Mar 2023 22:09:46 GMT
ENV PHP_VERSION=8.2.4
# Mon, 27 Mar 2023 22:09:50 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Mon, 27 Mar 2023 22:09:53 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Mon, 27 Mar 2023 22:10:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 27 Mar 2023 22:10:52 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:54:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 27 Mar 2023 22:54:47 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:54:52 GMT
RUN docker-php-ext-enable sodium
# Mon, 27 Mar 2023 22:54:56 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 27 Mar 2023 22:54:59 GMT
WORKDIR /var/www/html
# Mon, 27 Mar 2023 22:55:05 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 27 Mar 2023 22:55:08 GMT
STOPSIGNAL SIGQUIT
# Mon, 27 Mar 2023 22:55:11 GMT
EXPOSE 9000
# Mon, 27 Mar 2023 22:55:14 GMT
CMD ["php-fpm"]
# Tue, 28 Mar 2023 07:12:43 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 28 Mar 2023 07:12:47 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 28 Mar 2023 07:12:50 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 28 Mar 2023 07:12:54 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 28 Mar 2023 07:12:57 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 28 Mar 2023 07:13:00 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 28 Mar 2023 07:13:04 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 28 Mar 2023 07:13:07 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 28 Mar 2023 07:14:12 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 28 Mar 2023 07:14:18 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Mar 2023 07:14:21 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 07:14:24 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 07:14:28 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 28 Mar 2023 07:14:31 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 07:14:34 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 07:14:43 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 28 Mar 2023 07:14:46 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 28 Mar 2023 07:14:49 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 28 Mar 2023 07:14:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 07:14:56 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:735f9e60414e17ec59baef702f7013b7327899801df2ecf10123ce2727d8dea5`  
		Last Modified: Thu, 23 Mar 2023 05:25:53 GMT  
		Size: 29.6 MB (29634483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cdaed7fbf45d20bf0dcaf24949531440ccb33b76239b932e0caa3f080e337c11`  
		Last Modified: Tue, 28 Mar 2023 01:02:19 GMT  
		Size: 227.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:303aa2a4dd7ba9f132f3f0a45fcc1c3ac0c712e946516555e7b75dd61e41da28`  
		Last Modified: Tue, 28 Mar 2023 01:03:10 GMT  
		Size: 71.8 MB (71814424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:877c805149e9b40916c02cf22d8b5e6c77e471e4f0d03ec38b647980d5f0c10d`  
		Last Modified: Tue, 28 Mar 2023 01:02:19 GMT  
		Size: 226.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:673fd0f34cdfa68260d094a119bca2aad628445752a4d903a44427ecd7c6ddee`  
		Last Modified: Tue, 28 Mar 2023 01:02:20 GMT  
		Size: 12.1 MB (12092725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29fec0169db6bb54eaba71e9a9c436ea47e0de2d60151aac1932114f15712f96`  
		Last Modified: Tue, 28 Mar 2023 01:02:17 GMT  
		Size: 491.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2301e7f13a10b08440e8c1362c293f696e694245eddbeb73db238cc66616cd1b`  
		Last Modified: Tue, 28 Mar 2023 01:04:48 GMT  
		Size: 25.5 MB (25502153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4afaff17ecbe3f6bb91edb189f37f7c91c654975200cf93c6880292250307a07`  
		Last Modified: Tue, 28 Mar 2023 01:04:32 GMT  
		Size: 2.5 KB (2454 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88f2f2005deb44c17b8faba92cf342512b54196bf394c7953c0f7ec0b7183db8`  
		Last Modified: Tue, 28 Mar 2023 01:04:32 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0997b75f68a68f6a6c7929b1c43e7a879616666d7ead326e2ffb2f9983c4817`  
		Last Modified: Tue, 28 Mar 2023 01:04:32 GMT  
		Size: 9.2 KB (9191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ff852ea9739e6521ff89d08ec0e6500d4552c148bbc786668a821c80d863e58`  
		Last Modified: Tue, 28 Mar 2023 07:15:52 GMT  
		Size: 153.5 KB (153457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a74de6438cfb30d61e19ad29b597014249abcf35cea8fec4863610944b781f`  
		Last Modified: Tue, 28 Mar 2023 07:15:52 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2694e99b5d93e98ba408dae9c2b49a0b3570f1a0ec1a97c035694a4513107758`  
		Last Modified: Tue, 28 Mar 2023 07:15:56 GMT  
		Size: 4.1 MB (4073443 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5f3645a91227d737e1043b365ecd7295a3ad6054af3e038659bf847b8c9aff`  
		Last Modified: Tue, 28 Mar 2023 07:15:52 GMT  
		Size: 2.0 KB (2048 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b70bc4b5f50e38b8105c71a3ffe974d3576d450e586a1e17c87b42b3be02bef1`  
		Last Modified: Tue, 28 Mar 2023 07:15:52 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; ppc64le

```console
$ docker pull yourls@sha256:f85feefc991ccc4e3eaf226621aac70123c4d91b35acd60ed0b69674b92ed1e9
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **166.1 MB (166119777 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6f34ef1314c9c68127b8096ab35fe2d2518a2f918d0fda1c34cb031d41b50603`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Mar 2023 01:19:48 GMT
ADD file:fbd36b7667327dd30171fc49b8e028b8371fdbc7d30ee673808d508557f78bf1 in / 
# Thu, 23 Mar 2023 01:19:49 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 11:16:43 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Mar 2023 11:16:43 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Mar 2023 11:17:22 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 11:17:26 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 27 Mar 2023 22:30:55 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Mon, 27 Mar 2023 22:30:55 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:30:55 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:30:56 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 27 Mar 2023 22:30:56 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 27 Mar 2023 22:30:57 GMT
ENV PHP_VERSION=8.2.4
# Mon, 27 Mar 2023 22:30:58 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Mon, 27 Mar 2023 22:30:58 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Mon, 27 Mar 2023 22:31:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 27 Mar 2023 22:31:32 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:46:16 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 27 Mar 2023 22:46:17 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:46:19 GMT
RUN docker-php-ext-enable sodium
# Mon, 27 Mar 2023 22:46:19 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 27 Mar 2023 22:46:19 GMT
WORKDIR /var/www/html
# Mon, 27 Mar 2023 22:46:21 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 27 Mar 2023 22:46:21 GMT
STOPSIGNAL SIGQUIT
# Mon, 27 Mar 2023 22:46:21 GMT
EXPOSE 9000
# Mon, 27 Mar 2023 22:46:22 GMT
CMD ["php-fpm"]
# Tue, 28 Mar 2023 06:21:15 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 28 Mar 2023 06:21:17 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 28 Mar 2023 06:21:18 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 28 Mar 2023 06:21:19 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 28 Mar 2023 06:21:20 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 28 Mar 2023 06:21:21 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 28 Mar 2023 06:21:22 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 28 Mar 2023 06:21:23 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 28 Mar 2023 06:22:03 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 28 Mar 2023 06:22:04 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Mar 2023 06:22:05 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 06:22:06 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 06:22:07 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 28 Mar 2023 06:22:08 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 06:22:09 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 06:22:13 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 28 Mar 2023 06:22:15 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 28 Mar 2023 06:22:16 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 28 Mar 2023 06:22:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 06:22:22 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:8f472ad0a3fa58b4e304d1a974f25615d5bd3b7a99dff9c8202bd30facef0155`  
		Last Modified: Thu, 23 Mar 2023 01:24:22 GMT  
		Size: 35.3 MB (35288050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5512e0497df21360191b849f72d51f7703c3bd5d51e3a86e99f5f29e75c133f1`  
		Last Modified: Thu, 23 Mar 2023 12:17:14 GMT  
		Size: 228.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:62cd33d778b1f35bc7aba19bc6c01a581af85ccbdf01838e9cc40a2acb4da1e8`  
		Last Modified: Thu, 23 Mar 2023 12:17:36 GMT  
		Size: 86.6 MB (86632853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f90b7c47f5163af25830b86afe3a61c91bf54c82e24fabb73932f775777313aa`  
		Last Modified: Tue, 28 Mar 2023 00:39:24 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5708d261f5047687ecd0fda4365baff6d38ad670ea4ab3fbea7b4cbed227ec3`  
		Last Modified: Tue, 28 Mar 2023 00:39:23 GMT  
		Size: 12.3 MB (12310577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24c0bd2ec0a1367cc20c0c3e8d21ed4cc33abf5490dfefd31238252fcf171305`  
		Last Modified: Tue, 28 Mar 2023 00:39:22 GMT  
		Size: 492.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79da679c065a134354befeb3e5175625f433f7d84fb1b52e35ed1db6b316cf25`  
		Last Modified: Tue, 28 Mar 2023 00:40:51 GMT  
		Size: 27.6 MB (27609633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04e0d26ca4bc5ba18b9fdf5c2aebee6d186e8151b4bfb5a9ba5d50e556e8cb6b`  
		Last Modified: Tue, 28 Mar 2023 00:40:44 GMT  
		Size: 2.5 KB (2452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fcef3e5e8e757556371332381e9c02a8df84d456553635f376d8ab75bd496d`  
		Last Modified: Tue, 28 Mar 2023 00:40:44 GMT  
		Size: 247.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bceb72115ee6ec7d86bfbf7cf944f21c418ba4fbb7065b35802c73158ad4804d`  
		Last Modified: Tue, 28 Mar 2023 00:40:44 GMT  
		Size: 9.2 KB (9184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf496a0de012ce97574d3e6a0672ef4e36cdaca42b555272b9a17459622ad4be`  
		Last Modified: Tue, 28 Mar 2023 06:24:44 GMT  
		Size: 188.4 KB (188419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d378f56b6896ac2fde1799231106c0009163c198717370f84682d65ab1ef222`  
		Last Modified: Tue, 28 Mar 2023 06:24:44 GMT  
		Size: 330.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb2fd7e9e9d1eb52ffc99ce569226edee596b1a79e10f0459390283bf872078b`  
		Last Modified: Tue, 28 Mar 2023 06:24:45 GMT  
		Size: 4.1 MB (4073438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e70f39a02d4e474c44d3cc357dee4a99ef762a9c30130063e76861e34a902428`  
		Last Modified: Tue, 28 Mar 2023 06:24:44 GMT  
		Size: 2.0 KB (2050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b7130693483b7b167473f1b5bda2451b759058d020da93ba4af28da0722e021`  
		Last Modified: Tue, 28 Mar 2023 06:24:44 GMT  
		Size: 1.6 KB (1554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `yourls:fpm` - linux; s390x

```console
$ docker pull yourls@sha256:683e86123a467ab247188384b81ff357dd887025b02c173d03da5e1eefcef94b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **143.4 MB (143401611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35b45f52677a0f57d74e429b954da096e3ca49a1d2242b5d902942d5158fdd23`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["php-fpm"]`

```dockerfile
# Thu, 23 Mar 2023 00:44:06 GMT
ADD file:8b6d3f57adaa8af2e0599a6468c50b713d281165b4e61150850bedf587f7ad4f in / 
# Thu, 23 Mar 2023 00:44:08 GMT
CMD ["bash"]
# Thu, 23 Mar 2023 08:34:52 GMT
RUN set -eux; 	{ 		echo 'Package: php*'; 		echo 'Pin: release *'; 		echo 'Pin-Priority: -1'; 	} > /etc/apt/preferences.d/no-debian-php
# Thu, 23 Mar 2023 08:34:52 GMT
ENV PHPIZE_DEPS=autoconf 		dpkg-dev 		file 		g++ 		gcc 		libc-dev 		make 		pkg-config 		re2c
# Thu, 23 Mar 2023 08:35:08 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		$PHPIZE_DEPS 		ca-certificates 		curl 		xz-utils 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 23 Mar 2023 08:35:12 GMT
ENV PHP_INI_DIR=/usr/local/etc/php
# Mon, 27 Mar 2023 22:45:32 GMT
RUN set -eux; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	[ ! -d /var/www/html ]; 	mkdir -p /var/www/html; 	chown www-data:www-data /var/www/html; 	chmod 1777 /var/www/html
# Mon, 27 Mar 2023 22:45:32 GMT
ENV PHP_CFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:45:32 GMT
ENV PHP_CPPFLAGS=-fstack-protector-strong -fpic -fpie -O2 -D_LARGEFILE_SOURCE -D_FILE_OFFSET_BITS=64
# Mon, 27 Mar 2023 22:45:32 GMT
ENV PHP_LDFLAGS=-Wl,-O1 -pie
# Mon, 27 Mar 2023 22:45:32 GMT
ENV GPG_KEYS=39B641343D8C104B2B146DC3F9C39DC0B9698544 E60913E4DF209907D8E30D96659A97C9CF2A795A 1198C0117593497A5EC5C199286AF1F9897469DC
# Mon, 27 Mar 2023 22:45:32 GMT
ENV PHP_VERSION=8.2.4
# Mon, 27 Mar 2023 22:45:32 GMT
ENV PHP_URL=https://www.php.net/distributions/php-8.2.4.tar.xz PHP_ASC_URL=https://www.php.net/distributions/php-8.2.4.tar.xz.asc
# Mon, 27 Mar 2023 22:45:33 GMT
ENV PHP_SHA256=bc7bf4ca7ed0dd17647e3ea870b6f062fcb56b243bfdef3f59ff7f94e96176a8
# Mon, 27 Mar 2023 22:45:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends gnupg dirmngr; 	rm -rf /var/lib/apt/lists/*; 		mkdir -p /usr/src; 	cd /usr/src; 		curl -fsSL -o php.tar.xz "$PHP_URL"; 		if [ -n "$PHP_SHA256" ]; then 		echo "$PHP_SHA256 *php.tar.xz" | sha256sum -c -; 	fi; 		if [ -n "$PHP_ASC_URL" ]; then 		curl -fsSL -o php.tar.xz.asc "$PHP_ASC_URL"; 		export GNUPGHOME="$(mktemp -d)"; 		for key in $GPG_KEYS; do 			gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 		done; 		gpg --batch --verify php.tar.xz.asc php.tar.xz; 		gpgconf --kill all; 		rm -rf "$GNUPGHOME"; 	fi; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false
# Mon, 27 Mar 2023 22:45:44 GMT
COPY file:ce57c04b70896f77cc11eb2766417d8a1240fcffe5bba92179ec78c458844110 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:53:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		libargon2-dev 		libcurl4-openssl-dev 		libonig-dev 		libreadline-dev 		libsodium-dev 		libsqlite3-dev 		libssl-dev 		libxml2-dev 		zlib1g-dev 	; 		export 		CFLAGS="$PHP_CFLAGS" 		CPPFLAGS="$PHP_CPPFLAGS" 		LDFLAGS="$PHP_LDFLAGS" 	; 	docker-php-source extract; 	cd /usr/src/php; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	debMultiarch="$(dpkg-architecture --query DEB_BUILD_MULTIARCH)"; 	if [ ! -d /usr/include/curl ]; then 		ln -sT "/usr/include/$debMultiarch/curl" /usr/local/include/curl; 	fi; 	./configure 		--build="$gnuArch" 		--with-config-file-path="$PHP_INI_DIR" 		--with-config-file-scan-dir="$PHP_INI_DIR/conf.d" 				--enable-option-checking=fatal 				--with-mhash 				--with-pic 				--enable-ftp 		--enable-mbstring 		--enable-mysqlnd 		--with-password-argon2 		--with-sodium=shared 		--with-pdo-sqlite=/usr 		--with-sqlite3=/usr 				--with-curl 		--with-iconv 		--with-openssl 		--with-readline 		--with-zlib 				--disable-phpdbg 				--with-pear 				$(test "$gnuArch" = 's390x-linux-gnu' && echo '--without-pcre-jit') 		--with-libdir="lib/$debMultiarch" 				--disable-cgi 				--enable-fpm 		--with-fpm-user=www-data 		--with-fpm-group=www-data 	; 	make -j "$(nproc)"; 	find -type f -name '*.a' -delete; 	make install; 	find 		/usr/local 		-type f 		-perm '/0111' 		-exec sh -euxc ' 			strip --strip-all "$@" || : 		' -- '{}' + 	; 	make clean; 		cp -v php.ini-* "$PHP_INI_DIR/"; 		cd /; 	docker-php-source delete; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 	rm -rf /var/lib/apt/lists/*; 		pecl update-channels; 	rm -rf /tmp/pear ~/.pearrc; 		php --version
# Mon, 27 Mar 2023 22:53:25 GMT
COPY multi:869bde9dbeae74886a05c9e2107b3e3b4877116db8c6d9adbaff2719f9fb5262 in /usr/local/bin/ 
# Mon, 27 Mar 2023 22:53:26 GMT
RUN docker-php-ext-enable sodium
# Mon, 27 Mar 2023 22:53:26 GMT
ENTRYPOINT ["docker-php-entrypoint"]
# Mon, 27 Mar 2023 22:53:26 GMT
WORKDIR /var/www/html
# Mon, 27 Mar 2023 22:53:27 GMT
RUN set -eux; 	cd /usr/local/etc; 	if [ -d php-fpm.d ]; then 		sed 's!=NONE/!=!g' php-fpm.conf.default | tee php-fpm.conf > /dev/null; 		cp php-fpm.d/www.conf.default php-fpm.d/www.conf; 	else 		mkdir php-fpm.d; 		cp php-fpm.conf.default php-fpm.d/www.conf; 		{ 			echo '[global]'; 			echo 'include=etc/php-fpm.d/*.conf'; 		} | tee php-fpm.conf; 	fi; 	{ 		echo '[global]'; 		echo 'error_log = /proc/self/fd/2'; 		echo; echo '; https://github.com/docker-library/php/pull/725#issuecomment-443540114'; echo 'log_limit = 8192'; 		echo; 		echo '[www]'; 		echo '; php-fpm closes STDOUT on startup, so sending logs to /proc/self/fd/1 does not work.'; 		echo '; https://bugs.php.net/bug.php?id=73886'; 		echo 'access.log = /proc/self/fd/2'; 		echo; 		echo 'clear_env = no'; 		echo; 		echo '; Ensure worker stdout and stderr are sent to the main error log.'; 		echo 'catch_workers_output = yes'; 		echo 'decorate_workers_output = no'; 	} | tee php-fpm.d/docker.conf; 	{ 		echo '[global]'; 		echo 'daemonize = no'; 		echo; 		echo '[www]'; 		echo 'listen = 9000'; 	} | tee php-fpm.d/zz-docker.conf; 	mkdir -p "$PHP_INI_DIR/conf.d"; 	{ 		echo '; https://github.com/docker-library/php/issues/878#issuecomment-938595965'; 		echo 'fastcgi.logging = Off'; 	} > "$PHP_INI_DIR/conf.d/docker-fpm.ini"
# Mon, 27 Mar 2023 22:53:27 GMT
STOPSIGNAL SIGQUIT
# Mon, 27 Mar 2023 22:53:27 GMT
EXPOSE 9000
# Mon, 27 Mar 2023 22:53:27 GMT
CMD ["php-fpm"]
# Tue, 28 Mar 2023 02:17:25 GMT
LABEL org.opencontainers.image.title=YOURLS
# Tue, 28 Mar 2023 02:17:25 GMT
LABEL org.opencontainers.image.description=Your Own URL Shortener
# Tue, 28 Mar 2023 02:17:25 GMT
LABEL org.opencontainers.image.url=https://yourls.org/
# Tue, 28 Mar 2023 02:17:25 GMT
LABEL org.opencontainers.image.documentation=https://yourls.org/
# Tue, 28 Mar 2023 02:17:25 GMT
LABEL org.opencontainers.image.vendor=YOURLS Org
# Tue, 28 Mar 2023 02:17:25 GMT
LABEL org.opencontainers.image.authors=YOURLS
# Tue, 28 Mar 2023 02:17:25 GMT
LABEL org.opencontainers.image.licenses=MIT
# Tue, 28 Mar 2023 02:17:25 GMT
LABEL io.artifacthub.package.readme-url=https://raw.githubusercontent.com/YOURLS/YOURLS/master/README.md
# Tue, 28 Mar 2023 02:17:37 GMT
RUN set -eux;     docker-php-ext-install -j "$(nproc)" bcmath opcache pdo_mysql mysqli
# Tue, 28 Mar 2023 02:17:38 GMT
RUN {         echo 'opcache.memory_consumption=128';         echo 'opcache.interned_strings_buffer=8';         echo 'opcache.max_accelerated_files=4000';         echo 'opcache.revalidate_freq=2';         echo 'opcache.fast_shutdown=1';     } > /usr/local/etc/php/conf.d/opcache-recommended.ini
# Tue, 28 Mar 2023 02:17:38 GMT
ARG YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 02:17:38 GMT
ARG YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 02:17:38 GMT
LABEL org.opencontainers.image.version=1.9.2
# Tue, 28 Mar 2023 02:17:38 GMT
ENV YOURLS_VERSION=1.9.2
# Tue, 28 Mar 2023 02:17:38 GMT
ENV YOURLS_SHA256=62a95ba766d62f3305d75944cbfe12d5a90c08c88fbf2f6e67150d36412b916f
# Tue, 28 Mar 2023 02:17:40 GMT
RUN set -eux;     curl -o yourls.tar.gz -fsSL "https://github.com/YOURLS/YOURLS/archive/${YOURLS_VERSION}.tar.gz";     echo "$YOURLS_SHA256 *yourls.tar.gz" | sha256sum -c -;     tar -xf yourls.tar.gz -C /usr/src/;     mv "/usr/src/YOURLS-${YOURLS_VERSION}" /usr/src/yourls;     rm yourls.tar.gz;     chown -R www-data:www-data /usr/src/yourls
# Tue, 28 Mar 2023 02:17:40 GMT
COPY --chown=www-data:www-datafile:f5584b9849b80034920f4de5f1297cb1be461f765f3437b87ddf6c86daa6499d in /usr/src/yourls/user/ 
# Tue, 28 Mar 2023 02:17:40 GMT
COPY file:975ababf859e7cabd8184ab0b2b317a5d8d3ccb6f4922be7f2a5d28c20d075a2 in /usr/local/bin/ 
# Tue, 28 Mar 2023 02:17:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 28 Mar 2023 02:17:40 GMT
CMD ["php-fpm"]
```

-	Layers:
	-	`sha256:25d08e051bb75230bad82e3a7a054083beec6b4f6a46c8345c731582c297a408`  
		Last Modified: Thu, 23 Mar 2023 00:47:20 GMT  
		Size: 29.6 MB (29646820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fb65f262bf8becde8c3368266a1f67c2bb663b8697df528b2b273d3053d898d`  
		Last Modified: Thu, 23 Mar 2023 09:05:16 GMT  
		Size: 224.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d39eb42b7764a8cf9191ccafca9cfb745e96522d012b55e818afa39062a75f45`  
		Last Modified: Thu, 23 Mar 2023 09:05:26 GMT  
		Size: 71.6 MB (71628851 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73d4a6b504798f4e993e8c14ad74738d9021100d324f4c26cf5303de749f996f`  
		Last Modified: Tue, 28 Mar 2023 00:02:05 GMT  
		Size: 270.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ab96383bd17d7441232a3caea205cbacd434b57bef720aefae781acaae3d25a`  
		Last Modified: Tue, 28 Mar 2023 00:02:04 GMT  
		Size: 12.3 MB (12309425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1286aeca2a9815f791ecd94ab44cf553e769e721ee47d4a922f07053d982f2ec`  
		Last Modified: Tue, 28 Mar 2023 00:02:04 GMT  
		Size: 493.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e15ab8dc28eb4894125b6d3ed036f308c9148bd4e0621459c8fea955b9842439`  
		Last Modified: Tue, 28 Mar 2023 00:02:46 GMT  
		Size: 25.6 MB (25563680 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a9d003b07cf54a8f1d4c10401e395064012b388fffc7e761949eb6dabc89732`  
		Last Modified: Tue, 28 Mar 2023 00:02:43 GMT  
		Size: 2.5 KB (2450 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef6163a786ade5a4717a6257088d0672f0b9a164e8157e3fd3481bf5f2766d9f`  
		Last Modified: Tue, 28 Mar 2023 00:02:43 GMT  
		Size: 246.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf5eb03f41eb3bebde4c53679926366e122334c96deacd88b8dbd0a5ce4984df`  
		Last Modified: Tue, 28 Mar 2023 00:02:43 GMT  
		Size: 9.2 KB (9183 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:26f69203861a4723a4820ca74074c8194e14062b1afe6d4f8d5408fd540b691f`  
		Last Modified: Tue, 28 Mar 2023 02:18:38 GMT  
		Size: 162.6 KB (162597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46559dcc8f62a9104667bcf85d594a82ef13ea80dd066b1e05ee673f91d3188a`  
		Last Modified: Tue, 28 Mar 2023 02:18:37 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36568fa6656bf05a0e941af805e08495e2dcdee45b17b2942afd976ca506f4b5`  
		Last Modified: Tue, 28 Mar 2023 02:18:38 GMT  
		Size: 4.1 MB (4073438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a6a43d7e4a8ec242ef034dd5a8fa42b11fbbe2a669f4dccce32a8157767cb16`  
		Last Modified: Tue, 28 Mar 2023 02:18:37 GMT  
		Size: 2.1 KB (2053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe8278279e498800563eb01750295a7f90c9c46e11b44c11cb33045f862a4506`  
		Last Modified: Tue, 28 Mar 2023 02:18:37 GMT  
		Size: 1.6 KB (1553 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
